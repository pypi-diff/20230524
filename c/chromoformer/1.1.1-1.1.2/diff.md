# Comparing `tmp/chromoformer-1.1.1.tar.gz` & `tmp/chromoformer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromoformer-1.1.1.tar", last modified: Tue May  9 05:54:16 2023, max compression
+gzip compressed data, was "chromoformer-1.1.2.tar", last modified: Wed May 24 07:27:19 2023, max compression
```

## Comparing `chromoformer-1.1.1.tar` & `chromoformer-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:54:16.289229 chromoformer-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 05:54:00.000000 chromoformer-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-09 05:54:16.289229 chromoformer-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-09 05:54:00.000000 chromoformer-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:54:16.285229 chromoformer-1.1.1/chromoformer/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:54:16.289229 chromoformer-1.1.1/chromoformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 05:54:16.289229 chromoformer-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-09 05:54:01.000000 chromoformer-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:27:19.008883 chromoformer-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 07:27:02.000000 chromoformer-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-24 07:27:19.008883 chromoformer-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-24 07:27:02.000000 chromoformer-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:27:19.008883 chromoformer-1.1.2/chromoformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-24 07:27:02.000000 chromoformer-1.1.2/chromoformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-24 07:27:02.000000 chromoformer-1.1.2/chromoformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-05-24 07:27:02.000000 chromoformer-1.1.2/chromoformer/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17568 2023-05-24 07:27:02.000000 chromoformer-1.1.2/chromoformer/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-24 07:27:02.000000 chromoformer-1.1.2/chromoformer/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-24 07:27:02.000000 chromoformer-1.1.2/chromoformer/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:27:19.008883 chromoformer-1.1.2/chromoformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-24 07:27:18.000000 chromoformer-1.1.2/chromoformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-24 07:27:19.000000 chromoformer-1.1.2/chromoformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:27:18.000000 chromoformer-1.1.2/chromoformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 07:27:18.000000 chromoformer-1.1.2/chromoformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 07:27:18.000000 chromoformer-1.1.2/chromoformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:27:19.008883 chromoformer-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-24 07:27:04.000000 chromoformer-1.1.2/setup.py
```

### Comparing `chromoformer-1.1.1/LICENSE` & `chromoformer-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chromoformer-1.1.1/PKG-INFO` & `chromoformer-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromoformer
-Version: 1.1.1
+Version: 1.1.2
 Summary: Chromoformer - Pytorch
 Home-page: https://github.com/dohlee/chromoformer
 Author: Dohoon Lee
 Author-email: dohlee.bioinfo@gmail.com
 License: MIT
 Keywords: artificial intelligence,epigenomics,gene expression prediction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chromoformer-1.1.1/README.md` & `chromoformer-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chromoformer-1.1.1/chromoformer/data.py` & `chromoformer-1.1.2/chromoformer/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,29 +22,34 @@
 
 class ChromoformerDataset(Dataset):
     def __init__(
         self,
         meta,
         npy_dir,
         target_genes,
+        n_feats=7,
         i_max=8,
         binsizes=[2000, 500, 100],
         w_prom=40000,
         w_max=40000,
         regression=False,
     ):
         super(ChromoformerDataset, self).__init__()
 
         self.npy_dir = npy_dir
+        self.n_feats = n_feats
         self.target_genes = target_genes  # List of ENSGs.
 
         self.meta = pd.read_csv(meta)
+        self.regression = regression
 
-        if regression:
-            self.ensg2label = {r.gene_id: np.log2(r.expression + 1) for r in self.meta.to_records()}
+        if self.regression:
+            self.ensg2label = {
+                r.gene_id: np.log2(r.expression + 1) for r in self.meta.to_records()
+            }
         else:
             self.ensg2label = {r.gene_id: r.label for r in self.meta.to_records()}
 
         self.ensg2tss, self.ensg2pcres, self.ensg2scores = {}, {}, {}
         for r in self.meta.to_records():
             self.ensg2tss[r.gene_id] = (r.chrom, r.start, r.end, r.strand)
 
@@ -113,15 +118,18 @@
         if target_gene not in self.ensg2tss:
             print(target_gene)
 
         pcres, scores = self.ensg2pcres[target_gene], self.ensg2scores[target_gene]
         n_partners, n_dummies = len(pcres), self.i_max - len(pcres)
 
         item = {}
-        item["label"] = self.ensg2label[target_gene]
+        if self.regression:
+            item["label"] = torch.tensor(self.ensg2label[target_gene]).float()
+        else:
+            item["label"] = torch.tensor(self.ensg2label[target_genes]).long()
 
         item["promoter_feats"] = {}
         item["promoter_pad_masks"] = {}
         item["pcre_feats"] = {}
         item["pcre_pad_masks"] = {}
         item["interaction_masks"] = {}
 
@@ -139,15 +147,15 @@
                 end_p,
                 binsize,
                 max_n_bins,
                 strand_p,
                 window=self.w_prom,
             )
 
-            x_p = x_p.permute(1, 0).unsqueeze(0)  # 1 x max_n_bins x 7
+            x_p = x_p.permute(1, 0).unsqueeze(0)  # 1 x max_n_bins x n_feats
 
             mask_p = torch.ones([1, max_n_bins, max_n_bins], dtype=torch.bool)
             mask_p[
                 0,
                 left_pad_p : left_pad_p + n_bins_p,
                 left_pad_p : left_pad_p + n_bins_p,
             ] = 0
@@ -177,23 +185,25 @@
                 ] = 0
 
                 x_pcres.append(x_pcre)
                 mask_pcres.append(mask_pcre)
 
                 interaction_freq[0, i + 1] = score
 
-            x_pcres.append(torch.zeros([7, n_dummies * max_n_bins]))
+            x_pcres.append(torch.zeros([self.n_feats, n_dummies * max_n_bins]))
             x_pcres = torch.cat(x_pcres, axis=1).view(-1, self.i_max, max_n_bins)
             x_pcres = x_pcres.permute(1, 2, 0)  # i_max x max_n_bins x 7
 
             for _ in range(n_dummies):
                 m = torch.ones([1, max_n_bins, max_n_bins], dtype=torch.bool)
                 mask_pcres.append(m)
 
-            interaction_mask = torch.ones([self.i_max + 1, self.i_max + 1], dtype=torch.bool)
+            interaction_mask = torch.ones(
+                [self.i_max + 1, self.i_max + 1], dtype=torch.bool
+            )
             interaction_mask[: n_partners + 1, : n_partners + 1] = 0
 
             item["promoter_feats"][binsize] = x_p
             item["promoter_pad_masks"][binsize] = mask_p
             item["pcre_feats"][binsize] = x_pcres
             item["pcre_pad_masks"][binsize] = torch.stack(mask_pcres)
             item["interaction_masks"][binsize] = interaction_mask.unsqueeze(0)
```

### Comparing `chromoformer-1.1.1/chromoformer/modules.py` & `chromoformer-1.1.2/chromoformer/modules.py`

 * *Files identical despite different names*

### Comparing `chromoformer-1.1.1/chromoformer/net.py` & `chromoformer-1.1.2/chromoformer/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import torch.nn.functional as F
 import numpy as np
 
 from .modules import Transformer, PairwiseTransformer
 
 
 class EmbeddingTransformer(nn.Module):
-    def __init__(self, n_feats, n_layers, n_heads, d_model, d_ff, pos_enc=True, activation=F.relu):
+    def __init__(
+        self, n_feats, n_layers, n_heads, d_model, d_ff, pos_enc=True, activation=F.relu
+    ):
         super(EmbeddingTransformer, self).__init__()
 
         self.d_model = d_model
         self.lin_proj = nn.Linear(n_feats, self.d_model, bias=False)
 
         self.transformer = Transformer(
             n_layers, n_heads, self.d_model, self.d_model, d_ff, activation, gate=False
@@ -134,18 +136,22 @@
         # --> x : bsz x (max_n_interactions + 1) x max_n_bins x d_model
 
         x = x[:, :, max_n_bins // 2]  # Take the genomic bin representation at center.
         return x
 
 
 class RegulationTransformer(nn.Module):
-    def __init__(self, n_layers, n_heads, d_emb, d_model, d_ff, pos_enc=True, activation=F.relu):
+    def __init__(
+        self, n_layers, n_heads, d_emb, d_model, d_ff, pos_enc=True, activation=F.relu
+    ):
         super(RegulationTransformer, self).__init__()
 
-        self.transformer = Transformer(n_layers, n_heads, d_emb, d_model, d_ff, gate=True)
+        self.transformer = Transformer(
+            n_layers, n_heads, d_emb, d_model, d_ff, gate=True
+        )
 
     def forward(self, x, mask, bias):
         return self.transformer(x, mask, bias)
 
 
 class Chromoformer(nn.Module):
     def __init__(
@@ -238,15 +244,17 @@
         interaction_mask_100,
         interaction_freq,
     ):
         p_emb_2000_total, p_emb_2000 = self.embed2000(x_p_2000, pad_mask_p_2000)
         p_emb_500_total, p_emb_500 = self.embed500(x_p_500, pad_mask_p_500)
         p_emb_100_total, p_emb_100 = self.embed100(x_p_100, pad_mask_p_100)
 
-        pw_int_emb_2000 = self.pw_int2000(p_emb_2000_total, x_pcre_2000, pad_mask_pcre_2000)
+        pw_int_emb_2000 = self.pw_int2000(
+            p_emb_2000_total, x_pcre_2000, pad_mask_pcre_2000
+        )
         pw_int_emb_500 = self.pw_int500(p_emb_500_total, x_pcre_500, pad_mask_pcre_500)
         pw_int_emb_100 = self.pw_int100(p_emb_100_total, x_pcre_100, pad_mask_pcre_100)
 
         x_2000 = torch.cat([p_emb_2000, pw_int_emb_2000], axis=1)
         x_500 = torch.cat([p_emb_500, pw_int_emb_500], axis=1)
         x_100 = torch.cat([p_emb_100, pw_int_emb_100], axis=1)
 
@@ -306,15 +314,18 @@
         self.pairwise_interaction = nn.ModuleDict(
             {
                 str(binsize): PairwiseInteractionTransformer(**pairwise_interaction_kws)
                 for binsize in binsizes
             }
         )
         self.regulation = nn.ModuleDict(
-            {str(binsize): RegulationTransformer(**regulation_kws) for binsize in binsizes}
+            {
+                str(binsize): RegulationTransformer(**regulation_kws)
+                for binsize in binsizes
+            }
         )
         self.fc_head = nn.Sequential(
             nn.Linear(d_emb * 3, d_head),
             nn.ReLU(),
             nn.Linear(d_head, 2),
         )
 
@@ -326,15 +337,17 @@
         pcre_pad_masks,
         interaction_masks,
         interaction_freq,
     ):
         promoter_embeddings_full, promoter_embeddings_tss = {}, {}
         for binsize in self.binsizes:
             layer = self.embed[str(binsize)]
-            p_emb_full, p_emb = layer(promoter_feats[binsize], promoter_pad_masks[binsize])
+            p_emb_full, p_emb = layer(
+                promoter_feats[binsize], promoter_pad_masks[binsize]
+            )
             promoter_embeddings_full[binsize] = p_emb_full
             promoter_embeddings_tss[binsize] = p_emb
 
         pairwise_interaction_embeddings = {}
         for binsize in self.binsizes:
             layer = self.pairwise_interaction[str(binsize)]
             pairwise_interaction_embeddings[binsize] = layer(
@@ -353,15 +366,17 @@
             )
             for binsize in self.binsizes
         }
 
         x_out = {}
         for binsize in self.binsizes:
             layer = self.regulation[str(binsize)]
-            x_out[binsize] = layer(x_in[binsize], interaction_masks[binsize], bias=interaction_freq)
+            x_out[binsize] = layer(
+                x_in[binsize], interaction_masks[binsize], bias=interaction_freq
+            )
 
         x = torch.cat([x_out[binsize][:, 0] for binsize in self.binsizes], axis=1)
         x += torch.cat([x_in[binsize][:, 0] for binsize in self.binsizes], axis=1)
 
         return self.fc_head(x)
 
 
@@ -551,9 +566,11 @@
     print(out_regressor.sum())
     print(out_regressor.shape)
     # -0.1900, [8, 1]
 
     # ckpt = torch.load("test.pt")
     # model_classifier.load_state_dict(ckpt["net"])
 
-    ckpt = torch.load('converted/E003/chromoformer-reg-reproduction-E003-conf1-fold1.pt')
+    ckpt = torch.load(
+        "converted/E003/chromoformer-reg-reproduction-E003-conf1-fold1.pt"
+    )
     model_regressor.load_state_dict(ckpt["net"])
```

### Comparing `chromoformer-1.1.1/chromoformer/train.py` & `chromoformer-1.1.2/chromoformer/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,29 +77,33 @@
 wandb.config.update(config)
 
 meta = (
     pd.read_csv(args.meta).sample(frac=1, random_state=seed).reset_index(drop=True)
 )  # load and shuffle.
 
 if args.regression and "expression" not in meta.columns:
-    raise ValueError("`expression` column is required for training ChromoformerRegression model.")
+    raise ValueError(
+        "`expression` column is required for training ChromoformerRegression model."
+    )
 
 # Split genes into two sets (train/val).
 genes = set(meta.gene_id.unique())
 n_genes = len(genes)
 print("Target genes:", len(genes))
 
 qs = [
     meta[meta.split == 1].gene_id.tolist(),
     meta[meta.split == 2].gene_id.tolist(),
     meta[meta.split == 3].gene_id.tolist(),
     meta[meta.split == 4].gene_id.tolist(),
 ]
 
-train_genes = qs[(args.fold + 0) % 4] + qs[(args.fold + 1) % 4] + qs[(args.fold + 2) % 4]
+train_genes = (
+    qs[(args.fold + 0) % 4] + qs[(args.fold + 1) % 4] + qs[(args.fold + 2) % 4]
+)
 val_genes = qs[(args.fold + 3) % 4]
 
 wandb.config.update(
     {
         "n_train_genes": len(train_genes),
         "n_val_genes": len(val_genes),
     }
@@ -107,24 +111,26 @@
 
 print(len(train_genes), len(val_genes))
 
 train_dataset = ChromoformerDataset(
     args.meta,
     args.npy_dir,
     train_genes,
+    n_feats,
     i_max,
     args.binsizes,
     w_prom,
     w_max,
     regression=args.regression,
 )
 val_dataset = ChromoformerDataset(
     args.meta,
     args.npy_dir,
     val_genes,
+    n_feats,
     i_max,
     args.binsizes,
     w_prom,
     w_max,
     regression=args.regression,
 )
 
@@ -166,14 +172,17 @@
         for k, v in d.items():
             if isinstance(v, dict):
                 for _k, _v in v.items():
                     v[_k] = _v.cuda()
             else:
                 d[k] = v.cuda()
 
+        if args.regression:
+            d["label"] = d["label"].view(-1, 1)
+
         optimizer.zero_grad()
 
         out = model(
             d["promoter_feats"],
             d["promoter_pad_masks"],
             d["pcre_feats"],
             d["pcre_pad_masks"],
@@ -195,14 +204,15 @@
         if batch % 10 == 0:
             batch_loss = running_loss / 10.0
 
             train_out, train_label = map(torch.cat, (train_out, train_label))
 
             if args.regression:
                 train_pred = train_out.flatten()
+                train_label = train_label.flatten()
 
                 batch_r2 = metrics.r2_score(train_label, train_pred) * 100
                 batch_r = stats.pearsonr(train_label, train_pred)[0] * 100
 
                 bar.set_description(
                     f"E{epoch} {batch_loss:.4f}, lr={get_lr(optimizer)}, r2={batch_r2:.4f}, r={batch_r:.4f}"
                 )
@@ -216,15 +226,17 @@
                 )
             else:
                 train_score = train_out.softmax(axis=1)[:, 1]
                 train_pred = train_out.argmax(axis=1)
 
                 batch_acc = metrics.accuracy_score(train_label, train_pred) * 100
                 batch_auc = metrics.roc_auc_score(train_label, train_score) * 100
-                batch_ap = metrics.average_precision_score(train_label, train_score) * 100
+                batch_ap = (
+                    metrics.average_precision_score(train_label, train_score) * 100
+                )
 
                 bar.set_description(
                     f"E{epoch} {batch_loss:.4f}, lr={get_lr(optimizer)}, acc={batch_acc:.4f}, auc={batch_auc:.4f}, ap={batch_ap:.4f}"
                 )
 
                 wandb.log(
                     {
```

### Comparing `chromoformer-1.1.1/chromoformer.egg-info/PKG-INFO` & `chromoformer-1.1.2/chromoformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromoformer
-Version: 1.1.1
+Version: 1.1.2
 Summary: Chromoformer - Pytorch
 Home-page: https://github.com/dohlee/chromoformer
 Author: Dohoon Lee
 Author-email: dohlee.bioinfo@gmail.com
 License: MIT
 Keywords: artificial intelligence,epigenomics,gene expression prediction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chromoformer-1.1.1/setup.py` & `chromoformer-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chromoformer",
     packages=find_packages(exclude=[]),
     include_package_data=True,
-    version="1.1.1",
+    version="1.1.2",
     license="MIT",
     description="Chromoformer - Pytorch",
     author="Dohoon Lee",
     author_email="dohlee.bioinfo@gmail.com",
     long_description_content_type="text/markdown",
     url="https://github.com/dohlee/chromoformer",
     keywords=[
```

