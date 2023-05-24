# Comparing `tmp/scorecardpipeline-0.1.5.tar.gz` & `tmp/scorecardpipeline-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecardpipeline-0.1.5.tar", last modified: Sun May 21 07:08:58 2023, max compression
+gzip compressed data, was "scorecardpipeline-0.1.6.tar", last modified: Wed May 24 03:01:58 2023, max compression
```

## Comparing `scorecardpipeline-0.1.5.tar` & `scorecardpipeline-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 07:08:58.669523 scorecardpipeline-0.1.5/
--rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-04 06:14:30.000000 scorecardpipeline-0.1.5/LICENSE
--rw-r--r--   0 lubberit   (501) staff       (20)    33317 2023-05-21 07:08:58.669202 scorecardpipeline-0.1.5/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)    32435 2023-05-21 07:03:59.000000 scorecardpipeline-0.1.5/README.md
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 07:08:58.666802 scorecardpipeline-0.1.5/scorecardpipeline/
--rw-r--r--   0 lubberit   (501) staff       (20)      318 2023-05-21 07:08:50.000000 scorecardpipeline-0.1.5/scorecardpipeline/__init__.py
--rw-r--r--   0 lubberit   (501) staff       (20)    20443 2023-05-21 06:04:42.000000 scorecardpipeline-0.1.5/scorecardpipeline/excel_writer.py
--rw-r--r--   0 lubberit   (501) staff       (20)    19272 2023-05-21 06:49:47.000000 scorecardpipeline-0.1.5/scorecardpipeline/model.py
--rw-r--r--   0 lubberit   (501) staff       (20)    21517 2023-05-21 06:04:50.000000 scorecardpipeline-0.1.5/scorecardpipeline/processing.py
--rw-r--r--   0 lubberit   (501) staff       (20)    20072 2023-05-21 06:49:29.000000 scorecardpipeline-0.1.5/scorecardpipeline/utils.py
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-21 07:08:58.668694 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/
--rw-r--r--   0 lubberit   (501) staff       (20)    33317 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)      380 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/SOURCES.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/dependency_links.txt
--rw-r--r--   0 lubberit   (501) staff       (20)      205 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/requires.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       18 2023-05-21 07:08:58.000000 scorecardpipeline-0.1.5/scorecardpipeline.egg-info/top_level.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-21 07:08:58.669613 scorecardpipeline-0.1.5/setup.cfg
--rw-r--r--   0 lubberit   (501) staff       (20)     1788 2023-05-21 07:08:23.000000 scorecardpipeline-0.1.5/setup.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 03:01:58.945102 scorecardpipeline-0.1.6/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-04 06:14:30.000000 scorecardpipeline-0.1.6/LICENSE
+-rw-r--r--   0 lubberit   (501) staff       (20)    34395 2023-05-24 03:01:58.944735 scorecardpipeline-0.1.6/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)    33513 2023-05-24 02:51:13.000000 scorecardpipeline-0.1.6/README.md
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 03:01:58.942489 scorecardpipeline-0.1.6/scorecardpipeline/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1093 2023-05-24 03:01:33.000000 scorecardpipeline-0.1.6/scorecardpipeline/__init__.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    20443 2023-05-21 06:04:42.000000 scorecardpipeline-0.1.6/scorecardpipeline/excel_writer.py
+-rw-r--r--   0 lubberit   (501) staff       (20)     1502 2023-05-23 14:15:12.000000 scorecardpipeline-0.1.6/scorecardpipeline/logger.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    19468 2023-05-23 16:28:40.000000 scorecardpipeline-0.1.6/scorecardpipeline/model.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    21542 2023-05-23 15:37:48.000000 scorecardpipeline-0.1.6/scorecardpipeline/processing.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    26374 2023-05-24 02:56:33.000000 scorecardpipeline-0.1.6/scorecardpipeline/utils.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 03:01:58.944089 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/
+-rw-r--r--   0 lubberit   (501) staff       (20)    34395 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)      408 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)      205 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/requires.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       18 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/top_level.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-24 03:01:58.945199 scorecardpipeline-0.1.6/setup.cfg
+-rw-r--r--   0 lubberit   (501) staff       (20)     1788 2023-05-21 07:08:23.000000 scorecardpipeline-0.1.6/setup.py
```

### Comparing `scorecardpipeline-0.1.5/LICENSE` & `scorecardpipeline-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.5/PKG-INFO` & `scorecardpipeline-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-Metadata-Version: 2.1
-Name: scorecardpipeline
-Version: 0.1.5
-Summary: 评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
-Home-page: https://github.com/itlubber/scorecardpipeline
-Author: itlubber
-Author-email: itlubber@qq.com
-License: MIT
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# 评分卡pipeline建模包
 
-# scorecardpipeline
-
-评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，支持自定义模型报告输出
+`scorecardpipeline` 封装了 `toad`、`scorecardpy`、`optbinning` 等评分卡建模相关组件，`API` 风格与 `sklearn` 高度一致，支持 `pipeline` 式端到端评分卡建模、模型报告输出、导出 `PMML` 文件、超参数搜索等
 
 > 仓库地址：https://github.com/itlubber/scorecardpipeline
 > 
 > 博文地址：https://itlubber.art/archives/itlubber-scorecard-end2end
 > 
 > 微信公共号推文：https://mp.weixin.qq.com/s/eCTp4h0fau77xOgf_V28wQ
 > 
 > pipy包：https://pypi.org/project/scorecardpipeline/
+>
+> `scorecardpipeline` 教程：https://itlubber.art/upload/scorecardpipeline.html
+
+
+## 交流
+
+<table style="text-align:center !important;border=0;">
+    <tr>
+        <td>
+            <span>微信: itlubber</span>
+        </td>
+        <td>
+            <span>微信公众号: itlubber_art</span>
+        </td>
+    </tr>
+    <tr>
+        <td>
+            <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/>
+        </td>
+        <td>
+            <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/>
+        </td>
+    </tr>
+</table>
 
 
 ## 引言
 
 作为一名金融搬砖工作者，评分卡建模怎么也算是基操。本文主要对笔者日常使用的评分卡建模代码进行讲解，说明如何一步步从原始数据到最终评分卡模型以及如何解读产出的模型报告文档。
 
 本文所有代码已全部提交至笔者GITHUB公开仓库，各位看官按需取用，用完记得顺带给个star以鼓励笔者继续开源相关工作。
@@ -74,15 +77,22 @@
 + `processing` 中提供了数据前处理相关的方法：特征筛选方法（`FeatureSelection`、`StepwiseSelection`）、变量分箱方法（`Combiner`）、变量证据权重转换方法（`WOETransformer`），方法继承`sklearn.base`中的`BaseEstimator`和`TransformerMixin`，能够支持构建`pipeline`和超参数搜索
 + `model`中提供了基于`sklearn.linear_model.LogisticRegression`实现的`ITLubberLogisticRegression`，同时重写了`toad.ScoreCard`，以支持模型相关内容的输出
 + `excel_writer` 中提供了操作 `excel` 的一系列公共方法，包含设置条件格式、设置列宽、设置数字格式、插入指定样式的内容（`insert_value2sheet`）、插入图片数据（`insert_pic2sheet`）、插入`dataframe`数据内容（`insert_df2sheet`）、保存`excel`文件（`save`）等方法
 
 ### `scorecardpipeline` 安装
 
 ```bash
-pip install scorecardpipeline -i https://pypi.Python.org/simple/
+>> pip install scorecardpipeline -i https://pypi.Python.org/simple/
+
+Looking in indexes: https://pypi.Python.org/simple/
+Collecting scorecardpipeline
+  Downloading scorecardpipeline-0.1.5-py3-none-any.whl (36 kB)
+  ......
+Installing collected packages: sklearn-pandas, scorecardpy, sklearn2pmml, scorecardpipeline
+Successfully installed scorecardpipeline-0.1.5 scorecardpy-0.1.9.2 sklearn-pandas-2.2.0 sklearn2pmml-0.92.2
 ```
 
 
 ## 评分卡建模
 
 ### 数据准备
```

### Comparing `scorecardpipeline-0.1.5/README.md` & `scorecardpipeline-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,63 @@
-# scorecardpipeline
+Metadata-Version: 2.1
+Name: scorecardpipeline
+Version: 0.1.6
+Summary: 评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
+Home-page: https://github.com/itlubber/scorecardpipeline
+Author: itlubber
+Author-email: itlubber@qq.com
+License: MIT
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，支持自定义模型报告输出
+# 评分卡pipeline建模包
+
+`scorecardpipeline` 封装了 `toad`、`scorecardpy`、`optbinning` 等评分卡建模相关组件，`API` 风格与 `sklearn` 高度一致，支持 `pipeline` 式端到端评分卡建模、模型报告输出、导出 `PMML` 文件、超参数搜索等
 
 > 仓库地址：https://github.com/itlubber/scorecardpipeline
 > 
 > 博文地址：https://itlubber.art/archives/itlubber-scorecard-end2end
 > 
 > 微信公共号推文：https://mp.weixin.qq.com/s/eCTp4h0fau77xOgf_V28wQ
 > 
 > pipy包：https://pypi.org/project/scorecardpipeline/
+>
+> `scorecardpipeline` 教程：https://itlubber.art/upload/scorecardpipeline.html
+
+
+## 交流
+
+<table style="text-align:center !important;border=0;">
+    <tr>
+        <td>
+            <span>微信: itlubber</span>
+        </td>
+        <td>
+            <span>微信公众号: itlubber_art</span>
+        </td>
+    </tr>
+    <tr>
+        <td>
+            <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/>
+        </td>
+        <td>
+            <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/>
+        </td>
+    </tr>
+</table>
 
 
 ## 引言
 
 作为一名金融搬砖工作者，评分卡建模怎么也算是基操。本文主要对笔者日常使用的评分卡建模代码进行讲解，说明如何一步步从原始数据到最终评分卡模型以及如何解读产出的模型报告文档。
 
 本文所有代码已全部提交至笔者GITHUB公开仓库，各位看官按需取用，用完记得顺带给个star以鼓励笔者继续开源相关工作。
@@ -53,15 +98,22 @@
 + `processing` 中提供了数据前处理相关的方法：特征筛选方法（`FeatureSelection`、`StepwiseSelection`）、变量分箱方法（`Combiner`）、变量证据权重转换方法（`WOETransformer`），方法继承`sklearn.base`中的`BaseEstimator`和`TransformerMixin`，能够支持构建`pipeline`和超参数搜索
 + `model`中提供了基于`sklearn.linear_model.LogisticRegression`实现的`ITLubberLogisticRegression`，同时重写了`toad.ScoreCard`，以支持模型相关内容的输出
 + `excel_writer` 中提供了操作 `excel` 的一系列公共方法，包含设置条件格式、设置列宽、设置数字格式、插入指定样式的内容（`insert_value2sheet`）、插入图片数据（`insert_pic2sheet`）、插入`dataframe`数据内容（`insert_df2sheet`）、保存`excel`文件（`save`）等方法
 
 ### `scorecardpipeline` 安装
 
 ```bash
-pip install scorecardpipeline -i https://pypi.Python.org/simple/
+>> pip install scorecardpipeline -i https://pypi.Python.org/simple/
+
+Looking in indexes: https://pypi.Python.org/simple/
+Collecting scorecardpipeline
+  Downloading scorecardpipeline-0.1.5-py3-none-any.whl (36 kB)
+  ......
+Installing collected packages: sklearn-pandas, scorecardpy, sklearn2pmml, scorecardpipeline
+Successfully installed scorecardpipeline-0.1.5 scorecardpy-0.1.9.2 sklearn-pandas-2.2.0 sklearn2pmml-0.92.2
 ```
 
 
 ## 评分卡建模
 
 ### 数据准备
```

### Comparing `scorecardpipeline-0.1.5/scorecardpipeline/excel_writer.py` & `scorecardpipeline-0.1.6/scorecardpipeline/excel_writer.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.5/scorecardpipeline/model.py` & `scorecardpipeline-0.1.6/scorecardpipeline/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,36 +2,25 @@
 """
 @Time    : 2023/05/21 16:23
 @Author  : itlubber
 @Site    : itlubber.art
 """
 
 import os
-import toad
-import warnings
+import math
 import numpy as np
 import pandas as pd
 import scorecardpy as sc
-from scorecardpy.perf import eva_pks, eva_proc
-from optbinning import OptimalBinning
 import matplotlib.pyplot as plt
-from matplotlib import font_manager
-import seaborn as sns
-
+import toad
 import scipy
-import statsmodels.api as sm
 from statsmodels.stats.outliers_influence import variance_inflation_factor
-
-from sklearn.pipeline import Pipeline
-from sklearn.metrics import roc_curve, auc
 from sklearn.metrics import classification_report
 from sklearn.linear_model import LogisticRegression
-from sklearn.model_selection import train_test_split
 from sklearn.utils.validation import check_is_fitted
-from sklearn.ensemble import GradientBoostingClassifier
 from sklearn.base import BaseEstimator, TransformerMixin, ClassifierMixin
 
 from .utils import *
 from .processing import *
 
 
 class ITLubberLogisticRegression(LogisticRegression):
@@ -273,30 +262,40 @@
         self.base_effect = pd.Series(np.median(sub_score, axis=0), index = self.features_)
 
         return self
     
     def transform(self, x):
         return self.predict(x)
     
+    @staticmethod
+    def score_clip(score, clip=50):
+        clip_start = max(math.ceil(score.min() / clip) * clip, math.ceil(score.quantile(0.01) / clip) * clip)
+        clip_end = min(math.ceil(score.max() / clip) * clip, math.ceil(score.quantile(0.99) / clip) * clip)
+        return [i for i in range(clip_start, clip_end, clip)]
+    
     def scorecard_scale(self):
         scorecard_kedu = pd.DataFrame(
             [
                 ["base_odds", self.base_odds, "根据业务经验设置的基础比率（违约概率/正常概率），估算方法：（1-样本坏客户占比）/坏客户占比"],
                 ["base_score", self.base_score, "基础ODDS对应的分数"],
                 ["rate", self.rate, "设置分数的倍率"],
                 ["pdo", self.pdo, "表示分数增长PDO时，ODDS值增长到RATE倍"],
                 ["B", self.offset, "补偿值，计算方式：pdo / ln(rate)"],
                 ["A", self.factor, "刻度，计算方式：base_score - B * ln(base_odds)"],
             ],
             columns=["刻度项", "刻度值", "备注"],
         )
         return scorecard_kedu
     
-    def scorecard_points(self):
+    def scorecard_points(self, feature_map={}):
         card_points = self.export(to_frame=True).rename(columns={"name": "变量名称", "value": "变量分箱", "score": "对应分数"})
+        
+        if feature_map is not None and len(feature_map) > 0:
+            card_points.insert(loc=1, column="变量含义", value=[feature_map.get(c, "") for c in card_points["变量名称"]])
+        
         return card_points
     
     def scorecard2pmml(self, pmml: str = 'scorecard.pmml', debug: bool = False):
         """export a scorecard to pmml
 
         Args:
             pmml (str): io to write pmml file.
```

### Comparing `scorecardpipeline-0.1.5/scorecardpipeline/processing.py` & `scorecardpipeline-0.1.6/scorecardpipeline/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     def __init__(self, target="target", estimator="ols", direction="both", criterion="aic", max_iter=None, return_drop=True, exclude=None, intercept=True, p_value_enter=0.2, p_remove=0.01, p_enter=0.01, target_rm=False):
         """逐步回归筛选方法
 
         Args:
             target: 数据集中标签名称，默认 target
             estimator: 预估器，默认 ols，可选 "ols", "lr", "lasso", "ridge"，通常默认即可
             direction: 逐步回归方向，默认both，可选 "forward", "backward", "both"，通常默认即可
-            criterion: 评价指标，默认 aic，可选 "aic", "bic"，通常默认即可
+            criterion: 评价指标，默认 aic，可选 "aic", "bic", "ks", "auc"，通常默认即可
             max_iter: 最大迭代次数，sklearn中使用的参数，默认为 None
             return_drop: 是否返回特征剔除信息，默认 True
             exclude: 强制保留的某些特征
             intercept: 是否包含截距，默认为 True
             p_value_enter: 特征进入的 p 值，用于前向筛选时决定特征是否进入模型
             p_remove: 特征剔除的 p 值，用于后向剔除时决定特征是否要剔除
             p_enter: 特征 p 值，用于判断双向逐步回归是否剔除或者准入特征
@@ -235,15 +235,15 @@
         self.select_columns = None
         self.dropped = None
     
     def fit(self, x, y=None):
         x = x.copy()
         
         if self.max_iv is not None:
-            self.high_iv_feature_names_ = list(toad.quality(train, target=target, cpu_cores=-1, iv_only=True).query("iv > 1.0").index)
+            self.high_iv_feature_names_ = list(toad.quality(x, target=self.target, cpu_cores=-1, iv_only=True).query(f"iv > {self.max_iv}").index)
             x = x[[c for c in x.columns if c not in self.high_iv_feature_names_]]
         
         X = x.drop(columns=self.target)
         Y = x[self.target]
         
         self.feature_names_ = list(X.columns)
         cat_features_index = [i for i in range(len(self.feature_names_)) if self.feature_names_[i] not in X.select_dtypes("number").columns]
```

### Comparing `scorecardpipeline-0.1.5/scorecardpipeline/utils.py` & `scorecardpipeline-0.1.6/scorecardpipeline/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 """
 import warnings
 
 warnings.filterwarnings("ignore")
 
 import os
 import re
+import six
 import random
 import joblib
+import warnings
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib import font_manager
+from matplotlib.ticker import PercentFormatter
 import seaborn as sns
 from sklearn.metrics import roc_curve, auc
-
 import toad
 from optbinning import OptimalBinning
 
+from .logger import init_logger
+
 
 def seed_everything(seed: int, freeze_torch=False):
     """
     固定随机种子
     """
     random.seed(seed)
     os.environ['PYTHONHASHSEED'] = str(seed)
@@ -35,15 +39,16 @@
         import torch
         torch.manual_seed(seed)
         torch.cuda.manual_seed(seed)
         torch.backends.cudnn.deterministic = True
         torch.backends.cudnn.benchmark = True
 
 
-def init_setting(font_path=None, seed=None, freeze_torch=False):
+def init_setting(font_path=None, seed=None, freeze_torch=False, logger=False, **kwargs):
+    warnings.filterwarnings("ignore")
     pd.options.display.float_format = '{:.4f}'.format
     pd.set_option('display.max_colwidth', 300)
     plt.style.use('seaborn-ticks')
     if font_path:
         if not os.path.isfile(font_path):
             import wget
             font_path = wget.download("https://itlubber.art/upload/matplot_chinese.ttf", 'matplot_chinese.ttf')
@@ -58,22 +63,59 @@
     #         plt.rcParams['font.family'] = font.name
     #         break
     
     plt.rcParams['axes.unicode_minus'] = False
     
     if seed:
         seed_everything(seed, freeze_torch=freeze_torch)
+    
+    if logger:
+        return init_logger(**kwargs)
 
 
 def load_pickle(file):
     return joblib.load(file)
 
 
 def save_pickle(obj, file):
     joblib.dump(obj, file)
+    
+    
+def germancredit():
+    '''
+    German Credit Data
+    ------
+    Credit data that classifies debtors described by a set of attributes as good or bad credit risks. See source link below for detailed information.
+    [source](https://archive.ics.uci.edu/ml/datasets/Statlog+(German+Credit+Data))
+    '''
+    from pandas.api.types import CategoricalDtype
+    
+    data = pd.read_csv(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'germancredit.csv'))
+    
+    cate_levels = {
+            "status_of_existing_checking_account": ['... < 0 DM', '0 <= ... < 200 DM', '... >= 200 DM / salary assignments for at least 1 year', 'no checking account'], 
+            "credit_history": ["no credits taken/ all credits paid back duly", "all credits at this bank paid back duly", "existing credits paid back duly till now", "delay in paying off in the past", "critical account/ other credits existing (not at this bank)"], 
+            "savings_account_and_bonds": ["... < 100 DM", "100 <= ... < 500 DM", "500 <= ... < 1000 DM", "... >= 1000 DM", "unknown/ no savings account"],
+            "present_employment_since": ["unemployed", "... < 1 year", "1 <= ... < 4 years", "4 <= ... < 7 years", "... >= 7 years"], 
+            "personal_status_and_sex": ["male : divorced/separated", "female : divorced/separated/married", "male : single", "male : married/widowed", "female : single"], 
+            "other_debtors_or_guarantors": ["none", "co-applicant", "guarantor"], 
+            "property": ["real estate",  "building society savings agreement/ life insurance",  "car or other, not in attribute Savings account/bonds",  "unknown / no property"],
+            "other_installment_plans": ["bank", "stores", "none"],
+            "housing": ["rent", "own", "for free"], 
+            "job": ["unemployed/ unskilled - non-resident", "unskilled - resident", "skilled employee / official", "management/ self-employed/ highly qualified employee/ officer"],
+            "telephone": ["none", "yes, registered under the customers name"], 
+            "foreign_worker": ["yes", "no"]}
+    
+    def cate_type(levels):
+        return CategoricalDtype(categories=levels, ordered=True)
+    
+    for i in cate_levels.keys():
+        data[i] = data[i].astype(cate_type(cate_levels[i]))
+    
+    return data
 
 
 def round_float(num, decimal = 4):
     if ~pd.isnull(num) and isinstance(num, float):
         return float(str(num).split(".")[0] + "." + str(num).split(".")[1][:decimal])
     else:
         return num
@@ -133,17 +175,17 @@
                 _combiner = toad.transform.Combiner()
                 _combiner.fit(data[[feature, target]].dropna(), target, method="chi", min_samples=min_bin_size, n_bins=max_n_bins, **kwargs)
                 rule = {feature: [s.tolist() if isinstance(s, np.ndarray) else s for s in _combiner.export()[feature]] + [[np.nan] if dtype == "categorical" else np.nan]}
         
             combiner.update(rule)
         else:
             if method in ["step", "quantile"]:
-                combiner.fit(x, y=target, method=method, n_bins=max_n_bins, **kwargs)
+                combiner.fit(data[[feature, target]], y=target, method=method, n_bins=max_n_bins, **kwargs)
             else:
-                combiner.fit(x, y=target, method=method, min_samples=min_bin_size, n_bins=max_n_bins, **kwargs)
+                combiner.fit(data[[feature, target]], y=target, method=method, min_samples=min_bin_size, n_bins=max_n_bins, **kwargs)
     
     if len(rules) > 0:
         if isinstance(rules, (list, np.ndarray)):
             combiner.update({feature: rules})
         else:
             combiner.update(rules)
 
@@ -316,15 +358,15 @@
         ax[0].set_ylabel('% of Total Bad / Good', fontsize=fontsize)
 
         ax[0].set_xlim((0, 1))
         ax[0].set_ylim((0, 1))
         
         handles1, labels1 = ax[0].get_legend_handles_labels()
 
-        ax[0].legend(loc='upper center', ncol=len(labels1), bbox_to_anchor=(0.5, 1.1), frameon=False)
+        # ax[0].legend(loc='upper center', ncol=len(labels1), bbox_to_anchor=(0.5, 1.1), frameon=False)
 
         # ROC 曲线
         fpr, tpr, thresholds = roc_curve(target, score)
         auc_value = toad.metrics.AUC(score, target)
 
         ax[1].plot(fpr, tpr, color=colors[0], label="ROC Curve")
         ax[1].stackplot(fpr, tpr, color=colors[0], alpha=0.25)
@@ -360,33 +402,35 @@
                 os.makedirs(os.path.dirname(save), exist_ok=True)
                 
             plt.savefig(save, dpi=240, format="png", bbox_inches="tight")
 
         return fig
 
 
-def score_hist(score, y_true, figsize=(15, 10), bins=30, save=None, labels=["good", "bad"], anchor=1.05, **kwargs):
+def hist_plot(score, y_true, figsize=(15, 10), bins=30, save=None, labels=["坏样本", "好样本"], anchor=1.1, fontsize=14, **kwargs):
     fig, ax = plt.subplots(1, 1, figsize = figsize)
     palette = sns.diverging_palette(340, 267, n=2, s=100, l=40)
 
     sns.histplot(
-                x=score, hue=y_true.replace({i: v for i, v in enumerate(labels)}), element="step", stat="density", bins=bins, common_bins=True, common_norm=True, palette=palette, ax=ax, **kwargs
+                x=score, hue=y_true.replace({i: v for i, v in enumerate(labels)}), element="step", stat="probability", bins=bins, common_bins=True, common_norm=True, palette=palette, ax=ax, **kwargs
             )
 
     sns.despine()
-
+    
     ax.spines['top'].set_color("#2639E9")
     ax.spines['bottom'].set_color("#2639E9")
     ax.spines['right'].set_color("#2639E9")
     ax.spines['left'].set_color("#2639E9")
 
-    ax.set_xlabel("score")
-    ax.set_ylabel("density")
+    ax.set_xlabel("评分分布", fontsize=fontsize)
+    ax.set_ylabel("样本占比", fontsize=fontsize)
+    
+    ax.yaxis.set_major_formatter(PercentFormatter(1))
     
-    ax.legend(["坏样本", "好样本"], loc='upper center', ncol=len(y_true.unique()), bbox_to_anchor=(0.5, anchor), frameon=False, fontsize=14)
+    ax.legend(labels[:y_true.nunique()], loc='upper center', ncol=y_true.nunique(), bbox_to_anchor=(0.5, anchor), frameon=False, fontsize=fontsize)
     
     fig.tight_layout()
 
     if save:
         if os.path.dirname(save) != "" and not os.path.exists(os.path.dirname(save)):
             os.makedirs(os.path.dirname(save), exist_ok=True)
         
@@ -438,7 +482,88 @@
         if os.path.dirname(save) != "" and not os.path.exists(os.path.dirname(save)):
                 os.makedirs(os.path.dirname(save), exist_ok=True)
 
         fig.savefig(save, dpi=240, format="png", bbox_inches="tight")
 
     if result:
         return df_psi[["评分区间", f"{labels[0]}样本数", f"{labels[0]}样本占比", f"{labels[0]}坏样本率", f"{labels[1]}样本数", f"{labels[1]}样本占比", f"{labels[1]}坏样本率", f"{labels[1]}% - {labels[0]}%", f"ln({labels[1]}% / {labels[0]}%)", "分档PSI值", "总体PSI值"]]
+
+
+def dataframe_plot(df, row_height=0.4, font_size=14, header_color='#2639E9', row_colors=['#dae3f3', 'w'], edge_color='w', bbox=[0, 0, 1, 1], header_columns=0, ax=None, save=None, **kwargs):
+    data = df.copy()
+    for col in data.select_dtypes('datetime'):
+        data[col] = data[col].dt.strftime("%Y-%m-%d")
+
+    for col in data.select_dtypes('float'):
+        data[col] = data[col].apply(lambda x: np.nan if pd.isnull(x) else round(x, 4))
+
+    cols_width = [max(data[col].apply(lambda x:len(str(x).encode())).max(), len(str(col).encode())) / 8. for col in data.columns]
+
+    if ax is None:
+        size = (sum(cols_width), (len(data) + 1) * row_height)
+        fig, ax = plt.subplots(figsize=size)
+        ax.axis('off')
+
+    mpl_table = ax.table(cellText=data.values, colWidths=cols_width, bbox=bbox, colLabels=data.columns, **kwargs)
+
+    mpl_table.auto_set_font_size(False)
+    mpl_table.set_fontsize(font_size)
+
+    for k, cell in  six.iteritems(mpl_table._cells):
+        cell.set_edgecolor(edge_color)
+        if k[0] == 0 or k[1] < header_columns:
+            cell.set_text_props(weight='bold', color='w')
+            cell.set_facecolor(header_color)
+        else:
+            cell.set_facecolor(row_colors[k[0]%len(row_colors)])
+
+    fig.tight_layout()
+    
+    if save:
+        if os.path.dirname(save) != "" and not os.path.exists(os.path.dirname(save)):
+            os.makedirs(os.path.dirname(save))
+
+        fig.savefig(save, dpi=240, format="png", bbox_inches="tight")
+
+    return fig
+
+
+def distribution_plot(df, date="date", target="target", save=None, figsize=(10, 6), colors=["#2639E9", "#F76E6C", "#FE7715"], freq="M", anchor=0.94, result=False):
+    temp = df.set_index(date).assign(
+        好样本=lambda x: (x[target] == 0).astype(int),
+        坏样本=lambda x: (x[target] == 1).astype(int),
+    ).resample(freq).agg({"好样本": sum, "坏样本": sum})
+    
+    temp.index = [i.strftime("%Y-%m-%d") for i in temp.index]
+
+    fig, ax1 = plt.subplots(1, 1, figsize=figsize)
+    temp.plot(kind='bar', stacked=True, ax=ax1, color=colors[:2], hatch="/", legend=False)
+    ax1.tick_params(axis='x', labelrotation=-90)
+    ax1.set(xlabel=None)
+    ax1.set_ylabel('样本数')
+    ax1.set_title('不同时点数据集样本分布情况\n\n')
+
+    ax2 = plt.twinx()
+    (temp["坏样本"] / temp.sum(axis=1)).plot(ax=ax2, color=colors[-1], style="--", linewidth=2, label="坏样本率")
+    # sns.despine()
+
+    handles1, labels1 = ax1.get_legend_handles_labels()
+    handles2, labels2 = ax2.get_legend_handles_labels()
+    fig.legend(handles1 + handles2, labels1 + labels2, loc='upper center', ncol=len(labels1 + labels2), bbox_to_anchor=(0.5, anchor), frameon=False)
+
+    fig.tight_layout()
+
+    if save:
+        if os.path.dirname(save) != "" and not os.path.exists(os.path.dirname(save)):
+            os.makedirs(os.path.dirname(save))
+
+        fig.savefig(save, dpi=240, format="png", bbox_inches="tight")
+
+    if result:
+        temp = temp.reset_index().rename(columns={date: "日期", "index": "日期", 0: "好样本", 1: "坏样本"})
+        temp["样本总数"] = temp["坏样本"] + temp["好样本"]
+        temp["样本占比"] = temp["样本总数"] / temp["样本总数"].sum()
+        temp["好样本占比"] = temp["好样本"] / temp["好样本"].sum()
+        temp["坏样本占比"] = temp["坏样本"] / temp["坏样本"].sum()
+        temp["坏样本率"] = temp["坏样本"] / temp["样本总数"]
+
+        return temp[["日期", "样本总数", "样本占比", "好样本", "好样本占比", "坏样本", "坏样本占比", "坏样本率"]]
```

### Comparing `scorecardpipeline-0.1.5/scorecardpipeline.egg-info/PKG-INFO` & `scorecardpipeline-0.1.6/scorecardpipeline.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecardpipeline
-Version: 0.1.5
+Version: 0.1.6
 Summary: 评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
 Home-page: https://github.com/itlubber/scorecardpipeline
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,25 +15,49 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# scorecardpipeline
+# 评分卡pipeline建模包
 
-评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，支持自定义模型报告输出
+`scorecardpipeline` 封装了 `toad`、`scorecardpy`、`optbinning` 等评分卡建模相关组件，`API` 风格与 `sklearn` 高度一致，支持 `pipeline` 式端到端评分卡建模、模型报告输出、导出 `PMML` 文件、超参数搜索等
 
 > 仓库地址：https://github.com/itlubber/scorecardpipeline
 > 
 > 博文地址：https://itlubber.art/archives/itlubber-scorecard-end2end
 > 
 > 微信公共号推文：https://mp.weixin.qq.com/s/eCTp4h0fau77xOgf_V28wQ
 > 
 > pipy包：https://pypi.org/project/scorecardpipeline/
+>
+> `scorecardpipeline` 教程：https://itlubber.art/upload/scorecardpipeline.html
+
+
+## 交流
+
+<table style="text-align:center !important;border=0;">
+    <tr>
+        <td>
+            <span>微信: itlubber</span>
+        </td>
+        <td>
+            <span>微信公众号: itlubber_art</span>
+        </td>
+    </tr>
+    <tr>
+        <td>
+            <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/>
+        </td>
+        <td>
+            <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/>
+        </td>
+    </tr>
+</table>
 
 
 ## 引言
 
 作为一名金融搬砖工作者，评分卡建模怎么也算是基操。本文主要对笔者日常使用的评分卡建模代码进行讲解，说明如何一步步从原始数据到最终评分卡模型以及如何解读产出的模型报告文档。
 
 本文所有代码已全部提交至笔者GITHUB公开仓库，各位看官按需取用，用完记得顺带给个star以鼓励笔者继续开源相关工作。
@@ -74,15 +98,22 @@
 + `processing` 中提供了数据前处理相关的方法：特征筛选方法（`FeatureSelection`、`StepwiseSelection`）、变量分箱方法（`Combiner`）、变量证据权重转换方法（`WOETransformer`），方法继承`sklearn.base`中的`BaseEstimator`和`TransformerMixin`，能够支持构建`pipeline`和超参数搜索
 + `model`中提供了基于`sklearn.linear_model.LogisticRegression`实现的`ITLubberLogisticRegression`，同时重写了`toad.ScoreCard`，以支持模型相关内容的输出
 + `excel_writer` 中提供了操作 `excel` 的一系列公共方法，包含设置条件格式、设置列宽、设置数字格式、插入指定样式的内容（`insert_value2sheet`）、插入图片数据（`insert_pic2sheet`）、插入`dataframe`数据内容（`insert_df2sheet`）、保存`excel`文件（`save`）等方法
 
 ### `scorecardpipeline` 安装
 
 ```bash
-pip install scorecardpipeline -i https://pypi.Python.org/simple/
+>> pip install scorecardpipeline -i https://pypi.Python.org/simple/
+
+Looking in indexes: https://pypi.Python.org/simple/
+Collecting scorecardpipeline
+  Downloading scorecardpipeline-0.1.5-py3-none-any.whl (36 kB)
+  ......
+Installing collected packages: sklearn-pandas, scorecardpy, sklearn2pmml, scorecardpipeline
+Successfully installed scorecardpipeline-0.1.5 scorecardpy-0.1.9.2 sklearn-pandas-2.2.0 sklearn2pmml-0.92.2
 ```
 
 
 ## 评分卡建模
 
 ### 数据准备
```

### Comparing `scorecardpipeline-0.1.5/setup.py` & `scorecardpipeline-0.1.6/setup.py`

 * *Files identical despite different names*

