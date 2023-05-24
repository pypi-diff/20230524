# Comparing `tmp/dprox-0.1.0.tar.gz` & `tmp/dprox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dprox-0.1.0.tar", last modified: Sun May 21 15:40:01 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/hyper-pnp/submit/Delta-Prox/dist/.tmp-0q1o0s2a/dprox-0.1.1.tar", last modified: Wed May 24 08:14:56 2023, max compression
```

## Comparing `dprox-0.1.0.tar` & `dprox-0.1.1.tar`

### file list

```diff
@@ -1,165 +1,170 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      310 2023-05-21 15:40:01.413618 dprox-0.1.0/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3156 2023-05-10 07:07:21.000000 dprox-0.1.0/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.401618 dprox-0.1.0/dprox/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      105 2023-05-12 08:43:00.000000 dprox-0.1.0/dprox/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      276 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3612 2023-05-20 09:01:13.000000 dprox-0.1.0/dprox/algo/admm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5833 2023-05-20 09:14:46.000000 dprox-0.1.0/dprox/algo/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      515 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/hqs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      679 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/invert.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/lp/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       63 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/lp/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2355 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/lp/linear_solvers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13377 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/lp/solvers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6017 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/lp/utils.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/opt/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       41 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/opt/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1289 2023-05-13 14:56:20.000000 dprox-0.1.0/dprox/algo/opt/absorb.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/opt/equil.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2239 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/opt/merge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1074 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/algo/pc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/pgd.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4576 2023-05-20 09:37:39.000000 dprox-0.1.0/dprox/algo/problem.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/special/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       72 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6866 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/special/deq_utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/jacobian.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/layer_utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/optimizations.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/radam.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13962 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/deq_utils/solvers.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/special/unroll.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/algo/tune/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       23 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/tune/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12895 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/tune/autotune.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1850 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/tune/dpir.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/algo/tune/learnable.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.405618 dprox-0.1.0/dprox/linop/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-10 14:07:17.000000 dprox-0.1.0/dprox/linop/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7440 2023-05-20 03:13:06.000000 dprox-0.1.0/dprox/linop/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2126 2023-05-10 14:07:18.000000 dprox-0.1.0/dprox/linop/blackbox.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    15084 2023-05-20 09:13:41.000000 dprox-0.1.0/dprox/linop/comp_graph.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      445 2023-05-20 03:13:06.000000 dprox-0.1.0/dprox/linop/constaints.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2862 2023-05-20 03:12:27.000000 dprox-0.1.0/dprox/linop/constant.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5036 2023-05-12 06:37:57.000000 dprox-0.1.0/dprox/linop/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      464 2023-05-20 03:12:27.000000 dprox-0.1.0/dprox/linop/edge.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1219 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/linop/grad.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      339 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/linop/placeholder.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2560 2023-05-12 06:38:28.000000 dprox-0.1.0/dprox/linop/scale.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3439 2023-05-12 06:38:59.000000 dprox-0.1.0/dprox/linop/subsample.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2991 2023-05-20 03:13:06.000000 dprox-0.1.0/dprox/linop/sum.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2968 2023-05-20 03:12:27.000000 dprox-0.1.0/dprox/linop/variable.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3657 2023-05-20 03:12:27.000000 dprox-0.1.0/dprox/linop/vstack.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      306 2023-05-10 08:01:32.000000 dprox-0.1.0/dprox/proxfn/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2693 2023-05-20 01:26:10.000000 dprox-0.1.0/dprox/proxfn/base.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/fast/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/fast/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/fast/cs.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      884 2023-05-20 03:23:29.000000 dprox-0.1.0/dprox/proxfn/fast/csmri.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/fast/pr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/fast/spi.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3925 2023-05-13 14:56:20.000000 dprox-0.1.0/dprox/proxfn/fast/sr.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/linalg/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-05-10 08:37:58.000000 dprox-0.1.0/dprox/proxfn/linalg/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1782 2023-05-11 03:05:00.000000 dprox-0.1.0/dprox/proxfn/linalg/custom.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/linalg/solve/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      271 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5069 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/bicgstab.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1134 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/broyden.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6317 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/cg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6501 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/gmres.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1631 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/linalg/solve/plss.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/nlm/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/nlm/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/nlm/nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/nlm/patch_nlm.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/nonneg.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/norm.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/pnp/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/base.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/composite.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_unet.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.409618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/unet.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-05-20 02:09:19.000000 dprox-0.1.0/dprox/proxfn/pnp/denoisers/wrapper.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2902 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/proxfn/pnp/prior.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6025 2023-05-20 09:35:06.000000 dprox-0.1.0/dprox/proxfn/sum_square.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/proxfn/unrolling/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/unrolling/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/unrolling/dgu.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      482 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/proxfn/unrolling/prior.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      164 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      107 2023-05-12 09:12:18.000000 dprox-0.1.0/dprox/utils/containar.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-05-13 14:43:30.000000 dprox-0.1.0/dprox/utils/examples/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/csmri/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       82 2023-05-13 14:45:34.000000 dprox-0.1.0/dprox/utils/examples/csmri/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3011 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/csmri/common.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4146 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/csmri/dataset.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1993 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/utils/examples/csmri/misc.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/derain/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       40 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/derain/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2564 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/derain/custom_linop.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/energy_system/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      947 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/utils/examples/energy_system/__init__.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/examples/optic/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       46 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/optic/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5211 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/optic/common.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13167 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/optic/doe_model.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3063 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/examples/optic/unet.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2488 2023-05-14 13:57:57.000000 dprox-0.1.0/dprox/utils/examples/restoration.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/dprox/utils/init/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/init/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4704 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/init/mosaic.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      755 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/init/sr.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2130 2023-05-20 03:14:24.000000 dprox-0.1.0/dprox/utils/io.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2442 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/metrics.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1709 2023-05-20 08:50:17.000000 dprox-0.1.0/dprox/utils/misc.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2289 2023-04-12 02:15:00.000000 dprox-0.1.0/dprox/utils/psf2otf.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.401618 dprox-0.1.0/dprox.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      310 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4251 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      108 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-05-21 15:40:01.000000 dprox-0.1.0/dprox.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-21 15:40:01.413618 dprox-0.1.0/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      662 2023-05-21 15:39:51.000000 dprox-0.1.0/setup.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-21 15:40:01.413618 dprox-0.1.0/tests/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2715 2023-05-20 03:13:06.000000 dprox-0.1.0/tests/test_algorithms.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      316 2023-05-20 03:14:24.000000 dprox-0.1.0/tests/test_energy_system.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1101 2023-05-20 03:13:06.000000 dprox-0.1.0/tests/test_inverse_problems.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2119 2023-05-21 14:42:14.000000 dprox-0.1.0/tests/test_linear_solver.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3272 2023-05-12 08:09:14.000000 dprox-0.1.0/tests/test_linear_solver_grad.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5780 2023-05-20 03:12:27.000000 dprox-0.1.0/tests/test_linear_solver_torch.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2692 2023-05-20 03:13:06.000000 dprox-0.1.0/tests/test_linop.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      180 2023-05-20 03:13:06.000000 dprox-0.1.0/tests/test_linop_primitive.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1196 2023-05-20 09:38:13.000000 dprox-0.1.0/tests/test_ml_problems.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-05-24 08:14:56.000000 dprox-0.1.1/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3141 2023-05-22 07:49:24.000000 dprox-0.1.1/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      126 2023-05-22 12:58:17.000000 dprox-0.1.1/dprox/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/algo/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      276 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/algo/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3676 2023-05-24 07:18:47.000000 dprox-0.1.1/dprox/algo/admm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7654 2023-05-24 04:36:39.000000 dprox-0.1.1/dprox/algo/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      515 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/algo/hqs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      685 2023-05-24 07:17:40.000000 dprox-0.1.1/dprox/algo/invert.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/algo/lp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       63 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/algo/lp/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13337 2023-05-22 14:14:30.000000 dprox-0.1.1/dprox/algo/lp/solvers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6017 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/algo/lp/utils.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/algo/opt/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       41 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/opt/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1289 2023-05-13 14:56:20.000000 dprox-0.1.1/dprox/algo/opt/absorb.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2713 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/opt/equil.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2241 2023-05-22 07:49:41.000000 dprox-0.1.1/dprox/algo/opt/merge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1074 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/algo/pc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1370 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/pgd.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4625 2023-05-24 07:18:27.000000 dprox-0.1.1/dprox/algo/problem.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/algo/special/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       72 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/special/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6866 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/special/deq.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/algo/special/deq_utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/special/deq_utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1863 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/special/deq_utils/jacobian.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1332 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/special/deq_utils/layer_utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11133 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/special/deq_utils/optimizations.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8090 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/special/deq_utils/radam.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13962 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/special/deq_utils/solvers.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/special/unroll.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/algo/tune/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       23 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/tune/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12895 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/tune/autotune.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1850 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/tune/dpir.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      511 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/algo/tune/learnable.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/linalg/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-05-22 11:53:09.000000 dprox-0.1.1/dprox/linalg/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1785 2023-05-22 12:39:40.000000 dprox-0.1.1/dprox/linalg/custom.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/linalg/solve/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      410 2023-05-22 11:53:09.000000 dprox-0.1.1/dprox/linalg/solve/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6498 2023-05-22 14:14:30.000000 dprox-0.1.1/dprox/linalg/solve/cg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     9704 2023-05-22 14:14:30.000000 dprox-0.1.1/dprox/linalg/solve/minres.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3448 2023-05-22 14:14:30.000000 dprox-0.1.1/dprox/linalg/solve/plss.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/linop/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      648 2023-05-10 14:07:17.000000 dprox-0.1.1/dprox/linop/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7440 2023-05-20 03:13:06.000000 dprox-0.1.1/dprox/linop/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2365 2023-05-24 07:38:28.000000 dprox-0.1.1/dprox/linop/blackbox.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    15084 2023-05-20 09:13:41.000000 dprox-0.1.1/dprox/linop/comp_graph.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      445 2023-05-20 03:13:06.000000 dprox-0.1.1/dprox/linop/constaints.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2882 2023-05-24 07:43:37.000000 dprox-0.1.1/dprox/linop/constant.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5480 2023-05-24 07:43:49.000000 dprox-0.1.1/dprox/linop/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      464 2023-05-20 03:12:27.000000 dprox-0.1.1/dprox/linop/edge.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1219 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/linop/grad.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      489 2023-05-24 06:31:56.000000 dprox-0.1.1/dprox/linop/placeholder.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2580 2023-05-24 07:43:58.000000 dprox-0.1.1/dprox/linop/scale.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3459 2023-05-24 07:38:58.000000 dprox-0.1.1/dprox/linop/subsample.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3051 2023-05-24 07:44:13.000000 dprox-0.1.1/dprox/linop/sum.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2988 2023-05-24 07:44:22.000000 dprox-0.1.1/dprox/linop/variable.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3717 2023-05-24 07:44:41.000000 dprox-0.1.1/dprox/linop/vstack.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      285 2023-05-22 11:53:09.000000 dprox-0.1.1/dprox/proxfn/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2693 2023-05-20 01:26:10.000000 dprox-0.1.1/dprox/proxfn/base.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/fast/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       84 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/fast/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      711 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/fast/cs.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      884 2023-05-20 03:23:29.000000 dprox-0.1.1/dprox/proxfn/fast/csmri.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1721 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/fast/pr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2328 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/fast/spi.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3925 2023-05-13 14:56:20.000000 dprox-0.1.1/dprox/proxfn/fast/sr.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/linalg/
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/linalg/solve/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5069 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/proxfn/linalg/solve/bicgstab.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1134 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/proxfn/linalg/solve/broyden.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6501 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/proxfn/linalg/solve/gmres.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1631 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/proxfn/linalg/solve/plss.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/nlm/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       32 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/nlm/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4758 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/nlm/nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      301 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/nlm/patch_nlm.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      210 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/nonneg.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      606 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/norm.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/pnp/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       29 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      321 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      763 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/base.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3315 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/composite.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1694 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/TV_denoising.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6167 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/network_dncnn.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4157 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    16619 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/network_unet.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      870 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3258 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3916 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5264 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     5741 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      449 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12973 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4278 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     3226 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      835 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/unet/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       22 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/unet/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    21015 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12412 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/unet/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7588 2023-05-20 02:09:19.000000 dprox-0.1.1/dprox/proxfn/pnp/denoisers/wrapper.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2902 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/proxfn/pnp/prior.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5751 2023-05-24 07:40:18.000000 dprox-0.1.1/dprox/proxfn/sum_square.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/proxfn/unrolling/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       33 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/unrolling/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    13120 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/unrolling/dgu.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      482 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/proxfn/unrolling/prior.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/utils/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      173 2023-05-24 04:36:39.000000 dprox-0.1.1/dprox/utils/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1504 2023-05-24 04:36:39.000000 dprox-0.1.1/dprox/utils/containar.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/utils/examples/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       61 2023-05-13 14:43:30.000000 dprox-0.1.1/dprox/utils/examples/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/utils/examples/csmri/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       82 2023-05-13 14:45:34.000000 dprox-0.1.1/dprox/utils/examples/csmri/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3011 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/utils/examples/csmri/common.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4146 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/utils/examples/csmri/dataset.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2083 2023-05-22 15:23:16.000000 dprox-0.1.1/dprox/utils/examples/csmri/misc.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/utils/examples/derain/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       40 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/utils/examples/derain/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2564 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/utils/examples/derain/custom_linop.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/utils/examples/energy_system/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      947 2023-05-20 03:14:24.000000 dprox-0.1.1/dprox/utils/examples/energy_system/__init__.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/utils/examples/optic/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       46 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/utils/examples/optic/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     8995 2023-05-24 04:36:39.000000 dprox-0.1.1/dprox/utils/examples/optic/common.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    18284 2023-05-24 04:36:39.000000 dprox-0.1.1/dprox/utils/examples/optic/doe_model.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3063 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/utils/examples/optic/unet.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2488 2023-05-14 13:57:57.000000 dprox-0.1.1/dprox/utils/examples/restoration.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox/utils/init/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-04-12 02:15:00.000000 dprox-0.1.1/dprox/utils/init/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4705 2023-05-24 04:36:39.000000 dprox-0.1.1/dprox/utils/init/mosaic.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      756 2023-05-24 04:36:39.000000 dprox-0.1.1/dprox/utils/init/sr.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5735 2023-05-24 07:02:59.000000 dprox-0.1.1/dprox/utils/io.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4630 2023-05-24 04:36:39.000000 dprox-0.1.1/dprox/utils/metrics.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4958 2023-05-24 06:20:38.000000 dprox-0.1.1/dprox/utils/misc.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3978 2023-05-24 04:36:39.000000 dprox-0.1.1/dprox/utils/psf2otf.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      304 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     4287 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      108 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        6 2023-05-24 08:14:56.000000 dprox-0.1.1/dprox.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-24 08:14:56.000000 dprox-0.1.1/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      656 2023-05-24 08:14:28.000000 dprox-0.1.1/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-24 08:14:56.000000 dprox-0.1.1/tests/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2715 2023-05-20 03:13:06.000000 dprox-0.1.1/tests/test_algorithms.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1043 2023-05-24 07:09:33.000000 dprox-0.1.1/tests/test_derain.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      318 2023-05-22 14:14:30.000000 dprox-0.1.1/tests/test_energy_system.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1688 2023-05-23 08:23:24.000000 dprox-0.1.1/tests/test_inverse_problems.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      790 2023-05-24 07:49:26.000000 dprox-0.1.1/tests/test_jd23.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2586 2023-05-24 04:36:39.000000 dprox-0.1.1/tests/test_linear_solver.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     3280 2023-05-22 11:53:09.000000 dprox-0.1.1/tests/test_linear_solver_grad.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     6231 2023-05-24 08:13:09.000000 dprox-0.1.1/tests/test_linear_solver_torch.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     2692 2023-05-20 03:13:06.000000 dprox-0.1.1/tests/test_linop.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      180 2023-05-20 03:13:06.000000 dprox-0.1.1/tests/test_linop_primitive.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1198 2023-05-24 04:36:39.000000 dprox-0.1.1/tests/test_ml_problems.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dprox-0.1.0/README.md` & `dprox-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,15 @@
   <a href="https://arxiv.org/abs/2207.02849">![arXiv](https://img.shields.io/badge/arXiv-2207.02489-b31b1b.svg)</a>
 
 
 ```bash
 pip install dprox
 ```
 
-## Introduction
-
-$\nabla$-Prox is a domain-specific language (DSL) and compiler that transforms optimization problems into differentiable proximal solvers. Departing from handwriting these solvers and differentiating via autograd, $\nabla$-Prox requires only a few lines of code to define a solver that can be *specialized based on user requirements w.r.t memory constraints or training budget* by optimized algorithm unrolling, deep equilibrium learning, and deep reinforcement learning. $\nabla$-Prox makes it easier to prototype different learning-based bi-level optimization problems for a diverse range of applications. We compare our framework against existing methods with naive implementations. $\nabla$-Prox is significantly more compact in terms of lines of code and compares favorably in memory consumption in applications across domains.
+> $\nabla$-Prox is a domain-specific language (DSL) and compiler that transforms optimization problems into differentiable proximal solvers. Departing from handwriting these solvers and differentiating via autograd, $\nabla$-Prox requires only a few lines of code to define a solver that can be *specialized based on user requirements w.r.t memory constraints or training budget* by optimized algorithm unrolling, deep equilibrium learning, and deep reinforcement learning. $\nabla$-Prox makes it easier to prototype different learning-based bi-level optimization problems for a diverse range of applications. We compare our framework against existing methods with naive implementations. $\nabla$-Prox is significantly more compact in terms of lines of code and compares favorably in memory consumption in applications across domains.
 
 ## News
  
 **[Jan 21 2023]**  Release preview code.
 
 > 🚧 The code is still under construction, more features would be migrated from our dev code.
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
   &ensp; Differentiable Proximal Algorithm Modeling for Large-Scale
 Optimization Docs | Tutorials | Examples | Paper | Citation ![Version](https://
 img.shields.io/pypi/v/dprox) ![arXiv](https://img.shields.io/badge/arXiv-
-2207.02489-b31b1b.svg) ```bash pip install dprox ``` ## Introduction $\nabla$-
-Prox is a domain-specific language (DSL) and compiler that transforms
-optimization problems into differentiable proximal solvers. Departing from
-handwriting these solvers and differentiating via autograd, $\nabla$-Prox
-requires only a few lines of code to define a solver that can be *specialized
-based on user requirements w.r.t memory constraints or training budget* by
-optimized algorithm unrolling, deep equilibrium learning, and deep
-reinforcement learning. $\nabla$-Prox makes it easier to prototype different
-learning-based bi-level optimization problems for a diverse range of
-applications. We compare our framework against existing methods with naive
-implementations. $\nabla$-Prox is significantly more compact in terms of lines
-of code and compares favorably in memory consumption in applications across
-domains. ## News **[Jan 21 2023]** Release preview code. > ð§ The code is
-still under construction, more features would be migrated from our dev code. ##
-Getting Started ### Solver construction Consider a simple image deconvlution
-problem, where we seek to find a clean image $x$ given the blurred observation
-$y$ that minimizes the following objective function: $$ \arg \min_x { \frac{1}
-{2} |Dx - y|^2_2 + g(x) } $$ where $g(x)$ denotes an implicit plug-and-play
-denoiser prior. We could solve this problem in â-Prox with the following
-code: ```python from dprox import * from dprox.utils import * from
-dprox.utils.examples import * img = sample() psf = point_spread_function(15, 5)
-b = blurring(img, psf) x = Variable() data_term = sum_squares(conv(x, psf) - b)
-reg_term = deep_prior(x, denoiser='ffdnet_color') prob = Problem(data_term +
-reg_term) out = prob.solve(method='admm', x0=b) ``` Here is what we got, [docs/
-source/_static/example_deconv.png] ### Solver Specialization ```python ```
-Please refer to the [documentation]() site for more instructions on the
-efficient differentiation of proximal algorithm with â-Prox. ## Citation
-```bibtex @article{deltaprox2023, title={â-Prox: Differentiable Proximal
-Algorithm Modeling for Large-Scale Optimization}, author={Lai, Zeqiang and Wei,
-Kaixuan and Fu, Ying and HÃ¤rtel, Philipp and Heide, Felix}, journal={ACM
-Transactions on Graphics}, year={2023}, } ```
+2207.02489-b31b1b.svg) ```bash pip install dprox ``` > $\nabla$-Prox is a
+domain-specific language (DSL) and compiler that transforms optimization
+problems into differentiable proximal solvers. Departing from handwriting these
+solvers and differentiating via autograd, $\nabla$-Prox requires only a few
+lines of code to define a solver that can be *specialized based on user
+requirements w.r.t memory constraints or training budget* by optimized
+algorithm unrolling, deep equilibrium learning, and deep reinforcement
+learning. $\nabla$-Prox makes it easier to prototype different learning-based
+bi-level optimization problems for a diverse range of applications. We compare
+our framework against existing methods with naive implementations. $\nabla$-
+Prox is significantly more compact in terms of lines of code and compares
+favorably in memory consumption in applications across domains. ## News **[Jan
+21 2023]** Release preview code. > ð§ The code is still under construction,
+more features would be migrated from our dev code. ## Getting Started ###
+Solver construction Consider a simple image deconvlution problem, where we seek
+to find a clean image $x$ given the blurred observation $y$ that minimizes the
+following objective function: $$ \arg \min_x { \frac{1}{2} |Dx - y|^2_2 + g(x)
+} $$ where $g(x)$ denotes an implicit plug-and-play denoiser prior. We could
+solve this problem in â-Prox with the following code: ```python from dprox
+import * from dprox.utils import * from dprox.utils.examples import * img =
+sample() psf = point_spread_function(15, 5) b = blurring(img, psf) x = Variable
+() data_term = sum_squares(conv(x, psf) - b) reg_term = deep_prior(x,
+denoiser='ffdnet_color') prob = Problem(data_term + reg_term) out = prob.solve
+(method='admm', x0=b) ``` Here is what we got, [docs/source/_static/
+example_deconv.png] ### Solver Specialization ```python ``` Please refer to the
+[documentation]() site for more instructions on the efficient differentiation
+of proximal algorithm with â-Prox. ## Citation ```bibtex @article
+{deltaprox2023, title={â-Prox: Differentiable Proximal Algorithm Modeling for
+Large-Scale Optimization}, author={Lai, Zeqiang and Wei, Kaixuan and Fu, Ying
+and HÃ¤rtel, Philipp and Heide, Felix}, journal={ACM Transactions on Graphics},
+year={2023}, } ```
```

### Comparing `dprox-0.1.0/dprox/algo/admm.py` & `dprox-0.1.1/dprox/algo/admm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 
 import torch
 
 from dprox.proxfn import ProxFn, sum_squares, ext_sum_squares
 from dprox.linop import eval, adjoint
+from dprox.linalg import LinearSolveConfig
 
 from .base import Algorithm, expand
 from .invert import get_least_square_solver
 
 
 """ 
 Given a a list of proxable function
@@ -35,18 +36,18 @@
 
     def __init__(
         self,
         psi_fns: List[ProxFn],
         omega_fns: List[ProxFn],
         try_diagonalize=True,
         try_freq_diagonalize=True,
-        lin_solver_kwargs={}
+        linear_solve_config=LinearSolveConfig()
     ):
         super().__init__(psi_fns, omega_fns)
-        self.least_square = get_least_square_solver(psi_fns, omega_fns, try_diagonalize, try_freq_diagonalize, lin_solver_kwargs)
+        self.least_square = get_least_square_solver(psi_fns, omega_fns, try_diagonalize, try_freq_diagonalize, linear_solve_config)
 
     def _iter(self, state, rho, lam):
         x, v, u = state
         b = [v[i] - u[i] for i in range(len(self.psi_fns))]
         x = self.least_square.solve(b, rho)
 
         Kx = self.K.forward(x, return_list=True)  # cache Kx
```

### Comparing `dprox-0.1.0/dprox/algo/base.py` & `dprox-0.1.1/dprox/proxfn/sum_square.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,190 +1,180 @@
-import abc
-import torch
-import torch.nn as nn
-import numpy as np
 from typing import List
-from tqdm import tqdm
-
-from dprox.proxfn import ProxFn
-from dprox.linop import CompGraph, vstack
-from dprox.utils import to_torch_tensor
-
-
-def expand(r):
-    if len(r.shape) == 1:
-        r = r.view(r.shape[0], 1, 1, 1)
-    return r
-
-
-def auto_convert_to_tensor(names, batchify):
-    def outter_wrapper(fn):
-        def wrapper(*args, **kwargs):
-            for k, v in kwargs.items():
-                if k in names:
-                    if v is not None:
-                        kwargs[k] = to_tensor(v, batch=k in batchify)
-            return fn(*args, **kwargs)
-        return wrapper
-    return outter_wrapper
-
-
-def move(*args, device):
-    return [to_device(arg, device) for arg in args]
 
+import torch
 
-def to_device(x, device):
-    if x is None: return None
-    if isinstance(x, dict):
-        return {k: to_device(v, device) for k, v in x.items()}
-    return x.to(device)
-
-
-def to_tensor(x, batch=False):
-    if isinstance(x, dict):
-        return {k: to_tensor(v, batch) for k, v in x.items()}
-    return to_torch_tensor(x, batch)
-
+from dprox.linop import LinOp, vstack, LinOpFactory, eval, adjoint
+from dprox.linalg import linear_solve, LinearSolveConfig
 
-def isscalar(x):
-    return np.isscalar(x) or (isinstance(x, torch.Tensor) and len(x.shape) == 0)
+from . import ProxFn
 
 
-class Algorithm(nn.Module):
-    # class method
+class sum_squares(ProxFn):
+    """ |x|_2^2 
+    """
 
-    @abc.abstractclassmethod
-    def partition(cls, prox_fns: List[ProxFn]):
-        return NotImplementedError
+    def __init__(self, linop, b=None, eps=1e-7):
+        super().__init__(linop)
+        self.eps = eps
+        self._b = b
 
-    @classmethod
-    def create(cls, *args, **kwargs):
-        return cls(*args, **kwargs)
+    @property
+    def offset(self):
+        if self._b is not None:
+            return self.unwrap(self._b)
+        return super().offset
+
+    def _prox(self, v, lam):
+        return v / (1 + 2 * lam)
+
+    def grad(self, x):
+        tmp = eval(self.linop, x) - self.offset
+        out = adjoint(self.linop, tmp)
+        return out
+
+
+class ext_sum_squares(sum_squares):
+    def __init__(self, linop, eps=1e-7):
+        super().__init__(linop, eps=eps)
+
+    def setup(self, b):
+        # TODO: this might cause bugs, b might not be initialized
+        self.quad_b = b
+        return self
+
+    def solve(self, b, rho, eps=1e-6):
+        xtilde = 0
+        for v in b: xtilde += v
+        return self._prox(xtilde, rho, len(b))
+
+
+class weighted_sum_squares(sum_squares):
+    """ |Ax-b|_2^2 
+        (AtA + I)^-1(Atb + v)
+    """
+
+    def __init__(self, linop, weight: LinOp, b, eps=0):
+        super().__init__(linop, b, eps)
+        self.weight = weight
+        if self.weight.is_self_diag():
+            self._prox_fn = self._prox
+        elif self.weight.is_self_diag(freq=True):
+            self._prox_fn = self._prox_freq
+        else:
+            raise ValueError('weight {} must be diagonalizable'.format(weight))
 
-    # instance method
+    @property
+    def Ktb(self):
+        return adjoint(self.weight, self.unwrap(self._b))
 
-    def __init__(self, psi_fns: List[ProxFn], omega_fns: List[ProxFn]):
-        super().__init__()
-        self.psi_fns = nn.ModuleList(psi_fns)
-        self.omega_fns = nn.ModuleList(omega_fns)
-        self.K = CompGraph(vstack([fn.linop for fn in psi_fns]))
-        self.Kall = CompGraph(vstack([fn.linop for fn in psi_fns + omega_fns]))
+    def prox(self, v, lam):
+        return self._prox_fn(v, lam)
 
-    @property
-    def device(self):
-        return next(self.parameters()).device
+    def _prox(self, v, lam):
+        if len(lam.shape) == 1:
+            lam = lam.view(lam.shape[0], 1, 1, 1)
+        Ktb = self.Ktb.to(v.device)
+        diag = self.weight.get_diag(Ktb).to(v.device)
+        return (Ktb + lam * v) / (diag + lam)
+
+    def _prox_freq(self, v, lam):
+        Ktb = torch.fft.fftn(self.Ktb + lam * v, dim=[0, 1])
+        fout = (Ktb + self.eps) / (self.weight.get_diag(v, freq=True) + lam + self.eps)
+        return torch.real(torch.fft.ifftn(fout, dim=[0, 1]))
+
+
+class least_squares(ProxFn):
+    def __init__(
+        self,
+        quad_fns: List[ProxFn],
+        other_fns: List[ProxFn],
+        try_diagonalize=True,
+        try_freq_diagonalize=True,
+        fallback_solver='cg',
+        linear_solve_config=LinearSolveConfig(),
+    ):
+        self.quad_fns = quad_fns
+        self.other_fns = other_fns
+
+        self.try_freq_diagonalize = try_freq_diagonalize
+        self.try_diagonalize = try_diagonalize
+        self.fallback_solver = fallback_solver
+        self.linear_solve_config = linear_solve_config
+
+        linops = [fn.linop for fn in quad_fns + other_fns]
+        stacked = vstack(linops)
+        self.diagonalizable = stacked.is_gram_diag(freq=False) and try_diagonalize
+        self.freq_diagonalizable = stacked.is_gram_diag(freq=True) and try_diagonalize and try_freq_diagonalize
+
+        super().__init__(stacked)
+        # print(f'diagonalizable={self.diagonalizable}, freq_diagonalizable={self.freq_diagonalizable}')
+
+    def _prox(self, v, lam):
+        return self.solve([], lam, v=v)
+
+    def solve(self, b, rho, v=None, eps=1e-7):
+        if rho.ndim == 1: rho = rho.view(rho.shape[0], 1, 1, 1)
+        if self.diagonalizable or self.freq_diagonalizable:
+            return self.solve_direct(b, rho, v, eps)
+        else:
+            return self.solve_cg(b, rho, v, self.linear_solve_config)
+
+    def solve_direct(self, b, rho, v=None, eps=1e-7):
+        device = rho.device
+        Ktb = 0
+        for fn in self.quad_fns:
+            # TODO: ideally, we should rewrite the dag to remove offset,
+            # then we don't need to specially process sum's adjoint.
+            out = fn.dag.adjoint(fn.offset)
+            if isinstance(out, LinOp.MultOutput):
+                out = out[0]
+            Ktb += out
+        for i, fn in enumerate(self.other_fns):
+            Ktb += rho * fn.dag.adjoint(b[i])
+        if v is not None:
+            Ktb += rho * v
+
+        def get_diag(fn: ProxFn):
+            # TODO: hack for derain, don't forgot change it back, Ktb -> Ktb.shape
+            return fn.linop.get_diag(Ktb, freq=self.freq_diagonalizable)
+
+        diag = 0
+        for fn in self.quad_fns:
+            diag = diag + get_diag(fn).to(device)
+        for fn in self.other_fns:
+            diag = diag + rho * get_diag(fn).to(device)
+        if v is not None:
+            diag = diag + rho
+
+        if self.freq_diagonalizable:
+            Ktb = torch.fft.fftn(Ktb, dim=[-2, -1])
+            out = torch.real(torch.fft.ifftn((Ktb + eps) / (diag + eps), dim=[-2, -1]))
+        else:
+            out = Ktb / (diag + eps)
+
+        return out.float()
+
+    def solve_cg(self, b, rho, v=None, linear_solve_config=LinearSolveConfig()):
+        # KtKfun being a function that computes the matrix vector product KtK x
+
+        def KtK(x, **kwargs):
+            out = 0
+            for fn in self.quad_fns:
+                out += fn.dag.adjoint(fn.dag.forward(x))
+            for fn in self.other_fns:
+                out += rho * fn.dag.adjoint(fn.dag.forward(x))  # slow when rho is small
+            if v is not None:
+                out += rho * x
+            return out
+
+        linop = LinOpFactory(KtK, KtK)()
+
+        Ktb = 0
+        for fn in self.quad_fns:
+            Ktb += fn.dag.adjoint(fn.offset)
+        for i, fn in enumerate(self.other_fns):
+            Ktb += rho * fn.dag.adjoint(b[i])
+        if v is not None:
+            Ktb += rho * v
 
-    @auto_convert_to_tensor(['x0', 'rhos', 'lams'], batchify=['x0'])
-    def solve(self, x0=None, rhos=None, lams=None, max_iter=24, pbar=False):
-        x0, rhos, lams, max_iter = self.defaults(x0, rhos, lams, max_iter)
-        x0, rhos, lams = move(x0, rhos, lams, device=self.device)
-
-        state = self.initialize(x0)
-        state = self.iters(state, rhos, lams, max_iter, pbar)
-
-        return state[0]
-
-    def iters(self, state, rhos, lams, max_iter, pbar=False):
-        for iter in tqdm(range(max_iter), disable=not pbar):
-            rho = rhos[..., iter]
-            lam = {k: v[..., iter] for k, v in lams.items()}
-            self._notify_all_op_current_step(iter)
-            state = self.iter(state, rho, lam)
-        return state
-
-    def _notify_all_op_current_step(self, step):
-        for fn in self.psi_fns:
-            fn.step = step
-        for fn in self.omega_fns:
-            fn.step = step
-
-        def recursive_set_step(op, step):
-            op.step = step
-            for node in op.input_nodes:
-                recursive_set_step(node, step)
-
-        for op in [fn.linop for fn in self.psi_fns]:
-            recursive_set_step(op, step)
-        for op in [fn.linop for fn in self.omega_fns]:
-            recursive_set_step(op, step)
-
-    def iter(self, state, rho, lam):
-        self.Kall.update_vars([state[0]])
-        state = self._iter(state, rho, lam)
-        self.Kall.update_vars([state[0]])
-        return state
-
-    @abc.abstractmethod
-    def _iter(self, state, rho, lam):
-        return NotImplementedError
-
-    def _notify_all_op_current_step(self, step):
-        for fn in self.psi_fns:
-            fn.step = step
-        for fn in self.omega_fns:
-            fn.step = step
-
-        def recursive_set_step(op, step):
-            op.step = step
-            for node in op.input_nodes:
-                recursive_set_step(node, step)
-
-        for op in [fn.linop for fn in self.psi_fns]:
-            recursive_set_step(op, step)
-        for op in [fn.linop for fn in self.omega_fns]:
-            recursive_set_step(op, step)
-
-    def defaults(self, x0=None, rhos=None, lams=None, max_iter=24):
-        # TODO: initialize with defaults if not specified
-        if rhos is None: rhos = 1e-5
-        if lams is None: lams = 0.02
-
-        if isscalar(rhos): rhos = to_tensor([rhos] * max_iter)
-        if isscalar(lams): lams = {fn: to_tensor([lams] * max_iter) for fn in self.psi_fns}
-
-        lams = {k: to_tensor([v] * max_iter) if isscalar(v) else v for k, v in lams.items()}
-        return x0, rhos, lams, max_iter
-
-    # ---------------------------------------------------------------------------- #
-    #                  Helper functions for reinforcement learning                 #
-    # ---------------------------------------------------------------------------- #
-
-    def pack(self, state):
-        flatten = []
-        for s in state:
-            if isinstance(s, list): flatten += s
-            else: flatten += [s]
-        return torch.cat(flatten, dim=1)
-
-    #TODO: refactor
-    def unpack(self, tensor):
-        vars = list(torch.split(tensor,
-                                tensor.shape[1] // self.state_dim,
-                                dim=1))
-        splits = []
-        start, end = 0, 0
-        for d in self.state_split:
-            if d == 1:
-                splits.append(vars[start])
-                end += 1
-            else:
-                d = d[0]
-                end += d
-                splits.append(vars[start:end])
-            start = end
-        return splits
-
-    @abc.abstractproperty
-    def state_dim(self):
-        ans = 0
-        for s in self.state_split:
-            if isinstance(s, list): ans += sum(s)
-            else: ans += s
-        return ans
-
-    @abc.abstractproperty
-    def nparams(self):
-        return NotImplementedError
-
-    @abc.abstractproperty
-    def state_split(self):
-        return NotImplementedError
+        x_pred = linear_solve(linop, Ktb, config=linear_solve_config)
+        return x_pred
```

### Comparing `dprox-0.1.0/dprox/algo/hqs.py` & `dprox-0.1.1/dprox/algo/hqs.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/invert.py` & `dprox-0.1.1/dprox/algo/invert.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dprox.proxfn import least_squares, ext_sum_squares, least_squares
 from dprox.linop import Variable
 
 
-def get_least_square_solver(psi_fns, omega_fns, try_diagonalize, try_freq_diagonalize, lin_solver_kwargs):
+def get_least_square_solver(psi_fns, omega_fns, try_diagonalize, try_freq_diagonalize, linear_solve_config):
     prox_fns = psi_fns + omega_fns
 
     ext_sq = [fn for fn in omega_fns if isinstance(fn, ext_sum_squares)]
     for fn in ext_sq:
         other = [f for f in prox_fns if f is not fn]
         if all(isinstance(fn.linop, Variable) for fn in other):
             return ext_sq[0].setup([f.b for f in omega_fns if f is not fn and f not in ext_sq])
 
-    return least_squares(omega_fns, psi_fns, try_diagonalize, try_freq_diagonalize, lin_solver_kwargs=lin_solver_kwargs)
+    return least_squares(omega_fns, psi_fns, try_diagonalize, try_freq_diagonalize, linear_solve_config=linear_solve_config)
```

### Comparing `dprox-0.1.0/dprox/algo/lp/linear_solvers.py` & `dprox-0.1.1/dprox/proxfn/linalg/solve/plss.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,16 @@
 import torch
 import numpy as np
 from functools import partial
 
 
-def PCG(A, b, Minv=None, x_init=None, btol=1e-5, num_iters=100, verbose=False):
-    if Minv is None:
-        Minv = lambda x: x
-
-    if x_init is not None:
-        x = x_init
-    else:
-        x = torch.ones_like(b)
-        
-    r = A(x) - b
-    y = Minv(r)
-    # y = r
-    p = - y
-
-    bnorm = torch.linalg.norm(b)
-    
-    for iter in range(num_iters):
-        Ap = A(p)
-        ry = r.T @ y
-        alpha = ry / (p.T @ Ap)
-        x = x + alpha * p
-        r = r + alpha * Ap
-        y = Minv(r)
-        # y = r
-        beta = (r.T @ y) / ry
-        p = - y + beta * p
-        rnorm = torch.linalg.norm(r)
-        
-        if rnorm < btol * bnorm:
-            break
-    
-    if verbose:
-        print(iter + 1)
-    return x
-
-
 """Projected linear systems solver"""
-def PLSS(x0, A, b, atol=1e-6, btol=1e-6, maxiter=500, ord=2):
+def PLSS(A, b, x0=None, atol=1e-6, btol=1e-6, maxiter=500, ord=2):
+    x0 = torch.zeros_like(b)
+    
     m, n = A.shape
     x_min = xk = x0
     b_norm = torch.linalg.vector_norm(b, ord=ord)
     rk = A(xk) - b
     rk_norm_min = rk_norm = torch.linalg.vector_norm(rk, ord=ord)
     yk = A.adjoint(rk / rk_norm)
```

### Comparing `dprox-0.1.0/dprox/algo/lp/solvers.py` & `dprox-0.1.1/dprox/algo/lp/solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from collections import defaultdict
 from functools import partial
 
 import scipy
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 from tqdm import tqdm
 
-from .linear_solvers import PCG, PLSS
+from dprox.linalg.solve import PCG
 from .utils import *
 
 
 class LPConvergenceLoss(nn.Module):
     def __init__(self) -> None:
         super().__init__()
         
@@ -164,32 +163,32 @@
         ub[:-n] *= gamma_b * e[:-n]
         
         x = torch.zeros(n, 1, dtype=dtype, device=device)
         z = torch.zeros(m, 1, dtype=dtype, device=device)
         y = torch.zeros(m, 1, dtype=dtype, device=device)
         xtilde = torch.zeros_like(x)
     
-        btols = torch.logspace(-6, -10, 10000)
+        rtols = torch.logspace(-6, -10, 10000)
         history = defaultdict(lambda : [])
 
         # K = (AT @ A).to_dense() * rho + sigma * torch.eye(n, device=device, dtype=dtype)
         # L = torch.linalg.cholesky(K)  # K = L @ LT
         L = None
         
         ATAfun = LPATA_Func(A, AT, rho, sigma)
         ATAop = LinearOp(A_fun=ATAfun, AT_fun=ATAfun, shape=(n, n))
         
         M_constant = sigma * torch.ones(n, dtype=dtype, device=device)
         M = (M_constant + rho * (Acnorm ** 2)).unsqueeze(1)
         Minv = lambda x: x / M
         
         for k in tqdm(range(max_iters)):
-            btol = 1e-10 if k >= 10000 else btols[k]
+            rtol = 1e-10 if k >= 10000 else rtols[k]
             variables = x, z, y, xtilde
-            x, z, y, xtilde = self._solve_one_iter_precond(variables, c, A, AT, ATAop, Minv, lb, ub, btol, rho, sigma, alpha, L=L)
+            x, z, y, xtilde = self._solve_one_iter_precond(variables, c, A, AT, ATAop, Minv, lb, ub, rtol, rho, sigma, alpha, L=L)
                 
             if k % eval_freq == 0:
                 objval, r_norm, s_norm, eps_primal, eps_dual = self.eval_result(c, A, AT, d, e, gamma_c, gamma_b, x, z, y)                                
 
                 # update rho (residual balance)
                 if residual_balance and k % 1000 == 0 and k != 0:
                     if r_norm > 10 * eps_primal or eps_dual > 10 * s_norm:
@@ -237,24 +236,24 @@
                     
         objval, r_norm, s_norm, eps_primal, eps_dual = self.eval_result(c, A, AT, d, e, gamma_c, gamma_b, x, z, y)
         
         print(objval.item(), r_norm.item(), s_norm.item(), eps_primal.item(), eps_dual.item(), float(rho))
         results = objval, r_norm, s_norm, eps_primal, eps_dual
         return x * d / gamma_b, history, results
         
-    def _solve_one_iter_precond(self, variables, c, A, AT, ATAop, Minv, lb, ub, btol, rho, sigma, alpha, L=None):
+    def _solve_one_iter_precond(self, variables, c, A, AT, ATAop, Minv, lb, ub, rtol, rho, sigma, alpha, L=None):
         x, z, y, xtilde = variables
 
         # x-update
         right = sigma * x - c + AT @ (rho * z - y)
         if L is not None:  # seems very slow, why?
             tmp = torch.linalg.solve_triangular(L, right, upper=False)
             xtilde = torch.linalg.solve_triangular(L.T, tmp, upper=True)
         else:
-            xtilde = PCG(ATAop, right, Minv, x_init=xtilde.detach(), btol=btol, num_iters=200, verbose=False)
+            xtilde = PCG(ATAop, right, Minv, x0=xtilde.detach(), rtol=rtol, max_iters=200, verbose=False)
         ztilde = A @ (xtilde)
         x = alpha * xtilde + (1 - alpha) * x
 
         # z-update with relaxation
         z_hat = alpha * ztilde + (1 - alpha) * z
         z = torch.clip(z_hat + 1 / rho * y, min=lb, max=ub)
```

### Comparing `dprox-0.1.0/dprox/algo/lp/utils.py` & `dprox-0.1.1/dprox/algo/lp/utils.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/opt/absorb.py` & `dprox-0.1.1/dprox/algo/opt/absorb.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/opt/equil.py` & `dprox-0.1.1/dprox/algo/opt/equil.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/opt/merge.py` & `dprox-0.1.1/dprox/algo/opt/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Merge proximal operators together.
 
-from proximal.prox_fns import sum_squares, zero_prox
+# from proximal.prox_fns import sum_squares, zero_prox
 import numpy as np
 
 
 def merge_all(prox_fns):
     """Merge as many prox functions as possible.
     """
     while True:
```

### Comparing `dprox-0.1.0/dprox/algo/pc.py` & `dprox-0.1.1/dprox/algo/pc.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/pgd.py` & `dprox-0.1.1/dprox/algo/pgd.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/problem.py` & `dprox-0.1.1/dprox/algo/problem.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dprox.linop.constaints import matmul, less, equality
-from . import lp
 from typing import List, Union
 
 import torch
 
 from dprox.proxfn import ProxFn
+from dprox.linalg import LinearSolveConfig
 
 from . import opt
+from . import lp
 from .admm import ADMM, ADMM_vxu, LinearizedADMM
 from .base import Algorithm
 from .hqs import HQS
 from .pc import PockChambolle
 from .pgd import ProximalGradientDescent
 from .special import DEQSolver
 
@@ -57,42 +58,42 @@
         self,
         prox_fns: Union[ProxFn, List[ProxFn]],
         constraints=[],
         absorb=True,
         merge=True,
         try_diagonalize=True,
         try_freq_diagonalize=True,
-        lin_solver_kwargs={},
+        linear_solve_config=LinearSolveConfig(),
     ):
         self.prob = None
         if isinstance(prox_fns, matmul):
             self.prob = LPProblem(prox_fns, constraints)
-            return 
-        
+            return
+
         if isinstance(prox_fns, ProxFn):
             prox_fns = [prox_fns]
         self.prox_fns = prox_fns
 
         self.absorb = absorb
         self.merge = merge
 
         self.solver_args = dict(
             try_diagonalize=try_diagonalize,
             try_freq_diagonalize=try_freq_diagonalize,
-            lin_solver_kwargs=lin_solver_kwargs,
+            linear_solve_config=linear_solve_config,
         )
 
     @property
     def objective(self):
         return self.prox_fns
 
     def solve(self, method='admm', device='cuda', **kwargs):
         if self.prob is not None:
             return self.prob.solve()
-        
+
         # TODO: optimize has bug when scale is absorbed in test_ml_problems
         # prox_fns = optimize(self.prox_fns, merge=self.merge, absorb=self.absorb)
         prox_fns = self.prox_fns
         solver = compile(prox_fns, method=method, device=device, **self.solver_args)
         results = solver.solve(**kwargs)
         return results
```

### Comparing `dprox-0.1.0/dprox/algo/special/deq.py` & `dprox-0.1.1/dprox/algo/special/deq.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/special/deq_utils/jacobian.py` & `dprox-0.1.1/dprox/algo/special/deq_utils/jacobian.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/special/deq_utils/layer_utils.py` & `dprox-0.1.1/dprox/algo/special/deq_utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/special/deq_utils/optimizations.py` & `dprox-0.1.1/dprox/algo/special/deq_utils/optimizations.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/special/deq_utils/radam.py` & `dprox-0.1.1/dprox/algo/special/deq_utils/radam.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/special/deq_utils/solvers.py` & `dprox-0.1.1/dprox/algo/special/deq_utils/solvers.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/special/unroll.py` & `dprox-0.1.1/dprox/algo/special/unroll.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/tune/autotune.py` & `dprox-0.1.1/dprox/algo/tune/autotune.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/algo/tune/dpir.py` & `dprox-0.1.1/dprox/algo/tune/dpir.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/linop/__init__.py` & `dprox-0.1.1/dprox/linop/__init__.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/linop/base.py` & `dprox-0.1.1/dprox/linop/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/linop/blackbox.py` & `dprox-0.1.1/dprox/linop/blackbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,43 +13,47 @@
     forward : function
         Applies the operator to an input array and writes to an output.
     adjoint : function
         Applies the adjoint operator to an input array and writes to an output.
     norm_bound : float, optional
         An upper bound on the spectral norm of the operator.
     """
-    def get_black_box(arg):
-        return BlackBox(arg, forward, adjoint, diag, norm_bound)
+    def get_black_box(*args):
+        return BlackBox(*args, forward=forward, adjoint=adjoint, diag=diag, norm_bound=norm_bound)
     return get_black_box
 
 
 class BlackBox(LinOp):
     """A black-box lin op specified by the user.
     """
 
-    def __init__(self, arg, forward, adjoint, diag=None, norm_bound=None):
+    def __init__(self, *args, forward=None, adjoint=None, diag=None, norm_bound=None):
         self._forward = forward
         self._adjoint = adjoint
         self._norm_bound = norm_bound
         self._diag = diag
-        super(BlackBox, self).__init__([arg])
+        super(BlackBox, self).__init__(args)
 
-    def forward(self, inputs):
+    def forward(self, *inputs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
-        return self._forward(inputs, self.step)
+        if len(inputs) == 1:
+            return self._forward(inputs[0], step=self.step)
+        return self._forward(*inputs, step=self.step)
 
-    def adjoint(self, inputs):
+    def adjoint(self, *inputs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
-        return self._adjoint(inputs, self.step)
+        if len(inputs) == 1:
+            return self._adjoint(inputs[0], step=self.step)
+        return self._adjoint(*inputs, step=self.step)
 
     def norm_bound(self, input_mags):
         """Gives an upper bound on the magnitudes of the outputs given inputs.
 
         Parameters
         ----------
         input_mags : list
```

### Comparing `dprox-0.1.0/dprox/linop/comp_graph.py` & `dprox-0.1.1/dprox/linop/comp_graph.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/linop/constant.py` & `dprox-0.1.1/dprox/linop/constant.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             value = torch.tensor(value)
         self._value = value
 
     # ---------------------------------------------------------------------------- #
     #                                  Computation                                 #
     # ---------------------------------------------------------------------------- #
 
-    def forward(self, *value):
+    def forward(self, *value, **kwargs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
         return self.value
 
-    def adjoint(self, value):
+    def adjoint(self, value, **kwargs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
         return self.value*0
 
     # ---------------------------------------------------------------------------- #
```

### Comparing `dprox-0.1.0/dprox/linop/conv.py` & `dprox-0.1.1/dprox/linop/conv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from typing import Union
+
 import numpy as np
 import torch
 import torch.nn.functional as F
 import torch.nn as nn
 
-from dprox.utils.misc import batchify, to_ndarray
+from dprox.utils.misc import batchify, to_ndarray, to_torch_tensor
 from dprox.utils.psf2otf import psf2otf
 
 from .base import LinOp
+from .placeholder import Placeholder
 
 
 class conv(LinOp):
     """Circular convolution of the input with a kernel.
     """
 
     def __init__(self, arg, kernel):
@@ -22,21 +25,21 @@
         if shape not in self.cache:
             _, C, H, W = shape
             FB = psf2otf(self.kernel, [H, W, C])
             FB = batchify(torch.from_numpy(FB))
             self.cache[shape] = FB
         return self.cache[shape]
 
-    def forward(self, input):
+    def forward(self, input, **kwargs):
         FB = self._FB(input.shape).to(input.device)
         Fx = torch.fft.fftn(input, dim=[-2, -1])
         output = torch.real(torch.fft.ifftn(FB * Fx, dim=[-2, -1])).float()
         return output
 
-    def adjoint(self, input):
+    def adjoint(self, input, **kwargs):
         FB = self._FB(input.shape).to(input.device)
         Fx = torch.fft.fftn(input, dim=[-2, -1])
         output = torch.real(torch.fft.ifftn(torch.conj(FB) * Fx, dim=[-2, -1])).float()
         return output
 
     def is_diag(self, freq=False):
         return freq and self.input_nodes[0].is_diag(freq)
@@ -78,21 +81,33 @@
     return otf
 
 
 class conv_doe(LinOp):
     """Circular convolution of the input with a kernel.
     """
 
-    def __init__(self, arg, psf, circular=False):
+    def __init__(
+        self,
+        arg: LinOp,
+        psf: Union[Placeholder, torch.Tensor, np.array],
+        circular: bool = False
+    ):
         super().__init__([arg])
-        self.psf = nn.parameter.Parameter(psf)
+        self._psf = psf
         self.circular = circular
 
-    def forward(self, img):
-        psf = self.unwrap(self.psf).to(img.device)
+        if isinstance(psf, Placeholder):
+            def on_change(val):
+                self.psf = nn.parameter.Parameter(val)
+            self._psf.change(on_change)
+        else:
+            self.psf = nn.parameter.Parameter(to_torch_tensor(psf, batch=True))
+
+    def forward(self, img, **kwargs):
+        psf = self.psf.to(img.device)
 
         if not self.circular:
             # linearized conv
             target_side_length = 2 * img.shape[2]
             height_pad = (target_side_length - img.shape[2]) / 2
             width_pad = (target_side_length - img.shape[3]) / 2
             pad_top, pad_bottom = int(np.ceil(height_pad)), int(np.floor(height_pad))
@@ -104,15 +119,15 @@
         output = torch.real(torch.fft.ifftn(otf * Fx, dim=[-2, -1])).float()
 
         if not self.circular:
             output = output[:, :, pad_top:-pad_bottom, pad_left:-pad_right]
 
         return output
 
-    def adjoint(self, img):
+    def adjoint(self, img, **kwargs):
         psf = self.unwrap(self.psf).to(img.device)
 
         if not self.circular:
             # linearized conv
             target_side_length = 2 * img.shape[2]
             height_pad = (target_side_length - img.shape[2]) / 2
             width_pad = (target_side_length - img.shape[3]) / 2
```

### Comparing `dprox-0.1.0/dprox/linop/grad.py` & `dprox-0.1.1/dprox/linop/grad.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/linop/scale.py` & `dprox-0.1.1/dprox/linop/scale.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,22 +13,22 @@
         self.scalar = scalar
         super(scale, self).__init__([arg])
 
     # ---------------------------------------------------------------------------- #
     #                                  Computation                                 #
     # ---------------------------------------------------------------------------- #
 
-    def forward(self, input):
+    def forward(self, input, **kwargs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
         return input * self.scalar
 
-    def adjoint(self, input):
+    def adjoint(self, input, **kwargs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
         return self.forward(input)
 
     # ---------------------------------------------------------------------------- #
```

### Comparing `dprox-0.1.0/dprox/linop/subsample.py` & `dprox-0.1.1/dprox/linop/subsample.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
         super(mosaic, self).__init__([arg])
         self.cache = {}
 
     # ---------------------------------------------------------------------------- #
     #                                  Computation                                 #
     # ---------------------------------------------------------------------------- #
 
-    def forward(self, input):
+    def forward(self, input, **kwargs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
         mask = self._mask(input.shape).to(input.device)
         return mask * input
 
-    def adjoint(self, input):
+    def adjoint(self, input, **kwargs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
         return self.forward(input)
 
     @staticmethod
```

### Comparing `dprox-0.1.0/dprox/linop/sum.py` & `dprox-0.1.1/dprox/linop/sum.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 class sum(LinOp):
     """Sums its inputs.
     """
 
     def __init__(self, input_nodes):
         super(sum, self).__init__(input_nodes)
 
-    def forward(self, *inputs):
+    def forward(self, *inputs, **kwargs):
         """ Just sum all the inputs, all inputs should have the same shape
         """
         output = torch.zeros_like(inputs[0])
         for input in inputs:
             output += input.to(output.device)
         return output
 
-    def adjoint(self, input):
+    def adjoint(self, input, **kwargs):
         """ The adjoint of sum spread of the input to all its child
         """
         outputs = LinOp.MultOutput()
         for _ in self.input_nodes:
             outputs.append(input)
         if len(outputs) > 1:
             return outputs
@@ -75,27 +75,27 @@
 
 
 class copy(sum):
 
     def __init__(self, arg):
         super(copy, self).__init__([arg])
 
-    def forward(self, inputs):
+    def forward(self, inputs, **kwargs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
-        return super(copy, self).adjoint(inputs)
+        return super(copy, self).adjoint(inputs, **kwargs)
 
-    def adjoint(self, *inputs):
+    def adjoint(self, *inputs, **kwargs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
-        return super(copy, self).forward(*inputs)
+        return super(copy, self).forward(*inputs, **kwargs)
 
     def norm_bound(self, input_mags):
         """Gives an upper bound on the magnitudes of the outputs given inputs.
 
         Parameters
         ----------
         input_mags : list
```

### Comparing `dprox-0.1.0/dprox/linop/variable.py` & `dprox-0.1.1/dprox/linop/variable.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,22 +17,22 @@
         self.varname = name
         self.initval = None
 
     # ---------------------------------------------------------------------------- #
     #                                  Computation                                 #
     # ---------------------------------------------------------------------------- #
     
-    def forward(self, inputs):
+    def forward(self, inputs, **kwargs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
         return inputs
 
-    def adjoint(self, inputs):
+    def adjoint(self, inputs, **kwargs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
         return inputs
 
     # ---------------------------------------------------------------------------- #
```

### Comparing `dprox-0.1.0/dprox/linop/vstack.py` & `dprox-0.1.1/dprox/linop/vstack.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,24 @@
     def __init__(self, input_nodes):
         super(vstack, self).__init__(input_nodes)
 
     # ---------------------------------------------------------------------------- #
     #                                  Computation                                 #
     # ---------------------------------------------------------------------------- #
 
-    def forward(self, *inputs):
+    def forward(self, *inputs, **kwargs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
         if len(inputs) > 1:
             return LinOp.MultOutput(inputs)
         return inputs[0]
 
-    def adjoint(self, *inputs):
+    def adjoint(self, *inputs, **kwargs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
         if len(inputs) > 1:
             return LinOp.MultOutput(inputs)
         return inputs[0]
@@ -86,27 +86,27 @@
 class split(vstack):
 
     def __init__(self, output_nodes):
         self.output_nodes = output_nodes
         self.input_nodes = []
         super(split, self).__init__(output_nodes)
 
-    def forward(self, *inputs):
+    def forward(self, *inputs, **kwargs):
         """The forward operator.
 
         Reads from inputs and writes to outputs.
         """
-        return super(split, self).adjoint(*inputs)
+        return super(split, self).adjoint(*inputs, **kwargs)
 
-    def adjoint(self, *inputs):
+    def adjoint(self, *inputs, **kwargs):
         """The adjoint operator.
 
         Reads from inputs and writes to outputs.
         """
-        return super(split, self).forward(*inputs)
+        return super(split, self).forward(*inputs, **kwargs)
 
     def norm_bound(self, input_mags):
         """Gives an upper bound on the magnitudes of the outputs given inputs.
 
         Parameters
         ----------
         input_mags : list
```

### Comparing `dprox-0.1.0/dprox/proxfn/base.py` & `dprox-0.1.1/dprox/proxfn/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/fast/cs.py` & `dprox-0.1.1/dprox/proxfn/fast/cs.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/fast/csmri.py` & `dprox-0.1.1/dprox/proxfn/fast/csmri.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/fast/pr.py` & `dprox-0.1.1/dprox/proxfn/fast/pr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/fast/spi.py` & `dprox-0.1.1/dprox/proxfn/fast/spi.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/fast/sr.py` & `dprox-0.1.1/dprox/proxfn/fast/sr.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/linalg/custom.py` & `dprox-0.1.1/dprox/linalg/custom.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import dprox
 
 from .solve import SOLVERS
 
 
 @dataclass
 class LinearSolveConfig:
-    tol: float = 1e-5
+    rtol: float = 1e-6
     max_iters: int = 100
     verbose: bool = False
     solver_type: str = 'cg'
     solver_kwargs: dict = field(default_factory=dict)
 
 
 def build_solver(config: LinearSolveConfig):
     solve_fn = SOLVERS[config.solver_type]
     solve_fn = partial(solve_fn,
-                       tol=config.tol,
+                       rtol=config.rtol,
                        max_iters=config.max_iters,
                        verbose=config.verbose,
                        **config.solver_kwargs)
     return solve_fn
 
 
 def trainable_parameters(module):
```

### Comparing `dprox-0.1.0/dprox/proxfn/linalg/solve/bicgstab.py` & `dprox-0.1.1/dprox/proxfn/linalg/solve/bicgstab.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/linalg/solve/broyden.py` & `dprox-0.1.1/dprox/proxfn/linalg/solve/broyden.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/linalg/solve/cg.py` & `dprox-0.1.1/dprox/linalg/solve/cg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import torch
 import numpy as np
 
 # TODO: standardize the stopping criterion
+RTOL = 1e-6
+MAX_ITERS = 100
 
 
 def conjugate_gradient(
     A, b, 
-    x0=None, tol=1e-6, max_iters=100, verbose=False
+    x0=None, rtol=RTOL, max_iters=MAX_ITERS, verbose=False
 ):
 
     # Temp vars
     x = torch.zeros_like(b)
     r = torch.zeros_like(b)
     Ap = torch.zeros_like(b)
 
     # Initialize x
     if x0 is not None:
         x = x0
 
     # Compute residual
     r = A(x)
-    r *= -1.0
+    r *= - 1.0
     r += b
 
-    cg_tol = tol * torch.linalg.norm(b.ravel(), 2)  # Relative tol
+    cg_tol = rtol * torch.linalg.norm(b.ravel(), 2)  # Relative tolerence
 
     # CG iteration
     gamma_1 = p = None
     cg_iter = np.minimum(max_iters, np.prod(b.shape))
     for iter in range(cg_iter):
 
         # Check for convergence
@@ -63,15 +65,15 @@
         print(f'Not converged, r norm={normr.item()}')
     
     return x
 
 
 def conjugate_gradient2(
     A, b, 
-    x0=None, tol=1e-5, max_iters=500, verbose=False
+    x0=None, rtol=RTOL, max_iters=500, verbose=False
 ):
     # Solves A x = b
     x = torch.ones_like(b)
 
     if x0 is not None:
         print('use x init')
         x = x0
@@ -85,62 +87,63 @@
         alpha = rnorm / (d.ravel() @ Ad.ravel())
         x = x + alpha * d
         r = r - alpha * Ad
         rnorm2 = r.ravel() @ r.ravel()
         beta = rnorm2 / rnorm
         rnorm = rnorm2
         d = r + beta * d
-        if rnorm2 < tol:
-            if verbose: print(f'converge at iter={iter}, tol={tol}')
+        if rnorm2 < rtol:
+            if verbose: print(f'converge at iter={iter}, rtol={rtol}')
             break
 
     res = b - A(x)
     res = res.ravel() @ res.ravel()
     return x
 
 
-
-def PCG(A, b, Minv=None, x_init=None, btol=1e-5, num_iters=100, verbose=False):
+def PCG(
+    A, b, 
+    Minv=None, x0=None, rtol=RTOL, max_iters=MAX_ITERS, verbose=False
+):
+    """Preconditioned Conjugate Gradient Method"""
     if Minv is None:
         Minv = lambda x: x
 
-    if x_init is not None:
-        x = x_init
+    if x0 is not None:
+        x = x0
     else:
         x = torch.ones_like(b)
         
     r = A(x) - b
     y = Minv(r)
-    # y = r
     p = - y
 
-    bnorm = torch.linalg.norm(b)
+    bnorm = torch.linalg.vector_norm(b.ravel())
     
-    for iter in range(num_iters):
+    for iter in range(max_iters):
         Ap = A(p)
-        ry = r.T @ y
-        alpha = ry / (p.T @ Ap)
+        ry = r.ravel() @ y.ravel()
+        alpha = ry / (p.ravel() @ Ap.ravel())
         x = x + alpha * p
         r = r + alpha * Ap
         y = Minv(r)
         # y = r
-        beta = (r.T @ y) / ry
+        beta = (r.ravel() @ y.ravel()) / ry
         p = - y + beta * p
-        rnorm = torch.linalg.norm(r)
+        rnorm = torch.linalg.vector_norm(r.ravel())
         
-        if rnorm < btol * bnorm:
+        if rnorm < rtol * bnorm:
             break
     
     if verbose:
-        print(iter + 1)
+        print('#IT:', iter + 1)
     return x
 
 
-
-def cg_batch(A_bmm, B, M_bmm=None, X0=None, rtol=1e-5, atol=0., maxiter=None, verbose=False):
+def cg_batch(A_bmm, B, M_bmm=None, X0=None, rtol=RTOL, atol=0., maxiter=None, verbose=False):
     """Solves a batch of PD matrix linear systems using the preconditioned CG algorithm.
     This function solves a batch of matrix linear systems of the form
         A_i X_i = B_i,  i=1,...,K,
     where A_i is a n x n positive definite matrix and B_i is a n x m matrix,
     and X_i is the n x m matrix representing the solution for the ith system.
     Args:
         A_bmm: A callable that performs a batch matrix multiply of A and a K x n x m matrix.
@@ -228,18 +231,18 @@
             break
 
     end = time.perf_counter()
 
     if verbose:
         if optimal:
             print("Terminated in %d steps (reached maxiter). Took %.3f ms." %
-                  (k, (end - start) * 1000))
+                  (k, (end - start) * MAX_ITERS0))
         else:
             print("Terminated in %d steps (optimal). Took %.3f ms." %
-                  (k, (end - start) * 1000))
+                  (k, (end - start) * MAX_ITERS0))
 
 
     info = {
         "niter": k,
         "optimal": optimal
     }
```

### Comparing `dprox-0.1.0/dprox/proxfn/linalg/solve/gmres.py` & `dprox-0.1.1/dprox/proxfn/linalg/solve/gmres.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/nlm/nlm.py` & `dprox-0.1.1/dprox/proxfn/nlm/nlm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/norm.py` & `dprox-0.1.1/dprox/proxfn/norm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/base.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/base.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/composite.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/composite.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/TV_denoising.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/TV_denoising.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/basicblock.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_dncnn.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/network_dncnn.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/network_ffdnet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/network_unet.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/network_unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/__init__.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/conv.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/grunet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/layer.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/qrnn3d.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/batchnorm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/comm.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/replicate.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/qrnn/sync_batchnorm/unittest.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/unet/basicblock.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/models/unet/unet.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/denoisers/wrapper.py` & `dprox-0.1.1/dprox/proxfn/pnp/denoisers/wrapper.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/pnp/prior.py` & `dprox-0.1.1/dprox/proxfn/pnp/prior.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/proxfn/unrolling/dgu.py` & `dprox-0.1.1/dprox/proxfn/unrolling/dgu.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/utils/examples/csmri/common.py` & `dprox-0.1.1/dprox/utils/examples/csmri/common.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/utils/examples/csmri/dataset.py` & `dprox-0.1.1/dprox/utils/examples/csmri/dataset.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/utils/examples/csmri/misc.py` & `dprox-0.1.1/dprox/utils/examples/csmri/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,22 +38,23 @@
     target = torch.from_numpy(target)
     mask = torch.from_numpy(mask)
 
     y0 = fft2(target)
     y0[:, ~mask] = 0
     Aty0 = ifft2(y0)
 
+    # TODO: all sample should return [1, C, H, W] tensor, or [H, W, C] numpy
     y0 = y0.squeeze()  # [1, H, W] -> [H, W]
     Aty0 = Aty0.squeeze()
     target = target.squeeze()
 
     Aty0 = to_torch_tensor(Aty0, batch=True)
     y0 = to_torch_tensor(y0, batch=True)
     target = to_torch_tensor(target, batch=True)
-    mask = to_torch_tensor(mask, batch=True)
+    mask = to_torch_tensor(mask.unsqueeze(0), batch=True)
     return Aty0.real, y0, target, mask
 
 
 class Dataset(SingleImageDataset):
     def __init__(self, root):
         super().__init__(root, mode='gray')
         mask = loadmat(get_path('data/csmri/masks/radial_128_2.mat')).get('mask')
```

### Comparing `dprox-0.1.0/dprox/utils/examples/derain/custom_linop.py` & `dprox-0.1.1/dprox/utils/examples/derain/custom_linop.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/utils/examples/energy_system/__init__.py` & `dprox-0.1.1/dprox/utils/examples/energy_system/__init__.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/utils/examples/optic/unet.py` & `dprox-0.1.1/dprox/utils/examples/optic/unet.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/utils/examples/restoration.py` & `dprox-0.1.1/dprox/utils/examples/restoration.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/dprox/utils/init/mosaic.py` & `dprox-0.1.1/dprox/utils/init/mosaic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import cv2
 import torch
 import torch.nn as nn
 
+
 def uint2tensor4(img):
     if img.ndim == 2:
         img = np.expand_dims(img, axis=2)
     return torch.from_numpy(np.ascontiguousarray(img)).permute(2, 0, 1).float().div(255.).unsqueeze(0)
 
 def tensor2uint(img):
     img = img.data.squeeze().float().clamp(0, 1).cpu().numpy()
```

### Comparing `dprox-0.1.0/dprox/utils/init/sr.py` & `dprox-0.1.1/dprox/utils/init/sr.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+
 def shift_pixel(x, sf, upper_left=True):
     """shift pixel for super-resolution with different scale factors
     Args:
         x: WxHxC or WxH
         sf: scale factor
         upper_left: shift direction
     """
```

### Comparing `dprox-0.1.0/dprox.egg-info/SOURCES.txt` & `dprox-0.1.1/dprox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 dprox/algo/base.py
 dprox/algo/hqs.py
 dprox/algo/invert.py
 dprox/algo/pc.py
 dprox/algo/pgd.py
 dprox/algo/problem.py
 dprox/algo/lp/__init__.py
-dprox/algo/lp/linear_solvers.py
 dprox/algo/lp/solvers.py
 dprox/algo/lp/utils.py
 dprox/algo/opt/__init__.py
 dprox/algo/opt/absorb.py
 dprox/algo/opt/equil.py
 dprox/algo/opt/merge.py
 dprox/algo/special/__init__.py
@@ -31,14 +30,20 @@
 dprox/algo/special/deq_utils/optimizations.py
 dprox/algo/special/deq_utils/radam.py
 dprox/algo/special/deq_utils/solvers.py
 dprox/algo/tune/__init__.py
 dprox/algo/tune/autotune.py
 dprox/algo/tune/dpir.py
 dprox/algo/tune/learnable.py
+dprox/linalg/__init__.py
+dprox/linalg/custom.py
+dprox/linalg/solve/__init__.py
+dprox/linalg/solve/cg.py
+dprox/linalg/solve/minres.py
+dprox/linalg/solve/plss.py
 dprox/linop/__init__.py
 dprox/linop/base.py
 dprox/linop/blackbox.py
 dprox/linop/comp_graph.py
 dprox/linop/constaints.py
 dprox/linop/constant.py
 dprox/linop/conv.py
@@ -57,20 +62,16 @@
 dprox/proxfn/sum_square.py
 dprox/proxfn/fast/__init__.py
 dprox/proxfn/fast/cs.py
 dprox/proxfn/fast/csmri.py
 dprox/proxfn/fast/pr.py
 dprox/proxfn/fast/spi.py
 dprox/proxfn/fast/sr.py
-dprox/proxfn/linalg/__init__.py
-dprox/proxfn/linalg/custom.py
-dprox/proxfn/linalg/solve/__init__.py
 dprox/proxfn/linalg/solve/bicgstab.py
 dprox/proxfn/linalg/solve/broyden.py
-dprox/proxfn/linalg/solve/cg.py
 dprox/proxfn/linalg/solve/gmres.py
 dprox/proxfn/linalg/solve/plss.py
 dprox/proxfn/nlm/__init__.py
 dprox/proxfn/nlm/nlm.py
 dprox/proxfn/nlm/patch_nlm.py
 dprox/proxfn/pnp/__init__.py
 dprox/proxfn/pnp/prior.py
@@ -119,15 +120,17 @@
 dprox/utils/examples/optic/common.py
 dprox/utils/examples/optic/doe_model.py
 dprox/utils/examples/optic/unet.py
 dprox/utils/init/__init__.py
 dprox/utils/init/mosaic.py
 dprox/utils/init/sr.py
 tests/test_algorithms.py
+tests/test_derain.py
 tests/test_energy_system.py
 tests/test_inverse_problems.py
+tests/test_jd23.py
 tests/test_linear_solver.py
 tests/test_linear_solver_grad.py
 tests/test_linear_solver_torch.py
 tests/test_linop.py
 tests/test_linop_primitive.py
 tests/test_ml_problems.py
```

### Comparing `dprox-0.1.0/setup.py` & `dprox-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     'proximal',
     'opencv-python'
 ]
 
 
 setup(
     name='dprox',
-    description='A domain-specific language (DSL) and compiler that transforms optimization problems into differentiable proximal solvers.',
+    description='A domain-specific language and compiler that transforms optimization problems into differentiable proximal solvers.',
     url='https://github.com/princeton-computational-imaging/Delta-Prox',
     author='Zeqiang Lai',
     author_email='laizeqiang@outlook.com',
     packages=find_packages(),
-    version='0.1.0',
+    version='0.1.1',
     include_package_data=True,
     install_requires=deps,
 )
```

### Comparing `dprox-0.1.0/tests/test_algorithms.py` & `dprox-0.1.1/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/tests/test_inverse_problems.py` & `dprox-0.1.1/tests/test_jd23.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,25 @@
 from dprox import *
 from dprox.utils import *
-from dprox.utils import examples
+from dprox.utils.examples import *
+from dprox.linalg import LinearSolveConfig
 
-
-def test_csmri():
-    x0, y0, gt, mask = examples.csmri.sample()
+def test_jd2():
+    img = sample('face')
+    img = to_torch_tensor(img, batch=True).float()
+    psf = point_spread_function(15, 5)
+    b = blurring(img, psf)
+    b = mosaicing(b)
 
     x = Variable()
-    y = Placeholder()
-    data_term = csmri(x, mask, y)
-    reg_term = deep_prior(x, denoiser='unet')
-    prob = Problem(data_term + reg_term)
+    data_term = sum_squares(mosaic(conv(x, psf)) - b)
+    reg_term = deep_prior(x, denoiser='ffdnet_color')
+    prob = Problem(data_term + reg_term, linear_solve_config=LinearSolveConfig(max_iters=500))
 
-    y.value = y0
     max_iter = 24
-    rhos, sigmas = log_descent(30, 20, max_iter)
-    prob.solve(
-        method='admm',
-        device='cuda',
-        x0=x0, rhos=rhos, lams={reg_term: sigmas}, max_iter=max_iter, pbar=True
-    )
-    out = x.value.real
-
-    print(psnr(out, gt)) 
-    assert abs(psnr(out, gt) - 42.6) < 0.1
-    
-    
-def test_deconv():
-    img = examples.sample('face')
-    psf = examples.point_spread_function(15, 5)
-    b = examples.blurring(img, psf)
-
-    x = Variable()
-    data_term = sum_squares(conv(x, psf) - b)
-    reg_term = deep_prior(x, denoiser='ffdnet_color')
-    reg2 = nonneg(x)
-    prob = Problem(data_term + reg_term + reg2)
+    rhos, sigmas = log_descent(35, 30, max_iter)
+    out = prob.solve(method='admm', x0=b, rhos=rhos, lams={reg_term: sigmas}, max_iter=24, pbar=True)
 
-    out = prob.solve(method='admm', x0=b, pbar=True)
+    imshow(out)
+    print(psnr(out, img))  # 29.689
 
-    print(psnr(out, img)) 
-    assert abs(psnr(out, img) - 31.9) < 0.1
-    
+    assert psnr(out, img) - 29.9 < 0.1
```

### Comparing `dprox-0.1.0/tests/test_linear_solver_grad.py` & `dprox-0.1.1/tests/test_linear_solver_grad.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def auto_diff(seed):
     torch.manual_seed(seed)
     theta = torch.randn((32,32), requires_grad=True)
     K = theta * 2
     x = torch.randn((32))
-    b = K@x
+    b = K @ x
     b = b.clone().detach().requires_grad_(True)
 
     xhat = torch.linalg.solve(K, b)
 
     loss = xhat.mean()
     loss.backward()
 
@@ -28,15 +28,15 @@
 
 
 def differentiate_dloss_db(seed):
     torch.manual_seed(seed)
     theta = torch.randn((32,32), requires_grad=True)
     K = theta * 2
     x = torch.randn((32))
-    b = K@x
+    b = K @ x
     b = b.clone().detach().requires_grad_(True)
 
     xhat = torch.linalg.solve(K, b)
     xhat.retain_grad()
 
     loss = xhat.mean()
     loss.backward()
@@ -48,15 +48,15 @@
     
     
 def matrix_differentiate_dloss_dtheta(seed):
     torch.manual_seed(seed)
     theta = torch.randn((32,32), requires_grad=True)
     K = theta * 2
     x = torch.randn((32))
-    b = K@x
+    b = K @ x
     b = b.clone().detach().requires_grad_(True)
 
     xhat = torch.linalg.solve(K, b)
     xhat.retain_grad()
 
     loss = xhat.mean()
     loss.backward()
@@ -74,15 +74,15 @@
 
     
 def matrix_free_differentiate_dloss_dtheta(seed):
     torch.manual_seed(seed)
     theta = torch.randn((32,32), requires_grad=True)
     K = theta * 2
     x = torch.randn((32))
-    b = K@x
+    b = K @ x
     b = b.clone().detach().requires_grad_(True)
 
     xhat = torch.linalg.solve(K, b)
     xhat.retain_grad()
 
     loss = xhat.mean()
     loss.backward()
```

### Comparing `dprox-0.1.0/tests/test_linear_solver_torch.py` & `dprox-0.1.1/tests/test_linear_solver_torch.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,43 +28,49 @@
 
     def adjoint(self, x):
         return self.P.T @ self.P @ x
 
 
 def test_linear_solver_torch_forward():
     torch.manual_seed(seed)
-
-    P = torch.randn(5, 5)
-    A = P.T @ P
-    x = torch.randn(5)
+    
+    dtype = torch.float64
+    P = torch.randn(5, 5, dtype=dtype)
+    I = torch.eye(5, dtype=dtype)
+    mu = 0.5
+    A = P.T @ P + mu * I
+    x = torch.randn(5, dtype=dtype)
     b = A @ x
     b = b.clone().detach().requires_grad_(True)
 
     A = LinOp(A)
-    xhat = dprox.proxfn.linalg.linear_solve(A, b)
+    # xhat = dprox.linalg.linear_solve(A, b)
+    # xhat = dprox.linalg.solve.conjugate_gradient(A, b, max_iters=100)
+    xhat = dprox.linalg.solve.PCG(A, b, max_iters=100)    
 
+    print(xhat.dtype)
     print(torch.mean(torch.abs(xhat - x)))
     print(x)
     print(xhat)
-    assert torch.allclose(x, xhat, rtol=1e-3)
+    assert torch.allclose(x, xhat, rtol=1e-6)
 
 
 def test_linear_solver_torch_backward_db():
     # gradient with implicit differentiation
     torch.manual_seed(seed)
 
     P = torch.randn(5, 5)
     A = P.T @ P
     x = torch.randn(5)
     b = A @ x
     b = b.clone().detach().requires_grad_(True)
 
     A = LinOp(A)
 
-    xhat = dprox.proxfn.linalg.linear_solve(A, b)
+    xhat = dprox.linalg.linear_solve(A, b)
 
     xhat.mean().backward()
 
     grad1 = b.grad
 
     # gradient with unrolling
     torch.manual_seed(seed)
@@ -73,15 +79,15 @@
     A = P.T @ P
     x = torch.randn(5)
     b = A @ x
     b = b.clone().detach().requires_grad_(True)
 
     A = LinOp(A)
 
-    xhat = dprox.proxfn.linalg.solve.conjugate_gradient(A, b)
+    xhat = dprox.linalg.solve.conjugate_gradient(A, b)
 
     xhat.mean().backward()
 
     grad2 = b.grad
 
     print(grad1)
     print(grad2)
@@ -97,30 +103,30 @@
     A = SymmetricLinOp(P)
 
     x = torch.randn(5)
     with torch.no_grad():
         b = A(x)
     b = b.clone().detach().requires_grad_(True)
 
-    xhat = dprox.proxfn.linalg.linear_solve(A, b)
+    xhat = dprox.linalg.linear_solve(A, b)
     xhat.mean().backward()
     grad1 = A.P.grad
 
     # gradient with unrolling
     torch.manual_seed(seed)
 
     P = torch.randn(5, 5)
     A = SymmetricLinOp(P)
 
     x = torch.randn(5)
     with torch.no_grad():
         b = A(x)
     b = b.clone().detach().requires_grad_(True)
 
-    xhat = dprox.proxfn.linalg.solve.conjugate_gradient(A, b)
+    xhat = dprox.linalg.solve.conjugate_gradient(A, b)
     xhat.mean().backward()
     grad2 = A.P.grad
 
     # summary
     print('dtheta')
     print(grad1)
     print(grad2)
@@ -129,49 +135,53 @@
     assert torch.allclose(grad1, grad2, rtol=1e-2, atol=1e-2)
 
 
 def test_linear_solver_torch_backward_dtheta2():
     # gradient with implicit differentiation
     torch.manual_seed(seed)
 
-    P = torch.randn(5, 5)
-    A = LinOp(P @ P.T)
+    dtype = torch.float64
+    P = torch.randn(5, 5, dtype=dtype)
+    I = torch.eye(5, dtype=dtype)
+    mu = 0.5
+    A = LinOp(P @ P.T + mu * I)
 
-    x = torch.randn(5)
+    x = torch.randn(5, dtype=dtype)
     with torch.no_grad():
         b = A(x)
     b = b.clone().detach().requires_grad_(True)
 
-    xhat = dprox.proxfn.linalg.linear_solve(A, b)
+    xhat = dprox.linalg.linear_solve(A, b)
     xhat.mean().backward()
     grad1 = A.A.grad
 
     # gradient with unrolling
     # warning:
     torch.manual_seed(seed)
 
-    P = torch.randn(5, 5)
-    A = LinOp(P @ P.T)
+    P = torch.randn(5, 5, dtype=dtype)
+    A = LinOp(P @ P.T + mu * I)
 
-    x = torch.randn(5)
+    x = torch.randn(5, dtype=dtype)
     with torch.no_grad():
         b = A(x)
     b = b.clone().detach().requires_grad_(True)
 
-    xhat = dprox.proxfn.linalg.solve.conjugate_gradient(A, b)
+    # xhat = dprox.linalg.solve.conjugate_gradient(A, b)
+    xhat = dprox.linalg.solve.PCG(A, b, rtol=1e-6, max_iters=100, verbose=False)
     xhat.mean().backward()
     grad2 = A.A.grad  # grad2 is only correct at the diagonal items.
 
     # explicit solve
     torch.manual_seed(seed)
 
-    P = torch.randn(5, 5).requires_grad_(True)
-    A = P @ P.T
+    P = torch.randn(5, 5, dtype=dtype).requires_grad_(True)
+    A = P @ P.T + mu * I
     A.retain_grad()
-    x = torch.randn(5)
+    x = torch.randn(5, dtype=dtype)
     with torch.no_grad():
         b = A @ x
     b = b.clone().detach().requires_grad_(True)
 
     xhat = torch.linalg.solve(A, b)
     xhat.mean().backward()
 
@@ -192,15 +202,15 @@
     x = dprox.Variable((1,1,10,10))
     psf = torch.randn((1,5,5))
     KtK = dprox.conv_doe(x, psf=psf).gram
     
     x = torch.randn(1,1,10,10)
     b = KtK(x)
     
-    xhat = dprox.proxfn.linalg.linear_solve(KtK, b)
+    xhat = dprox.linalg.linear_solve(KtK, b)
     
     print(x.squeeze()[0])
     print(xhat.squeeze()[0])
     print((xhat-x).abs().mean())
     
     assert torch.allclose(xhat, x, atol=0.5, rtol=1)
     
@@ -210,15 +220,15 @@
     x = dprox.Variable((1,1,10,10))
     psf = torch.randn((1,5,5))
     KtK = dprox.conv_doe(x, psf=psf).gram
     
     x = torch.randn(1,1,10,10)
     b = KtK(x)
     
-    xhat = dprox.proxfn.linalg.linear_solve(KtK, b)
+    xhat = dprox.linalg.linear_solve(KtK, b)
     
     xhat.mean().backward()
     
     grad1 = KtK.psf.grad
     print(KtK.psf.grad)
     print(x.squeeze()[0])
     print(xhat.squeeze()[0])
@@ -228,15 +238,15 @@
     x = dprox.Variable((1,1,10,10))
     psf = torch.randn((1,5,5))
     KtK = dprox.conv_doe(x, psf=psf).gram
     
     x = torch.randn(1,1,10,10)
     b = KtK(x)
     
-    xhat = dprox.proxfn.linalg.solve.conjugate_gradient(KtK, b)
+    xhat = dprox.linalg.solve.conjugate_gradient(KtK, b)
     
     xhat.mean().backward()
     
     grad2 = KtK.psf.grad
     print(KtK.psf.grad)
     print(x.squeeze()[0])
     print(xhat.squeeze()[0])
@@ -251,14 +261,14 @@
     x = dprox.Variable((1,1,10,10))
     psf = torch.randn((1,5,5))
     KtK = dprox.conv_doe(x, psf=psf).gram
     
     x = torch.randn(1,1,10,10)
     b = KtK(x)
     
-    xhat = dprox.proxfn.linalg.linear_solve(KtK, b)
+    xhat = dprox.linalg.linear_solve(KtK, b)
     
     xhat.mean().backward()
     
     print(KtK.psf.grad)
     # TODO: need a finite difference method to check gradient
```

### Comparing `dprox-0.1.0/tests/test_linop.py` & `dprox-0.1.1/tests/test_linop.py`

 * *Files identical despite different names*

### Comparing `dprox-0.1.0/tests/test_ml_problems.py` & `dprox-0.1.1/tests/test_ml_problems.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import numpy as np
 import dprox as dp
 
+
 def test_lsq():
     x = dp.Variable((3,3))
     rhs = np.array([[1, 2, 3],[4,5,6],[7,8,9]])
     prob = dp.Problem(dp.sum_squares(2*x - rhs))
     prob.solve('admm', x0=np.zeros((3,3)))
     print(x.value)
 
     assert (x.value.cpu().numpy() == rhs / 2).all()
     
+
 def test_lsq1():
     x = dp.Variable((3,3))
     rhs = np.array([[1, 2, 3],[4,5,6],[7,8,9]])
     prob = dp.Problem(dp.sum_squares(2*x, rhs))
     prob.solve('admm', x0=np.zeros((3,3)))
     print(x.value)
```

