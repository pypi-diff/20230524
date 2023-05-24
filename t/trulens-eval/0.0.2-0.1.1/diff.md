# Comparing `tmp/trulens_eval-0.0.2-py3-none-any.whl.zip` & `tmp/trulens_eval-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 61731 bytes, number of entries: 23
 -rw-r--r--  2.0 unx     4782 b- defN 23-May-23 22:00 trulens_eval/Example_TruBot.py
 -rw-r--r--  2.0 unx     2422 b- defN 23-May-23 22:00 trulens_eval/Leaderboard.py
--rw-r--r--  2.0 unx      406 b- defN 23-May-24 13:04 trulens_eval/__init__.py
+-rw-r--r--  2.0 unx      406 b- defN 23-May-24 13:07 trulens_eval/__init__.py
 -rw-r--r--  2.0 unx     5401 b- defN 23-May-23 22:00 trulens_eval/benchmark.py
 -rw-r--r--  2.0 unx     3443 b- defN 23-May-23 22:00 trulens_eval/feedback_prompts.py
 -rw-r--r--  2.0 unx      949 b- defN 23-May-23 22:00 trulens_eval/keys.py
 -rw-r--r--  2.0 unx     3325 b- defN 23-May-23 22:00 trulens_eval/provider_apis.py
 -rw-r--r--  2.0 unx    12097 b- defN 23-May-23 22:00 trulens_eval/slackbot.py
 -rw-r--r--  2.0 unx     5455 b- defN 23-May-23 22:00 trulens_eval/test_tru_chain.py
 -rw-r--r--  2.0 unx    10400 b- defN 23-May-23 22:00 trulens_eval/tru.py
@@ -14,12 +14,12 @@
 -rw-r--r--  2.0 unx    30260 b- defN 23-May-23 22:00 trulens_eval/tru_feedback.py
 -rw-r--r--  2.0 unx     3478 b- defN 23-May-23 22:00 trulens_eval/util.py
 -rw-r--r--  2.0 unx     8618 b- defN 23-May-23 22:00 trulens_eval/pages/Evaluations.py
 -rw-r--r--  2.0 unx     1322 b- defN 23-May-23 22:00 trulens_eval/pages/Progress.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 22:00 trulens_eval/pages/__init__.py
 -rw-r--r--  2.0 unx      929 b- defN 23-May-23 22:00 trulens_eval/ux/add_logo.py
 -rw-r--r--  2.0 unx    29567 b- defN 23-May-23 22:00 trulens_eval/ux/trulens_logo.svg
--rw-r--r--  2.0 unx    12696 b- defN 23-May-24 13:04 trulens_eval-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 13:04 trulens_eval-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-May-24 13:04 trulens_eval-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1909 b- defN 23-May-24 13:04 trulens_eval-0.0.2.dist-info/RECORD
+-rw-r--r--  2.0 unx    12696 b- defN 23-May-24 13:07 trulens_eval-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 13:07 trulens_eval-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-May-24 13:07 trulens_eval-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1909 b- defN 23-May-24 13:07 trulens_eval-0.1.1.dist-info/RECORD
 23 files, 187039 bytes uncompressed, 58651 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: trulens_eval/ux/add_logo.py
 Comment: 
 
 Filename: trulens_eval/ux/trulens_logo.svg
 Comment: 
 
-Filename: trulens_eval-0.0.2.dist-info/METADATA
+Filename: trulens_eval-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: trulens_eval-0.0.2.dist-info/WHEEL
+Filename: trulens_eval-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: trulens_eval-0.0.2.dist-info/top_level.txt
+Filename: trulens_eval-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: trulens_eval-0.0.2.dist-info/RECORD
+Filename: trulens_eval-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trulens_eval/__init__.py

```diff
@@ -1,12 +1,12 @@
 """
 Imports of most common parts of the library. Should include everything to get started.
 """
 
-__version__ = "0.0.2"
+__version__ = "0.1.1"
 
 from trulens_eval.tru_chain import TruChain
 from trulens_eval.tru_feedback import Feedback
 from trulens_eval.tru_feedback import OpenAI
 from trulens_eval.tru_feedback import Huggingface
 from trulens_eval.tru import Tru
```

## Comparing `trulens_eval-0.0.2.dist-info/METADATA` & `trulens_eval-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trulens-eval
-Version: 0.0.2
+Version: 0.1.1
 Summary: Library with langchain instrumentation to evaluate LLM based applications.
 Home-page: https://www.trulens.org
 Author: Truera Inc
 Author-email: all@truera.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

## Comparing `trulens_eval-0.0.2.dist-info/RECORD` & `trulens_eval-0.1.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 trulens_eval/Example_TruBot.py,sha256=vUPkVRoR0DBTIyp7UifHP6TdEQU0ppI6YGFAfLOulHw,4782
 trulens_eval/Leaderboard.py,sha256=AEPQhBQkqG11WqcQoxtyGIaGkXsNIBrsRBlu9nL8pGw,2422
-trulens_eval/__init__.py,sha256=6ptmVFd4MO_667tSrAz86Wgnv4i510U0WkckRhajxYg,406
+trulens_eval/__init__.py,sha256=hOsLHLysruE2YqhSgPWQ4Q3g5RCLZY84AzYnDcqKx_c,406
 trulens_eval/benchmark.py,sha256=LHVnqYTudYpOJ2iry7De41jLfO2FImZqprUlaUkOiKA,5401
 trulens_eval/feedback_prompts.py,sha256=DgW4_f_4g018tYNwca1D1taJhhdwaf2fDR9J8s0Upls,3443
 trulens_eval/keys.py,sha256=5HwSGVImj1742PRYo0iV9SC_92VO-3B3f7vH8503fd4,949
 trulens_eval/provider_apis.py,sha256=vSEzQmPvE2OuJvHZLqaqB_BLXyWODKd1PrZSY1wUVyk,3325
 trulens_eval/slackbot.py,sha256=L8rJnTapQV_gl_eCJFL-5SauS2zSWM4lMWggJ8g7AS4,12097
 trulens_eval/test_tru_chain.py,sha256=fEpZzCB1OaCfQ3AVe7yjShxxxFJrmR9E660o_47yZIU,5455
 trulens_eval/tru.py,sha256=gq6QVKkapVB21jTarU0uKZCo8Y4ldwDnk2yDMrRnIaA,10400
@@ -13,11 +13,11 @@
 trulens_eval/tru_feedback.py,sha256=yNCBzvsVUPqyaRsLzFqZn8IWPKrVep-IgZWZUfPAHgw,30260
 trulens_eval/util.py,sha256=0Ih7QhEcCz8cRfb9idaFc-nHe7cfop65KByIkcbfO84,3478
 trulens_eval/pages/Evaluations.py,sha256=6zxLRBVX4-iPxTkTa7LhPAGMz6e3hth3jmtmzwDA-9o,8618
 trulens_eval/pages/Progress.py,sha256=YztP-JVWCgdiuT5Qu8TCXQGliWOfGpx6DuAoyyeh0ZY,1322
 trulens_eval/pages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 trulens_eval/ux/add_logo.py,sha256=nlK4cdfbRiasTkMiP14akmvtxhSy7GLb3Wb_vd0m8GA,929
 trulens_eval/ux/trulens_logo.svg,sha256=92RLTgG0YDPEtZcQWWI7aXTYZAW4wAOAkIIgKUbTiW8,29567
-trulens_eval-0.0.2.dist-info/METADATA,sha256=DhGUFzmX5aH00NYVOk8Nb9PafQLjAber6zRRWrIDgSM,12696
-trulens_eval-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-trulens_eval-0.0.2.dist-info/top_level.txt,sha256=AKIBExe5S-v-TbsBrhe1ctF06PubKoYmWNS9rJ1Rb_o,13
-trulens_eval-0.0.2.dist-info/RECORD,,
+trulens_eval-0.1.1.dist-info/METADATA,sha256=LN4nKXN5zaatdd_5ZnVFfoNlDlZ0V0z7SdOgH6sRcXk,12696
+trulens_eval-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+trulens_eval-0.1.1.dist-info/top_level.txt,sha256=AKIBExe5S-v-TbsBrhe1ctF06PubKoYmWNS9rJ1Rb_o,13
+trulens_eval-0.1.1.dist-info/RECORD,,
```

