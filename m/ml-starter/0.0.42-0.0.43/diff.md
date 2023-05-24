# Comparing `tmp/ml-starter-0.0.42.tar.gz` & `tmp/ml-starter-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.42.tar", last modified: Wed May 24 17:09:27 2023, max compression
+gzip compressed data, was "ml-starter-0.0.43.tar", last modified: Wed May 24 20:25:15 2023, max compression
```

## Comparing `ml-starter-0.0.42.tar` & `ml-starter-0.0.43.tar`

### file list

```diff
@@ -1,167 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.145402 ml-starter-0.0.42/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 17:09:11.000000 ml-starter-0.0.42/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 17:09:11.000000 ml-starter-0.0.42/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 17:09:27.145402 ml-starter-0.0.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-24 17:09:11.000000 ml-starter-0.0.42/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.105401 ml-starter-0.0.42/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.105401 ml-starter-0.0.42/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.109401 ml-starter-0.0.42/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.109401 ml-starter-0.0.42/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.113401 ml-starter-0.0.42/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.113401 ml-starter-0.0.42/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.113401 ml-starter-0.0.42/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.121401 ml-starter-0.0.42/ml/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41279 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60788 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.121401 ml-starter-0.0.42/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.125401 ml-starter-0.0.42/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.125401 ml-starter-0.0.42/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.129402 ml-starter-0.0.42/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.129402 ml-starter-0.0.42/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.129402 ml-starter-0.0.42/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.129402 ml-starter-0.0.42/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.133401 ml-starter-0.0.42/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.133401 ml-starter-0.0.42/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.137401 ml-starter-0.0.42/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.145402 ml-starter-0.0.42/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.145402 ml-starter-0.0.42/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.145402 ml-starter-0.0.42/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-24 17:09:11.000000 ml-starter-0.0.42/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 17:09:11.000000 ml-starter-0.0.42/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-24 17:09:11.000000 ml-starter-0.0.42/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 17:09:11.000000 ml-starter-0.0.42/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 17:09:27.145402 ml-starter-0.0.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-24 17:09:11.000000 ml-starter-0.0.42/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.535650 ml-starter-0.0.43/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 20:25:01.000000 ml-starter-0.0.43/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 20:25:01.000000 ml-starter-0.0.43/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 20:25:15.535650 ml-starter-0.0.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-24 20:25:01.000000 ml-starter-0.0.43/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.507649 ml-starter-0.0.43/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.507649 ml-starter-0.0.43/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.507649 ml-starter-0.0.43/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.511649 ml-starter-0.0.43/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.511649 ml-starter-0.0.43/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.511649 ml-starter-0.0.43/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.515649 ml-starter-0.0.43/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.515649 ml-starter-0.0.43/ml/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16701 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40856 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26329 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60524 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/models/pretrained/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.515649 ml-starter-0.0.43/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.519650 ml-starter-0.0.43/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.519650 ml-starter-0.0.43/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.519650 ml-starter-0.0.43/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.523650 ml-starter-0.0.43/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.523650 ml-starter-0.0.43/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.523650 ml-starter-0.0.43/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.523650 ml-starter-0.0.43/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.523650 ml-starter-0.0.43/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.527650 ml-starter-0.0.43/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.531650 ml-starter-0.0.43/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.535650 ml-starter-0.0.43/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-24 20:25:01.000000 ml-starter-0.0.43/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:25:15.535650 ml-starter-0.0.43/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 20:25:15.000000 ml-starter-0.0.43/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-24 20:25:15.000000 ml-starter-0.0.43/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:25:15.000000 ml-starter-0.0.43/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 20:25:15.000000 ml-starter-0.0.43/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-24 20:25:15.000000 ml-starter-0.0.43/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-24 20:25:01.000000 ml-starter-0.0.43/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 20:25:01.000000 ml-starter-0.0.43/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-24 20:25:01.000000 ml-starter-0.0.43/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 20:25:01.000000 ml-starter-0.0.43/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 20:25:15.535650 ml-starter-0.0.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-24 20:25:01.000000 ml-starter-0.0.43/setup.py
```

### Comparing `ml-starter-0.0.42/LICENSE` & `ml-starter-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/PKG-INFO` & `ml-starter-0.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.42
+Version: 0.0.43
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.42/README.md` & `ml-starter-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/api.py` & `ml-starter-0.0.43/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/core/common_types.py` & `ml-starter-0.0.43/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/core/config.py` & `ml-starter-0.0.43/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/core/env.py` & `ml-starter-0.0.43/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/core/registry.py` & `ml-starter-0.0.43/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/core/state.py` & `ml-starter-0.0.43/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/launchers/base.py` & `ml-starter-0.0.43/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/launchers/mp.py` & `ml-starter-0.0.43/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/launchers/slurm.py` & `ml-starter-0.0.43/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/launchers/torchrun.py` & `ml-starter-0.0.43/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/loggers/base.py` & `ml-starter-0.0.43/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/loggers/meter.py` & `ml-starter-0.0.43/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/loggers/multi.py` & `ml-starter-0.0.43/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/loggers/stdout.py` & `ml-starter-0.0.43/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/loggers/tensorboard.py` & `ml-starter-0.0.43/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/lr_schedulers/base.py` & `ml-starter-0.0.43/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/lr_schedulers/constant.py` & `ml-starter-0.0.43/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.43/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.43/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/lr_schedulers/linear.py` & `ml-starter-0.0.43/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.43/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.43/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/activations.py` & `ml-starter-0.0.43/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/base.py` & `ml-starter-0.0.43/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/embeddings.py` & `ml-starter-0.0.43/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/init.py` & `ml-starter-0.0.43/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/kmeans.py` & `ml-starter-0.0.43/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/lora.py` & `ml-starter-0.0.43/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/norms.py` & `ml-starter-0.0.43/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/parallel.py` & `ml-starter-0.0.43/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/pretrained/blip.py` & `ml-starter-0.0.43/ml/models/pretrained/blip.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,44 +5,44 @@
 
 .. highlight:: python
 .. code-block:: python
 
     from ml.models.pretrained.blip import pretrained_blip
 
     model = pretrained_blip("ViT-B")
+    predictor = model.predictor()
 
     image = PIL.Image.open(image_path)
+    embedding = predictor.predict(image)
 
 The choices for the model key are:
 
 - ``ViT-B``
 - ``ViT-B-CapFilt``
 - ``ViT-L``
 """
 
 import argparse
 import logging
 from dataclasses import dataclass
-from pathlib import Path
 from typing import Literal, Sequence, Union, get_args
 
 import numpy as np
 import PIL.Image
 import torch
 import torch.nn.functional as F
 import torchvision.transforms.functional as V
 from omegaconf import MISSING
 from torch import Tensor, nn
-from torchvision.datasets.utils import download_url
 
 from ml.core.config import conf_field
-from ml.core.env import get_model_dir
 from ml.models.activations import ActivationType, get_activation
 from ml.models.init import init_
 from ml.models.norms import NormType, get_norm_linear
+from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
@@ -98,14 +98,30 @@
     img_size=224,
     patch_size=16,
     embed_dim=768,
     depth=12,
     num_heads=12,
 )
 
+VIT_BASE_CAPFILT = ViTParams(
+    img_size=224,
+    patch_size=16,
+    embed_dim=768,
+    depth=12,
+    num_heads=12,
+)
+
+VIT_LARGE = ViTParams(
+    img_size=224,
+    patch_size=16,
+    embed_dim=1024,
+    depth=16,
+    num_heads=24,
+)
+
 
 PRETRAINED_MODEL_SIZES: dict[PretrainedBlipKey, ModelParams] = {
     # ViT-B models
     "ViT-B": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_base.pth",
         vit=VIT_BASE,
     ),
@@ -114,42 +130,50 @@
         vit=VIT_BASE,
     ),
     "ViT-B-Flickr30k": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_base_retrieval_flickr.pth",
         vit=VIT_BASE,
     ),
     "ViT-B-VQA": ModelParams(
-        url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_vqa.pth", vit=VIT_BASE
+        url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_vqa.pth",
+        vit=VIT_BASE,
     ),
     "ViT-B-NLVR2": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_base_nlvr.pth",
         vit=VIT_BASE,
     ),
     # ViT-B-CapFilt models
     "ViT-B-CapFilt": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_base_capfilt_large.pth",
+        vit=VIT_BASE_CAPFILT,
     ),
     "ViT-B-CapFilt-Coco": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_base_caption_capfilt_large.pth",
+        vit=VIT_BASE_CAPFILT,
     ),
     "ViT-B-CapFilt-VQA": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_base_vqa_capfilt_large.pth",
+        vit=VIT_BASE_CAPFILT,
     ),
     # ViT-L models
     "ViT-L": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_large.pth",
+        vit=VIT_LARGE,
     ),
     "ViT-L-Coco-Retrieval": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_large_retrieval_coco.pth",
+        vit=VIT_LARGE,
     ),
     "ViT-L-Flickr30k": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_large_retrieval_flickr.pth",
+        vit=VIT_LARGE,
     ),
     "ViT-L-Coco-Captioning": ModelParams(
         url="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_large_caption.pth",
+        vit=VIT_LARGE,
     ),
 }
 
 
 class PatchEmbed(nn.Module):
     """Gets patch embeddings for an input image.
 
@@ -415,22 +439,16 @@
             x = self.get_input_image(image)
             x = self.model(x.unsqueeze(0)).squeeze(0)[0]
         return x
 
 
 def pretrained_blip(key: PretrainedBlipKey, *, device: BaseDevice | None = None) -> Blip:
     device = AutoDevice.detect_device() if device is None else device
-    ckpt_path = get_model_dir() / "BLIP" / f"{key}.pth"
     model_args = PRETRAINED_MODEL_SIZES[key]
-
-    # Downloads the checkpoint, if it doesn't exist.
-    if not ckpt_path.is_file():
-        ckpt_path.parent.mkdir(exist_ok=True)
-        download_url(model_args.url, str(ckpt_path.parent), ckpt_path.name)
-        assert ckpt_path.is_file(), f"Failed to download {ckpt_path}"
+    ckpt_path = ensure_downloaded(model_args.url, "BLIP", f"{key}.pth")
 
     with Timer("loading model checkpoint", spinner=True):
         ckpt = torch.load(ckpt_path, map_location="cpu")["model"]
         # Filters jut the visual encoder weights.
         ckpt = {k: v for k, v in ckpt.items() if k.startswith("visual_encoder.")}
 
     with Timer("building model skeleton", spinner=True), init_empty_weights():
@@ -453,18 +471,15 @@
     parser.add_argument("key", type=str, choices=get_args(PretrainedBlipKey))
     args = parser.parse_args()
 
     configure_logging()
 
     # Gets an image of a peach from Wikipedia.
     peach_url = "https://upload.wikimedia.org/wikipedia/commons/9/9e/Autumn_Red_peaches.jpg"
-    img_path = Path("/tmp/peach.jpg")
-    if not img_path.exists():
-        download_url(peach_url, str(img_path.parent), filename=img_path.name)
-
+    img_path = ensure_downloaded(peach_url, "peach.jpg", is_tmp=True)
     image = PIL.Image.open(img_path)
 
     model = pretrained_blip(args.key)
     predictor = model.predictor()
 
     # Outputs the embedding for a given image.
     embedding = predictor.predict(image)
```

### Comparing `ml-starter-0.0.42/ml/models/pretrained/clip.py` & `ml-starter-0.0.43/ml/models/pretrained/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,16 @@
 
 import numpy as np
 import PIL.Image
 import torch
 import torch.nn.functional as F
 import torchvision
 from torch import Tensor, nn
-from torchvision.datasets.utils import download_url
 
-from ml.core.env import get_model_dir
+from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.logging import configure_logging
 
 logger = logging.getLogger(__name__)
 
 URL_PREFIX = "https://openaipublic.azureedge.net/clip/models"
@@ -186,18 +185,15 @@
         return text
 
     return _clean
 
 
 class ClipTokenizer:
     def __init__(self) -> None:
-        vocab_file_name = "CLIP_vocabulary.txt.gz"
-        bpe_path = get_model_dir() / vocab_file_name
-        if not bpe_path.exists():
-            download_url(CLIP_VOCABULARY, get_model_dir(), filename=vocab_file_name)
+        bpe_path = ensure_downloaded(CLIP_VOCABULARY, "CLIP", "CLIP_vocabulary.txt.gz")
         self.byte_encoder = bytes_to_unicode()
         self.byte_decoder = {v: k for k, v in self.byte_encoder.items()}
         merges_unzipped = gzip.open(bpe_path).read().decode("utf-8").split("\n")
         merges_unzipped = merges_unzipped[1 : 49152 - 256 - 2 + 1]
         merges = [tuple(merge.split()) for merge in merges_unzipped]
         vocab = list(bytes_to_unicode().values())
         vocab = vocab + [v + "</w>" for v in vocab]
@@ -1049,34 +1045,27 @@
         return model
 
 
 def get_pretrained_path(key: PretrainedClipSize) -> Path:
     if key not in PRETRAINED_MODELS:
         raise KeyError(f"Invalid CLIP model key {key}; choices are {list(PRETRAINED_MODELS.keys())}")
     model_url = PRETRAINED_MODELS[key]
-    save_path = (get_model_dir() / f"CLIP_{key}").resolve()
-    filename = "ckpt.pt"
-    filepath = save_path / filename
-    if not filepath.exists():
-        download_url(model_url, str(save_path), filename=filename)
-    return filepath
+    return ensure_downloaded(model_url, "CLIP", f"{key}_ckpt.pt")
 
 
 def test_pretrained_model() -> None:
     parser = argparse.ArgumentParser(description="Tests a pretraiend CLIP model")
     parser.add_argument("key", type=str, choices=get_args(PretrainedClipSize))
     args = parser.parse_args()
 
     configure_logging()
 
     # Gets an image of a peach from Wikipedia.
     peach_url = "https://upload.wikimedia.org/wikipedia/commons/9/9e/Autumn_Red_peaches.jpg"
-    img_path = Path("/tmp/peach.jpg")
-    if not img_path.exists():
-        download_url(peach_url, str(img_path.parent), filename=img_path.name)
+    img_path = ensure_downloaded(peach_url, "peach.jpg", is_tmp=True)
 
     peach_img = PIL.Image.open(img_path)
     pos_desc = "A picture of an Autumn Red peach"
     neg_desc = "An Instagram photo of a cute puppy"
 
     # Loads the JIT'd model and the regular model.
     auto_device = AutoDevice.detect_device()
```

### Comparing `ml-starter-0.0.42/ml/models/pretrained/hubert.py` & `ml-starter-0.0.43/ml/models/pretrained/hubert.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,17 @@
 from dataclasses import dataclass
 from typing import Literal, cast, get_args
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
-from torchvision.datasets.utils import download_url
 
-from ml.core.env import get_model_dir
 from ml.models.activations import ActivationType, get_activation
-from ml.utils.data import check_sha256
+from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
 
 PretrainedHubertSize = Literal["base", "large", "extra_large"]
 
@@ -523,21 +521,17 @@
 ) -> Hubert:
     with Timer("building empty model", spinner=True):
         model = Hubert(config)
 
     # Loads the model weights.
     if load_weights:
         model_fname = f"{size}.bin"
-        model_path = get_model_dir() / "hubert" / model_fname
 
         with Timer("downloading checkpoint", spinner=True):
-            if not model_path.is_file() or not check_sha256(model_path, sha256):
-                model_path.parent.mkdir(exist_ok=True)
-                download_url(ckpt_url, str(model_path.parent), model_fname)
-                assert model_path.is_file(), f"Failed to download {model_path}"
+            model_path = ensure_downloaded(ckpt_url, "hubert", model_fname, sha256=sha256)
 
         with Timer("loading checkpoint", spinner=True):
             ckpt = torch.load(model_path, map_location="cpu")
             if remove_prefix:
                 ckpt = {k[len(remove_prefix) :]: v for k, v in ckpt.items()}
             ckpt = {k: v for k, v in ckpt.items() if k not in EXCLUDE_KEYS}
             model.load_state_dict(ckpt)
```

### Comparing `ml-starter-0.0.42/ml/models/pretrained/llama.py` & `ml-starter-0.0.43/ml/models/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/models/pretrained/rwkv.py` & `ml-starter-0.0.43/ml/models/pretrained/rwkv.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,16 @@
 import logging
 from dataclasses import dataclass
 from typing import Any, Iterator, Literal, Sequence, get_args
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
-from torchvision.datasets.utils import download_url
 
-from ml.core.env import get_model_dir
+from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
@@ -269,29 +268,22 @@
         return probs, states_out
 
     def predictor(self) -> "RwkvPredictor":
         return RwkvPredictor(self)
 
 
 def get_tokenizer() -> Any:
-    tokenizer_path = get_model_dir() / "RWKV" / "tokenizer.json"
-
     try:
         from tokenizers import Tokenizer
 
     except ImportError:
         raise ImportError("Please install tokenizers with: `pip install tokenizers`")
 
-    # Downloads the model if it doesn't exist
-    if not tokenizer_path.is_file():
-        tokenizer_path.parent.mkdir(exist_ok=True)
-        download_url(TOKENIZER_URL, str(tokenizer_path.parent), tokenizer_path.name)
-        assert tokenizer_path.is_file(), f"Failed to download {tokenizer_path}"
-
-    return Tokenizer.from_file(str(tokenizer_path.resolve()))
+    tokenizer_path = ensure_downloaded(TOKENIZER_URL, "RWKV", "tokenizer.json")
+    return Tokenizer.from_file(str(tokenizer_path))
 
 
 class RwkvPredictor:
     def __init__(self, rwkv_model: Rwkv, *, device: BaseDevice | None = None) -> None:
         """Provides an API for sampling from the RWKV model.
 
         Args:
@@ -345,22 +337,16 @@
                 break
             if i < max_len - 1:
                 probs, state = self.model(self.device.tensor_to(torch.tensor([[token]])), state)
 
 
 def pretrained_rwkv(key: PretrainedRwkvKey, *, device: BaseDevice | None = None) -> Rwkv:
     device = AutoDevice.detect_device() if device is None else device
-    ckpt_path = get_model_dir() / "RWKV" / f"{key}.pth"
     model_args = PRETRAINED_MODEL_SIZES[key]
-
-    # Downloads the model if it doesn't exist
-    if not ckpt_path.is_file():
-        ckpt_path.parent.mkdir(exist_ok=True)
-        download_url(model_args.url, str(ckpt_path.parent), ckpt_path.name)
-        assert ckpt_path.is_file(), f"Failed to download {ckpt_path}"
+    ckpt_path = ensure_downloaded(model_args.url, "RWKV", f"{key}.pth")
 
     with Timer("loading model checkpoint", spinner=True):
         ckpt = torch.load(ckpt_path, map_location="cpu")
 
     with Timer("building model skeleton", spinner=True), init_empty_weights():
         model = Rwkv(model_args.emb_dim, 50277, model_args.num_layers)
```

### Comparing `ml-starter-0.0.42/ml/models/pretrained/sam.py` & `ml-starter-0.0.43/ml/models/pretrained/sam.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 from typing import Any, Literal, Type, cast, get_args
 
 import numpy as np
 import PIL.Image
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
-from torchvision.datasets.utils import download_url
 from torchvision.transforms.functional import resize, to_pil_image
 
-from ml.core.env import get_model_dir
+from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.logging import configure_logging
 
 PretrainedSamSize = Literal["ViT-H", "ViT-L", "ViT-B"]
 
 ImageFormat = Literal["RGB", "BGR"]
@@ -1490,19 +1489,15 @@
         self.input_w = None
 
 
 def get_pretrained_path(key: PretrainedSamSize) -> Path:
     if key not in PRETRAINED_MODELS:
         raise KeyError(f"Invalid CLIP model key {key}; choices are {list(PRETRAINED_MODELS.keys())}")
     model_url = PRETRAINED_MODELS[key].url
-    save_path = (get_model_dir() / f"SAM_{key}").resolve()
-    filename = "ckpt.pt"
-    filepath = save_path / filename
-    if not filepath.exists():
-        download_url(model_url, str(save_path), filename=filename)
+    filepath = ensure_downloaded(model_url, "SAM", f"{key}_ckpt.pt")
     return filepath
 
 
 def pretrained_sam(key: PretrainedSamSize, *, skip_weights: bool = False) -> Sam:
     config = PRETRAINED_MODELS[key]
 
     prompt_embed_dim = 256
@@ -1560,17 +1555,15 @@
     parser.add_argument("key", type=str, choices=get_args(PretrainedSamSize))
     args = parser.parse_args()
 
     configure_logging()
 
     # Gets an image of a peach from Wikipedia.
     peach_url = "https://upload.wikimedia.org/wikipedia/commons/9/9e/Autumn_Red_peaches.jpg"
-    img_path = Path("/tmp/peach.jpg")
-    if not img_path.exists():
-        download_url(peach_url, str(img_path.parent), filename=img_path.name)
+    img_path = ensure_downloaded(peach_url, "peach.jpg", is_tmp=True)
 
     model = pretrained_sam(cast(PretrainedSamSize, args.key))
     predictor = model.predictor()
 
     peach_img = PIL.Image.open(img_path)
     predictor.set_image(np.array(peach_img))
```

### Comparing `ml-starter-0.0.42/ml/optimizers/adam.py` & `ml-starter-0.0.43/ml/optimizers/adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     foreach: bool = conf_field(False, help="Whether to use the foreach variant of the optimizer")
     capturable: bool = conf_field(False, help="Whether to use capturable AdamW pathway")
     differentiable: bool = conf_field(False, help="Whether to use differentiable AdamW")
     fused: bool = conf_field(False, help="Whether to use the fused optimizer")
 
 
 @register_optimizer("adam", AdamOptimizerConfig)
-class AdamOptimizer(BaseOptimizer[AdamOptimizerConfig]):
+class AdamOptimizer(BaseOptimizer[AdamOptimizerConfig, Adam]):
     def get(self, model: nn.Module) -> Adam:
         b1, b2 = self.config.betas
 
         return Adam(
             model.parameters(),
             lr=self.config.lr,
             betas=(b1, b2),
```

### Comparing `ml-starter-0.0.42/ml/optimizers/adan.py` & `ml-starter-0.0.43/ml/optimizers/adan.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     lr: float = conf_field(1e-3, help="Learning rate")
     betas: tuple[float, float, float] = conf_field((0.1, 0.1, 0.001), help="Beta coefficients")
     eps: float = conf_field(1e-4, help="Epsilon term")
     weight_decay: float = conf_field(1e-5, help="Weight decay regularization to use")
 
 
 @register_optimizer("adan", AdanOptimizerConfig)
-class AdanOptimizer(BaseOptimizer[AdanOptimizerConfig]):
+class AdanOptimizer(BaseOptimizer[AdanOptimizerConfig, Adan]):
     def get(self, model: nn.Module) -> Adan:
         b1, b2, b3 = self.config.betas
 
         return Adan(
             model.parameters(),
             lr=self.config.lr,
             betas=(b1, b2, b3),
```

### Comparing `ml-starter-0.0.42/ml/optimizers/sgd.py` & `ml-starter-0.0.43/ml/optimizers/sgd.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     momentum: float = conf_field(0.0, help="Momentum term for all parameters")
     dampening: float = conf_field(0.0, help="Dampening for momentum")
     nesterov: bool = conf_field(False, help="Enable Nesterov momentum")
     weight_decay: float = conf_field(1e-5, help="Weight decay regularization to use")
 
 
 @register_optimizer("sgd", SGDOptimizerConfig)
-class SGDOptimizer(BaseOptimizer[SGDOptimizerConfig]):
+class SGDOptimizer(BaseOptimizer[SGDOptimizerConfig, SGD]):
     def get(self, model: nn.Module) -> SGD:
         return SGD(
             model.parameters(),
             lr=self.config.lr,
             momentum=self.config.momentum,
             dampening=self.config.dampening,
             nesterov=self.config.nesterov,
```

### Comparing `ml-starter-0.0.42/ml/optimizers/shampoo.py` & `ml-starter-0.0.43/ml/optimizers/shampoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     momentum: float = conf_field(0.0, help="Momentum")
     weight_decay: float = conf_field(0.0, help="Weight decay")
     epsilon: float = conf_field(1e-4, help="Epsilon")
     update_freq: int = conf_field(1, help="Update frequency")
 
 
 @register_optimizer("shampoo", ShampooOptimizerConfig)
-class ShampooOptimizer(BaseOptimizer[ShampooOptimizerConfig]):
+class ShampooOptimizer(BaseOptimizer[ShampooOptimizerConfig, Shampoo]):
     def get(self, model: nn.Module) -> Shampoo:
         return Shampoo(
             model.parameters(),
             lr=self.config.lr,
             momentum=self.config.momentum,
             weight_decay=self.config.weight_decay,
             epsilon=self.config.epsilon,
```

### Comparing `ml-starter-0.0.42/ml/scripts/cli.py` & `ml-starter-0.0.43/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/scripts/stage.py` & `ml-starter-0.0.43/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/scripts/train.py` & `ml-starter-0.0.43/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/base.py` & `ml-starter-0.0.43/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.43/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.43/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/collate.py` & `ml-starter-0.0.43/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.43/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.43/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.43/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.43/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.43/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/utils.py` & `ml-starter-0.0.43/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.43/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/environments/base.py` & `ml-starter-0.0.43/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/environments/utils.py` & `ml-starter-0.0.43/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/environments/worker.py` & `ml-starter-0.0.43/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/losses/reduce.py` & `ml-starter-0.0.43/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/rl/base.py` & `ml-starter-0.0.43/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/rl/replay.py` & `ml-starter-0.0.43/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/tasks/sl/base.py` & `ml-starter-0.0.43/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/base.py` & `ml-starter-0.0.43/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/learning.py` & `ml-starter-0.0.43/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/compile.py` & `ml-starter-0.0.43/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.43/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.43/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.43/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.43/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.43/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.43/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.43/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.43/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.43/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/rl.py` & `ml-starter-0.0.43/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/trainers/sl.py` & `ml-starter-0.0.43/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/argparse.py` & `ml-starter-0.0.43/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/atomic.py` & `ml-starter-0.0.43/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/augmentation.py` & `ml-starter-0.0.43/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/caching.py` & `ml-starter-0.0.43/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/checkpoint.py` & `ml-starter-0.0.43/ml/utils/checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from torchvision.datasets.utils import download_url
 
 from ml.core.env import get_model_dir
 from ml.core.registry import Objects, register_model, register_task
 from ml.models.base import BaseModel
 from ml.tasks.base import BaseTask
 from ml.trainers.base import BaseTrainer
+from ml.utils.data import check_md5, check_sha256
 from ml.utils.device.auto import AutoDevice
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
@@ -36,14 +37,15 @@
     Returns:
         The instantiated objects.
     """
     if isinstance(config, (str, Path)):
         config = cast(DictConfig, OmegaConf.load(config))
     elif isinstance(config, dict):
         config = OmegaConf.create(config)
+    Objects.update_config(config)
     Objects.resolve_config(config)
     return Objects.parse_raw_config(config)
 
 
 def get_checkpoint_path(trainer: BaseTrainer, config_path: str | Path, ckpt_path: str | Path | None) -> Path:
     if ckpt_path is not None:
         ckpt_path = Path(ckpt_path)
@@ -141,31 +143,45 @@
             device = AutoDevice.detect_device()
             device.module_to(model)
             device.module_to(task)
 
     return model, task
 
 
-def ensure_downloaded(url: str, dname: str, fname: str, md5: str | None = None) -> Path:
-    """Ensures that a URL has been downloaded to a given directory.
+def ensure_downloaded(
+    url: str,
+    *dnames: str,
+    md5: str | None = None,
+    sha256: str | None = None,
+    is_tmp: bool = False,
+) -> Path:
+    """Ensures that a checkpoint URL has been downloaded.
+
+    This basically just provides a nice way of organizing pre-trained models,
+    by saving them to a consistent location.
 
     Args:
         url: The URL to download.
-        dname: The directory to download to (note that this is relative to the
-            model directory).
-        fname: The filename to download to.
+        dnames: The directory to download to (note that this is relative to the
+            model directory). The final name should be the file name
         md5: The MD5 hash of the file, if known.
+        sha256: The SHA256 hash of the file, if known.
+        is_tmp: If set, use ``tmp/`` instead of ``get_model_dir()``
 
     Returns:
         The path to the downloaded file.
     """
-    (root := get_model_dir() / dname).mkdir(parents=True, exist_ok=True)
-    filepath = root / fname
-    if not filepath.exists():
+    assert len(dnames) >= 1, "Must provide at least 1 directory name"
+    filepath = Path("tmp") if is_tmp else get_model_dir()
+    for dname in dnames:
+        filepath = filepath / dname
+    (root := filepath.parent).mkdir(parents=True, exist_ok=True)
+    if not filepath.exists() or not check_sha256(filepath, sha256) or not check_md5(filepath, md5):
         download_url(url, root=root, filename=filepath.name, md5=md5)
+        assert filepath.is_file(), f"Failed to download {url} to {filepath}"
     return filepath
 
 
 def get_state_dict_prefix(state_dict: Mapping[str, T], prefix: str) -> Mapping[str, T]:
     """Gets the state dict with a prefix removed from the keys.
 
     Args:
```

### Comparing `ml-starter-0.0.42/ml/utils/cli.py` & `ml-starter-0.0.43/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/colors.py` & `ml-starter-0.0.43/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/config.py` & `ml-starter-0.0.43/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/data.py` & `ml-starter-0.0.43/ml/utils/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,47 +117,53 @@
             return valid_items
         case "test":
             return test_items
         case _:
             raise ValueError(f"Invalid phase: {phase}")
 
 
-def check_md5(file_path: str | Path, hash_str: str, chunk_size: int = 2**16, use_tqdm: bool = True) -> bool:
+def check_md5(file_path: str | Path, hash_str: str | None, chunk_size: int = 2**16, use_tqdm: bool = True) -> bool:
     """Checks the MD5 of the downloaded file.
 
     Args:
         file_path: Path to the downloaded file.
-        hash_str: Expected MD5 of the file.
+        hash_str: Expected MD5 of the file; if None, return True.
         chunk_size: Size of the chunks to read from the file.
         use_tqdm: Whether to use tqdm to show progress.
 
     Returns:
         True if the MD5 matches, False otherwise.
     """
+    if hash_str is None:
+        return True
+
     md5 = hashlib.md5()
 
     with open(file_path, "rb") as f:
         for chunk in tqdm.tqdm(iter(lambda: f.read(chunk_size), b""), disable=not use_tqdm, delay=1.0):
             md5.update(chunk)
 
     return md5.hexdigest() == hash_str
 
 
-def check_sha256(file_path: str | Path, hash_str: str, chunk_size: int = 2**16, use_tqdm: bool = True) -> bool:
+def check_sha256(file_path: str | Path, hash_str: str | None, chunk_size: int = 2**16, use_tqdm: bool = True) -> bool:
     """Checks the SHA256 of the downloaded file.
 
     Args:
         file_path: Path to the downloaded file.
-        hash_str: Expected SHA256 of the file.
+        hash_str: Expected SHA256 of the file; if None, return True.
         chunk_size: Size of the chunks to read from the file.
         use_tqdm: Whether to use tqdm to show progress.
 
     Returns:
         True if the SHA256 matches, False otherwise.
     """
+    if hash_str is None:
+        return True
+
     sha256 = hashlib.sha256()
 
     with open(file_path, "rb") as f:
         for chunk in tqdm.tqdm(iter(lambda: f.read(chunk_size), b""), disable=not use_tqdm, delay=1.0):
             sha256.update(chunk)
 
     return sha256.hexdigest() == hash_str
```

### Comparing `ml-starter-0.0.42/ml/utils/datetime.py` & `ml-starter-0.0.43/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/device/auto.py` & `ml-starter-0.0.43/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/device/base.py` & `ml-starter-0.0.43/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/device/cpu.py` & `ml-starter-0.0.43/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/device/gpu.py` & `ml-starter-0.0.43/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/device/metal.py` & `ml-starter-0.0.43/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/distributed.py` & `ml-starter-0.0.43/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/image.py` & `ml-starter-0.0.43/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/large_models.py` & `ml-starter-0.0.43/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/logging.py` & `ml-starter-0.0.43/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/meter.py` & `ml-starter-0.0.43/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/parallel.py` & `ml-starter-0.0.43/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/staging.py` & `ml-starter-0.0.43/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/timer.py` & `ml-starter-0.0.43/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/torch_distributed.py` & `ml-starter-0.0.43/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml/utils/video.py` & `ml-starter-0.0.43/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.43/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.42
+Version: 0.0.43
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.42/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.43/ml_starter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 ml/models/pretrained/rwkv.py
 ml/models/pretrained/sam.py
 ml/optimizers/__init__.py
 ml/optimizers/adam.py
 ml/optimizers/adamw.py
 ml/optimizers/adan.py
 ml/optimizers/base.py
+ml/optimizers/common.py
 ml/optimizers/sgd.py
 ml/optimizers/shampoo.py
 ml/optimizers/types.py
 ml/scripts/__init__.py
 ml/scripts/cli.py
 ml/scripts/launch.py
 ml/scripts/resolve.py
```

### Comparing `ml-starter-0.0.42/pyproject.toml` & `ml-starter-0.0.43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.42/setup.py` & `ml-starter-0.0.43/setup.py`

 * *Files identical despite different names*

