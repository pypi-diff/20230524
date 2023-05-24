# Comparing `tmp/DeltaTopic-0.0.2.tar.gz` & `tmp/DeltaTopic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeltaTopic-0.0.2.tar", last modified: Tue Apr 25 04:34:56 2023, max compression
+gzip compressed data, was "DeltaTopic-0.1.0.tar", last modified: Wed May 24 02:28:55 2023, max compression
```

## Comparing `DeltaTopic-0.0.2.tar` & `DeltaTopic-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.488361 DeltaTopic-0.0.2/DeltaTopic/
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-15 05:16:01.000000 DeltaTopic-0.0.2/DeltaTopic/__init__.py
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/DeltaTopic/nn/
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    10596 2023-04-15 05:19:11.000000 DeltaTopic-0.0.2/DeltaTopic/nn/TrainingPlan.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-14 21:10:15.000000 DeltaTopic-0.0.2/DeltaTopic/nn/__init__.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    29553 2023-03-10 21:06:37.000000 DeltaTopic-0.0.2/DeltaTopic/nn/base_components.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    10652 2023-03-10 21:06:37.000000 DeltaTopic-0.0.2/DeltaTopic/nn/base_model.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     9128 2023-03-10 21:06:37.000000 DeltaTopic-0.0.2/DeltaTopic/nn/dataloader_util.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    40251 2023-04-25 02:21:55.000000 DeltaTopic-0.0.2/DeltaTopic/nn/modelhub.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    14127 2023-04-25 02:16:43.000000 DeltaTopic-0.0.2/DeltaTopic/nn/module.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    27768 2023-04-25 03:32:03.000000 DeltaTopic-0.0.2/DeltaTopic/nn/util.py
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/DeltaTopic/run/
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     3459 2023-04-24 23:03:26.000000 DeltaTopic-0.0.2/DeltaTopic/run/BALSAM.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     4088 2023-04-15 05:19:11.000000 DeltaTopic-0.0.2/DeltaTopic/run/DeltaTopic.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-14 21:33:20.000000 DeltaTopic-0.0.2/DeltaTopic/run/__init__.py
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.488361 DeltaTopic-0.0.2/DeltaTopic.egg-info/
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      396 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/PKG-INFO
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      560 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/SOURCES.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        1 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/dependency_links.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       99 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/entry_points.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      120 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/requires.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       11 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/top_level.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      396 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/PKG-INFO
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      684 2023-04-15 00:58:13.000000 DeltaTopic-0.0.2/README.md
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       79 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/setup.cfg
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      880 2023-04-25 04:34:46.000000 DeltaTopic-0.0.2/setup.py
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-05-24 02:28:55.175260 DeltaTopic-0.1.0/
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-05-24 02:28:55.175260 DeltaTopic-0.1.0/DeltaTopic/
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/__init__.py
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-05-24 02:28:55.175260 DeltaTopic-0.1.0/DeltaTopic/datasets/
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      106 2023-05-20 19:40:41.000000 DeltaTopic-0.1.0/DeltaTopic/datasets/__init__.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      566 2023-05-22 20:27:29.000000 DeltaTopic-0.1.0/DeltaTopic/datasets/_datasets.py
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-05-24 02:28:55.175260 DeltaTopic-0.1.0/DeltaTopic/nn/
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    10596 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/nn/TrainingPlan.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/nn/__init__.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    34122 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/nn/base_components.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    10652 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/nn/base_model.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     9128 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/nn/dataloader_util.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    23677 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/nn/modelhub.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    13284 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/nn/module.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    27977 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/nn/util.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     8693 2023-05-24 02:02:26.000000 DeltaTopic-0.1.0/DeltaTopic/nn/util_benchmark.py
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-05-24 02:28:55.175260 DeltaTopic-0.1.0/DeltaTopic/run/
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     3459 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/run/BALSAM.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     4088 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/run/DeltaTopic.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/DeltaTopic/run/__init__.py
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-05-24 02:28:55.175260 DeltaTopic-0.1.0/DeltaTopic.egg-info/
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      340 2023-05-24 02:28:55.000000 DeltaTopic-0.1.0/DeltaTopic.egg-info/PKG-INFO
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      665 2023-05-24 02:28:55.000000 DeltaTopic-0.1.0/DeltaTopic.egg-info/SOURCES.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        1 2023-05-24 02:28:55.000000 DeltaTopic-0.1.0/DeltaTopic.egg-info/dependency_links.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       98 2023-05-24 02:28:55.000000 DeltaTopic-0.1.0/DeltaTopic.egg-info/entry_points.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      120 2023-05-24 02:28:55.000000 DeltaTopic-0.1.0/DeltaTopic.egg-info/requires.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       11 2023-05-24 02:28:55.000000 DeltaTopic-0.1.0/DeltaTopic.egg-info/top_level.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     1072 2023-04-27 03:05:24.000000 DeltaTopic-0.1.0/LICENSE
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      340 2023-05-24 02:28:55.175260 DeltaTopic-0.1.0/PKG-INFO
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     2842 2023-05-24 01:51:08.000000 DeltaTopic-0.1.0/README.md
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       79 2023-05-24 02:28:55.175260 DeltaTopic-0.1.0/setup.cfg
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      879 2023-05-24 02:24:17.000000 DeltaTopic-0.1.0/setup.py
```

### Comparing `DeltaTopic-0.0.2/DeltaTopic/nn/TrainingPlan.py` & `DeltaTopic-0.1.0/DeltaTopic/nn/TrainingPlan.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytorch_lightning as pl
 import torch
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from DeltaTopic.nn.base_model import BaseModuleClass
 
 class TrainingPlan(pl.LightningModule):
     """
-    Lightning module task to train scvi-tools modules.
+    Lightning module task to train deltaTopic modules.
 
     Parameters
     ----------
     module
         A module instance from class ``BaseModuleClass``.
     lr
         Learning rate used for optimization.
```

### Comparing `DeltaTopic-0.0.2/DeltaTopic/nn/base_components.py` & `DeltaTopic-0.1.0/DeltaTopic/nn/base_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-"""base components for VAE, ETM, pathway-guided connection"""
 import collections
 from typing import Iterable, List
 import torch
 from torch import nn as nn
 from torch.distributions import Normal
 from torch.nn import ModuleList
 import torch.nn.functional as F
@@ -437,17 +435,42 @@
                                 one_hot_cat_list_layer = one_hot_cat_list
                             x = torch.cat((x, *one_hot_cat_list_layer), dim=-1)
                         x = layer(x)
         return x
 
 class DeltaTopicEncoder(nn.Module):
     """
-    Maksed latent encoder with two input heads --> one shared latent space
-    Options to incorporate categorical variables as one-hot vectors
+    A two-headed encoder that maps the two inputs into a shared latent space through a stack of individual and shared fully-connected layers.
+
+    Parameters
+    ----------
+    n_input_list
+        List of the dimension of two input tensors
+    n_output
+        The dimensionality of the output
+    mask
+        The mask to apply to the first layer (experimental)
+    mask_first
+        Transpose the mask if set to false (experimental)
+    n_hidden
+        The number of nodes per hidden layer
+    n_layers_individual
+        The number of fully-connected hidden layers for the individual encoder
+    n_layers_shared
+        The number of fully-connected hidden layers for the shared encoder
+    dropout_rate
+        Dropout rate to apply to each of the hidden layers
+    use_batch_norm
+        Whether to have `BatchNorm` layers or not
+    log_variational
+        Whether to apply log(1+x) transformation to the input
+    combine_method
+        the method to combine the two latent space, either "add" or "concatenate"
     """
+    
     def __init__(
         self,
         n_input_list: List[int],
         n_output: int,
         mask: torch.Tensor = None,
         mask_first: bool = True,
         n_hidden: int = 128,
@@ -494,15 +517,25 @@
             dropout_rate=dropout_rate,
         )
 
         self.mean_encoder = nn.Linear(n_hidden, n_output)
         self.var_encoder = nn.Linear(n_hidden, n_output)
 
     def forward(self, x: torch.Tensor, y: torch.Tensor, *cat_list: int):
+        '''
+        Forward pass for DeltaTopicEncoder
         
+        Parameters
+        ----------
+        x
+            First input tensor, e.g., spliced RNA count
+        y   
+            Second input tensorm, e.g., unsplice RNA count
+    
+        '''
         if self.log_variational:
             x_ = torch.log(1 + x)
             y_ = torch.log(1 + y)
         
         q_x = self.encoders[0](x_, *cat_list)
         q_y = self.encoders[1](y_, *cat_list)
         
@@ -518,28 +551,30 @@
         q_v = torch.exp(torch.clamp(self.var_encoder(q), -4.0, 4.0)/2.)
         latent = reparameterize_gaussian(q_m, q_v)
 
         return q_m, q_v, latent
     
 class DeltaTopicDecoder(nn.Module):
     """
-    The decoder for DeltaTopic model
-    - Model the topic specific post-transcription factor for each gene between spliced and unplisced transcripts 
-
-    Testing script:
-import torch
-from nn.base_components import DeltaETMDecoder
-test_decoder = DeltaETMDecoder(n_input=10, n_output=100)
-input = torch.randn(2, 10) # batch_size 2, 10 LVs
-output = test_decoder(input, 0)
-
-log_beta = test_decoder.beta(test_decoder.rho.expand([test_decoder.n_input,-1]))
-hh = test_decoder.hid(input)
-pr = torch.mm(torch.exp(hh),torch.exp(log_beta))
+    Decoder network for DeltaTopic, a generative network with spike and slab prior for rho and delta.
 
+    Parameters
+    ----------
+    n_input
+        The dimensionality of the input
+    n_output
+        The dimensionality of the output
+    pip0_rho
+        posterior inclusion probability prior for rho
+    pip0_delta
+        posterior inclusion probability prior for delta
+    v0_rho
+        variance for rho slab
+    vo_delta
+        variance for delta slab            
     """
     def __init__(
         self,
         n_input: int,
         n_output: int,
         pip0_rho = 0.1,
         pip0_delta = 0.1,
@@ -570,58 +605,107 @@
         self.log_softmax = nn.LogSoftmax(dim=-1)
     
     
     def forward(
         self,
         z: torch.Tensor,
     ):
+        '''
+        forward pass for DeltaTopicDecoder
+        
+        Parameters
+        ----------
+        z
+            the input the of the decoder, e.g., latent variable from DeltaTopicEncoder
+        '''
         theta = self.soft_max(z)
         rho = self.get_beta(self.spike_logit_rho, self.slab_mean_rho, self.slab_lnvar_rho, self.bias_gene)
         rho_kl = self.sparse_kl_loss(self.logit_0_rho, self.lnvar_0_rho, self.spike_logit_rho, self.slab_mean_rho, self.slab_lnvar_rho)
         
         delta = self.get_beta(self.spike_logit_delta, self.slab_mean_delta, self.slab_lnvar_delta, self.bias_gene)
         delta_kl = self.sparse_kl_loss(self.logit_0_delta, self.lnvar_0_delta, self.spike_logit_delta, self.slab_mean_delta, self.slab_lnvar_delta)
         
         return rho, delta, rho_kl, delta_kl, theta 
     
     def get_rho_delta(
         self,
     ):
+        '''
+        Helper function to get rho and delta
+        '''
         rho = self.get_beta(self.spike_logit_rho, self.slab_mean_rho, self.slab_lnvar_rho, self.bias_gene)
         delta = self.get_beta(self.spike_logit_delta, self.slab_mean_delta, self.slab_lnvar_delta, self.bias_gene)
         
         return rho, delta 
     
     def get_beta(self, 
         spike_logit: torch.Tensor,
         slab_mean: torch.Tensor, 
         slab_lnvar: torch.Tensor,
         bias_gene: torch.Tensor, 
     ): 
+        '''
+        Get a spike and slab sample using reparameterization trick
+        
+        Parameters
+        ----------
+        spike_logit
+            logit of spike probability
+        slab_mean
+            mean of slab
+        slab_lnvar
+            log variance of slab
+        bias_gene
+            gene-level bias
+        '''
         pip = torch.sigmoid(spike_logit)
         mean = slab_mean * pip
         var = pip * (1 - pip) * torch.square(slab_mean)
         var = var + pip * torch.exp(slab_lnvar)
         eps = torch.randn_like(var)
 
         return mean + eps * torch.sqrt(var) - bias_gene
     
     def soft_max(self, 
                  z: torch.Tensor,
-    ):    
+    ):  
+        '''
+        softmax function
+        
+        Parameters
+        ----------
+        z
+            input tensor
+        '''  
         return torch.exp(self.log_softmax(z))
     
     def sparse_kl_loss(
         self,
         logit_0, 
         lnvar_0,
         spike_logit,
         slab_mean,
         slab_lnvar,
-    ):                           
+    ):  
+        '''
+        Compute KL divergence between spike and slab piors and posteriors
+        
+        Parameters
+        ----------
+        logit_0
+            logit of spike probability (prior)
+        lnvar_0
+            log variance of slab (prior)
+        spike_logit
+            logit of spike probability (posterior)
+        slab_mean
+            mean of slab (posterior)            
+        slab_lnvar
+            log variance of slab (posterior)        
+        '''                         
         ## PIP KL between p and p0
         ## p * ln(p / p0) + (1-p) * ln(1-p/1-p0)
         ## = p * ln(p / 1-p) + ln(1-p) +
         ##   p * ln(1-p0 / p0) - ln(1-p0)
         ## = sigmoid(logit) * logit - softplus(logit)
         ##   - sigmoid(logit) * logit0 + softplus(logit0)
         pip_hat = torch.sigmoid(spike_logit)
@@ -631,15 +715,26 @@
         sq_term = torch.exp(-lnvar_0) * (torch.square(slab_mean) + torch.exp(slab_lnvar))
         kl_g = -0.5 * (1. + slab_lnvar - lnvar_0 - sq_term)
         ## Combine both logit and Gaussian KL
         return torch.sum(kl_pip + pip_hat * kl_g) # return a number sum over [N_topics, N_genes]
 
 class BALSAMDecoder(nn.Module):
     """
-    Decoder for Bayesian ETM model 
+    Decoder network for BALSAM model, a generative network with spike and slab prior for beta parameter.
+    
+    Parameters
+    ----------
+    n_input: int
+        The input dimension of the decoder, e.g., number of topics.
+    n_output: int
+        The output dimension of decoder, e.g., tumber of genes.
+    pip0: float
+        The prior probability of spike in the spike and slab prior.
+    v0: float
+        The prior variance of slab in the spike and slab prior.
     """
     def __init__(
         self,
         n_input: int,
         n_output: int,
         pip0 = 0.1,
         v0 = 1,
@@ -660,54 +755,103 @@
         self.log_softmax = nn.LogSoftmax(dim=-1)
     
     
     def forward(
         self,
         z: torch.Tensor,
     ):
+        '''
+        forward pass of the decoder network.
+        
+        Parameters
+        ----------
+        z: torch.Tensor
+            The input tensor of the decoder, e.g., the latent representation from the encoder.
+        '''
         theta = self.soft_max(z)
         rho = self.get_beta(self.spike_logit, self.slab_mean, self.slab_lnvar, self.bias_d)
         rho_kl = self.sparse_kl_loss(self.logit_0, self.lnvar_0, self.spike_logit, self.slab_mean, self.slab_lnvar)
         
         return rho, rho_kl, theta 
     
     def get_rho(
         self,
     ):
+        '''
+        A helper function to get rho.
+        '''
         rho = self.get_beta(self.spike_logit, self.slab_mean, self.slab_lnvar, self.bias_d)
         
         return rho
     
     def get_beta(self, 
         spike_logit: torch.Tensor,
         slab_mean: torch.Tensor, 
         slab_lnvar: torch.Tensor,
         bias_d: torch.Tensor,
     ): 
+        '''
+        Sample beta using the repameterization trick
+        
+        Parameters
+        ----------
+        spike_logit: torch.Tensor
+            The logit of spike probability.
+        slab_mean: torch.Tensor
+            The mean of slab.
+        slab_lnvar: torch.Tensor
+            The log variance of slab.
+        bias_d: torch.Tensor
+            The bias term in the GLM model.    
+        '''
         pip = torch.sigmoid(spike_logit)
         mean = slab_mean * pip
         var = pip * (1 - pip) * torch.square(slab_mean)
         var = var + pip * torch.exp(slab_lnvar)
         eps = torch.randn_like(var)
 
         return mean + eps * torch.sqrt(var) - bias_d
     
     def soft_max(self, 
                  z: torch.Tensor,
-    ):    
+    ):  
+        ''' 
+        softmax function
+        
+        Parameters
+        ----------
+        z: torch.Tensor
+            The input tensor.
+        ''' 
         return torch.exp(self.log_softmax(z))
     
     def sparse_kl_loss(
         self,
         logit_0, 
         lnvar_0,
         spike_logit,
         slab_mean,
         slab_lnvar,
-    ):                           
+    ):  
+        '''
+        Compute the KL divergence between spike and slab prior and the posterior.
+        
+        Parameters
+        ----------
+        logit_0: torch.Tensor
+            The logit prior of spike probability.
+        lnvar_0: torch.Tensor
+            The log variance prior of slab. 
+        spike_logit: torch.Tensor
+            The logit of spike probability.
+        slab_mean: torch.Tensor
+            The mean of slab.
+        slab_lnvar: torch.Tensor
+            The log variance of slab.        
+        '''                         
         ## PIP KL between p and p0
         ## p * ln(p / p0) + (1-p) * ln(1-p/1-p0)
         ## = p * ln(p / 1-p) + ln(1-p) +
         ##   p * ln(1-p0 / p0) - ln(1-p0)
         ## = sigmoid(logit) * logit - softplus(logit)
         ##   - sigmoid(logit) * logit0 + softplus(logit0)
         pip_hat = torch.sigmoid(spike_logit)
@@ -716,17 +860,31 @@
         ## Gaussian KL between N(μ,ν) and N(0, v0) 
         sq_term = torch.exp(-lnvar_0) * (torch.square(slab_mean) + torch.exp(slab_lnvar))
         kl_g = -0.5 * (1. + slab_lnvar - lnvar_0 - sq_term)
         ## Combine both logit and Gaussian KL
         return torch.sum(kl_pip + pip_hat * kl_g) # return a number sum over [N_topics, N_genes]
                               
 class BALSAMEncoder(nn.Module):
-    
     """
-    BayesianETM Encoder
+    Encoder for BALSAM model, encodes the input data into a latent topic representation.
+    
+    Parameters
+    ----------
+    n_input: int
+        The number of input features.
+    n_output: int
+        The number of output features.
+    n_hidden: int
+        The number of hidden units.
+    n_layers_individual: int
+        The number of layers in the network.
+    use_batch_norm: bool
+        Whether to use batch normalization.
+    log_variational: bool
+        Whether to apply log(1+x) to the input.         
     """
     def __init__(
         self,
         n_input: int,
         n_output: int,
         n_hidden: int = 128,
         n_layers_individual: int = 3,
@@ -746,15 +904,17 @@
                     use_batch_norm = use_batch_norm
                 )
 
         self.mean_encoder = nn.Linear(n_hidden, n_output)
         self.var_encoder = nn.Linear(n_hidden, n_output)
 
     def forward(self, x: torch.Tensor, *cat_list: int):
-        
+        '''
+        forward pass of the encoder
+        '''
         if self.log_variational:
             x_ = torch.log(1 + x)
     
         q = self.encoder(x_, *cat_list)    
         q_m = self.mean_encoder(q)
         q_v = torch.exp(torch.clamp(self.var_encoder(q), -4.0, 4.0)/2.)
         latent = reparameterize_gaussian(q_m, q_v)
```

### Comparing `DeltaTopic-0.0.2/DeltaTopic/nn/base_model.py` & `DeltaTopic-0.1.0/DeltaTopic/nn/base_model.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.2/DeltaTopic/nn/dataloader_util.py` & `DeltaTopic-0.1.0/DeltaTopic/nn/dataloader_util.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.2/DeltaTopic/nn/module.py` & `DeltaTopic-0.1.0/DeltaTopic/nn/module.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,32 @@
 from DeltaTopic.nn.base_model import BaseModuleClass, LossRecorder, auto_move_data
 from DeltaTopic.nn.base_components import DeltaTopicEncoder, BALSAMDecoder, BALSAMEncoder, DeltaTopicDecoder
 
 torch.backends.cudnn.benchmark = True
 
 class BALSAM_module(BaseModuleClass):
     """
-    The BALASM module
+    BALASM module
+    
+    Parameters
+    ----------
+    n_genes
+        number of genes
+    n_latent
+        dimension of latent space
+    n_layers_encoder_individual
+        number of individual layers in the encoder
+    dim_hidden_encoder
+        dimension of the hidden layers in the encoder
+    pip0_rho
+        scaling factor for rho loss, default 0.1
+    kl_weight_beta: 
+        scaling factor for KL, default 1.0
+    log_variational
+        Log(data+1) prior to encoding for numerical stability. Not normalization.
     """
 
     def __init__(
         self,
         n_genes: int,
         n_latent: int = 32,
         n_layers_encoder_individual: int = 2,
@@ -91,14 +108,16 @@
     
     def sample_from_posterior_z(
         self, 
         x: torch.Tensor,
         deterministic: bool = True,
         output_softmax_z: bool = True, 
     ):
+        """Sample from the posterior z
+        """
         inference_out = self.inference(x)
         if deterministic:
             z = inference_out["qz_m"]
         else:
             z = inference_out["z"]
         if output_softmax_z:
             generative_outputs = self.generative(z)
@@ -107,15 +126,16 @@
     
     @auto_move_data
     def get_reconstruction_loss(
         self,
         x: torch.Tensor,
     ) -> torch.Tensor:
         """
-        Returns the 
+        Returns the reconstruction loss for a batch of data. 
+        
         Parameters
         ----------
         x
             tensor of values with shape ``(batch_size, n_input)``
         
         Returns
         -------
@@ -141,35 +161,15 @@
         inference_outputs,
         generative_outputs, # this is important to include
         kl_weight=1.0,
         #kl_weight_beta = 1.0,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
 
         """
-        Return the reconstruction loss and the Kullback divergences.
-        Parameters
-        ----------
-        x
-            tensor of values with shape ``(batch_size, n_input)``
-            or ``(batch_size, n_input_fish)`` depending on the mode
-        local_l_mean
-            tensor of means of the prior distribution of latent variable l
-            with shape (batch_size, 1)
-        local_l_var
-            tensor of variances of the prior distribution of latent variable l
-            with shape (batch_size, 1)
-        batch_index
-            array that indicates which batch the cells belong to with shape ``batch_size``
-        y
-            tensor of cell-types labels with shape (batch_size, n_labels)
-        mode
-            indicates which head/tail to use in the joint network
-        Returns
-        -------
-        the reconstruction loss and the Kullback divergences
+        Agrregates the likelihood and KL divergences to form the loss function.
         """
         kl_weight_beta = self.kl_weight_beta
         x = tensors[_CONSTANTS.X_KEY]
         qz_m = inference_outputs["qz_m"]
         qz_v = inference_outputs["qz_v"]
         rho_kl = generative_outputs["rho_kl"]
         
@@ -206,19 +206,19 @@
     n_latent
         dimension of latent space
     n_layers_encoder_individual
         number of individual layers in the encoder
     dim_hidden_encoder
         dimension of the hidden layers in the encoder
     pip0_rho
-        default 0.1
+        scaling factor for rho loss, default 0.1
     pip0_delta
-        default 0.1
+        scaling factor for delta loss, default 0.1
     kl_weight_beta: 
-        default 1.0
+        scaling factor for KL, default 1.0
     log_variational
         Log(data+1) prior to encoding for numerical stability. Not normalization.
     """
 
     def __init__(
         self,
         n_genes: int,
@@ -260,15 +260,15 @@
                                         )
 
     def dir_llik(self, 
                  xx: torch.Tensor, 
                  aa: torch.Tensor,
     ) -> torch.Tensor:
         '''
-        Dirichlet log-likelihood:
+        Return the Dirichlet log-likelihood for a batch.
         '''
         reconstruction_loss = None 
         
         term1 = (torch.lgamma(torch.sum(aa, dim=-1)) -
                 torch.lgamma(torch.sum(aa + xx, dim=-1))) #[n_batch]
         term2 = torch.sum(torch.where(xx > 0,
                             torch.lgamma(aa + xx) -
@@ -304,14 +304,18 @@
     def sample_from_posterior_z(
         self, 
         x: torch.Tensor,
         y: torch.Tensor,
         deterministic: bool = True,
         output_softmax_z: bool = True, 
     ):
+        """
+        sample from the posterior of latent space z
+        """
+        
         inference_out = self.inference(x,y)
         if deterministic: # average of the two means WITHOUT sampling
             z = inference_out["q_m"]
         else: # sampling 
             z = inference_out["z"]
         if output_softmax_z:
             generative_outputs = self.generative(z)
@@ -321,25 +325,22 @@
     @auto_move_data
     def get_reconstruction_loss(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
     ) -> torch.Tensor:
         """
-        Returns the 
+        Returns the reconstruction loss for the given batch.
 
         Parameters
         ----------
         x
             tensor of values with shape ``(batch_size, n_input)``
-        
-        Returns
-        -------
-        type
-            tensor of means of the scaled frequencies
+        y  
+            tensor of values with shape ``(batch_size, n_input)``
 
         """
         inference_out = self.inference(x, y)
         z = inference_out["z"]
         gen_out = self.generative(z)
         theta = gen_out["theta"]
                
@@ -361,38 +362,15 @@
         inference_outputs,
         generative_outputs, # this is important to include
         kl_weight=1.0,
         kl_weight_beta = 1.0,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
 
         """
-        Return the reconstruction loss and the Kullback divergences.
-
-        Parameters
-        ----------
-        x
-            tensor of values with shape ``(batch_size, n_input)``
-            or ``(batch_size, n_input_fish)`` depending on the mode
-        local_l_mean
-            tensor of means of the prior distribution of latent variable l
-            with shape (batch_size, 1)
-        local_l_var
-            tensor of variances of the prior distribution of latent variable l
-            with shape (batch_size, 1)
-        batch_index
-            array that indicates which batch the cells belong to with shape ``batch_size``
-        y
-            tensor of cell-types labels with shape (batch_size, n_labels)
-        mode
-            indicates which head/tail to use in the joint network
-
-
-        Returns
-        -------
-        the reconstruction loss and the Kullback divergences
+        Aggregate the kl and likelihood to form the loss.
 
         """
         kl_weight_beta = self.kl_weight_beta
         x = tensors[_CONSTANTS.X_KEY]
         y = tensors[_CONSTANTS.PROTEIN_EXP_KEY]
         q_m = inference_outputs["q_m"]
         q_v = inference_outputs["q_v"]
```

### Comparing `DeltaTopic-0.0.2/DeltaTopic/nn/util.py` & `DeltaTopic-0.1.0/DeltaTopic/nn/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,15 @@
         >>> model.to_device(0)          # also moves model to GPU 0
         """
         my_device = torch.device(device)
         self.module.to(my_device)
 
     @property
     def device(self):
+        """Device model is on."""
         device = list(set(p.device for p in self.module.parameters()))
         if len(device) > 1:
             raise RuntimeError("Model tensors on multiple devices.")
         return device[0]
 
     def _make_data_loader(
         self,
@@ -313,26 +314,30 @@
 
     @property
     def validation_indices(self):
         return self.validation_indices_
 
     @train_indices.setter
     def train_indices(self, value):
+        """indices for training set."""
         self.train_indices_ = value
 
     @test_indices.setter
     def test_indices(self, value):
+        """indices for test set."""
         self.test_indices_ = value
 
     @validation_indices.setter
     def validation_indices(self, value):
+        """indices for validation set."""
         self.validation_indices_ = value
 
     @is_trained.setter
     def is_trained(self, value):
+        """Flag to indicate whether model is trained."""
         self.is_trained_ = value
 
     @property
     def history(self):
         """Returns computed metrics during training."""
         return self.history_
```

### Comparing `DeltaTopic-0.0.2/DeltaTopic/run/BALSAM.py` & `DeltaTopic-0.1.0/DeltaTopic/run/BALSAM.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.2/DeltaTopic/run/DeltaTopic.py` & `DeltaTopic-0.1.0/DeltaTopic/run/DeltaTopic.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.2/DeltaTopic.egg-info/SOURCES.txt` & `DeltaTopic-0.1.0/DeltaTopic.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 DeltaTopic/__init__.py
 DeltaTopic.egg-info/PKG-INFO
 DeltaTopic.egg-info/SOURCES.txt
 DeltaTopic.egg-info/dependency_links.txt
 DeltaTopic.egg-info/entry_points.txt
 DeltaTopic.egg-info/requires.txt
 DeltaTopic.egg-info/top_level.txt
+DeltaTopic/datasets/__init__.py
+DeltaTopic/datasets/_datasets.py
 DeltaTopic/nn/TrainingPlan.py
 DeltaTopic/nn/__init__.py
 DeltaTopic/nn/base_components.py
 DeltaTopic/nn/base_model.py
 DeltaTopic/nn/dataloader_util.py
 DeltaTopic/nn/modelhub.py
 DeltaTopic/nn/module.py
 DeltaTopic/nn/util.py
+DeltaTopic/nn/util_benchmark.py
 DeltaTopic/run/BALSAM.py
 DeltaTopic/run/DeltaTopic.py
 DeltaTopic/run/__init__.py
```

### Comparing `DeltaTopic-0.0.2/setup.py` & `DeltaTopic-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DeltaTopic',
     packages=find_packages(),
     author='Yichen Zhang',
-    version='0.0.2',
+    version='0.1.0',
     description="Packages to implement BALSAM and DeltaTopic as described in the paper: Unraveling dynamically-encoded latent transcriptomic patterns in pancreatic cancer cells by topic modelling",
     url="https://github.com/causalpathlab/deltaTopic",
     entry_points={'console_scripts':
         ['BALSAM = DeltaTopic.run.BALSAM:main',
         'DeltaTopic = DeltaTopic.run.DeltaTopic:main']
     },
     install_requires=['pandas==1.4.1',
                       'torch==2.0.0', 
                       'h5py==3.6.0', 
-                      'numpy==1.21.5', 
+                      'numpy==1.21.0', 
                       'anndata==0.7.8',
                       'pytorch_lightning==1.9.0', 
                       'scanpy==1.9.3', 
-                      'scipy ==1.8.0']
+                      'scipy==1.8.0']
 )
```

