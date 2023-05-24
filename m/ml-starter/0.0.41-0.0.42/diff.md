# Comparing `tmp/ml-starter-0.0.41.tar.gz` & `tmp/ml-starter-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.41.tar", last modified: Sat May 20 07:38:31 2023, max compression
+gzip compressed data, was "ml-starter-0.0.42.tar", last modified: Wed May 24 17:09:27 2023, max compression
```

## Comparing `ml-starter-0.0.41.tar` & `ml-starter-0.0.42.tar`

### file list

```diff
@@ -1,166 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.974888 ml-starter-0.0.41/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 07:38:18.000000 ml-starter-0.0.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 07:38:18.000000 ml-starter-0.0.41/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-20 07:38:31.974888 ml-starter-0.0.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-20 07:38:18.000000 ml-starter-0.0.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.942887 ml-starter-0.0.41/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.942887 ml-starter-0.0.41/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.946887 ml-starter-0.0.41/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.950887 ml-starter-0.0.41/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.950887 ml-starter-0.0.41/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.950887 ml-starter-0.0.41/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.954887 ml-starter-0.0.41/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.954887 ml-starter-0.0.41/ml/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41279 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60788 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.954887 ml-starter-0.0.41/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.958887 ml-starter-0.0.41/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.958887 ml-starter-0.0.41/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.958887 ml-starter-0.0.41/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.966888 ml-starter-0.0.41/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.970888 ml-starter-0.0.41/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.970888 ml-starter-0.0.41/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.974888 ml-starter-0.0.41/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-20 07:38:18.000000 ml-starter-0.0.41/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 07:38:18.000000 ml-starter-0.0.41/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-20 07:38:18.000000 ml-starter-0.0.41/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 07:38:18.000000 ml-starter-0.0.41/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 07:38:31.974888 ml-starter-0.0.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-20 07:38:18.000000 ml-starter-0.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.145402 ml-starter-0.0.42/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 17:09:11.000000 ml-starter-0.0.42/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 17:09:11.000000 ml-starter-0.0.42/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 17:09:27.145402 ml-starter-0.0.42/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-24 17:09:11.000000 ml-starter-0.0.42/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.105401 ml-starter-0.0.42/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.105401 ml-starter-0.0.42/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.109401 ml-starter-0.0.42/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.109401 ml-starter-0.0.42/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.113401 ml-starter-0.0.42/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.113401 ml-starter-0.0.42/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.113401 ml-starter-0.0.42/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.121401 ml-starter-0.0.42/ml/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41279 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60788 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/models/pretrained/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.121401 ml-starter-0.0.42/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.125401 ml-starter-0.0.42/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.125401 ml-starter-0.0.42/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.129402 ml-starter-0.0.42/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.129402 ml-starter-0.0.42/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.129402 ml-starter-0.0.42/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.129402 ml-starter-0.0.42/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.133401 ml-starter-0.0.42/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.133401 ml-starter-0.0.42/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.137401 ml-starter-0.0.42/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.145402 ml-starter-0.0.42/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.145402 ml-starter-0.0.42/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-24 17:09:11.000000 ml-starter-0.0.42/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:09:27.145402 ml-starter-0.0.42/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-24 17:09:27.000000 ml-starter-0.0.42/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-24 17:09:11.000000 ml-starter-0.0.42/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 17:09:11.000000 ml-starter-0.0.42/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-24 17:09:11.000000 ml-starter-0.0.42/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 17:09:11.000000 ml-starter-0.0.42/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 17:09:27.145402 ml-starter-0.0.42/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-24 17:09:11.000000 ml-starter-0.0.42/setup.py
```

### Comparing `ml-starter-0.0.41/LICENSE` & `ml-starter-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/PKG-INFO` & `ml-starter-0.0.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.41
+Version: 0.0.42
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.41/README.md` & `ml-starter-0.0.42/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/api.py` & `ml-starter-0.0.42/ml/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     "AsyncEnvironmentWorker",
     "AsyncIterableDataset",
     "AsyncWorkerPool",
     "atomic_save",
     "AutoDevice",
     "BaseDevice",
     "BaseEnvironmentWorker",
+    "BaseLearningTrainer",
+    "BaseLearningTrainerConfig",
     "BaseLRScheduler",
     "BaseLRSchedulerConfig",
     "BaseModel",
     "BaseModelConfig",
     "BaseOptimizer",
     "BaseOptimizerConfig",
     "BaseTask",
@@ -47,14 +49,15 @@
     "collate",
     "CollateMode",
     "colorize",
     "ColumnParallelLinear",
     "conf_field",
     "configure_logging",
     "DictIndex",
+    "ensure_downloaded",
     "Environment",
     "format_timedelta",
     "from_args",
     "get_activation",
     "get_args",
     "get_cache_dir",
     "get_data_dir",
@@ -76,14 +79,15 @@
     "get_norm_3d",
     "get_norm_linear",
     "get_positional_embeddings",
     "get_random_port",
     "get_rank_optional",
     "get_rank",
     "get_run_dir",
+    "get_state_dict_prefix",
     "get_type_from_string",
     "get_worker_info",
     "get_world_size_optional",
     "get_world_size",
     "init_",
     "init_and_run",
     "init_dist",
@@ -164,16 +168,14 @@
     "SyncEnvironmentWorker",
     "SyncWorkerPool",
     "test_dataset",
     "test_environment",
     "timeout",
     "Timer",
     "transforms",
-    "VanillaTrainer",
-    "VanillaTrainerConfig",
     "VideoFileDataset",
     "WorkerPool",
     "write_gif",
     "write_video",
 ]
 
 from ml.core.common_types import Batch, Loss, Output
@@ -241,22 +243,22 @@
     SyncWorkerPool,
     WorkerPool,
 )
 from ml.tasks.losses.reduce import cast_reduce_type, reduce
 from ml.tasks.rl.base import ReinforcementLearningTask, ReinforcementLearningTaskConfig
 from ml.tasks.sl.base import SupervisedLearningTask, SupervisedLearningTaskConfig
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig
+from ml.trainers.learning import BaseLearningTrainer, BaseLearningTrainerConfig
 from ml.trainers.rl import ReinforcementLearningTrainer, ReinforcementLearningTrainerConfig
 from ml.trainers.sl import SupervisedLearningTrainer, SupervisedLearningTrainerConfig
-from ml.trainers.vanilla import VanillaTrainer, VanillaTrainerConfig
 from ml.utils.argparse import from_args, get_args, get_type_from_string
 from ml.utils.atomic import atomic_save, open_atomic
 from ml.utils.augmentation import get_image_mask
 from ml.utils.caching import DictIndex, cached_object
-from ml.utils.checkpoint import instantiate_config, load_model_and_task
+from ml.utils.checkpoint import ensure_downloaded, get_state_dict_prefix, instantiate_config, load_model_and_task
 from ml.utils.checks import assert_no_nans
 from ml.utils.colors import colorize
 from ml.utils.data import check_md5, check_sha256, get_dataset_split_for_phase, get_dataset_splits, get_worker_info
 from ml.utils.datetime import format_timedelta
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.distributed import (
```

### Comparing `ml-starter-0.0.41/ml/core/common_types.py` & `ml-starter-0.0.42/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/core/config.py` & `ml-starter-0.0.42/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/core/env.py` & `ml-starter-0.0.42/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/core/registry.py` & `ml-starter-0.0.42/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/core/state.py` & `ml-starter-0.0.42/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/launchers/base.py` & `ml-starter-0.0.42/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/launchers/mp.py` & `ml-starter-0.0.42/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/launchers/slurm.py` & `ml-starter-0.0.42/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/launchers/torchrun.py` & `ml-starter-0.0.42/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/loggers/base.py` & `ml-starter-0.0.42/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/loggers/meter.py` & `ml-starter-0.0.42/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/loggers/multi.py` & `ml-starter-0.0.42/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/loggers/stdout.py` & `ml-starter-0.0.42/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/loggers/tensorboard.py` & `ml-starter-0.0.42/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/lr_schedulers/base.py` & `ml-starter-0.0.42/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/lr_schedulers/constant.py` & `ml-starter-0.0.42/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.42/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.42/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/lr_schedulers/linear.py` & `ml-starter-0.0.42/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.42/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.42/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/activations.py` & `ml-starter-0.0.42/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/base.py` & `ml-starter-0.0.42/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/embeddings.py` & `ml-starter-0.0.42/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/init.py` & `ml-starter-0.0.42/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/lora.py` & `ml-starter-0.0.42/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/norms.py` & `ml-starter-0.0.42/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/parallel.py` & `ml-starter-0.0.42/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/pretrained/blip.py` & `ml-starter-0.0.42/ml/models/pretrained/blip.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/pretrained/clip.py` & `ml-starter-0.0.42/ml/models/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/pretrained/hubert.py` & `ml-starter-0.0.42/ml/models/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/pretrained/llama.py` & `ml-starter-0.0.42/ml/models/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/pretrained/rwkv.py` & `ml-starter-0.0.42/ml/models/pretrained/rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/models/pretrained/sam.py` & `ml-starter-0.0.42/ml/models/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/optimizers/adam.py` & `ml-starter-0.0.42/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/optimizers/adamw.py` & `ml-starter-0.0.42/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/optimizers/adan.py` & `ml-starter-0.0.42/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/optimizers/base.py` & `ml-starter-0.0.42/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/optimizers/sgd.py` & `ml-starter-0.0.42/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/optimizers/shampoo.py` & `ml-starter-0.0.42/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/scripts/cli.py` & `ml-starter-0.0.42/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/scripts/stage.py` & `ml-starter-0.0.42/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/scripts/train.py` & `ml-starter-0.0.42/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/base.py` & `ml-starter-0.0.42/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.42/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.42/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/collate.py` & `ml-starter-0.0.42/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.42/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.42/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.42/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.42/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.42/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/utils.py` & `ml-starter-0.0.42/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.42/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/environments/base.py` & `ml-starter-0.0.42/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/environments/utils.py` & `ml-starter-0.0.42/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/environments/worker.py` & `ml-starter-0.0.42/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/losses/reduce.py` & `ml-starter-0.0.42/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/rl/base.py` & `ml-starter-0.0.42/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/rl/replay.py` & `ml-starter-0.0.42/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/tasks/sl/base.py` & `ml-starter-0.0.42/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/base.py` & `ml-starter-0.0.42/ml/trainers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
             logger.info("Saved config to %s", config_path)
 
 
 @dataclass
 class CheckpointConfig:
     save_every_n_steps: int | None = conf_field(None, help="Save a checkpoint every N steps")
     only_save_most_recent: bool = conf_field(False, help="Only keep the most recent checkpoint")
+    load_from_ckpt_path: str | None = conf_field(None, help="If set, load initial model weights from this path")
 
 
 @dataclass
 class BaseTrainerConfig(BaseConfig):
     """Defines the base config for all trainers."""
 
     exp_name: str = conf_field(II("exp_name:null"), help="The name of the training job")
```

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/compile.py` & `ml-starter-0.0.42/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.42/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.42/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.42/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.42/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.42/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.42/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.42/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.42/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.42/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/trainers/rl.py` & `ml-starter-0.0.42/ml/trainers/rl.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from ml.core.config import conf_field
 from ml.core.registry import register_trainer
 from ml.lr_schedulers.base import BaseLRScheduler
 from ml.optimizers.base import BaseOptimizer
 from ml.tasks.rl.base import ReinforcementLearningTask
 from ml.trainers.base import ModelT
-from ml.trainers.vanilla import TrainingFinishedError, VanillaTrainer, VanillaTrainerConfig
+from ml.trainers.learning import BaseLearningTrainer, BaseLearningTrainerConfig, TrainingFinishedError
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class SamplingConfig:
@@ -36,28 +36,28 @@
     min_trajectory_length: int = conf_field(1, help="Minimum length of trajectories to collect")
     max_trajectory_length: int | None = conf_field(None, help="Maximum length of trajectories to collect")
     force_sync: bool = conf_field(False, help="Force workers to run in sync mode rather than async mode")
     optimal: bool = conf_field(False, help="Whether to choose the optimal action or sample from the policy")
 
 
 @dataclass
-class ReinforcementLearningTrainerConfig(VanillaTrainerConfig):
+class ReinforcementLearningTrainerConfig(BaseLearningTrainerConfig):
     sampling: SamplingConfig = conf_field(SamplingConfig())
 
 
 ReinforcementLearningTrainerConfigT = TypeVar(
     "ReinforcementLearningTrainerConfigT",
     bound=ReinforcementLearningTrainerConfig,
 )
 ReinforcementLearningTaskT = TypeVar("ReinforcementLearningTaskT", bound=ReinforcementLearningTask)
 
 
 @register_trainer("rl", ReinforcementLearningTrainerConfig)
 class ReinforcementLearningTrainer(
-    VanillaTrainer[ReinforcementLearningTrainerConfigT, ModelT, ReinforcementLearningTaskT],
+    BaseLearningTrainer[ReinforcementLearningTrainerConfigT, ModelT, ReinforcementLearningTaskT],
     Generic[ReinforcementLearningTrainerConfigT, ModelT, ReinforcementLearningTaskT],
 ):
     def train(
         self,
         model: ModelT,
         task: ReinforcementLearningTaskT,
         optimizer: BaseOptimizer,
```

### Comparing `ml-starter-0.0.41/ml/trainers/sl.py` & `ml-starter-0.0.42/ml/trainers/sl.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ml.core.config import conf_field
 from ml.core.registry import register_trainer
 from ml.core.state import State
 from ml.lr_schedulers.base import BaseLRScheduler
 from ml.optimizers.base import BaseOptimizer
 from ml.tasks.sl.base import SupervisedLearningTask
 from ml.trainers.base import ModelT
-from ml.trainers.vanilla import TrainingFinishedError, VanillaTrainer, VanillaTrainerConfig
+from ml.trainers.learning import BaseLearningTrainer, BaseLearningTrainerConfig, TrainingFinishedError
 from ml.utils.device.base import InfinitePrefetcher
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class EpochDoneError(Exception):
@@ -45,30 +45,30 @@
 @dataclass
 class BatchScheduleConfig:
     num_steps: int = conf_field(MISSING, help="Number of steps to run for")
     num_batches: int = conf_field(MISSING, help="Number of minibatches for a given step")
 
 
 @dataclass
-class SupervisedLearningTrainerConfig(VanillaTrainerConfig):
+class SupervisedLearningTrainerConfig(BaseLearningTrainerConfig):
     validation: ValidationConfig = conf_field(ValidationConfig())
     batches_per_step: int = conf_field(1, help="Batches per training step, to simulate larger effective batch sizes")
     batches_per_step_schedule: list[BatchScheduleConfig] | None = conf_field(
         None,
         help="A schedule for the number of minibatches per step, as a list of (step_count, num_batches) tuples.",
     )
 
 
 SupervisedLearningTrainerConfigT = TypeVar("SupervisedLearningTrainerConfigT", bound=SupervisedLearningTrainerConfig)
 SupervisedLearningTaskT = TypeVar("SupervisedLearningTaskT", bound=SupervisedLearningTask)
 
 
 @register_trainer("sl", SupervisedLearningTrainerConfig)
 class SupervisedLearningTrainer(
-    VanillaTrainer[SupervisedLearningTrainerConfigT, ModelT, SupervisedLearningTaskT],
+    BaseLearningTrainer[SupervisedLearningTrainerConfigT, ModelT, SupervisedLearningTaskT],
     Generic[SupervisedLearningTrainerConfigT, ModelT, SupervisedLearningTaskT],
 ):
     @functools.lru_cache()
     def batches_per_step_schedule(self) -> list[tuple[int, int]] | None:
         schedule = self.config.batches_per_step_schedule
         if schedule is None:
             return None
```

### Comparing `ml-starter-0.0.41/ml/trainers/vanilla.py` & `ml-starter-0.0.42/ml/trainers/learning.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 class TrainingFinishedError(Exception):
     pass
 
 
 @dataclass
-class VanillaTrainerConfig(
+class BaseLearningTrainerConfig(
     ProfilerTrainerConfig,
     GradientClippingConfig,
     MixedPrecisionTrainerConfig,
     GPUStatsConfig,
     CPUStatsConfig,
     CompileConfig,
     TrainerParallelConfig,
@@ -55,27 +55,27 @@
     set_to_none: bool = conf_field(True, help="Mode for clearing optimizer gradients")
     deterministic: bool = conf_field(False, help="If set, use determinstic algorithms")
     use_tf32: bool = conf_field(True, help="If set, use TensorFloat32")
     detect_anomaly: bool = conf_field(False, help="Whether to detect anomalies")
     detect_anomaly_check_nan: bool = conf_field(False, help="Whether to check for NaNs when detecting anomalies")
 
 
-VanillaTrainerConfigT = TypeVar("VanillaTrainerConfigT", bound=VanillaTrainerConfig)
+BaseLearningTrainerConfigT = TypeVar("BaseLearningTrainerConfigT", bound=BaseLearningTrainerConfig)
 
 
-class VanillaTrainer(
-    ProfilerTrainerMixin[VanillaTrainerConfigT, ModelT, TaskT],
-    GradientClippingTrainerMixin[VanillaTrainerConfigT, ModelT, TaskT],
-    MixedPrecisionTrainerMixin[VanillaTrainerConfigT, ModelT, TaskT],
-    GPUStatsMixin[VanillaTrainerConfigT, ModelT, TaskT],
-    CPUStatsMixin[VanillaTrainerConfigT, ModelT, TaskT],
-    CompileMixin[VanillaTrainerConfigT, ModelT, TaskT],
-    ParallelMixin[VanillaTrainerConfigT, ModelT, TaskT],
-    BaseTrainer[VanillaTrainerConfigT, ModelT, TaskT],
-    Generic[VanillaTrainerConfigT, ModelT, TaskT],
+class BaseLearningTrainer(
+    ProfilerTrainerMixin[BaseLearningTrainerConfigT, ModelT, TaskT],
+    GradientClippingTrainerMixin[BaseLearningTrainerConfigT, ModelT, TaskT],
+    MixedPrecisionTrainerMixin[BaseLearningTrainerConfigT, ModelT, TaskT],
+    GPUStatsMixin[BaseLearningTrainerConfigT, ModelT, TaskT],
+    CPUStatsMixin[BaseLearningTrainerConfigT, ModelT, TaskT],
+    CompileMixin[BaseLearningTrainerConfigT, ModelT, TaskT],
+    ParallelMixin[BaseLearningTrainerConfigT, ModelT, TaskT],
+    BaseTrainer[BaseLearningTrainerConfigT, ModelT, TaskT],
+    Generic[BaseLearningTrainerConfigT, ModelT, TaskT],
 ):
     def train_step(
         self,
         *,
         task_model: nn.Module,
         batches: Iterator[Batch],
         state: State,
@@ -203,17 +203,15 @@
     ) -> tuple[Optimizer, SchedulerAdapter]:
         with Timer("building optimizer", 0.1, spinner=True):
             optim = optimizer.get(task_model)
         with Timer("building learning rate scheduler", 0.1, spinner=True):
             lr_sched = lr_scheduler.get(optim)
         return optim, lr_sched
 
-    def _get_state(
-        self,
-        task: TaskT,
-        model: ModelT,
-        optim: Optimizer,
-        lr_sched: SchedulerAdapter,
-    ) -> State:
+    def _get_state(self, task: TaskT, model: ModelT, optim: Optimizer, lr_sched: SchedulerAdapter) -> State:
         if (ckpt_path := self.get_ckpt_path()).exists():
             return self.load_checkpoint(ckpt_path, task, model, optim, lr_sched)
+        if self.config.checkpoint.load_from_ckpt_path is not None:
+            ckpt_path = Path(self.config.checkpoint.load_from_ckpt_path)
+            assert ckpt_path.exists(), f"Checkpoint path {ckpt_path} does not exist."
+            self.load_checkpoint(ckpt_path, task, model, optim, lr_sched)
         return State.init_state()
```

### Comparing `ml-starter-0.0.41/ml/utils/argparse.py` & `ml-starter-0.0.42/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/atomic.py` & `ml-starter-0.0.42/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/augmentation.py` & `ml-starter-0.0.42/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/caching.py` & `ml-starter-0.0.42/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/checkpoint.py` & `ml-starter-0.0.42/ml/utils/checkpoint.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 These functions can be used to load a model from an arbitrary config file
 and checkpoint. Note that there might be some issues if you move the checkpoint
 around places.
 """
 
 import logging
 from pathlib import Path
-from typing import TypeVar, cast
+from typing import Mapping, TypeVar, cast
 
 import torch
 from omegaconf import DictConfig, OmegaConf
+from torchvision.datasets.utils import download_url
 
+from ml.core.env import get_model_dir
 from ml.core.registry import Objects, register_model, register_task
 from ml.models.base import BaseModel
 from ml.tasks.base import BaseTask
 from ml.trainers.base import BaseTrainer
 from ml.utils.device.auto import AutoDevice
 from ml.utils.timer import Timer
 
@@ -137,7 +139,40 @@
 
         if to_device:
             device = AutoDevice.detect_device()
             device.module_to(model)
             device.module_to(task)
 
     return model, task
+
+
+def ensure_downloaded(url: str, dname: str, fname: str, md5: str | None = None) -> Path:
+    """Ensures that a URL has been downloaded to a given directory.
+
+    Args:
+        url: The URL to download.
+        dname: The directory to download to (note that this is relative to the
+            model directory).
+        fname: The filename to download to.
+        md5: The MD5 hash of the file, if known.
+
+    Returns:
+        The path to the downloaded file.
+    """
+    (root := get_model_dir() / dname).mkdir(parents=True, exist_ok=True)
+    filepath = root / fname
+    if not filepath.exists():
+        download_url(url, root=root, filename=filepath.name, md5=md5)
+    return filepath
+
+
+def get_state_dict_prefix(state_dict: Mapping[str, T], prefix: str) -> Mapping[str, T]:
+    """Gets the state dict with a prefix removed from the keys.
+
+    Args:
+        state_dict: The state dict to get the prefix from.
+        prefix: The prefix to remove.
+
+    Returns:
+        The state dict with the prefix removed.
+    """
+    return {k[len(prefix) :]: v for k, v in state_dict.items() if k.startswith(prefix)}
```

### Comparing `ml-starter-0.0.41/ml/utils/cli.py` & `ml-starter-0.0.42/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/colors.py` & `ml-starter-0.0.42/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/config.py` & `ml-starter-0.0.42/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/data.py` & `ml-starter-0.0.42/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/datetime.py` & `ml-starter-0.0.42/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/device/auto.py` & `ml-starter-0.0.42/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/device/base.py` & `ml-starter-0.0.42/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/device/cpu.py` & `ml-starter-0.0.42/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/device/gpu.py` & `ml-starter-0.0.42/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/device/metal.py` & `ml-starter-0.0.42/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/distributed.py` & `ml-starter-0.0.42/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/image.py` & `ml-starter-0.0.42/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/large_models.py` & `ml-starter-0.0.42/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/logging.py` & `ml-starter-0.0.42/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/meter.py` & `ml-starter-0.0.42/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/parallel.py` & `ml-starter-0.0.42/ml/utils/parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,21 +48,21 @@
 - ``Model parallel groups``: ``[[0, 1], [2, 3], [4, 5], [6, 7]]``
 - ``Data parallel groups``: ``[[0, 4], [1, 5], [2, 6], [3, 7]]``
 - ``Pipeline parallel groups``: ``[[0, 2], [1, 3], [4, 6], [5, 7]]``
 """
 
 import logging
 from dataclasses import dataclass
-from typing import Any
+from typing import Any, Literal, overload
 
 import torch
 import torch.distributed
 from torch import Tensor
 from torch.distributed import ProcessGroup
-from torch.distributed.distributed_c10d import Backend, ReduceOp
+from torch.distributed.distributed_c10d import Backend, ReduceOp, Work, _get_default_group, is_initialized
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class _GroupInfo:
     """Information and helper functions for a process group.
@@ -82,15 +82,23 @@
     """
 
     group: ProcessGroup
     global_ranks: list[int]
     rank: int
     world_size: int
 
-    def reduce(self, tensor: Tensor, op: Any = ReduceOp.SUM, async_op: bool = False) -> Tensor:
+    @overload
+    def reduce(self, tensor: Tensor, op: Any = ReduceOp.SUM, *, async_op: Literal[False] = False) -> Tensor:
+        ...
+
+    @overload
+    def reduce(self, tensor: Tensor, op: Any = ReduceOp.SUM, *, async_op: Literal[True]) -> Work:
+        ...
+
+    def reduce(self, tensor: Tensor, op: Any = ReduceOp.SUM, *, async_op: bool = False) -> Tensor | Work:
         """Reduces the tensor across all processes in the group.
 
         Consider two tensors in the same process group on different processes,
         with values ``[1, 2, 3]`` and ``[4, 5, 6]``. After calling this
         function, both tensors will have the value ``[5, 7, 9]``.
 
         Args:
@@ -99,16 +107,16 @@
             async_op: Whether to perform the operation asynchronously.
 
         Returns:
             The reduced tensor.
         """
         if self.world_size == 1:
             return tensor
-        torch.distributed.all_reduce(tensor, op=op, group=self.group, async_op=async_op)
-        return tensor
+        work = torch.distributed.all_reduce(tensor, op=op, group=self.group, async_op=async_op)
+        return work if async_op else tensor
 
     def split(self, tensor: Tensor, dim: int = 0) -> Tensor:
         """Splits the tensor across all processes in the group.
 
         Consider a tensor with shape ``[8, 4]`` split across 4 processes. After
         calling this function, each process will have a tensor with shape
         ``[2, 4]``.
@@ -121,51 +129,68 @@
             The split tensor.
         """
         if self.world_size == 1:
             return tensor
         slice_len = tensor.shape[dim] // self.world_size
         return tensor.narrow(dim, self.rank * slice_len, slice_len)
 
-    def gather(self, tensor: Tensor, dim: int = -1, async_op: bool = False) -> Tensor:
+    @overload
+    def gather(self, tensor: Tensor, dim: int = -1, *, async_op: Literal[False] = False) -> Tensor:
+        ...
+
+    @overload
+    def gather(self, tensor: Tensor, dim: int = -1, *, async_op: Literal[True]) -> Work:
+        ...
+
+    def gather(self, tensor: Tensor, dim: int = -1, *, async_op: bool = False) -> Tensor | Work:
         """Gathers the tensor across all processes in the group.
 
         Consider a tensor with shape ``[2, 4]`` split across 4 processes. After
         calling this function, the process with rank 0 will have a tensor with
         shape ``[8, 4]``.
 
         Args:
             tensor: The tensor to gather.
             dim: The dimension to gather along.
             async_op: Whether to perform the operation asynchronously.
 
         Returns:
-            The gathered tensor.
+            The gathered tensor, or a work pointer if async.
         """
         if self.world_size == 1:
             return tensor
         output = [torch.empty_like(tensor) for _ in range(self.world_size)]
-        torch.distributed.all_gather(output, tensor, group=self.group, async_op=async_op)
-        return torch.cat(output, dim=dim)
+        work = torch.distributed.all_gather(output, tensor, group=self.group, async_op=async_op)
+        return work if async_op else torch.cat(output, dim=dim)
 
 
 @dataclass
 class _GroupsInfos:
     mp: _GroupInfo
     pp: _GroupInfo
     dp: _GroupInfo
 
 
 _parallel_group_info: _GroupsInfos | None = None
+_default_group_info: _GroupInfo | None = None
 
 
 def parallel_group_info() -> _GroupsInfos:
     assert _parallel_group_info is not None
     return _parallel_group_info
 
 
+def default_group_info() -> _GroupInfo | None:
+    global _default_group_info
+    if _default_group_info is None and is_initialized():
+        rank, world_size = torch.distributed.get_rank(), torch.distributed.get_world_size()
+        _default_group_info = _GroupInfo(_get_default_group(), list(range(world_size)), rank, world_size)
+    return _default_group_info
+
+
 class ParallismError(Exception):
     pass
 
 
 def init_parallelism(
     model_parallelism: int = 1,
     pipeline_parallelism: int = 1,
```

### Comparing `ml-starter-0.0.41/ml/utils/staging.py` & `ml-starter-0.0.42/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/timer.py` & `ml-starter-0.0.42/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/torch_distributed.py` & `ml-starter-0.0.42/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml/utils/video.py` & `ml-starter-0.0.42/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.42/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.41
+Version: 0.0.42
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.41/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.42/ml_starter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 ml/lr_schedulers/scripts/__init__.py
 ml/lr_schedulers/scripts/plot.py
 ml/models/__init__.py
 ml/models/activations.py
 ml/models/base.py
 ml/models/embeddings.py
 ml/models/init.py
+ml/models/kmeans.py
 ml/models/lora.py
 ml/models/norms.py
 ml/models/parallel.py
 ml/models/pretrained/__init__.py
 ml/models/pretrained/blip.py
 ml/models/pretrained/clip.py
 ml/models/pretrained/hubert.py
@@ -87,17 +88,17 @@
 ml/tasks/rl/__init__.py
 ml/tasks/rl/base.py
 ml/tasks/rl/replay.py
 ml/tasks/sl/__init__.py
 ml/tasks/sl/base.py
 ml/trainers/__init__.py
 ml/trainers/base.py
+ml/trainers/learning.py
 ml/trainers/rl.py
 ml/trainers/sl.py
-ml/trainers/vanilla.py
 ml/trainers/mixins/__init__.py
 ml/trainers/mixins/compile.py
 ml/trainers/mixins/cpu_stats.py
 ml/trainers/mixins/data_parallel.py
 ml/trainers/mixins/gpu_stats.py
 ml/trainers/mixins/grad_clipping.py
 ml/trainers/mixins/heartbeat.py
```

### Comparing `ml-starter-0.0.41/pyproject.toml` & `ml-starter-0.0.42/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.41/setup.py` & `ml-starter-0.0.42/setup.py`

 * *Files identical despite different names*

