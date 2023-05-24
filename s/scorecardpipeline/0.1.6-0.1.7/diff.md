# Comparing `tmp/scorecardpipeline-0.1.6.tar.gz` & `tmp/scorecardpipeline-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecardpipeline-0.1.6.tar", last modified: Wed May 24 03:01:58 2023, max compression
+gzip compressed data, was "scorecardpipeline-0.1.7.tar", last modified: Wed May 24 08:23:41 2023, max compression
```

## Comparing `scorecardpipeline-0.1.6.tar` & `scorecardpipeline-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 03:01:58.945102 scorecardpipeline-0.1.6/
--rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-04 06:14:30.000000 scorecardpipeline-0.1.6/LICENSE
--rw-r--r--   0 lubberit   (501) staff       (20)    34395 2023-05-24 03:01:58.944735 scorecardpipeline-0.1.6/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)    33513 2023-05-24 02:51:13.000000 scorecardpipeline-0.1.6/README.md
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 03:01:58.942489 scorecardpipeline-0.1.6/scorecardpipeline/
--rw-r--r--   0 lubberit   (501) staff       (20)     1093 2023-05-24 03:01:33.000000 scorecardpipeline-0.1.6/scorecardpipeline/__init__.py
--rw-r--r--   0 lubberit   (501) staff       (20)    20443 2023-05-21 06:04:42.000000 scorecardpipeline-0.1.6/scorecardpipeline/excel_writer.py
--rw-r--r--   0 lubberit   (501) staff       (20)     1502 2023-05-23 14:15:12.000000 scorecardpipeline-0.1.6/scorecardpipeline/logger.py
--rw-r--r--   0 lubberit   (501) staff       (20)    19468 2023-05-23 16:28:40.000000 scorecardpipeline-0.1.6/scorecardpipeline/model.py
--rw-r--r--   0 lubberit   (501) staff       (20)    21542 2023-05-23 15:37:48.000000 scorecardpipeline-0.1.6/scorecardpipeline/processing.py
--rw-r--r--   0 lubberit   (501) staff       (20)    26374 2023-05-24 02:56:33.000000 scorecardpipeline-0.1.6/scorecardpipeline/utils.py
-drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 03:01:58.944089 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/
--rw-r--r--   0 lubberit   (501) staff       (20)    34395 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/PKG-INFO
--rw-r--r--   0 lubberit   (501) staff       (20)      408 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/SOURCES.txt
--rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/dependency_links.txt
--rw-r--r--   0 lubberit   (501) staff       (20)      205 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/requires.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       18 2023-05-24 03:01:58.000000 scorecardpipeline-0.1.6/scorecardpipeline.egg-info/top_level.txt
--rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-24 03:01:58.945199 scorecardpipeline-0.1.6/setup.cfg
--rw-r--r--   0 lubberit   (501) staff       (20)     1788 2023-05-21 07:08:23.000000 scorecardpipeline-0.1.6/setup.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 08:23:41.117275 scorecardpipeline-0.1.7/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1065 2023-05-04 06:14:30.000000 scorecardpipeline-0.1.7/LICENSE
+-rw-r--r--   0 lubberit   (501) staff       (20)    34150 2023-05-24 08:23:41.116935 scorecardpipeline-0.1.7/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)    33268 2023-05-24 08:12:04.000000 scorecardpipeline-0.1.7/README.md
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 08:23:41.114724 scorecardpipeline-0.1.7/scorecardpipeline/
+-rw-r--r--   0 lubberit   (501) staff       (20)     1093 2023-05-24 06:27:33.000000 scorecardpipeline-0.1.7/scorecardpipeline/__init__.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    20443 2023-05-21 06:04:42.000000 scorecardpipeline-0.1.7/scorecardpipeline/excel_writer.py
+-rw-r--r--   0 lubberit   (501) staff       (20)     1502 2023-05-23 14:15:12.000000 scorecardpipeline-0.1.7/scorecardpipeline/logger.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    19467 2023-05-24 05:58:24.000000 scorecardpipeline-0.1.7/scorecardpipeline/model.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    21542 2023-05-23 15:37:48.000000 scorecardpipeline-0.1.7/scorecardpipeline/processing.py
+-rw-r--r--   0 lubberit   (501) staff       (20)    29807 2023-05-24 06:29:22.000000 scorecardpipeline-0.1.7/scorecardpipeline/utils.py
+drwxr-xr-x   0 lubberit   (501) staff       (20)        0 2023-05-24 08:23:41.116372 scorecardpipeline-0.1.7/scorecardpipeline.egg-info/
+-rw-r--r--   0 lubberit   (501) staff       (20)    34150 2023-05-24 08:23:41.000000 scorecardpipeline-0.1.7/scorecardpipeline.egg-info/PKG-INFO
+-rw-r--r--   0 lubberit   (501) staff       (20)      408 2023-05-24 08:23:41.000000 scorecardpipeline-0.1.7/scorecardpipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)        1 2023-05-24 08:23:41.000000 scorecardpipeline-0.1.7/scorecardpipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)      205 2023-05-24 08:23:41.000000 scorecardpipeline-0.1.7/scorecardpipeline.egg-info/requires.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       18 2023-05-24 08:23:41.000000 scorecardpipeline-0.1.7/scorecardpipeline.egg-info/top_level.txt
+-rw-r--r--   0 lubberit   (501) staff       (20)       38 2023-05-24 08:23:41.117377 scorecardpipeline-0.1.7/setup.cfg
+-rw-r--r--   0 lubberit   (501) staff       (20)     1788 2023-05-21 07:08:23.000000 scorecardpipeline-0.1.7/setup.py
```

### Comparing `scorecardpipeline-0.1.6/LICENSE` & `scorecardpipeline-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.6/PKG-INFO` & `scorecardpipeline-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecardpipeline
-Version: 0.1.6
+Version: 0.1.7
 Summary: 评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
 Home-page: https://github.com/itlubber/scorecardpipeline
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -32,32 +32,18 @@
 > pipy包：https://pypi.org/project/scorecardpipeline/
 >
 > `scorecardpipeline` 教程：https://itlubber.art/upload/scorecardpipeline.html
 
 
 ## 交流
 
-<table style="text-align:center !important;border=0;">
-    <tr>
-        <td>
-            <span>微信: itlubber</span>
-        </td>
-        <td>
-            <span>微信公众号: itlubber_art</span>
-        </td>
-    </tr>
-    <tr>
-        <td>
-            <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/>
-        </td>
-        <td>
-            <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/>
-        </td>
-    </tr>
-</table>
+|  微信 |  微信公众号 |
+| :---: | :----: |
+| <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/> | <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/> |
+|  itlubber  | itlubber_art |
 
 
 ## 引言
 
 作为一名金融搬砖工作者，评分卡建模怎么也算是基操。本文主要对笔者日常使用的评分卡建模代码进行讲解，说明如何一步步从原始数据到最终评分卡模型以及如何解读产出的模型报告文档。
 
 本文所有代码已全部提交至笔者GITHUB公开仓库，各位看官按需取用，用完记得顺带给个star以鼓励笔者继续开源相关工作。
```

### Comparing `scorecardpipeline-0.1.6/README.md` & `scorecardpipeline-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,32 +11,18 @@
 > pipy包：https://pypi.org/project/scorecardpipeline/
 >
 > `scorecardpipeline` 教程：https://itlubber.art/upload/scorecardpipeline.html
 
 
 ## 交流
 
-<table style="text-align:center !important;border=0;">
-    <tr>
-        <td>
-            <span>微信: itlubber</span>
-        </td>
-        <td>
-            <span>微信公众号: itlubber_art</span>
-        </td>
-    </tr>
-    <tr>
-        <td>
-            <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/>
-        </td>
-        <td>
-            <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/>
-        </td>
-    </tr>
-</table>
+|  微信 |  微信公众号 |
+| :---: | :----: |
+| <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/> | <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/> |
+|  itlubber  | itlubber_art |
 
 
 ## 引言
 
 作为一名金融搬砖工作者，评分卡建模怎么也算是基操。本文主要对笔者日常使用的评分卡建模代码进行讲解，说明如何一步步从原始数据到最终评分卡模型以及如何解读产出的模型报告文档。
 
 本文所有代码已全部提交至笔者GITHUB公开仓库，各位看官按需取用，用完记得顺带给个star以鼓励笔者继续开源相关工作。
```

### Comparing `scorecardpipeline-0.1.6/scorecardpipeline/__init__.py` & `scorecardpipeline-0.1.7/scorecardpipeline/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .logger import init_logger
 from .utils import *
 from .processing import FeatureSelection, FeatureImportanceSelector, StepwiseSelection, Combiner, WOETransformer
 from .model import ITLubberLogisticRegression, ScoreCard
 from .excel_writer import ExcelWriter
 
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 __all__ = (
     __version__
     , FeatureSelection, FeatureImportanceSelector, StepwiseSelection, Combiner, WOETransformer
     , ITLubberLogisticRegression, ScoreCard
     , Pipeline, KS, AUC, PSI
     , init_logger, init_setting, load_pickle, save_pickle, germancredit
```

### Comparing `scorecardpipeline-0.1.6/scorecardpipeline/excel_writer.py` & `scorecardpipeline-0.1.7/scorecardpipeline/excel_writer.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.6/scorecardpipeline/logger.py` & `scorecardpipeline-0.1.7/scorecardpipeline/logger.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.6/scorecardpipeline/model.py` & `scorecardpipeline-0.1.7/scorecardpipeline/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
             x_tick_break = x_tick_break,
             show_plot = show_plot,
             return_distr_dat = return_distr_dat,
         )
     
     @staticmethod
     def score_hist(score, y_true, figsize=(15, 10), bins=20, save=None, **kwargs):
-        score_hist(score, y_true, figsize=figsize, bins=bins, save=save, **kwargs)
+        hist_plot(score, y_true, figsize=figsize, bins=bins, save=save, **kwargs)
     
     def _format_rule(self, rule, decimal = 4, **kwargs):
         bins = self.format_bins(rule['bins'])
         scores = np.around(rule['scores'], decimals = decimal).tolist()
         
         return dict(zip(bins, scores))
```

### Comparing `scorecardpipeline-0.1.6/scorecardpipeline/processing.py` & `scorecardpipeline-0.1.7/scorecardpipeline/processing.py`

 * *Files identical despite different names*

### Comparing `scorecardpipeline-0.1.6/scorecardpipeline/utils.py` & `scorecardpipeline-0.1.7/scorecardpipeline/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -185,16 +185,15 @@
     
     if len(rules) > 0:
         if isinstance(rules, (list, np.ndarray)):
             combiner.update({feature: rules})
         else:
             combiner.update(rules)
 
-    feature_bin = combiner.export()[feature]
-    feature_bin_dict = feature_bins(np.array(feature_bin))
+    feature_bin_dict = feature_bins(np.array(combiner[feature]))
     
     df_bin = combiner.transform(data[[feature, target]], labels=False)
     
     table = df_bin[[feature, target]].groupby([feature, target]).agg(len).unstack()
     table.columns.name = None
     table = table.rename(columns = {0 : '好样本数', 1 : '坏样本数'}).fillna(0)
     if "好样本数" not in table.columns:
@@ -435,61 +434,112 @@
             os.makedirs(os.path.dirname(save), exist_ok=True)
         
         plt.savefig(save, dpi=240, format="png", bbox_inches="tight")
     
     return fig
 
 
-def psi_plot(expected, actual, labels=["预期", "实际"], save=None, colors=["#2639E9", "#F76E6C", "#FE7715"], figsize=(15, 8), anchor=0.94, width=0.35, result=False):
-    expected = expected.rename(columns={"分箱": "评分区间", "样本总数": f"{labels[0]}样本数", "样本占比": f"{labels[0]}样本占比", "坏样本率": f"{labels[0]}坏样本率"})
-    actual = actual.rename(columns={"分箱": "评分区间", "样本总数": f"{labels[1]}样本数", "样本占比": f"{labels[1]}样本占比", "坏样本率": f"{labels[1]}坏样本率"})
-    df_psi = expected.merge(actual, on="评分区间", how="outer").replace(np.nan, 0)
+def psi_plot(expected, actual, labels=["预期", "实际"], save=None, colors=["#2639E9", "#F76E6C", "#FE7715"], figsize=(15, 8), anchor=0.94, width=0.35, result=False, plot=True, max_len=None):
+    expected = expected.rename(columns={"样本总数": f"{labels[0]}样本数", "样本占比": f"{labels[0]}样本占比", "坏样本率": f"{labels[0]}坏样本率"})
+    actual = actual.rename(columns={"样本总数": f"{labels[1]}样本数", "样本占比": f"{labels[1]}样本占比", "坏样本率": f"{labels[1]}坏样本率"})
+    df_psi = expected.merge(actual, on="分箱", how="outer").replace(np.nan, 0)
     df_psi[f"{labels[1]}% - {labels[0]}%"] = df_psi[f"{labels[1]}样本占比"] - df_psi[f"{labels[0]}样本占比"]
     df_psi[f"ln({labels[1]}% / {labels[0]}%)"] = np.log(df_psi[f"{labels[1]}样本占比"] / df_psi[f"{labels[0]}样本占比"])
     df_psi["分档PSI值"] = (df_psi[f"{labels[1]}% - {labels[0]}%"] * df_psi[f"ln({labels[1]}% / {labels[0]}%)"])
     df_psi = df_psi.fillna(0).replace(np.inf, 0).replace(-np.inf, 0)
     df_psi["总体PSI值"] = df_psi["分档PSI值"].sum()
     
-    x = df_psi['评分区间']
-    x_indexes = np.arange(len(x))
-    fig, ax1 = plt.subplots(figsize=figsize)
+    if plot:
+        x = df_psi['分箱'].apply(lambda l: l if max_len is None else str(l)[:max_len] + "...")
+        x_indexes = np.arange(len(x))
+        fig, ax1 = plt.subplots(figsize=figsize)
+
+        ax1.bar(x_indexes - width / 2, df_psi[f'{labels[0]}样本占比'], width, label=f'{labels[0]}样本占比', color=colors[0], hatch="/")
+        ax1.bar(x_indexes + width / 2, df_psi[f'{labels[1]}样本占比'], width, label=f'{labels[1]}样本占比', color=colors[1], hatch="\\")
+
+        ax1.set_ylabel('样本占比: 分箱内样本数 / 样本总数')
+        ax1.set_xticks(x_indexes)
+        ax1.set_xticklabels(x)
+        ax1.tick_params(axis='x', labelrotation=90)
+
+        ax2 = ax1.twinx()
+        ax2.plot(df_psi["分箱"], df_psi[f"{labels[0]}坏样本率"], color=colors[0], label=f"{labels[0]}坏样本率", linestyle=(5, (10, 3)))
+        ax2.plot(df_psi["分箱"], df_psi[f"{labels[1]}坏样本率"], color=colors[1], label=f"{labels[1]}坏样本率", linestyle=(5, (10, 3)))
 
-    ax1.bar(x_indexes - width / 2, df_psi[f'{labels[0]}样本占比'], width, label=f'{labels[0]}样本占比', color=colors[0], hatch="/")
-    ax1.bar(x_indexes + width / 2, df_psi[f'{labels[1]}样本占比'], width, label=f'{labels[1]}样本占比', color=colors[1], hatch="\\")
+        ax2.scatter(df_psi["分箱"], df_psi[f"{labels[0]}坏样本率"], marker=".")
+        ax2.scatter(df_psi["分箱"], df_psi[f"{labels[1]}坏样本率"], marker=".")
 
-    ax1.set_ylabel('样本占比: 评分区间内样本数 / 样本总数')
-    ax1.set_xticks(x_indexes)
-    ax1.set_xticklabels(x)
-    ax1.tick_params(axis='x', labelrotation=90)
+        ax2.set_ylabel('坏样本率: 坏样本数 / 样本总数')
+        
+        fig.suptitle(f"{labels[0]} vs {labels[1]} 群体稳定性指数(PSI): {df_psi['分档PSI值'].sum():.4f}\n\n")
 
-    ax2 = ax1.twinx()
-    ax2.plot(df_psi["评分区间"], df_psi[f"{labels[0]}坏样本率"], color=colors[0], label=f"{labels[0]}坏样本率", linestyle=(5, (10, 3)))
-    ax2.plot(df_psi["评分区间"], df_psi[f"{labels[1]}坏样本率"], color=colors[1], label=f"{labels[1]}坏样本率", linestyle=(5, (10, 3)))
+        handles1, labels1 = ax1.get_legend_handles_labels()
+        handles2, labels2 = ax2.get_legend_handles_labels()
+        fig.legend(handles1 + handles2, labels1 + labels2, loc='upper center', ncol=len(labels1 + labels2), bbox_to_anchor=(0.5, anchor), frameon=False)
 
-    ax2.scatter(df_psi["评分区间"], df_psi[f"{labels[0]}坏样本率"], marker=".")
-    ax2.scatter(df_psi["评分区间"], df_psi[f"{labels[1]}坏样本率"], marker=".")
+        fig.tight_layout()
 
-    ax2.set_ylabel('坏样本率: 坏样本数 / 样本总数')
-    
-    fig.suptitle(f"{labels[0]} vs {labels[1]} 群体稳定性指数(PSI): {df_psi['分档PSI值'].sum():.4f}\n\n")
+        if save:
+            if os.path.dirname(save) != "" and not os.path.exists(os.path.dirname(save)):
+                    os.makedirs(os.path.dirname(save), exist_ok=True)
 
-    handles1, labels1 = ax1.get_legend_handles_labels()
-    handles2, labels2 = ax2.get_legend_handles_labels()
-    fig.legend(handles1 + handles2, labels1 + labels2, loc='upper center', ncol=len(labels1 + labels2), bbox_to_anchor=(0.5, anchor), frameon=False)
+            fig.savefig(save, dpi=240, format="png", bbox_inches="tight")
 
-    fig.tight_layout()
+    if result:
+        return df_psi[["分箱", f"{labels[0]}样本数", f"{labels[0]}样本占比", f"{labels[0]}坏样本率", f"{labels[1]}样本数", f"{labels[1]}样本占比", f"{labels[1]}坏样本率", f"{labels[1]}% - {labels[0]}%", f"ln({labels[1]}% / {labels[0]}%)", "分档PSI值", "总体PSI值"]]
 
-    if save:
-        if os.path.dirname(save) != "" and not os.path.exists(os.path.dirname(save)):
-                os.makedirs(os.path.dirname(save), exist_ok=True)
 
-        fig.savefig(save, dpi=240, format="png", bbox_inches="tight")
+def csi_plot(expected, actual, score_bins, labels=["预期", "实际"], save=None, colors=["#2639E9", "#F76E6C", "#FE7715"], figsize=(15, 8), anchor=0.94, width=0.35, result=False, plot=True, max_len=None):
+    expected = expected.rename(columns={"样本总数": f"{labels[0]}样本数", "样本占比": f"{labels[0]}样本占比", "坏样本率": f"{labels[0]}坏样本率"})
+    actual = actual.rename(columns={"样本总数": f"{labels[1]}样本数", "样本占比": f"{labels[1]}样本占比", "坏样本率": f"{labels[1]}坏样本率"})
+    df_csi = expected.merge(actual, on="分箱", how="outer").replace(np.nan, 0)
+    df_csi[f"{labels[1]}% - {labels[0]}%"] = df_csi[f"{labels[1]}样本占比"] - df_csi[f"{labels[0]}样本占比"]
+    df_csi = df_csi.merge(pd.DataFrame({"分箱": feature_bins(score_bins["bins"]).values(), "对应分数": score_bins["scores"]}), on="分箱", how="left").replace(np.nan, 0)
+    df_csi["分档CSI值"] = (df_csi[f"{labels[1]}% - {labels[0]}%"] * df_csi["对应分数"])
+    df_csi = df_csi.fillna(0).replace(np.inf, 0).replace(-np.inf, 0)
+    df_csi["总体CSI值"] = df_csi["分档CSI值"].sum()
+    
+    if plot:
+        x = df_csi['分箱'].apply(lambda l: l if max_len is None else str(l)[:max_len] + "...")
+        x_indexes = np.arange(len(x))
+        fig, ax1 = plt.subplots(figsize=figsize)
+
+        ax1.bar(x_indexes - width / 2, df_csi[f'{labels[0]}样本占比'], width, label=f'{labels[0]}样本占比', color=colors[0], hatch="/")
+        ax1.bar(x_indexes + width / 2, df_csi[f'{labels[1]}样本占比'], width, label=f'{labels[1]}样本占比', color=colors[1], hatch="\\")
+
+        ax1.set_ylabel('样本占比: 分箱内样本数 / 样本总数')
+        ax1.set_xticks(x_indexes)
+        ax1.set_xticklabels(x)
+        ax1.tick_params(axis='x', labelrotation=90)
+
+        ax2 = ax1.twinx()
+        ax2.plot(df_csi["分箱"], df_csi[f"{labels[0]}坏样本率"], color=colors[0], label=f"{labels[0]}坏样本率", linestyle=(5, (10, 3)))
+        ax2.plot(df_csi["分箱"], df_csi[f"{labels[1]}坏样本率"], color=colors[1], label=f"{labels[1]}坏样本率", linestyle=(5, (10, 3)))
+
+        ax2.scatter(df_csi["分箱"], df_csi[f"{labels[0]}坏样本率"], marker=".")
+        ax2.scatter(df_csi["分箱"], df_csi[f"{labels[1]}坏样本率"], marker=".")
+
+        ax2.set_ylabel('坏样本率: 坏样本数 / 样本总数')
+        
+        fig.suptitle(f"{labels[0]} vs {labels[1]} 特征稳定性指标(CSI): {df_csi['分档CSI值'].sum():.4f}\n\n")
+
+        handles1, labels1 = ax1.get_legend_handles_labels()
+        handles2, labels2 = ax2.get_legend_handles_labels()
+        fig.legend(handles1 + handles2, labels1 + labels2, loc='upper center', ncol=len(labels1 + labels2), bbox_to_anchor=(0.5, anchor), frameon=False)
+
+        fig.tight_layout()
+
+        if save:
+            if os.path.dirname(save) != "" and not os.path.exists(os.path.dirname(save)):
+                    os.makedirs(os.path.dirname(save), exist_ok=True)
 
+            fig.savefig(save, dpi=240, format="png", bbox_inches="tight")
+    
     if result:
-        return df_psi[["评分区间", f"{labels[0]}样本数", f"{labels[0]}样本占比", f"{labels[0]}坏样本率", f"{labels[1]}样本数", f"{labels[1]}样本占比", f"{labels[1]}坏样本率", f"{labels[1]}% - {labels[0]}%", f"ln({labels[1]}% / {labels[0]}%)", "分档PSI值", "总体PSI值"]]
+        return df_csi[["分箱", f"{labels[0]}样本数", f"{labels[0]}样本占比", f"{labels[0]}坏样本率", f"{labels[1]}样本数", f"{labels[1]}样本占比", f"{labels[1]}坏样本率", f"{labels[1]}% - {labels[0]}%", "对应分数", "分档CSI值", "总体CSI值"]]
 
 
 def dataframe_plot(df, row_height=0.4, font_size=14, header_color='#2639E9', row_colors=['#dae3f3', 'w'], edge_color='w', bbox=[0, 0, 1, 1], header_columns=0, ax=None, save=None, **kwargs):
     data = df.copy()
     for col in data.select_dtypes('datetime'):
         data[col] = data[col].dt.strftime("%Y-%m-%d")
```

### Comparing `scorecardpipeline-0.1.6/scorecardpipeline.egg-info/PKG-INFO` & `scorecardpipeline-0.1.7/scorecardpipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecardpipeline
-Version: 0.1.6
+Version: 0.1.7
 Summary: 评分卡pipeline建模包，封装toad、scorecardpy、optbinning等评分卡建模相关组件，API风格与sklearn高度一致，自持自定义模型报告输出
 Home-page: https://github.com/itlubber/scorecardpipeline
 Author: itlubber
 Author-email: itlubber@qq.com
 License: MIT
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
@@ -32,32 +32,18 @@
 > pipy包：https://pypi.org/project/scorecardpipeline/
 >
 > `scorecardpipeline` 教程：https://itlubber.art/upload/scorecardpipeline.html
 
 
 ## 交流
 
-<table style="text-align:center !important;border=0;">
-    <tr>
-        <td>
-            <span>微信: itlubber</span>
-        </td>
-        <td>
-            <span>微信公众号: itlubber_art</span>
-        </td>
-    </tr>
-    <tr>
-        <td>
-            <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/>
-        </td>
-        <td>
-            <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/>
-        </td>
-    </tr>
-</table>
+|  微信 |  微信公众号 |
+| :---: | :----: |
+| <img src="https://itlubber.art//upload/itlubber.png" alt="itlubber.png" width="50%" border=0/> | <img src="https://itlubber.art//upload/itlubber_art.png" alt="itlubber_art.png" width="50%" border=0/> |
+|  itlubber  | itlubber_art |
 
 
 ## 引言
 
 作为一名金融搬砖工作者，评分卡建模怎么也算是基操。本文主要对笔者日常使用的评分卡建模代码进行讲解，说明如何一步步从原始数据到最终评分卡模型以及如何解读产出的模型报告文档。
 
 本文所有代码已全部提交至笔者GITHUB公开仓库，各位看官按需取用，用完记得顺带给个star以鼓励笔者继续开源相关工作。
```

### Comparing `scorecardpipeline-0.1.6/setup.py` & `scorecardpipeline-0.1.7/setup.py`

 * *Files identical despite different names*

