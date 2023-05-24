# Comparing `tmp/fluidsim-0.7.2.tar.gz` & `tmp/fluidsim-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidsim-0.7.2.tar", last modified: Thu Jan  5 14:02:13 2023, max compression
+gzip compressed data, was "fluidsim-0.7.3.tar", last modified: Wed May 24 11:14:10 2023, max compression
```

## Comparing `fluidsim-0.7.2.tar` & `fluidsim-0.7.3.tar`

### file list

```diff
@@ -1,363 +1,363 @@
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.584727 fluidsim-0.7.2/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2036 2020-04-20 13:03:27.000000 fluidsim-0.7.2/.appveyor.yml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      195 2022-03-03 16:23:16.000000 fluidsim-0.7.2/.gitlab-ci.yml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      874 2022-03-29 14:43:46.000000 fluidsim-0.7.2/.hgignore
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1548 2023-01-05 14:01:17.000000 fluidsim-0.7.2/.hgtags
--rw-rw-r--   0 pierre    (1000) pierre    (1000)        5 2021-01-11 13:08:11.000000 fluidsim-0.7.2/.readthedocs.req
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      507 2022-03-03 16:23:16.000000 fluidsim-0.7.2/.readthedocs.yml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1258 2020-11-02 10:53:23.000000 fluidsim-0.7.2/.travis.yml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1043 2022-03-03 16:23:16.000000 fluidsim-0.7.2/AUTHORS.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    11073 2023-01-05 13:56:34.000000 fluidsim-0.7.2/CHANGES.rst
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1262 2020-04-20 13:03:27.000000 fluidsim-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 pierre    (1000) pierre    (1000)    21781 2020-04-20 13:03:27.000000 fluidsim-0.7.2/LICENSE.txt
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      124 2022-11-30 21:15:41.000000 fluidsim-0.7.2/MANIFEST.in
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5166 2022-10-28 07:09:48.000000 fluidsim-0.7.2/Makefile
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5354 2023-01-05 14:02:13.584727 fluidsim-0.7.2/PKG-INFO
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5528 2022-03-10 10:26:25.000000 fluidsim-0.7.2/README.rst
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      103 2021-02-01 15:53:47.000000 fluidsim-0.7.2/environment.yml
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.488732 fluidsim-0.7.2/fluidsim/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4117 2022-03-25 09:19:22.000000 fluidsim-0.7.2/fluidsim/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1594 2023-01-05 14:02:09.000000 fluidsim-0.7.2/fluidsim/_version.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1584 2021-01-08 06:29:50.000000 fluidsim-0.7.2/fluidsim/_version.tpl
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.488732 fluidsim-0.7.2/fluidsim/base/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      267 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.492732 fluidsim-0.7.2/fluidsim/base/forcing/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      262 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/forcing/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    16313 2022-03-25 09:19:22.000000 fluidsim-0.7.2/fluidsim/base/forcing/anisotropic.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5511 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/forcing/base.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6310 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/forcing/kolmogorov.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    16554 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/base/forcing/milestone.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    28185 2022-03-09 06:08:40.000000 fluidsim-0.7.2/fluidsim/base/forcing/specific.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3170 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/forcing/test_kolmogorov.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    16115 2022-07-22 09:55:23.000000 fluidsim-0.7.2/fluidsim/base/init_fields.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.496732 fluidsim-0.7.2/fluidsim/base/output/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6337 2022-10-12 12:42:46.000000 fluidsim-0.7.2/fluidsim/base/output/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.500732 fluidsim-0.7.2/fluidsim/base/output/__pythran__/
--rw-------   0 pierre    (1000) pierre    (1000)    34150 2022-10-28 07:10:31.000000 fluidsim-0.7.2/fluidsim/base/output/__pythran__/increments.cpp
--rw-------   0 pierre    (1000) pierre    (1000)    31093 2022-09-07 13:05:05.000000 fluidsim-0.7.2/fluidsim/base/output/__pythran__/spatiotemporal_spectra.cpp
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    22105 2022-10-28 07:09:48.000000 fluidsim-0.7.2/fluidsim/base/output/base.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1825 2022-09-02 20:09:21.000000 fluidsim-0.7.2/fluidsim/base/output/cross_corr3d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7765 2022-09-02 20:09:21.000000 fluidsim-0.7.2/fluidsim/base/output/horiz_means.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    17246 2022-10-13 09:02:43.000000 fluidsim-0.7.2/fluidsim/base/output/increments.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1143 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/output/model.xmf
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    12143 2022-10-28 07:09:48.000000 fluidsim-0.7.2/fluidsim/base/output/phys_fields.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2172 2022-10-28 07:09:48.000000 fluidsim-0.7.2/fluidsim/base/output/phys_fields1d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13388 2022-11-21 01:35:53.000000 fluidsim-0.7.2/fluidsim/base/output/phys_fields2d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    12857 2022-10-28 07:09:48.000000 fluidsim-0.7.2/fluidsim/base/output/phys_fields3d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7581 2023-01-03 15:05:50.000000 fluidsim-0.7.2/fluidsim/base/output/print_stdout.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5756 2022-10-13 09:02:43.000000 fluidsim-0.7.2/fluidsim/base/output/prob_dens_func.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8711 2022-10-13 09:02:43.000000 fluidsim-0.7.2/fluidsim/base/output/spatial_means.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    54902 2022-09-02 20:09:21.000000 fluidsim-0.7.2/fluidsim/base/output/spatiotemporal_spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3979 2022-09-02 20:09:21.000000 fluidsim-0.7.2/fluidsim/base/output/spect_energy_budget.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9051 2022-10-28 07:09:48.000000 fluidsim-0.7.2/fluidsim/base/output/spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10962 2022-10-28 07:09:48.000000 fluidsim-0.7.2/fluidsim/base/output/spectra3d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4559 2022-10-18 18:26:05.000000 fluidsim-0.7.2/fluidsim/base/output/spectra_multidim.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    31383 2022-09-02 20:09:21.000000 fluidsim-0.7.2/fluidsim/base/output/temporal_spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    16167 2022-09-02 20:09:21.000000 fluidsim-0.7.2/fluidsim/base/output/time_signals_fft.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2347 2021-02-18 09:08:08.000000 fluidsim-0.7.2/fluidsim/base/params.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.500732 fluidsim-0.7.2/fluidsim/base/preprocess/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      226 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/preprocess/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1926 2022-07-22 08:03:03.000000 fluidsim-0.7.2/fluidsim/base/preprocess/base.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    11395 2022-10-12 12:51:53.000000 fluidsim-0.7.2/fluidsim/base/preprocess/pseudo_spect.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1165 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/base/preprocess/test.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      260 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/setofvariables.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.500732 fluidsim-0.7.2/fluidsim/base/solvers/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      209 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/base/solvers/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7628 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/solvers/base.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      941 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/solvers/finite_diff.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2018 2021-01-08 06:29:50.000000 fluidsim-0.7.2/fluidsim/base/solvers/info_base.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8481 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/base/solvers/pseudo_spect.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.504731 fluidsim-0.7.2/fluidsim/base/sphericalharmo/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      219 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/sphericalharmo/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      576 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/sphericalharmo/output.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1407 2022-10-28 07:09:48.000000 fluidsim-0.7.2/fluidsim/base/sphericalharmo/phys_fields.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1574 2022-03-07 14:13:23.000000 fluidsim-0.7.2/fluidsim/base/sphericalharmo/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3583 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/sphericalharmo/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    11876 2022-03-09 06:08:40.000000 fluidsim-0.7.2/fluidsim/base/state.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.504731 fluidsim-0.7.2/fluidsim/base/test/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/test/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      528 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/test/test_base_solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2508 2022-03-25 09:19:22.000000 fluidsim-0.7.2/fluidsim/base/test/test_base_solver_ps.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      696 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/base/test/test_params.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.504731 fluidsim-0.7.2/fluidsim/base/time_stepping/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      202 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/base/time_stepping/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.504731 fluidsim-0.7.2/fluidsim/base/time_stepping/__pythran__/
--rw-------   0 pierre    (1000) pierre    (1000)   340864 2022-09-02 01:40:11.000000 fluidsim-0.7.2/fluidsim/base/time_stepping/__pythran__/pseudo_spect.cpp
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13738 2022-09-05 19:07:07.000000 fluidsim-0.7.2/fluidsim/base/time_stepping/base.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4779 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/base/time_stepping/finite_diff.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    31636 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/base/time_stepping/pseudo_spect.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7779 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/base/time_stepping/simple.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.508731 fluidsim-0.7.2/fluidsim/base/turb_model/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      744 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/turb_model/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3633 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/turb_model/base.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2966 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/turb_model/smagorinsky.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1236 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/turb_model/stress_tensor.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1396 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/base/turb_model/test_turb_model.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.508731 fluidsim-0.7.2/fluidsim/extend_simul/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      420 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/extend_simul/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    17237 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/extend_simul/spatial_means_regions_milestone.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3134 2022-03-25 09:19:22.000000 fluidsim-0.7.2/fluidsim/magic.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.508731 fluidsim-0.7.2/fluidsim/operators/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      194 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/operators/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.512731 fluidsim-0.7.2/fluidsim/operators/__pythran__/
--rw-------   0 pierre    (1000) pierre    (1000)    67229 2022-10-28 07:10:29.000000 fluidsim-0.7.2/fluidsim/operators/__pythran__/operators2d.cpp
--rw-------   0 pierre    (1000) pierre    (1000)   229484 2022-10-28 07:10:31.000000 fluidsim-0.7.2/fluidsim/operators/__pythran__/operators3d.cpp
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4286 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/operators/base.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1340 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/operators/op_finitediff1d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5324 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/operators/op_finitediff2d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1041 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/operators/operators0d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3174 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/operators/operators1d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20725 2022-10-13 09:04:57.000000 fluidsim-0.7.2/fluidsim/operators/operators2d.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    41920 2022-10-13 09:04:57.000000 fluidsim-0.7.2/fluidsim/operators/operators3d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2214 2022-10-13 09:04:57.000000 fluidsim-0.7.2/fluidsim/operators/sphericalharmo.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.512731 fluidsim-0.7.2/fluidsim/operators/test/
--rw-r--r--   0 pierre    (1000) pierre    (1000)        0 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/operators/test/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9490 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/operators/test/test_operators2d.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10650 2022-03-09 06:08:40.000000 fluidsim-0.7.2/fluidsim/operators/test/test_operators3d.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.512731 fluidsim-0.7.2/fluidsim/solvers/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1166 2022-03-25 09:19:22.000000 fluidsim-0.7.2/fluidsim/solvers/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.512731 fluidsim-0.7.2/fluidsim/solvers/ad1d/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      212 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1626 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/init_fields.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.516731 fluidsim-0.7.2/fluidsim/solvers/ad1d/output/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1183 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/output/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      260 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/output/print_stdout.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.516731 fluidsim-0.7.2/fluidsim/solvers/ad1d/pseudo_spect/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      223 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/pseudo_spect/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2915 2021-02-18 09:08:08.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/pseudo_spect/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1800 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/pseudo_spect/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      256 2021-02-18 09:08:08.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/pseudo_spect/test_solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3455 2021-02-18 09:08:08.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1309 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2968 2022-10-28 07:09:48.000000 fluidsim-0.7.2/fluidsim/solvers/ad1d/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.516731 fluidsim-0.7.2/fluidsim/solvers/burgers1d/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      172 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/burgers1d/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.516731 fluidsim-0.7.2/fluidsim/solvers/burgers1d/skew_sym/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      230 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/burgers1d/skew_sym/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1871 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/burgers1d/skew_sym/solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      291 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/burgers1d/skew_sym/test_solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4021 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/burgers1d/solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1130 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/burgers1d/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.516731 fluidsim-0.7.2/fluidsim/solvers/models0d/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      185 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.516731 fluidsim-0.7.2/fluidsim/solvers/models0d/lorenz/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      186 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/lorenz/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.520730 fluidsim-0.7.2/fluidsim/solvers/models0d/lorenz/output/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1107 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/lorenz/output/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5186 2022-02-27 20:30:48.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/lorenz/output/print_stdout.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4368 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/lorenz/solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.520730 fluidsim-0.7.2/fluidsim/solvers/models0d/predaprey/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      206 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/predaprey/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.520730 fluidsim-0.7.2/fluidsim/solvers/models0d/predaprey/output/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1398 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/predaprey/output/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5147 2022-02-27 20:30:48.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/predaprey/output/print_stdout.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3985 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/predaprey/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1185 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/test_lorenz.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1013 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/models0d/test_predaprey.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.520730 fluidsim-0.7.2/fluidsim/solvers/nl1d/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      171 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/nl1d/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3138 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/nl1d/solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4634 2022-01-04 11:09:50.000000 fluidsim-0.7.2/fluidsim/solvers/nl1d/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.520730 fluidsim-0.7.2/fluidsim/solvers/ns2d/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      494 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.524730 fluidsim-0.7.2/fluidsim/solvers/ns2d/__pythran__/
--rw-------   0 pierre    (1000) pierre    (1000)    99678 2022-09-02 01:40:17.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/__pythran__/solver.cpp
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.524730 fluidsim-0.7.2/fluidsim/solvers/ns2d/bouss/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      426 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/bouss/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9276 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/bouss/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5120 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/bouss/state.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3365 2022-10-20 07:30:17.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/bouss/test_solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1601 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/forcing.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5752 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/init_fields.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.524730 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3677 2022-02-27 20:30:48.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.524730 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/__pythran__/
--rw-------   0 pierre    (1000) pierre    (1000)    43516 2022-09-02 01:40:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/__pythran__/spatiotemporal_spectra.cpp
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3291 2021-04-02 13:55:48.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/print_stdout.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10363 2022-10-13 08:59:01.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spatial_means.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3015 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spatiotemporal_spectra.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5504 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spect_energy_budget.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6554 2022-10-13 09:03:19.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1561 2020-08-26 07:38:01.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spectra_multidim.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7506 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6027 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/state.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.528730 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      239 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1941 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/forcing.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4618 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/init_fields.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.532730 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7077 2022-02-27 20:30:48.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13208 2022-10-13 09:05:05.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/_old_miguel_frequency_spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    36810 2022-10-13 09:05:02.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/_old_miguel_spatio_temporal_spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      921 2022-10-12 09:19:42.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/phys_fields.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5908 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/print_stdout.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    15444 2022-10-13 08:59:01.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/spatial_means.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19038 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/spect_energy_budget.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14160 2022-10-13 09:03:19.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7939 2020-08-26 07:38:01.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/spectra_multidim.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9654 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9644 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    12654 2022-10-20 07:37:59.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/test_solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5626 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/time_stepping.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10501 2022-11-21 02:00:34.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/test_solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2544 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/test_with_uxuy.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4805 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns2d/with_uxuy.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.532730 fluidsim-0.7.2/fluidsim/solvers/ns3d/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      342 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.532730 fluidsim-0.7.2/fluidsim/solvers/ns3d/bouss/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      210 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/bouss/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7083 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/bouss/solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2664 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/bouss/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.536729 fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/
--rwxrwxr-x   0 pierre    (1000) pierre    (1000)     2875 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.536729 fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/__pythran__/
--rw-------   0 pierre    (1000) pierre    (1000)    10483 2022-09-02 01:40:18.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/__pythran__/watu.cpp
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6417 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/milestone.py
--rwxrwxr-x   0 pierre    (1000) pierre    (1000)     7163 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/watu.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6151 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/init_fields.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.536729 fluidsim-0.7.2/fluidsim/solvers/ns3d/output/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3699 2022-05-19 07:23:23.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/output/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.536729 fluidsim-0.7.2/fluidsim/solvers/ns3d/output/__pythran__/
--rw-------   0 pierre    (1000) pierre    (1000)    45471 2022-09-02 01:40:20.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/output/__pythran__/spatiotemporal_spectra.cpp
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2738 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/output/print_stdout.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13896 2022-10-13 08:59:01.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/output/spatial_means.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5509 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/output/spatiotemporal_spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10890 2022-04-28 08:50:46.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/output/spect_energy_budget.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    18854 2022-05-19 07:23:23.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/output/spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9976 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/solver.py
--rwxrwxr-x   0 pierre    (1000) pierre    (1000)     6111 2022-03-09 06:08:40.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/state.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.536729 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      229 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.540729 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/__pythran__/
--rw-------   0 pierre    (1000) pierre    (1000)    12226 2022-09-02 01:40:21.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/__pythran__/solver.cpp
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.540729 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/output/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2794 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/output/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13302 2022-10-13 08:59:01.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/output/spatial_means.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4630 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/output/spect_energy_budget.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7371 2022-03-25 09:19:22.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/output/spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8397 2022-03-07 20:19:58.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/solver.py
--rwxrwxr-x   0 pierre    (1000) pierre    (1000)     1523 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9106 2022-05-19 07:23:23.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/test_solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    20320 2022-10-28 07:09:48.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/test_solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      883 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/time_stepping.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1683 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/try_load.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1739 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/ns3d/try_save.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.548729 fluidsim-0.7.2/fluidsim/solvers/plate2d/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      244 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2265 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/dimensional.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2510 2020-05-12 21:13:23.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/forcing.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3449 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/init_fields.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2709 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/operators.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.548729 fluidsim-0.7.2/fluidsim/solvers/plate2d/output/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3642 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/output/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      963 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/output/correl_Mordant.m
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    26141 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/output/correlations_freq.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      502 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/output/print_stdout.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8748 2022-10-13 08:59:01.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/output/spatial_means.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8819 2022-10-13 09:04:29.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/output/spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10639 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3227 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      743 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/test_dimensional.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4256 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/plate2d/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.552729 fluidsim-0.7.2/fluidsim/solvers/sphere/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      274 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sphere/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.552729 fluidsim-0.7.2/fluidsim/solvers/sphere/ns2d/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      234 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sphere/ns2d/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4325 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/sphere/ns2d/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1469 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sphere/ns2d/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.556728 fluidsim-0.7.2/fluidsim/solvers/sphere/sw1l/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      236 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sphere/sw1l/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6564 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sphere/sw1l/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5017 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sphere/sw1l/state.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1558 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sphere/sw1l/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.560728 fluidsim-0.7.2/fluidsim/solvers/sw1l/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      336 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.560728 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      262 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.564728 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/modified/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      190 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/modified/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2166 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/modified/output.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5051 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/modified/solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2748 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/modified/test_solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6994 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7958 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2667 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/test_solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7951 2022-03-09 06:08:40.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/forcing.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4880 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/init_fields.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.568728 fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      180 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2247 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/output.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4939 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5113 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3913 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.568728 fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      198 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      538 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/output.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     7003 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     7882 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2624 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/test_solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)    10636 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/operators.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.572728 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9114 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     6241 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/_old_spatial_means.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    21711 2020-05-12 21:13:26.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/_old_spect_energy_budg.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    12650 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/increments.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    13358 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/normal_mode.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3768 2022-02-27 20:30:48.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/print_stdout.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    17620 2022-10-13 08:59:01.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/spatial_means.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    28237 2020-05-12 21:13:26.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/spect_energy_budget.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    19404 2022-10-13 09:03:19.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/output/spectra.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8873 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/solver.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    10140 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2205 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/test_operators.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6597 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/sw1l/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.576727 fluidsim-0.7.2/fluidsim/solvers/waves2d/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      173 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/waves2d/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4666 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/solvers/waves2d/solver.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      838 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/solvers/waves2d/state.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1463 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/solvers/waves2d/test_solver.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.576727 fluidsim-0.7.2/fluidsim/util/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1799 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/util/__init__.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.576727 fluidsim-0.7.2/fluidsim/util/__pythran__/
--rw-------   0 pierre    (1000) pierre    (1000)    16670 2022-09-02 01:40:15.000000 fluidsim-0.7.2/fluidsim/util/__pythran__/mini_oper_modif_resol.cpp
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.580727 fluidsim-0.7.2/fluidsim/util/console/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      182 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/util/console/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2834 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/util/console/__main__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8097 2021-01-20 14:49:47.000000 fluidsim-0.7.2/fluidsim/util/console/bench.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     8949 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/util/console/bench_analysis.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    12215 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/util/console/profile.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2281 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/util/console/test_bench.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1813 2020-11-02 10:53:23.000000 fluidsim-0.7.2/fluidsim/util/console/test_profile.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     9880 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/util/console/util.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1945 2020-04-20 13:03:27.000000 fluidsim-0.7.2/fluidsim/util/frequency_modulation.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2551 2020-11-25 14:48:46.000000 fluidsim-0.7.2/fluidsim/util/mini_oper_modif_resol.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4019 2022-02-03 09:40:16.000000 fluidsim-0.7.2/fluidsim/util/output.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.584727 fluidsim-0.7.2/fluidsim/util/scripts/
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      363 2022-11-18 16:39:37.000000 fluidsim-0.7.2/fluidsim/util/scripts/__init__.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      652 2022-11-18 16:39:23.000000 fluidsim-0.7.2/fluidsim/util/scripts/ipy_load.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1771 2022-05-19 07:23:23.000000 fluidsim-0.7.2/fluidsim/util/scripts/modif_resolution.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3676 2022-11-29 20:38:00.000000 fluidsim-0.7.2/fluidsim/util/scripts/restart.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      180 2022-11-18 16:40:58.000000 fluidsim-0.7.2/fluidsim/util/scripts/test_ipy_load.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      863 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/util/scripts/test_modif_resolution.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     2307 2022-03-03 16:23:16.000000 fluidsim-0.7.2/fluidsim/util/scripts/test_restart.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1264 2022-04-28 08:50:46.000000 fluidsim-0.7.2/fluidsim/util/scripts/test_turb_trandom_anisotropic.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    14074 2022-11-29 20:38:00.000000 fluidsim-0.7.2/fluidsim/util/scripts/turb_trandom_anisotropic.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1770 2022-03-25 09:19:22.000000 fluidsim-0.7.2/fluidsim/util/test_util.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     5271 2022-09-02 13:06:20.000000 fluidsim-0.7.2/fluidsim/util/testing.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    27160 2022-10-13 11:43:31.000000 fluidsim-0.7.2/fluidsim/util/util.py
-drwxrwxr-x   0 pierre    (1000) pierre    (1000)        0 2023-01-05 14:02:13.488732 fluidsim-0.7.2/fluidsim.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     5354 2023-01-05 14:02:13.000000 fluidsim-0.7.2/fluidsim.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)    11410 2023-01-05 14:02:13.000000 fluidsim-0.7.2/fluidsim.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-01-05 14:02:13.000000 fluidsim-0.7.2/fluidsim.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1867 2023-01-05 14:02:13.000000 fluidsim-0.7.2/fluidsim.egg-info/entry_points.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)      803 2023-01-05 14:02:13.000000 fluidsim-0.7.2/fluidsim.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       17 2023-01-05 14:02:13.000000 fluidsim-0.7.2/fluidsim.egg-info/top_level.txt
--rwxrwxr-x   0 pierre    (1000) pierre    (1000)      165 2021-02-01 15:53:47.000000 fluidsim-0.7.2/postBuild
--rw-rw-r--   0 pierre    (1000) pierre    (1000)    11060 2022-03-25 09:19:22.000000 fluidsim-0.7.2/pylintrc
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1243 2023-01-04 09:29:01.000000 fluidsim-0.7.2/pyproject.toml
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     3318 2023-01-05 14:02:13.584727 fluidsim-0.7.2/setup.cfg
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     6035 2022-11-30 21:15:41.000000 fluidsim-0.7.2/setup.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)      615 2020-11-02 10:53:23.000000 fluidsim-0.7.2/setup_build.py
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     4498 2021-02-02 08:39:23.000000 fluidsim-0.7.2/setup_configure.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      654 2020-04-20 13:03:27.000000 fluidsim-0.7.2/site.cfg.default
--rw-rw-r--   0 pierre    (1000) pierre    (1000)     1794 2023-01-04 08:53:16.000000 fluidsim-0.7.2/tox.ini
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.669810 fluidsim-0.7.3/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2036 2020-12-03 09:47:00.000000 fluidsim-0.7.3/.appveyor.yml
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      195 2023-03-08 11:13:07.000000 fluidsim-0.7.3/.gitlab-ci.yml
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      874 2022-11-24 10:48:01.000000 fluidsim-0.7.3/.hgignore
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1595 2023-05-24 11:11:45.000000 fluidsim-0.7.3/.hgtags
+-rw-r--r--   0 augier3pi (23665) all-users   (513)        5 2022-01-14 09:58:02.000000 fluidsim-0.7.3/.readthedocs.req
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      507 2022-02-11 11:20:01.000000 fluidsim-0.7.3/.readthedocs.yml
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1258 2022-01-14 09:58:02.000000 fluidsim-0.7.3/.travis.yml
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1043 2022-11-24 10:48:01.000000 fluidsim-0.7.3/AUTHORS.rst
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    11341 2023-05-24 09:38:50.000000 fluidsim-0.7.3/CHANGES.rst
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1262 2020-12-03 09:47:00.000000 fluidsim-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    21781 2020-12-03 09:47:00.000000 fluidsim-0.7.3/LICENSE.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      124 2022-11-30 15:02:59.000000 fluidsim-0.7.3/MANIFEST.in
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5166 2022-11-24 10:48:01.000000 fluidsim-0.7.3/Makefile
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5355 2023-05-24 11:14:10.669810 fluidsim-0.7.3/PKG-INFO
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5528 2022-11-24 10:48:01.000000 fluidsim-0.7.3/README.rst
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      103 2022-01-14 09:58:02.000000 fluidsim-0.7.3/environment.yml
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.625809 fluidsim-0.7.3/fluidsim/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4031 2023-05-24 08:58:12.000000 fluidsim-0.7.3/fluidsim/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1594 2023-05-24 09:29:36.000000 fluidsim-0.7.3/fluidsim/_version.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1584 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/_version.tpl
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.629809 fluidsim-0.7.3/fluidsim/base/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      267 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.629809 fluidsim-0.7.3/fluidsim/base/forcing/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      262 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/forcing/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    16310 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/forcing/anisotropic.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5510 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/forcing/base.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6309 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/forcing/kolmogorov.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    16544 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/forcing/milestone.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    28179 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/forcing/specific.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3170 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/forcing/test_kolmogorov.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    16106 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/init_fields.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.633809 fluidsim-0.7.3/fluidsim/base/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6336 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.633809 fluidsim-0.7.3/fluidsim/base/output/__pythran__/
+-rw-------   0 augier3pi (23665) all-users   (513)    34882 2023-05-24 09:29:39.000000 fluidsim-0.7.3/fluidsim/base/output/__pythran__/increments.cpp
+-rw-------   0 augier3pi (23665) all-users   (513)    31093 2022-11-30 14:27:57.000000 fluidsim-0.7.3/fluidsim/base/output/__pythran__/spatiotemporal_spectra.cpp
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    22100 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/base.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1824 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/cross_corr3d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7764 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/horiz_means.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    17244 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/increments.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1143 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/base/output/model.xmf
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    12142 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/phys_fields.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2172 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/output/phys_fields1d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    13388 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/output/phys_fields2d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    12857 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/output/phys_fields3d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7580 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/print_stdout.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5755 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/prob_dens_func.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     8710 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/spatial_means.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    54902 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/output/spatiotemporal_spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3978 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/spect_energy_budget.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     9051 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/output/spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    10961 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/spectra3d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4559 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/output/spectra_multidim.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    31383 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/output/temporal_spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    16163 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/output/time_signals_fft.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2347 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/base/params.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.633809 fluidsim-0.7.3/fluidsim/base/preprocess/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      226 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/base/preprocess/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1926 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/base/preprocess/base.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    11395 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/preprocess/pseudo_spect.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1163 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/preprocess/test.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      260 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/base/setofvariables.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.633809 fluidsim-0.7.3/fluidsim/base/solvers/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      209 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/base/solvers/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7627 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/solvers/base.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      940 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/solvers/finite_diff.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2018 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/base/solvers/info_base.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     8480 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/solvers/pseudo_spect.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.633809 fluidsim-0.7.3/fluidsim/base/sphericalharmo/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      219 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/base/sphericalharmo/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      576 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/base/sphericalharmo/output.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1407 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/sphericalharmo/phys_fields.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1574 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/sphericalharmo/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3583 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/base/sphericalharmo/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    11875 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/state.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.637809 fluidsim-0.7.3/fluidsim/base/test/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)        0 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/base/test/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      528 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/base/test/test_base_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2508 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/test/test_base_solver_ps.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      696 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/base/test/test_params.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.637809 fluidsim-0.7.3/fluidsim/base/time_stepping/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      202 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/base/time_stepping/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.637809 fluidsim-0.7.3/fluidsim/base/time_stepping/__pythran__/
+-rw-------   0 augier3pi (23665) all-users   (513)   327898 2023-05-24 09:29:39.000000 fluidsim-0.7.3/fluidsim/base/time_stepping/__pythran__/pseudo_spect.cpp
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    13735 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/time_stepping/base.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4779 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/base/time_stepping/finite_diff.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    31634 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/time_stepping/pseudo_spect.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7779 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/base/time_stepping/simple.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.637809 fluidsim-0.7.3/fluidsim/base/turb_model/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      744 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/turb_model/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3631 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/turb_model/base.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2965 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/turb_model/smagorinsky.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1235 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/base/turb_model/stress_tensor.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1396 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/base/turb_model/test_turb_model.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.637809 fluidsim-0.7.3/fluidsim/extend_simul/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      420 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/extend_simul/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    17235 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/extend_simul/spatial_means_regions_milestone.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3134 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/magic.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.637809 fluidsim-0.7.3/fluidsim/operators/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      194 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/operators/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/operators/__pythran__/
+-rw-------   0 augier3pi (23665) all-users   (513)    68869 2023-05-24 09:29:39.000000 fluidsim-0.7.3/fluidsim/operators/__pythran__/operators2d.cpp
+-rw-------   0 augier3pi (23665) all-users   (513)   237438 2023-05-24 09:29:41.000000 fluidsim-0.7.3/fluidsim/operators/__pythran__/operators3d.cpp
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4286 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/operators/base.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1340 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/operators/op_finitediff1d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5323 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/operators/op_finitediff2d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1041 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/operators/operators0d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3174 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/operators/operators1d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    20722 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/operators/operators2d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    41912 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/operators/operators3d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2213 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/operators/sphericalharmo.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/operators/test/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)        0 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/operators/test/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     9489 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/operators/test/test_operators2d.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    10650 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/operators/test/test_operators3d.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/solvers/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1166 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/solvers/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/solvers/ad1d/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      212 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1626 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/init_fields.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/solvers/ad1d/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1183 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/output/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      260 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/output/print_stdout.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/solvers/ad1d/pseudo_spect/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      223 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/pseudo_spect/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2914 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/pseudo_spect/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1800 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/pseudo_spect/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      256 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/pseudo_spect/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3453 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1309 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2967 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ad1d/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/solvers/burgers1d/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      172 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/burgers1d/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/solvers/burgers1d/skew_sym/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      230 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/burgers1d/skew_sym/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1870 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/burgers1d/skew_sym/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      291 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/burgers1d/skew_sym/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4020 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/burgers1d/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1129 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/burgers1d/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/solvers/models0d/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      185 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.641810 fluidsim-0.7.3/fluidsim/solvers/models0d/lorenz/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      186 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/lorenz/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.645810 fluidsim-0.7.3/fluidsim/solvers/models0d/lorenz/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1107 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/lorenz/output/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5185 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/lorenz/output/print_stdout.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4368 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/lorenz/solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.645810 fluidsim-0.7.3/fluidsim/solvers/models0d/predaprey/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      206 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/predaprey/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.645810 fluidsim-0.7.3/fluidsim/solvers/models0d/predaprey/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1398 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/predaprey/output/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5146 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/predaprey/output/print_stdout.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3985 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/predaprey/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1185 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/test_lorenz.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1013 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/models0d/test_predaprey.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.645810 fluidsim-0.7.3/fluidsim/solvers/nl1d/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      171 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/nl1d/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3136 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/nl1d/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4632 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/nl1d/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.645810 fluidsim-0.7.3/fluidsim/solvers/ns2d/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      494 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.645810 fluidsim-0.7.3/fluidsim/solvers/ns2d/__pythran__/
+-rw-------   0 augier3pi (23665) all-users   (513)    99829 2023-05-24 09:29:42.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/__pythran__/solver.cpp
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.645810 fluidsim-0.7.3/fluidsim/solvers/ns2d/bouss/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      426 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/bouss/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     9274 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/bouss/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5118 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/bouss/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3363 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/bouss/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1600 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/forcing.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5751 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/init_fields.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.649810 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3677 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.649810 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/__pythran__/
+-rw-------   0 augier3pi (23665) all-users   (513)    46269 2023-05-24 09:29:42.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/__pythran__/spatiotemporal_spectra.cpp
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3291 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/print_stdout.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    10362 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spatial_means.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3014 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spatiotemporal_spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5502 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spect_energy_budget.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6553 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1561 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spectra_multidim.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7505 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6026 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/state.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.649810 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      239 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1940 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/forcing.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4617 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/init_fields.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.649810 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7077 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    13207 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/_old_miguel_frequency_spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    36809 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/_old_miguel_spatio_temporal_spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      920 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/phys_fields.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5908 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/print_stdout.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    15443 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/spatial_means.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    19037 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/spect_energy_budget.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    14158 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7939 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/spectra_multidim.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     9652 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     9643 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    12651 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5626 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/time_stepping.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    10498 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2544 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/test_with_uxuy.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4803 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns2d/with_uxuy.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.653810 fluidsim-0.7.3/fluidsim/solvers/ns3d/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      342 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.653810 fluidsim-0.7.3/fluidsim/solvers/ns3d/bouss/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      210 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/bouss/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7081 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/bouss/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2663 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/bouss/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.653810 fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/
+-rwxr-xr-x   0 augier3pi (23665) all-users   (513)     2875 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.653810 fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/__pythran__/
+-rw-------   0 augier3pi (23665) all-users   (513)     9263 2023-05-24 09:29:43.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/__pythran__/watu.cpp
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6413 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/milestone.py
+-rwxr-xr-x   0 augier3pi (23665) all-users   (513)     7162 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/watu.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6151 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/init_fields.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.653810 fluidsim-0.7.3/fluidsim/solvers/ns3d/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3699 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/output/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.653810 fluidsim-0.7.3/fluidsim/solvers/ns3d/output/__pythran__/
+-rw-------   0 augier3pi (23665) all-users   (513)    48300 2023-05-24 09:29:42.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/output/__pythran__/spatiotemporal_spectra.cpp
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2738 2022-01-14 15:48:40.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/output/print_stdout.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    13894 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/output/spatial_means.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5508 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/output/spatiotemporal_spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    10885 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/output/spect_energy_budget.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    18847 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/output/spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     9973 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/solver.py
+-rwxr-xr-x   0 augier3pi (23665) all-users   (513)     6110 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/state.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.653810 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      229 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.653810 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/__pythran__/
+-rw-------   0 augier3pi (23665) all-users   (513)    10367 2023-05-24 09:29:42.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/__pythran__/solver.cpp
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.653810 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2794 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/output/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    13300 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/output/spatial_means.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4628 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/output/spect_energy_budget.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7370 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/output/spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     8395 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/solver.py
+-rwxr-xr-x   0 augier3pi (23665) all-users   (513)     1523 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     9103 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    20314 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      883 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/time_stepping.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1683 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/try_load.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1739 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/ns3d/try_save.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.657810 fluidsim-0.7.3/fluidsim/solvers/plate2d/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      244 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2264 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/dimensional.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2510 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/forcing.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3449 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/init_fields.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2709 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/operators.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.657810 fluidsim-0.7.3/fluidsim/solvers/plate2d/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3642 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/output/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      963 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/output/correl_Mordant.m
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    26135 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/output/correlations_freq.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      502 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/output/print_stdout.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     8746 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/output/spatial_means.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     8818 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/output/spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    10638 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3227 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      742 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/test_dimensional.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4255 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/plate2d/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.657810 fluidsim-0.7.3/fluidsim/solvers/sphere/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      274 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sphere/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.657810 fluidsim-0.7.3/fluidsim/solvers/sphere/ns2d/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      234 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sphere/ns2d/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4324 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sphere/ns2d/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1468 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sphere/ns2d/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.657810 fluidsim-0.7.3/fluidsim/solvers/sphere/sw1l/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      236 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sphere/sw1l/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6563 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sphere/sw1l/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5017 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sphere/sw1l/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1557 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sphere/sw1l/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.661810 fluidsim-0.7.3/fluidsim/solvers/sw1l/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      336 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.661810 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      262 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.661810 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/modified/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      190 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/modified/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2166 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/modified/output.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5050 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/modified/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2748 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/modified/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6993 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7958 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2667 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7951 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/forcing.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4880 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/init_fields.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.661810 fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      180 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2247 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/output.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4938 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5112 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3913 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.661810 fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      198 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      538 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/output.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7002 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     7880 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2624 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/test_solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    10635 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/operators.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.665810 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     9114 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6241 2022-07-19 08:59:52.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/_old_spatial_means.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    21707 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/_old_spect_energy_budg.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    12650 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/increments.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    13358 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/normal_mode.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3768 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/print_stdout.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    17616 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/spatial_means.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    28230 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/spect_energy_budget.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    19402 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/output/spectra.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     8872 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    10140 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2204 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/test_operators.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6597 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/solvers/sw1l/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.665810 fluidsim-0.7.3/fluidsim/solvers/waves2d/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      173 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/waves2d/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4663 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/solvers/waves2d/solver.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      838 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/solvers/waves2d/state.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1463 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/solvers/waves2d/test_solver.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.665810 fluidsim-0.7.3/fluidsim/util/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1799 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/util/__init__.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.665810 fluidsim-0.7.3/fluidsim/util/__pythran__/
+-rw-------   0 augier3pi (23665) all-users   (513)    17667 2023-05-24 09:29:43.000000 fluidsim-0.7.3/fluidsim/util/__pythran__/mini_oper_modif_resol.cpp
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.665810 fluidsim-0.7.3/fluidsim/util/console/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      182 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/util/console/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2834 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/util/console/__main__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     8097 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/util/console/bench.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     8949 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/util/console/bench_analysis.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    12215 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/util/console/profile.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2280 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/util/console/test_bench.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1813 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/util/console/test_profile.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     9880 2022-02-11 11:20:01.000000 fluidsim-0.7.3/fluidsim/util/console/util.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1945 2020-12-03 09:47:00.000000 fluidsim-0.7.3/fluidsim/util/frequency_modulation.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2549 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/util/mini_oper_modif_resol.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4019 2022-01-14 09:58:02.000000 fluidsim-0.7.3/fluidsim/util/output.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.669810 fluidsim-0.7.3/fluidsim/util/scripts/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      363 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/util/scripts/__init__.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      139 2023-05-24 08:58:12.000000 fluidsim-0.7.3/fluidsim/util/scripts/ipy_load.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1771 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/util/scripts/modif_resolution.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3676 2022-11-28 15:38:07.000000 fluidsim-0.7.3/fluidsim/util/scripts/restart.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      180 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/util/scripts/test_ipy_load.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      863 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/util/scripts/test_modif_resolution.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     2307 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/util/scripts/test_restart.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1264 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/util/scripts/test_turb_trandom_anisotropic.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    14073 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/util/scripts/turb_trandom_anisotropic.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1770 2022-11-24 10:48:01.000000 fluidsim-0.7.3/fluidsim/util/test_util.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5270 2023-05-24 07:56:46.000000 fluidsim-0.7.3/fluidsim/util/testing.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    24157 2023-05-24 08:58:12.000000 fluidsim-0.7.3/fluidsim/util/util.py
+drwxr-xr-x   0 augier3pi (23665) all-users   (513)        0 2023-05-24 11:14:10.629809 fluidsim-0.7.3/fluidsim.egg-info/
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     5355 2023-05-24 11:14:09.000000 fluidsim-0.7.3/fluidsim.egg-info/PKG-INFO
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    11410 2023-05-24 11:14:10.000000 fluidsim-0.7.3/fluidsim.egg-info/SOURCES.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)        1 2023-05-24 11:14:09.000000 fluidsim-0.7.3/fluidsim.egg-info/dependency_links.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1867 2023-05-24 11:14:09.000000 fluidsim-0.7.3/fluidsim.egg-info/entry_points.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      827 2023-05-24 11:14:09.000000 fluidsim-0.7.3/fluidsim.egg-info/requires.txt
+-rw-r--r--   0 augier3pi (23665) all-users   (513)       17 2023-05-24 11:14:09.000000 fluidsim-0.7.3/fluidsim.egg-info/top_level.txt
+-rwxr-xr-x   0 augier3pi (23665) all-users   (513)      165 2022-01-14 09:58:02.000000 fluidsim-0.7.3/postBuild
+-rw-r--r--   0 augier3pi (23665) all-users   (513)    11060 2022-11-24 10:48:01.000000 fluidsim-0.7.3/pylintrc
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1243 2023-05-02 13:51:44.000000 fluidsim-0.7.3/pyproject.toml
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     3332 2023-05-24 11:14:10.669810 fluidsim-0.7.3/setup.cfg
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     6036 2023-05-24 09:39:22.000000 fluidsim-0.7.3/setup.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      615 2022-01-14 09:58:02.000000 fluidsim-0.7.3/setup_build.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     4498 2022-01-14 09:58:02.000000 fluidsim-0.7.3/setup_configure.py
+-rw-r--r--   0 augier3pi (23665) all-users   (513)      654 2020-12-03 09:47:00.000000 fluidsim-0.7.3/site.cfg.default
+-rw-r--r--   0 augier3pi (23665) all-users   (513)     1826 2023-03-08 12:55:39.000000 fluidsim-0.7.3/tox.ini
```

### Comparing `fluidsim-0.7.2/.appveyor.yml` & `fluidsim-0.7.3/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/.hgignore` & `fluidsim-0.7.3/.hgignore`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/.hgtags` & `fluidsim-0.7.3/.hgtags`

 * *Files 5% similar despite different names*

```diff
@@ -26,7 +26,8 @@
 3fc0f975b8acba07fbd5625692981e41ce9eca07 0.6.1rc1
 9f4b41654c564bc0bb544b36b7f637e2a51f289a 0.6.1
 6502318129a8c077954876a2baa86f7a65bd7498 0.7.0rc0
 a84794596e4364e2c4254a6f5b970a53fcfe1c79 0.7.0rc1
 ac74b33ad131d8a5921e1e21ef635bcb337c29de 0.7.0
 154d186825dc048de44c9dddbb6c0bb9f7d1b0a0 0.7.1
 79814dbd68aefe12f0a1e37872fe8d501c54f03d 0.7.2
+aaf7ee93003337a6a4b73e057268ad460355f011 0.7.3
```

### Comparing `fluidsim-0.7.2/.travis.yml` & `fluidsim-0.7.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/AUTHORS.rst` & `fluidsim-0.7.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/CHANGES.rst` & `fluidsim-0.7.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,21 @@
 
 ..
   Unreleased_
   -----------
 
 .. towncrier release notes start
 
+0.7.3_ (2023-05-24)
+-------------------
+
+- Official support for only Python 3.9, 3.10 and 3.11.
+
+- Few improvements for `Fluidsimfoam
+  <https://foss.heptapod.net/fluiddyn/fluidsimfoam>`_.
 
 0.7.2_ (2023-01-05)
 -------------------
 
 - New module :mod:`fluidsim_core.output.remaining_clock_time`.
 
 0.7.1_ (2022-11-30)
@@ -292,15 +299,16 @@
 
 0.0.1a
 ------
 
 - Split the package fluiddyn between one base package and specialized
   packages.
 
-.. _Unreleased: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.7.2...branch%2Fdefault
+.. _Unreleased: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.7.3...branch%2Fdefault
+.. _0.7.2: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.7.2...0.7.3
 .. _0.7.2: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.7.1...0.7.2
 .. _0.7.1: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.7.0...0.7.1
 .. _0.7.0: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.6.1...0.7.0
 .. _0.6.1: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.6.0...0.6.1
 .. _0.6.0: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.5.1...0.6.0
 .. _0.5.1: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.5.0...0.5.1
 .. _0.5.0: https://foss.heptapod.net/fluiddyn/fluidsim/-/compare/0.4.1...0.5.0
```

### Comparing `fluidsim-0.7.2/CONTRIBUTING.md` & `fluidsim-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/LICENSE.txt` & `fluidsim-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/Makefile` & `fluidsim-0.7.3/Makefile`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/PKG-INFO` & `fluidsim-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidsim
-Version: 0.7.2
+Version: 0.7.3
 Summary: Framework for studying fluid dynamics with simulations.
 Home-page: https://fluidsim.readthedocs.io
 Author: Pierre Augier
 Author-email: pierre.augier@legi.cnrs.fr
 License: CeCILL
 Project-URL: Source, https://foss.heptapod.net/fluiddyn/fluidsim
 Project-URL: Documentation, https://fluidsim.readthedocs.io
@@ -13,17 +13,17 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Provides-Extra: doc
 Provides-Extra: fft
 Provides-Extra: sphere
 Provides-Extra: mpi
 Provides-Extra: test
 Provides-Extra: dev
```

### Comparing `fluidsim-0.7.2/README.rst` & `fluidsim-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/__init__.py` & `fluidsim-0.7.3/fluidsim/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,19 +70,15 @@
         )
 
 from ._version import __version__, get_local_version
 
 from fluiddyn.io import FLUIDSIM_PATH
 
 # has to be done before importing util
-try:
-    path_dir_results = Path(FLUIDSIM_PATH)
-except TypeError:
-    # to be able to import for transonic
-    path_dir_results = None
+from fluidsim_core.paths import path_dir_results
 
 from .util import (
     available_solver_keys,
     import_module_solver_from_key,
     import_simul_class_from_key,
     load_sim_for_plot,
     load_state_phys_file,
```

### Comparing `fluidsim-0.7.2/fluidsim/_version.py` & `fluidsim-0.7.3/fluidsim/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 https://www.python.org/dev/peps/pep-0440/#local-version-identifiers
 https://github.com/pypa/setuptools_scm#setuptools_scm
 
 """
 
 # NOTE: Version autogenerated by setup.py. Do not manually edit here.
 # Update version in lib/fluidsim_core/_version.py instead.
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 
 __all__ = ["__version__", "get_local_version", "__about__"]
 
 try:
     from pyfiglet import figlet_format
```

### Comparing `fluidsim-0.7.2/fluidsim/_version.tpl` & `fluidsim-0.7.3/fluidsim/_version.tpl`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/forcing/anisotropic.py` & `fluidsim-0.7.3/fluidsim/base/forcing/anisotropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     def __init__(self, sim):
         super().__init__(sim)
 
         if self.params.forcing.normalized.type == "particular_k":
             raise NotImplementedError
 
     def _create_params_coarse(self, fft_size):
-
         params_coarse = super()._create_params_coarse(fft_size)
 
         self.angle = angle = ensure_radians(self.params.forcing[self.tag].angle)
 
         tmp = self.params.forcing.tcrandom_anisotropic
         try:
             delta_angle = tmp.delta_angle
@@ -161,15 +160,14 @@
             self.params.oper.nz
         except AttributeError:
             ndim = 2
         else:
             ndim = 3
 
         if delta_angle is None:
-
             self.khmin_forcing = np.sin(angle) * self.kmin_forcing
             self.kvmin_forcing = np.cos(angle) * self.kmin_forcing
 
             if ndim == 2:
                 Kh = self.oper_coarse.KX
                 Kv = self.oper_coarse.KY
             else:
@@ -193,15 +191,14 @@
                 )
 
             COND_NO_F = np.logical_or(COND_NO_F_KH, COND_NO_F_KV)
             COND_NO_F[self.oper_coarse.shapeK_loc[0] // 2] = True
             COND_NO_F[:, self.oper_coarse.shapeK_loc[1] - 1] = True
 
         else:
-
             if ndim == 2:
                 K = np.sqrt(self.oper_coarse.KX**2 + self.oper_coarse.KY**2)
                 Kv = self.oper_coarse.KY
             else:
                 K = np.sqrt(
                     self.oper_coarse.Kx**2
                     + self.oper_coarse.Ky**2
```

### Comparing `fluidsim-0.7.2/fluidsim/base/forcing/base.py` & `fluidsim-0.7.3/fluidsim/base/forcing/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,14 @@
     def __init__(self, sim):
         params = sim.params
         self.type_forcing = params.forcing.type
 
         dict_classes = sim.info.solver.classes.Forcing.import_classes()
 
         if self.type_forcing not in dict_classes:
-
             # temporary trick to open old simulations
             if self.type_forcing == "random" and "tcrandom" in dict_classes:
                 self.type_forcing = "tcrandom"
                 params.forcing.__dict__["tcrandom"] = params.forcing["random"]
             else:
                 if mpi.rank == 0:
                     print("dict_classes:", dict_classes)
```

### Comparing `fluidsim-0.7.2/fluidsim/base/forcing/kolmogorov.py` & `fluidsim-0.7.3/fluidsim/base/forcing/kolmogorov.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         if not hasattr(params.forcing, "kolmo"):
             params.forcing._set_child(
                 "kolmo",
                 attribs={"ik": 3, "amplitude": None, "letter_gradient": None},
             )
 
     def __init__(self, sim):
-
         if len(sim.oper.axes) == 3:
             self._key_forced_default = "vx_fft"
         else:
             self._key_forced_default = "ux_fft"
 
         super().__init__(sim)
```

### Comparing `fluidsim-0.7.2/fluidsim/base/forcing/milestone.py` & `fluidsim-0.7.3/fluidsim/base/forcing/milestone.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 def step(x, limit, smoothness):
     return 0.5 * (np.tanh((-x + limit) / smoothness) + 1)
 
 
 class PeriodicUniform:
     def __init__(self, speed_max, length, length_acc, lx):
-
         self.speed_max = speed_max
 
         sign = np.sign(speed_max)
         x_uni = length - 2 * length_acc
         t_uni = x_uni / abs(speed_max)
         self.acc = sign * speed_max**2 / (2 * length_acc)
         t_a = speed_max / self.acc
@@ -41,15 +40,14 @@
         self.t_4 = self.t_3 + t_uni
 
         self.x_0 = lx / 2 - sign * length / 2
         self.x_1 = self.x_4 = self.x_0 + sign * length_acc
         self.x_2 = self.x_3 = self.x_0 + sign * (length_acc + x_uni)
 
     def get_speed(self, time):
-
         speed_max = self.speed_max
         acc = self.acc
         t_1 = self.t_1
         t_2 = self.t_2
         t_3 = self.t_3
         t_4 = self.t_4
 
@@ -70,15 +68,14 @@
             return -speed_max
         # acceleration 3
         elif time > t_4:
             t = time - t_4
             return -speed_max + acc * t
 
     def get_locations(self, time):
-
         speed_max = self.speed_max
         acc = self.acc
         t_1 = self.t_1
         t_2 = self.t_2
         t_3 = self.t_3
         t_4 = self.t_4
 
@@ -232,15 +229,14 @@
             sinusoidal = self.params_milestone.movement.sinusoidal
             self._half_length = sinusoidal.length / 2
             self._omega = 2 * pi / sinusoidal.period
             self.get_locations = self.get_locations_sinusoidal
             self.get_speed = self.get_speed_sinusoidal
 
         elif type_movement == "periodic_uniform":
-
             params_pu = self.params_milestone.movement.periodic_uniform
             periodic_uniform = PeriodicUniform(
                 params_pu.speed,
                 params_pu.length,
                 params_pu.length_acc,
                 sim.params.oper.Lx,
             )
@@ -254,15 +250,14 @@
             self.get_locations = get_locations
             self.get_speed = periodic_uniform.get_speed
             self.period = periodic_uniform.period
         else:
             raise NotImplementedError
 
     def get_solid_field(self, time):
-
         if mpi.rank > 0 and (self._is_using_coarse_oper or self.ndim == 3):
             return (None,) * 3
 
         oper = self.oper_coarse
         lx = oper.Lx
         radius = self.params_milestone.objects.diameter / 2
 
@@ -295,15 +290,14 @@
         ) * np.ones(self.number_objects)
         return x_coors, self.y_coors
 
     def get_speed_sinusoidal(self, time):
         return self._half_length * self._omega * cos(self._omega * time - pi / 2)
 
     def check_plot_solid(self, time):
-
         solid, x_coors, y_coors = self.get_solid_field(time)
 
         fig, ax = plt.subplots()
         oper_c = self.oper_coarse
         lx = oper_c.Lx
         ly = oper_c.Ly
 
@@ -314,15 +308,14 @@
         pcmesh = ax.pcolormesh(xs, ys, solid)
         ax.axis("equal")
         ax.set_xlim((0, lx))
         ax.set_ylim((0, ly))
         fig.colorbar(pcmesh)
 
     def check_plot_forcing(self, time):
-
         self.compute(time)
 
         try:
             fx = self.fstate.state_phys.get_var("ux")
         except ValueError:
             raise NotImplementedError(
                 "check_plot_forcing is not implemented for this solver. "
@@ -348,15 +341,14 @@
 
         ax.axis("equal")
         ax.set_xlim((0, lx))
         ax.set_ylim((0, ly))
         fig.colorbar(pcmesh)
 
     def check_with_animation(self, number_frames=40, interval=500):
-
         oper_c = self.oper_coarse
 
         lx = oper_c.Lx
         ly = oper_c.Ly
 
         nx = oper_c.nx
         ny = oper_c.ny
@@ -424,15 +416,14 @@
             self.oper_coarse_shapeK_loc,
         )
 
         self.sim.oper.ifft_as_arg(self.solid_fft, self.solid)
         return self.solid
 
     def compute(self, time=None):
-
         sim = self.sim
 
         if time is None:
             time = sim.time_stepping.t
 
         solid, x_coors, y_coors = self.get_solid_field(time)
 
@@ -453,15 +444,14 @@
             fy_fft = sim.oper.fft(fy)
             if sim.params.oper.NO_SHEAR_MODES:
                 sim.oper.dealiasing(fx_fft, fy_fft)
             self.fstate.init_statespect_from(ux_fft=fx_fft, uy_fft=fy_fft)
 
 
 if __name__ == "__main__":
-
     # from time import perf_counter
 
     from fluidsim.solvers.ns2d.with_uxuy import Simul
 
     # from fluidsim.solvers.ns2d.solver import Simul
 
     params = Simul.create_default_params()
```

### Comparing `fluidsim-0.7.2/fluidsim/base/forcing/specific.py` & `fluidsim-0.7.3/fluidsim/base/forcing/specific.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     tag = "specific"
 
     @classmethod
     def _complete_params_with_default(cls, params):
         params.forcing.available_types.append(cls.tag)
 
     def __init__(self, sim):
-
         self.sim = sim
         self.oper = sim.oper
         self.params = sim.params
 
 
 class SpecificForcingPseudoSpectralSimple(SpecificForcing):
     """Specific forcing for pseudo-spectra solvers"""
@@ -159,15 +158,14 @@
         if any(np.greater(shape_forcing, shape)):
             raise NotImplementedError(
                 "The resolution is too small for the required forcing: "
                 f"any(np.greater({shape_forcing}, {shape}))"
             )
 
     def __init__(self, sim):
-
         super().__init__(sim)
 
         params = sim.params
 
         self.forcing_fft = SetOfVariables(
             like=sim.state.state_spect, info="forcing_fft", value=0.0
         )
@@ -451,15 +449,14 @@
                     "constant_rate_of": None,
                 },
             )
 
             params.forcing._set_doc("How the forcing is normalized")
 
     def __init__(self, sim):
-
         super().__init__(sim)
 
         params_norm = self.params.forcing.normalized
 
         if not hasattr(params_norm, "constant_rate_of"):
             params_norm._set_attr("constant_rate_of", None)
 
@@ -743,15 +740,14 @@
 
         try:
             params.forcing.random
         except AttributeError:
             params.forcing._set_child("random", {"only_positive": False})
 
     def __init__(self, sim):
-
         super().__init__(sim)
 
         if self.params.forcing.random.only_positive:
             self._min_val = None
         else:
             self._min_val = -1
 
@@ -786,19 +782,17 @@
             params.forcing.tcrandom
         except AttributeError:
             params.forcing._set_child(
                 "tcrandom", {"time_correlation": "based_on_forcing_rate"}
             )
 
     def __init__(self, sim):
-
         super().__init__(sim)
 
         if mpi.rank == 0:
-
             self._forcing_state_file_path = (
                 Path(sim.output.path_run) / "_forcing_state.txt"
             )
 
             if self._forcing_state_file_path.exists():
                 with open(self._forcing_state_file_path) as file:
                     lines = file.readlines()
```

### Comparing `fluidsim-0.7.2/fluidsim/base/forcing/test_kolmogorov.py` & `fluidsim-0.7.3/fluidsim/base/forcing/test_kolmogorov.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/init_fields.py` & `fluidsim-0.7.3/fluidsim/base/init_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
 """
         )
 
         dict_classes = info_solver.classes.InitFields.import_classes()
         iter_complete_params(params, info_solver, dict_classes.values())
 
     def __init__(self, sim):
-
         self.sim = sim
         params = sim.params
         oper = sim.oper
 
         self.params = params
         self.oper = oper
 
@@ -135,29 +134,27 @@
         params.init_fields.available_types.append(cls.tag)
 
     def __init__(self, sim):
         self.sim = sim
 
 
 class InitFieldsFromFile(SpecificInitFields):
-
     tag = "from_file"
 
     @classmethod
     def _complete_params_with_default(cls, params):
         super()._complete_params_with_default(params)
         params.init_fields._set_child(cls.tag, attribs={"path": ""})
         params.init_fields.from_file._set_doc(
             """
 path: str
 """
         )
 
     def __call__(self):
-
         # Warning: this function is for 2d pseudo-spectral solver!
         # We have to write something more general.
 
         params = self.sim.params
 
         path_file = params.init_fields.from_file.path
         if isinstance(path_file, Path):
@@ -297,15 +294,14 @@
             self.sim.state.statespect_from_statephys()
             self.sim.state.statephys_from_statespect()
         self.sim.time_stepping.t = time
         self.sim.time_stepping.it = it
 
 
 def fill_field_fft_2d(field_fft_in, field_fft_out):
-
     [nk0_seq, nk1_seq] = field_fft_out.shape
     [nk0_seq_in, nk1_seq_in] = field_fft_in.shape
 
     nk0_min = min(nk0_seq, nk0_seq_in)
     nk1_min = min(nk1_seq, nk1_seq_in)
 
     # it is a little bit complicate to take into account ky
@@ -315,15 +311,14 @@
     for ik0 in range(1, nk0_min // 2):
         for ik1 in range(nk1_min):
             field_fft_out[ik0, ik1] = field_fft_in[ik0, ik1]
             field_fft_out[-ik0, ik1] = field_fft_in[-ik0, ik1]
 
 
 def fill_field_fft_3d(field_fft_in, field_fft_out, oper_in, oper_out):
-
     [nk0, nk1, nk2] = field_fft_out.shape
     [nk0_in, nk1_in, nk2_in] = field_fft_in.shape
 
     nk0_min = min(nk0, nk0_in)
     nk1_min = min(nk1, nk1_in)
     nk2_min = min(nk2, nk2_in)
 
@@ -339,15 +334,14 @@
                     kx_adim,
                     ky_adim,
                     kz_adim,
                 )
 
 
 class InitFieldsFromSimul(SpecificInitFields):
-
     tag = "from_simul"
 
     def __call__(self):
         self.sim.init_fields.get_state_from_simul = self._get_state_from_simul
 
     def _make_state_spect_2d(self, sim_in):
         sim = self.sim
@@ -386,15 +380,14 @@
             field_fft_in = sim_in.state.state_spect[index_key]
             field_fft_new_res = state_spect[index_key]
             fill_field_fft_3d(field_fft_in, field_fft_new_res, oper_in, sim.oper)
 
         return state_spect
 
     def _get_state_from_simul(self, sim_in):
-
         # Warning: this function is for 2d pseudo-spectral solver!
         # We have to write something more general.
         # It should be done directly in the operators.
 
         if mpi.nb_proc > 1:
             raise NotImplementedError(
                 "THIS METHOD WON'T BE IMPLEMENTED IN MPI. "
@@ -436,27 +429,25 @@
             #     else:
             #         sim.state.state_spect[k] = self.oper.create_arrayK(value=0.0)
 
         sim.state.statephys_from_statespect()
 
 
 class InitFieldsInScript(SpecificInitFields):
-
     tag = "in_script"
 
     def __call__(self):
         self.sim.state.is_initialized = False
         self.sim.output.print_stdout(
             "Manual initialization of the fields is selected. "
             "Do not forget to initialize them."
         )
 
 
 class InitFieldsConstant(SpecificInitFields):
-
     tag = "constant"
 
     @classmethod
     def _complete_params_with_default(cls, params):
         super()._complete_params_with_default(params)
         params.init_fields._set_child(cls.tag, attribs={"value": 1.0})
         params.init_fields.constant._set_doc(
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/__init__.py` & `fluidsim-0.7.3/fluidsim/base/output/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,14 @@
         "Creation of the file "
         + path_out
         + "\nOpen it with a Xdmf reader to read the output files."
     )
 
 
 def run():
-
     parser = argparse.ArgumentParser(
         prog="fluidsim-create-xml-description",
         description=create_description_xmf_file.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
 
     parser.add_argument(
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/__pythran__/increments.cpp` & `fluidsim-0.7.3/fluidsim/base/output/__pythran__/increments.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #include <pythonic/core.hpp>
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
-#include <pythonic/include/types/bool.hpp>
 #include <pythonic/include/types/float64.hpp>
-#include <pythonic/include/types/numpy_texpr.hpp>
 #include <pythonic/include/types/int32.hpp>
+#include <pythonic/include/types/bool.hpp>
+#include <pythonic/include/types/numpy_texpr.hpp>
 #include <pythonic/include/types/ndarray.hpp>
+#include <pythonic/types/float64.hpp>
+#include <pythonic/types/bool.hpp>
 #include <pythonic/types/ndarray.hpp>
 #include <pythonic/types/numpy_texpr.hpp>
-#include <pythonic/types/float64.hpp>
 #include <pythonic/types/int32.hpp>
-#include <pythonic/types/bool.hpp>
 #include <pythonic/include/builtins/abs.hpp>
 #include <pythonic/include/builtins/getattr.hpp>
 #include <pythonic/include/builtins/range.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
 #include <pythonic/include/numpy/empty.hpp>
 #include <pythonic/include/numpy/sum.hpp>
 #include <pythonic/include/operator_/mul.hpp>
@@ -31,156 +31,163 @@
 #include <pythonic/builtins/tuple.hpp>
 #include <pythonic/numpy/empty.hpp>
 #include <pythonic/numpy/sum.hpp>
 #include <pythonic/operator_/mul.hpp>
 #include <pythonic/operator_/pow.hpp>
 #include <pythonic/operator_/sub.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_increments
+namespace 
 {
-  struct __transonic__
+  namespace __pythran_increments
   {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    struct __transonic__
     {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct strfunc_from_pdf
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 = bool>
-    struct type
+    struct strfunc_from_pdf
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef __type1 __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::empty{})>::type>::type __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type4;
-      typedef __type4 __type5;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
-      typedef decltype(std::declval<__type3>()(std::declval<__type6>())) __type7;
-      typedef typename pythonic::assignable<__type7>::type __type8;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type9;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SIZE{}, std::declval<__type5>())) __type11;
-      typedef decltype(std::declval<__type9>()(std::declval<__type11>())) __type12;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type12>::type::iterator>::value_type>::type __type13;
-      typedef __type13 __type14;
-      typedef indexable<__type14> __type15;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type16;
-      typedef typename pythonic::assignable<__type1>::type __type17;
-      typedef __type17 __type18;
-      typedef decltype(std::declval<__type16>()(std::declval<__type18>())) __type19;
-      typedef typename pythonic::assignable<__type19>::type __type20;
-      typedef typename __combined<__type17,__type20>::type __type21;
-      typedef __type21 __type22;
-      typedef long __type24;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type14>(), std::declval<__type24>())) __type25;
-      typedef decltype(std::declval<__type22>()[std::declval<__type25>()]) __type26;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type26>(), std::declval<__type26>())) __type31;
-      typedef decltype(std::declval<__type16>()(std::declval<__type31>())) __type32;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sum{})>::type>::type __type33;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type34;
-      typedef __type34 __type35;
-      typedef decltype(std::declval<__type35>()[std::declval<__type14>()]) __type37;
-      typedef decltype(std::declval<__type22>()[std::declval<__type14>()]) __type40;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type41;
-      typedef __type41 __type42;
-      typedef decltype(pythonic::builtins::pow(std::declval<__type40>(), std::declval<__type42>())) __type43;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type37>(), std::declval<__type43>())) __type44;
-      typedef decltype(std::declval<__type33>()(std::declval<__type44>())) __type45;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type45>())) __type46;
-      typedef container<typename std::remove_reference<__type46>::type> __type47;
-      typedef typename __combined<__type8,__type15,__type47>::type __type48;
-      typedef __type48 __type49;
-      typedef typename pythonic::returnable<__type49>::type __type50;
-      typedef __type2 __ptype0;
-      typedef __type50 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 = bool>
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 = bool>
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef __type1 __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::empty{})>::type>::type __type3;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type4;
+        typedef __type4 __type5;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
+        typedef decltype(std::declval<__type3>()(std::declval<__type6>())) __type7;
+        typedef typename pythonic::assignable<__type7>::type __type8;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type9;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SIZE{}, std::declval<__type5>())) __type11;
+        typedef decltype(std::declval<__type9>()(std::declval<__type11>())) __type12;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type12>::type::iterator>::value_type>::type __type13;
+        typedef __type13 __type14;
+        typedef indexable<__type14> __type15;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type16;
+        typedef typename pythonic::assignable<__type1>::type __type17;
+        typedef __type17 __type18;
+        typedef decltype(std::declval<__type16>()(std::declval<__type18>())) __type19;
+        typedef typename pythonic::assignable<__type19>::type __type20;
+        typedef typename __combined<__type17,__type20>::type __type21;
+        typedef __type21 __type22;
+        typedef decltype(pythonic::types::as_const(std::declval<__type22>())) __type23;
+        typedef long __type25;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type14>(), std::declval<__type25>())) __type26;
+        typedef decltype(std::declval<__type23>()[std::declval<__type26>()]) __type27;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type27>(), std::declval<__type27>())) __type33;
+        typedef decltype(std::declval<__type16>()(std::declval<__type33>())) __type34;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sum{})>::type>::type __type35;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type36;
+        typedef __type36 __type37;
+        typedef decltype(pythonic::types::as_const(std::declval<__type37>())) __type38;
+        typedef decltype(std::declval<__type38>()[std::declval<__type14>()]) __type40;
+        typedef decltype(std::declval<__type23>()[std::declval<__type14>()]) __type44;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type45;
+        typedef __type45 __type46;
+        typedef decltype(pythonic::builtins::pow(std::declval<__type44>(), std::declval<__type46>())) __type47;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type40>(), std::declval<__type47>())) __type48;
+        typedef decltype(std::declval<__type35>()(std::declval<__type48>())) __type49;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type34>(), std::declval<__type49>())) __type50;
+        typedef container<typename std::remove_reference<__type50>::type> __type51;
+        typedef typename __combined<__type8,__type15,__type51>::type __type52;
+        typedef __type52 __type53;
+        typedef typename pythonic::returnable<__type53>::type __type54;
+        typedef __type2 __ptype0;
+        typedef __type54 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 = bool>
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0 rxs, argument_type1 pdf, argument_type2 values, argument_type3 order, argument_type4 absolute= false) const
+      ;
+    }  ;
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0&& rxs, argument_type1&& pdf, argument_type2&& values, argument_type3&& order, argument_type4 absolute= false) const
-    ;
-  }  ;
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
+    typename __transonic__::type::result_type __transonic__::operator()() const
     {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.1"));
-      return tmp_global;
-    }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-  inline
-  typename strfunc_from_pdf::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type strfunc_from_pdf::operator()(argument_type0&& rxs, argument_type1&& pdf, argument_type2&& values, argument_type3&& order, argument_type4 absolute) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
-    typedef __type0 __type1;
-    typedef typename pythonic::assignable<__type1>::type __type2;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type3;
-    typedef __type2 __type4;
-    typedef decltype(std::declval<__type3>()(std::declval<__type4>())) __type5;
-    typedef typename pythonic::assignable<__type5>::type __type6;
-    typedef typename __combined<__type2,__type6>::type __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::empty{})>::type>::type __type9;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type10;
-    typedef __type10 __type11;
-    typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type11>())) __type12;
-    typedef decltype(std::declval<__type9>()(std::declval<__type12>())) __type13;
-    typedef typename pythonic::assignable<__type13>::type __type14;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type15;
-    typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SIZE{}, std::declval<__type11>())) __type17;
-    typedef decltype(std::declval<__type15>()(std::declval<__type17>())) __type18;
-    typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type18>::type::iterator>::value_type>::type __type19;
-    typedef __type19 __type20;
-    typedef indexable<__type20> __type21;
-    typedef __type7 __type22;
-    typedef long __type24;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type20>(), std::declval<__type24>())) __type25;
-    typedef decltype(std::declval<__type22>()[std::declval<__type25>()]) __type26;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type26>(), std::declval<__type26>())) __type31;
-    typedef decltype(std::declval<__type3>()(std::declval<__type31>())) __type32;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sum{})>::type>::type __type33;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type34;
-    typedef __type34 __type35;
-    typedef decltype(std::declval<__type35>()[std::declval<__type20>()]) __type37;
-    typedef decltype(std::declval<__type22>()[std::declval<__type20>()]) __type40;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type41;
-    typedef __type41 __type42;
-    typedef decltype(pythonic::builtins::pow(std::declval<__type40>(), std::declval<__type42>())) __type43;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type37>(), std::declval<__type43>())) __type44;
-    typedef decltype(std::declval<__type33>()(std::declval<__type44>())) __type45;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type45>())) __type46;
-    typedef container<typename std::remove_reference<__type46>::type> __type47;
-    typedef typename __combined<__type14,__type21,__type47>::type __type48;
-    typedef typename pythonic::assignable<__type48>::type __type49;
-    __type8 values_ = values;
-    __type49 S_order = pythonic::numpy::functor::empty{}(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, rxs));
-    if (absolute)
-    {
-      values_ = pythonic::builtins::functor::abs{}(values_);
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
     }
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+    inline
+    typename strfunc_from_pdf::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type strfunc_from_pdf::operator()(argument_type0 rxs, argument_type1 pdf, argument_type2 values, argument_type3 order, argument_type4 absolute) const
     {
-      long  __target140028817350592 = pythonic::builtins::getattr(pythonic::types::attr::SIZE{}, rxs);
-      for (long  irx=0L; irx < __target140028817350592; irx += 1L)
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
+      typedef __type0 __type1;
+      typedef typename pythonic::assignable<__type1>::type __type2;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type3;
+      typedef __type2 __type4;
+      typedef decltype(std::declval<__type3>()(std::declval<__type4>())) __type5;
+      typedef typename pythonic::assignable<__type5>::type __type6;
+      typedef typename __combined<__type2,__type6>::type __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::empty{})>::type>::type __type9;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type10;
+      typedef __type10 __type11;
+      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type11>())) __type12;
+      typedef decltype(std::declval<__type9>()(std::declval<__type12>())) __type13;
+      typedef typename pythonic::assignable<__type13>::type __type14;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type15;
+      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SIZE{}, std::declval<__type11>())) __type17;
+      typedef decltype(std::declval<__type15>()(std::declval<__type17>())) __type18;
+      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type18>::type::iterator>::value_type>::type __type19;
+      typedef __type19 __type20;
+      typedef indexable<__type20> __type21;
+      typedef __type7 __type22;
+      typedef decltype(pythonic::types::as_const(std::declval<__type22>())) __type23;
+      typedef long __type25;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type20>(), std::declval<__type25>())) __type26;
+      typedef decltype(std::declval<__type23>()[std::declval<__type26>()]) __type27;
+      typedef decltype(pythonic::operator_::sub(std::declval<__type27>(), std::declval<__type27>())) __type33;
+      typedef decltype(std::declval<__type3>()(std::declval<__type33>())) __type34;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sum{})>::type>::type __type35;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type36;
+      typedef __type36 __type37;
+      typedef decltype(pythonic::types::as_const(std::declval<__type37>())) __type38;
+      typedef decltype(std::declval<__type38>()[std::declval<__type20>()]) __type40;
+      typedef decltype(std::declval<__type23>()[std::declval<__type20>()]) __type44;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type45;
+      typedef __type45 __type46;
+      typedef decltype(pythonic::builtins::pow(std::declval<__type44>(), std::declval<__type46>())) __type47;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type40>(), std::declval<__type47>())) __type48;
+      typedef decltype(std::declval<__type35>()(std::declval<__type48>())) __type49;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type34>(), std::declval<__type49>())) __type50;
+      typedef container<typename std::remove_reference<__type50>::type> __type51;
+      typedef typename __combined<__type14,__type21,__type51>::type __type52;
+      typedef typename pythonic::assignable<__type52>::type __type53;
+      __type8 values_ = values;
+      __type53 S_order = pythonic::numpy::functor::empty{}(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, rxs));
+      if (absolute)
+      {
+        values_ = pythonic::builtins::functor::abs{}(values_);
+      }
       {
-        S_order.fast(irx) = pythonic::operator_::mul(pythonic::builtins::functor::abs{}(pythonic::operator_::sub(values_.fast(pythonic::types::make_tuple(irx, 1L)), values_.fast(pythonic::types::make_tuple(irx, 0L)))), pythonic::numpy::functor::sum{}(pythonic::operator_::mul(pdf.fast(irx), pythonic::builtins::pow(values_.fast(irx), order))));
+        long  __target139658376662224 = pythonic::builtins::getattr(pythonic::types::attr::SIZE{}, rxs);
+        for (long  irx=0L; irx < __target139658376662224; irx += 1L)
+        {
+          S_order.fast(irx) = pythonic::operator_::mul(pythonic::builtins::functor::abs{}(pythonic::operator_::sub(pythonic::types::as_const(values_).fast(pythonic::types::make_tuple(irx, 1L)), pythonic::types::as_const(values_).fast(pythonic::types::make_tuple(irx, 0L)))), pythonic::numpy::functor::sum{}(pythonic::operator_::mul(pythonic::types::as_const(pdf).fast(irx), pythonic::builtins::pow(pythonic::types::as_const(values_).fast(irx), order))));
+        }
       }
+      return S_order;
     }
-    return S_order;
   }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_increments::__transonic__()());
 inline
 typename __pythran_increments::strfunc_from_pdf::type<pythonic::types::ndarray<npy_int32,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, double, bool>::result_type strfunc_from_pdf0(pythonic::types::ndarray<npy_int32,pythonic::types::pshape<long>>&& rxs, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& pdf, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& values, double&& order, bool&& absolute) 
@@ -537,17 +544,17 @@
                                          Methods,
                                          ""
     );
     #endif
     if(! theModule)
         PYTHRAN_RETURN;
     PyObject * theDoc = Py_BuildValue("(sss)",
-                                      "0.12.0",
-                                      "2022-10-28 09:10:31.391139",
-                                      "3c0e732109693a4b0389754c09e9870547a1cb2060d40588674edb06dc9e62c1");
+                                      "0.13.1",
+                                      "2023-05-24 11:29:39.298951",
+                                      "73194a1181a3d795a9e99319b62f4bb2efdd40dc09f9ed476112ee2672957415");
     if(! theDoc)
         PYTHRAN_RETURN;
     PyModule_AddObject(theModule,
                        "__pythran__",
                        theDoc);
 
     PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/__pythran__/spatiotemporal_spectra.cpp` & `fluidsim-0.7.3/fluidsim/base/output/__pythran__/spatiotemporal_spectra.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 #include <pythonic/include/types/float32.hpp>
-#include <pythonic/include/types/float64.hpp>
 #include <pythonic/include/types/ndarray.hpp>
-#include <pythonic/types/float32.hpp>
+#include <pythonic/include/types/float64.hpp>
 #include <pythonic/types/float64.hpp>
 #include <pythonic/types/ndarray.hpp>
+#include <pythonic/types/float32.hpp>
 #include <pythonic/include/builtins/ValueError.hpp>
 #include <pythonic/include/builtins/enumerate.hpp>
 #include <pythonic/include/builtins/len.hpp>
 #include <pythonic/include/builtins/print.hpp>
 #include <pythonic/include/builtins/str/__mod__.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
 #include <pythonic/include/numpy/arange.hpp>
@@ -160,15 +160,15 @@
     typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0&& times, argument_type1&& tmin, argument_type2&& tmax) const
     ;
   }  ;
   inline
   typename __transonic__::type::result_type __transonic__::operator()() const
   {
     {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.0"));
+      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.1"));
       return tmp_global;
     }
   }
   template <typename argument_type0 , typename argument_type1 >
   inline
   typename find_index_first_l::type<argument_type0, argument_type1>::result_type find_index_first_l::operator()(argument_type0&& arr, argument_type1&& value) const
   {
@@ -665,17 +665,17 @@
                                          Methods,
                                          ""
     );
     #endif
     if(! theModule)
         PYTHRAN_RETURN;
     PyObject * theDoc = Py_BuildValue("(sss)",
-                                      "0.11.0",
-                                      "2022-09-07 15:05:05.635849",
-                                      "5649b206c9a3bc82b27c489ba6a9213635d768447aa586c7d07fab000ffd4d38");
+                                      "0.12.0",
+                                      "2022-11-30 15:27:57.545072",
+                                      "71c4583a576e4b24f7e61ffcddbbc62d4d9c4bea9965d1a05aa42fd10e38f89a");
     if(! theDoc)
         PYTHRAN_RETURN;
     PyModule_AddObject(theModule,
                        "__pythran__",
                        theDoc);
 
     PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/base.py` & `fluidsim-0.7.3/fluidsim/base/output/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,14 @@
         self.post_init()
 
     def post_init(self):
         sim = self.sim
         super().post_init()
 
         if mpi.rank == 0:
-
             objects_to_print = {
                 "sim.oper": sim.oper,
                 "sim.state": sim.state,
                 "sim.time_stepping": sim.time_stepping,
                 "sim.init_fields": sim.init_fields,
             }
 
@@ -260,15 +259,14 @@
         ):
             super()._save_info_solver_params_xml(
                 replace=replace,
                 comment=f"FluidSim {fluidsim.get_local_version()}",
             )
 
     def init_with_initialized_state(self):
-
         if (
             hasattr(self, "_has_been_initialized_with_state")
             and self._has_been_initialized_with_state
         ):
             return
 
         else:
@@ -309,15 +307,14 @@
 
         try:
             self.print_size_in_Mo(self.sim.state.state_spect, "state_spect")
         except AttributeError:
             self.print_size_in_Mo(self.sim.state.state_phys, "state_phys")
 
     def one_time_step(self):
-
         for k in self.params.periods_print._get_key_attribs():
             period = self.params.periods_print.__dict__[k]
             if period != 0:
                 self.__dict__[k]._online_print()
 
         if self.params.ONLINE_PLOT_OK:
             for k in self.params.periods_plot._get_key_attribs():
@@ -455,15 +452,14 @@
 
         """
         return get_mean_values_from_path(
             self.path_run, tmin, tmax, use_cache, customize
         )
 
     def _compute_mean_values(self, tmin, tmax):
-
         result = {}
 
         try:
             result["N"] = self.sim.params.N
         except AttributeError:
             pass
 
@@ -534,15 +530,14 @@
         self,
         output,
         period_save=0,
         period_plot=0,
         has_to_plot_saved=False,
         arrays_1st_time=None,
     ):
-
         sim = output.sim
         params = sim.params
 
         self.output = output
         self.sim = sim
         self.oper = sim.oper
         self.params = params
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/cross_corr3d.py` & `fluidsim-0.7.3/fluidsim/base/output/cross_corr3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     small_key = key[:-4]
     if len(small_key) == 2 and small_key.startswith("v"):
         return small_key[1:]
     return small_key
 
 
 class CrossCorrelations(BaseSpectra):
-
     _tag = "cross_corr"
 
     def compute(self):
         """compute the values at one time."""
 
         keys = self.sim.state.keys_state_spect
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/horiz_means.py` & `fluidsim-0.7.3/fluidsim/base/output/horiz_means.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         not yet been created (and cannot yet be modified)! This is why one
         needs to create a function that will be called later to modify
         ``info_solver``.
 
         """
 
         def modif_info_solver(info_solver):
-
             info_solver.classes.Output.classes._set_child(
                 cls._tag,
                 attribs={
                     "module_name": cls._module_name,
                     "class_name": cls.__name__,
                 },
             )
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/increments.py` & `fluidsim-0.7.3/fluidsim/base/output/increments.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,14 @@
                     )
 
         pdf_timemean /= nt
 
         return pdf_timemean, values_inc_timemean, nb_rx_to_plot
 
     def plot_pdf(self, tmin=0, tmax=None, key_var="ux", order=0, nb_rx_to_plot=5):
-
         irx_to_plot = np.arange(
             0, self.rxs.size, self.rxs.size / nb_rx_to_plot
         ).astype(int)
         nb_rx_to_plot = irx_to_plot.size
 
         (
             pdf_timemean,
@@ -475,15 +474,14 @@
 
         ax1.set_xlabel(key_var)
         ax1.set_ylabel(r"PDF x $\delta v^" + repr(order) + "$")
 
         colors = ["k", "y", "r", "b", "g", "m", "c"]
 
         for irxp, irx in enumerate(irx_to_plot):
-
             print("color = {}, rx = {}".format(colors[irxp], self.rxs[irx]))
 
             val_inc = values_inc_timemean[irxp]
 
             ax1.plot(
                 val_inc,
                 pdf_timemean[irxp] * val_inc**order,
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/model.xmf` & `fluidsim-0.7.3/fluidsim/base/output/model.xmf`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/output/phys_fields.py` & `fluidsim-0.7.3/fluidsim/base/output/phys_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,14 @@
     """A set of physical field files."""
 
     time_from_path = staticmethod(time_from_path)
 
     def _get_field_to_plot_from_file(
         self, path_file, key, equation, skip_vars=()
     ):
-
         with h5py.File(path_file, "r") as file:
             time = file["state_phys"].attrs["time"]
             dset = file["state_phys"][key]
 
             if equation is None:
                 return dset[...], time
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/phys_fields1d.py` & `fluidsim-0.7.3/fluidsim/base/output/phys_fields1d.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/output/phys_fields2d.py` & `fluidsim-0.7.3/fluidsim/base/output/phys_fields2d.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/output/phys_fields3d.py` & `fluidsim-0.7.3/fluidsim/base/output/phys_fields3d.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/output/print_stdout.py` & `fluidsim-0.7.3/fluidsim/base/output/print_stdout.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
             if not os.path.exists(self.path_file):
                 self.file = open(self.path_file, "w")
             else:
                 self.file = open(self.path_file, "r+")
                 self.file.seek(0, 2)  # go to the end of the file
 
     def complete_init_with_state(self):
-
         self.energy0 = self.output.compute_energy()
 
         if self.period_print == 0:
             return
 
         self.energy_temp = self.energy0 + 0.0
         self.t_last_print_info = -self.period_print
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/prob_dens_func.py` & `fluidsim-0.7.3/fluidsim/base/output/prob_dens_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
             "bin_edges_u": bin_edges_u,
         }
         return dict_pdf
 
     def load(self):
         """load the saved pdf and return a dictionary."""
         with h5py.File(self.path_file, "r") as h5file:
-
             dset_pdf_eta = h5file["pdf_eta"]
             dset_bin_edges_eta = h5file["bin_edges_eta"]
 
             pdf_eta = dset_pdf_eta[...]
             bin_edges_eta = dset_bin_edges_eta[...]
 
             dset_pdf_u = h5file["pdf_u"]
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/spatial_means.py` & `fluidsim-0.7.3/fluidsim/base/output/spatial_means.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
         if self.period_save != 0:
             # saved for each initialization to help detecting bugs
             self._save_one_time()
             self.t_last_save = self.sim.time_stepping.t
 
     def _init_files(self, arrays_1st_time=None):
-
         if mpi.rank == 0:
             if not os.path.exists(self.path_file):
                 self.file = open(self.path_file, "w")
             else:
                 self.file = open(self.path_file, "r+")
                 # to go to the end of the file
                 self.file.seek(0, os.SEEK_END)
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/spatiotemporal_spectra.py` & `fluidsim-0.7.3/fluidsim/base/output/spatiotemporal_spectra.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/output/spect_energy_budget.py` & `fluidsim-0.7.3/fluidsim/base/output/spect_energy_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     def _complete_params_with_default(params):
         tag = "spect_energy_budg"
 
         params.output.periods_save._set_attrib(tag, 0)
         params.output._set_child(tag, attribs={"HAS_TO_PLOT_SAVED": False})
 
     def __init__(self, output):
-
         params = output.sim.params
         self.nx = params.oper.nx
 
         self.spectrum2D_from_fft = output.sim.oper.spectrum2D_from_fft
         self.spectra1D_from_fft = output.sim.oper.spectra1D_from_fft
         self.sum_wavenumbers = output.sim.oper.sum_wavenumbers
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/spectra.py` & `fluidsim-0.7.3/fluidsim/base/output/spectra.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/output/spectra3d.py` & `fluidsim-0.7.3/fluidsim/base/output/spectra3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,14 @@
         )
         with h5py.File(self.path_file1d, "r") as h5file:
             for key in ("kx", "ky", "kz"):
                 results[key] = h5file[key][...]
         return results
 
     def load_kzkh_mean(self, tmin=None, tmax=None, key_to_load=None):
-
         if not os.path.exists(self.path_file_kzkh):
             raise RuntimeError(
                 self.path_file_kzkh
                 + " does not exist. Can't load values from it."
             )
 
         results = self._load_mean_file(
```

### Comparing `fluidsim-0.7.2/fluidsim/base/output/spectra_multidim.py` & `fluidsim-0.7.3/fluidsim/base/output/spectra_multidim.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/output/temporal_spectra.py` & `fluidsim-0.7.3/fluidsim/base/output/temporal_spectra.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/output/time_signals_fft.py` & `fluidsim-0.7.3/fluidsim/base/output/time_signals_fft.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,22 +269,20 @@
                 "q_array_ik": q_array_ik,
                 "d_array_ik": d_array_ik,
                 "a_array_ik": a_array_ik,
             }
             return dict_results
 
     def load(self):
-
         if not os.path.exists(self.path_file):
             raise ValueError(
                 "no file time_sigK.h5 in\n" + self.output.dir_save_run
             )
 
         with h5py.File(self.path_file, "r+") as file:
-
             dset_times = file["times"]
             times = dset_times[...]
 
             dict_results = {}
             dict_results["times"] = times
 
             dict_results["nb_shells"] = file.attrs["nb_shells"]
@@ -327,15 +325,14 @@
         sig_d_fft = dict_results["sig_d_fft"]
 
         kh_shell = dict_results["kh_shell"]
         omega_shell = dict_results["omega_shell"]
         period_shell = 2 * np.pi / omega_shell
 
         for ish in range(nb_shells):
-
             fig, ax1 = self.output.figure_axe()
             ax1.set_xlabel("$t/T$")
             ax1.set_ylabel("signals (s$^{-1}$)")
             ax1.set_title(
                 "signals eigenmodes, ikh = {:.2f}\n".format(
                     (kh_shell[ish] / self.sim.oper.deltak)
                 )
@@ -357,15 +354,14 @@
 
         fig, ax1 = self.output.figure_axe()
         ax1.set_xlabel(r"$\omega$")
         ax1.set_ylabel("kh_shell")
         ax1.loglog(kh_shell, omega_shell, "o", linewidth=2)
 
     def time_spectrum(self, sig_long):
-
         Nt = sig_long.size
         stepit0 = int(np.fix(self.nt / 2.0))
 
         nb_spectra = 0
         it0 = 0
         spect = np.zeros([self.nt // 2 + 1])
         while it0 + self.nt < Nt:
```

### Comparing `fluidsim-0.7.2/fluidsim/base/params.py` & `fluidsim-0.7.3/fluidsim/base/params.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/preprocess/base.py` & `fluidsim-0.7.3/fluidsim/base/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/preprocess/pseudo_spect.py` & `fluidsim-0.7.3/fluidsim/base/preprocess/pseudo_spect.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/preprocess/test.py` & `fluidsim-0.7.3/fluidsim/base/preprocess/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 from fluidsim.base.solvers.pseudo_spect import SimulBasePseudoSpectral
 
 from fluidsim.util.testing import TestSimul, skip_if_no_fluidfft
 
 
 @skip_if_no_fluidfft
 class TestPreprocessPS(TestSimul):
-
     Simul = SimulBasePseudoSpectral
 
     @classmethod
     def init_params(cls):
-
         cls.params = params = SimulBasePseudoSpectral.create_default_params()
         params.short_name_type_run = "test_preprocess_ps"
         nh = 16
         Lh = 2 * np.pi
         params.oper.nx = nh
         params.oper.ny = nh
         params.oper.Lx = Lh
```

### Comparing `fluidsim-0.7.2/fluidsim/base/solvers/base.py` & `fluidsim-0.7.3/fluidsim/base/solvers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,14 @@
         return tendencies
 
 
 Simul = SimulBase
 
 
 if __name__ == "__main__":
-
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
     params.time_stepping.USE_CFL = False
     params.time_stepping.t_end = 2.0
     params.time_stepping.deltat0 = 0.1
```

### Comparing `fluidsim-0.7.2/fluidsim/base/solvers/finite_diff.py` & `fluidsim-0.7.3/fluidsim/base/solvers/finite_diff.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from fluidsim.base.solvers.base import InfoSolverBase
 
 
 class InfoSolverFiniteDiff(InfoSolverBase):
     """Contain the information on a solver."""
 
     def _init_root(self):
-
         super()._init_root()
 
         # self.classes.State.module_name = 'fluidsim.base.state'
         # self.classes.State.class_name = 'StateBase'
 
         self.classes.TimeStepping.module_name = (
             "fluidsim.base.time_stepping.finite_diff"
```

### Comparing `fluidsim-0.7.2/fluidsim/base/solvers/info_base.py` & `fluidsim-0.7.3/fluidsim/base/solvers/info_base.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/solvers/pseudo_spect.py` & `fluidsim-0.7.3/fluidsim/base/solvers/pseudo_spect.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,14 @@
         return tendencies
 
 
 Simul = SimulBasePseudoSpectral
 
 
 if __name__ == "__main__":
-
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
 
     nh = 16
```

### Comparing `fluidsim-0.7.2/fluidsim/base/sphericalharmo/output.py` & `fluidsim-0.7.3/fluidsim/base/sphericalharmo/output.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/sphericalharmo/phys_fields.py` & `fluidsim-0.7.3/fluidsim/base/sphericalharmo/phys_fields.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/sphericalharmo/solver.py` & `fluidsim-0.7.3/fluidsim/base/sphericalharmo/solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/sphericalharmo/state.py` & `fluidsim-0.7.3/fluidsim/base/sphericalharmo/state.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/state.py` & `fluidsim-0.7.3/fluidsim/base/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,14 @@
         info_solver.classes.State.keys_phys_needed = ["ux", "uy"]
 
         info_solver.classes.State._set_attribs(
             {"keys_state_spect": ["ux_fft", "uy_fft"]}
         )
 
     def __init__(self, sim, oper=None):
-
         super().__init__(sim, oper)
 
         self.keys_state_spect = sim.info.solver.classes.State.keys_state_spect
         self.state_spect = SetOfVariables(
             keys=self.keys_state_spect,
             shape_variable=self.oper.shapeK_loc,
             dtype=np.complex128,
```

### Comparing `fluidsim-0.7.2/fluidsim/base/test/test_base_solver.py` & `fluidsim-0.7.3/fluidsim/base/test/test_base_solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/test/test_base_solver_ps.py` & `fluidsim-0.7.3/fluidsim/base/test/test_base_solver_ps.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/test/test_params.py` & `fluidsim-0.7.3/fluidsim/base/test/test_params.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/time_stepping/__pythran__/pseudo_spect.cpp` & `fluidsim-0.7.3/fluidsim/base/time_stepping/__pythran__/pseudo_spect.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -2,630 +2,470 @@
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 #include <pythonic/include/types/float64.hpp>
-#include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/include/types/complex128.hpp>
-#include <pythonic/types/ndarray.hpp>
+#include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/types/float64.hpp>
+#include <pythonic/types/ndarray.hpp>
 #include <pythonic/types/complex128.hpp>
 #include <pythonic/include/builtins/None.hpp>
 #include <pythonic/include/builtins/dict.hpp>
 #include <pythonic/include/builtins/pythran/static_list.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
+#include <pythonic/include/numpy/copyto.hpp>
 #include <pythonic/include/numpy/exp.hpp>
 #include <pythonic/include/operator_/add.hpp>
 #include <pythonic/include/operator_/div.hpp>
 #include <pythonic/include/operator_/iadd.hpp>
 #include <pythonic/include/operator_/idiv.hpp>
 #include <pythonic/include/operator_/mul.hpp>
 #include <pythonic/include/operator_/neg.hpp>
 #include <pythonic/include/types/complex.hpp>
 #include <pythonic/include/types/slice.hpp>
 #include <pythonic/include/types/str.hpp>
 #include <pythonic/builtins/None.hpp>
 #include <pythonic/builtins/dict.hpp>
 #include <pythonic/builtins/pythran/static_list.hpp>
 #include <pythonic/builtins/tuple.hpp>
+#include <pythonic/numpy/copyto.hpp>
 #include <pythonic/numpy/exp.hpp>
 #include <pythonic/operator_/add.hpp>
 #include <pythonic/operator_/div.hpp>
 #include <pythonic/operator_/iadd.hpp>
 #include <pythonic/operator_/idiv.hpp>
 #include <pythonic/operator_/mul.hpp>
 #include <pythonic/operator_/neg.hpp>
 #include <pythonic/types/complex.hpp>
 #include <pythonic/types/slice.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_pseudo_spect
+namespace 
 {
-  struct __transonic__
+  namespace __pythran_pseudo_spect
   {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    struct __transonic__
     {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct arguments_blocks
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::static_list{})>::type>::type __type1;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type2;
+        typedef decltype(std::declval<__type1>()(std::declval<__type2>())) __type3;
+        typedef pythonic::types::dict<__type0,__type3> __type4;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type5;
+        typedef decltype(std::declval<__type1>()(std::declval<__type5>())) __type6;
+        typedef pythonic::types::dict<__type0,__type6> __type7;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type8;
+        typedef decltype(std::declval<__type1>()(std::declval<__type8>())) __type9;
+        typedef pythonic::types::dict<__type0,__type9> __type10;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type11;
+        typedef decltype(std::declval<__type1>()(std::declval<__type11>())) __type12;
+        typedef pythonic::types::dict<__type0,__type12> __type13;
+        typedef typename __combined<__type4,__type7,__type10,__type13>::type __type14;
+        typedef typename pythonic::returnable<__type14>::type __type15;
+        typedef __type15 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct rk4_step3
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef pythonic::types::none_type __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 state_spect, argument_type1 state_spect_tmp, argument_type2 tendencies_3, argument_type3 dt) const
+      ;
+    }  ;
+    struct rk4_step2
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 , typename argument_type6 >
+      struct type
+      {
+        typedef pythonic::types::none_type __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 , typename argument_type6 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5, argument_type6>::result_type operator()(argument_type0 state_spect, argument_type1 state_spect_tmp, argument_type2 state_spect_1_approx, argument_type3 tendencies_2, argument_type4 diss, argument_type5 diss2, argument_type6 dt) const
+      ;
+    }  ;
+    struct rk4_step1
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      struct type
+      {
+        typedef pythonic::types::none_type __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0 state_spect, argument_type1 state_spect_tmp, argument_type2 state_spect_12_approx2, argument_type3 tendencies_1, argument_type4 diss2, argument_type5 dt) const
+      ;
+    }  ;
+    struct rk2_exact
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      struct type
+      {
+        typedef pythonic::types::none_type __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0 tendencies_d, argument_type1 tendencies_d0, argument_type2 tendencies_1, argument_type3 tendencies_1_shift, argument_type4 phaseshift) const
+      ;
+    }  ;
+    struct rk2_tendencies_d
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef pythonic::types::none_type __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 tendencies_d, argument_type1 tendencies_0, argument_type2 tendencies_1_shift, argument_type3 phaseshift) const
+      ;
+    }  ;
+    struct exact_lin_compute
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef pythonic::types::none_type __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 f_lin, argument_type1 exact, argument_type2 exact2, argument_type3 dt) const
+      ;
+    }  ;
+    struct compute_phaseshift_terms
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type2;
+        typedef __type2 __type3;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type1>(), std::declval<__type3>())) __type4;
+        typedef typename pythonic::returnable<__type4>::type __type5;
+        typedef __type5 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 phase_alpha, argument_type1 phase_beta, argument_type2 phaseshift_alpha, argument_type3 phaseshift_beta) const
+      ;
+    }  ;
+    struct div_inplace
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef __type1 __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type3;
+        typedef __type3 __type4;
+        typedef __type4 __type5;
+        typedef typename pythonic::assignable<__type1>::type __type6;
+        typedef typename __combined<__type6,__type4>::type __type7;
+        typedef __type7 __type8;
+        typedef typename pythonic::returnable<__type8>::type __type9;
+        typedef __type2 __ptype0;
+        typedef __type5 __ptype1;
+        typedef __type9 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      inline
+      typename type<argument_type0, argument_type1>::result_type operator()(argument_type0 arr, argument_type1 phaseshift) const
+      ;
+    }  ;
+    struct mul
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0 phaseshift, argument_type1 state_spect, argument_type2 output) const
+      ;
+    }  ;
+    struct mean_with_phaseshift
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 tendencies_0, argument_type1 tendencies_1_shift, argument_type2 phaseshift, argument_type3 output) const
+      ;
+    }  ;
+    struct step_like_RK2
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      struct type
+      {
+        typedef pythonic::types::none_type __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0 state_spect, argument_type1 dt, argument_type2 tendencies, argument_type3 diss, argument_type4 diss2) const
+      ;
+    }  ;
+    struct step_Euler
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0 state_spect, argument_type1 dt, argument_type2 tendencies, argument_type3 diss, argument_type4 output) const
+      ;
+    }  ;
+    struct step_Euler_inplace
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef pythonic::types::none_type __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 state_spect, argument_type1 dt, argument_type2 tendencies, argument_type3 diss) const
+      ;
     }  ;
     inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct arguments_blocks
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    typename __transonic__::type::result_type __transonic__::operator()() const
+    {
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
+    }
+    inline
+    typename arguments_blocks::type::result_type arguments_blocks::operator()() const
     {
       typedef pythonic::types::str __type0;
       typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::static_list{})>::type>::type __type1;
       typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type2;
       typedef decltype(std::declval<__type1>()(std::declval<__type2>())) __type3;
       typedef pythonic::types::dict<__type0,__type3> __type4;
       typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type5;
       typedef decltype(std::declval<__type1>()(std::declval<__type5>())) __type6;
       typedef pythonic::types::dict<__type0,__type6> __type7;
-      typedef typename __combined<__type4,__type7>::type __type8;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type9;
-      typedef decltype(std::declval<__type1>()(std::declval<__type9>())) __type10;
-      typedef pythonic::types::dict<__type0,__type10> __type11;
-      typedef typename __combined<__type8,__type11>::type __type12;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type13;
-      typedef decltype(std::declval<__type1>()(std::declval<__type13>())) __type14;
-      typedef pythonic::types::dict<__type0,__type14> __type15;
-      typedef typename __combined<__type12,__type15>::type __type16;
-      typedef typename pythonic::returnable<__type16>::type __type17;
-      typedef __type17 result_type;
-    }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct rk4_step3
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
-    {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef long __type4;
-      typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type4>())) __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type5>(), std::declval<__type7>())) __type8;
-      typedef decltype(pythonic::operator_::add(std::declval<__type1>(), std::declval<__type8>())) __type9;
-      typedef __type9 __type10;
-      typedef pythonic::types::none_type __type11;
-      typedef typename pythonic::returnable<__type11>::type __type12;
-      typedef __type10 __ptype0;
-      typedef __type12 result_type;
-    }  
-    ;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type8;
+      typedef decltype(std::declval<__type1>()(std::declval<__type8>())) __type9;
+      typedef pythonic::types::dict<__type0,__type9> __type10;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>(), std::declval<__type0>())) __type11;
+      typedef decltype(std::declval<__type1>()(std::declval<__type11>())) __type12;
+      typedef pythonic::types::dict<__type0,__type12> __type13;
+      typedef typename __combined<__type4,__type7,__type10,__type13>::type __type14;
+      typedef typename pythonic::assignable<__type14>::type __type15;
+      {
+        static typename arguments_blocks::type::result_type tmp_global = __type15{{{ pythonic::types::str("exact_lin_compute"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("f_lin"), pythonic::types::str("exact"), pythonic::types::str("exact2"), pythonic::types::str("dt"))) }, { pythonic::types::str("rk2_tendencies_d"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("tendencies_d"), pythonic::types::str("tendencies_0"), pythonic::types::str("tendencies_1_shift"), pythonic::types::str("phaseshift"))) }, { pythonic::types::str("rk2_exact"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("tendencies_d"), pythonic::types::str("tendencies_d0"), pythonic::types::str("tendencies_1"), pythonic::types::str("tendencies_1_shift"), pythonic::types::str("phaseshift"))) }, { pythonic::types::str("rk4_step1"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("state_spect"), pythonic::types::str("state_spect_tmp"), pythonic::types::str("state_spect_12_approx2"), pythonic::types::str("tendencies_1"), pythonic::types::str("diss2"), pythonic::types::str("dt"))) }, { pythonic::types::str("rk4_step2"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("state_spect"), pythonic::types::str("state_spect_tmp"), pythonic::types::str("state_spect_1_approx"), pythonic::types::str("tendencies_2"), pythonic::types::str("diss"), pythonic::types::str("diss2"), pythonic::types::str("dt"))) }, { pythonic::types::str("rk4_step3"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("state_spect"), pythonic::types::str("state_spect_tmp"), pythonic::types::str("tendencies_3"), pythonic::types::str("dt"))) }}};
+        return tmp_global;
+      }
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& state_spect, argument_type1&& state_spect_tmp, argument_type2&& tendencies_3, argument_type3&& dt) const
-    ;
-  }  ;
-  struct rk4_step2
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 , typename argument_type6 >
-    struct type
+    typename rk4_step3::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type rk4_step3::operator()(argument_type0 state_spect, argument_type1 state_spect_tmp, argument_type2 tendencies_3, argument_type3 dt) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type6>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef long __type2;
-      typedef decltype(pythonic::operator_::div(std::declval<__type1>(), std::declval<__type2>())) __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type4;
-      typedef __type4 __type5;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type5>())) __type6;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type7;
-      typedef __type7 __type8;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type8>())) __type9;
-      typedef __type9 __type10;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type11;
-      typedef __type11 __type12;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type13;
-      typedef __type13 __type14;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type12>(), std::declval<__type14>())) __type15;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type5>())) __type18;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type18>(), std::declval<__type8>())) __type20;
-      typedef decltype(pythonic::operator_::add(std::declval<__type15>(), std::declval<__type20>())) __type21;
-      typedef __type21 __type22;
-      typedef pythonic::types::none_type __type23;
-      typedef typename pythonic::returnable<__type23>::type __type24;
-      typedef __type10 __ptype1;
-      typedef __type22 __ptype2;
-      typedef __type24 result_type;
-    }  
-    ;
+      pythonic::numpy::functor::copyto{}(state_spect, pythonic::operator_::add(state_spect_tmp, pythonic::operator_::mul(pythonic::operator_::div(dt, 6L), tendencies_3)));
+      return pythonic::builtins::None;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 , typename argument_type6 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5, argument_type6>::result_type operator()(argument_type0&& state_spect, argument_type1&& state_spect_tmp, argument_type2&& state_spect_1_approx, argument_type3&& tendencies_2, argument_type4&& diss, argument_type5&& diss2, argument_type6&& dt) const
-    ;
-  }  ;
-  struct rk4_step1
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    struct type
+    typename rk4_step2::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5, argument_type6>::result_type rk4_step2::operator()(argument_type0 state_spect, argument_type1 state_spect_tmp, argument_type2 state_spect_1_approx, argument_type3 tendencies_2, argument_type4 diss, argument_type5 diss2, argument_type6 dt) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef long __type2;
-      typedef decltype(pythonic::operator_::div(std::declval<__type1>(), std::declval<__type2>())) __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type4;
-      typedef __type4 __type5;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type5>())) __type6;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type7;
-      typedef __type7 __type8;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type8>())) __type9;
-      typedef __type9 __type10;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type11;
-      typedef __type11 __type12;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type12>(), std::declval<__type5>())) __type14;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type8>())) __type18;
-      typedef decltype(pythonic::operator_::add(std::declval<__type14>(), std::declval<__type18>())) __type19;
-      typedef __type19 __type20;
-      typedef pythonic::types::none_type __type21;
-      typedef typename pythonic::returnable<__type21>::type __type22;
-      typedef __type10 __ptype3;
-      typedef __type20 __ptype4;
-      typedef __type22 result_type;
-    }  
-    ;
+      pythonic::types::as_const(state_spect_tmp)[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] += pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::div(dt, 3L), diss2), tendencies_2);
+      pythonic::numpy::functor::copyto{}(state_spect_1_approx, pythonic::operator_::add(pythonic::operator_::mul(state_spect, diss), pythonic::operator_::mul(pythonic::operator_::mul(dt, diss2), tendencies_2)));
+      return pythonic::builtins::None;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0&& state_spect, argument_type1&& state_spect_tmp, argument_type2&& state_spect_12_approx2, argument_type3&& tendencies_1, argument_type4&& diss2, argument_type5&& dt) const
-    ;
-  }  ;
-  struct rk2_exact
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-    struct type
+    typename rk4_step1::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type rk4_step1::operator()(argument_type0 state_spect, argument_type1 state_spect_tmp, argument_type2 state_spect_12_approx2, argument_type3 tendencies_1, argument_type4 diss2, argument_type5 dt) const
     {
-      typedef double __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
-      typedef __type3 __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type7;
-      typedef __type7 __type8;
-      typedef decltype(pythonic::operator_::div(std::declval<__type6>(), std::declval<__type8>())) __type9;
-      typedef decltype(pythonic::operator_::add(std::declval<__type4>(), std::declval<__type9>())) __type10;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type10>())) __type11;
-      typedef decltype(pythonic::operator_::add(std::declval<__type2>(), std::declval<__type11>())) __type12;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type12>())) __type13;
-      typedef __type13 __type14;
-      typedef pythonic::types::none_type __type15;
-      typedef typename pythonic::returnable<__type15>::type __type16;
-      typedef __type14 __ptype5;
-      typedef __type16 result_type;
-    }  
-    ;
+      pythonic::types::as_const(state_spect_tmp)[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] += pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::div(dt, 3L), diss2), tendencies_1);
+      pythonic::numpy::functor::copyto{}(state_spect_12_approx2, pythonic::operator_::add(pythonic::operator_::mul(state_spect, diss2), pythonic::operator_::mul(pythonic::operator_::div(dt, 2L), tendencies_1)));
+      return pythonic::builtins::None;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0&& tendencies_d, argument_type1&& tendencies_d0, argument_type2&& tendencies_1, argument_type3&& tendencies_1_shift, argument_type4&& phaseshift) const
-    ;
-  }  ;
-  struct rk2_tendencies_d
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    typename rk2_exact::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type rk2_exact::operator()(argument_type0 tendencies_d, argument_type1 tendencies_d0, argument_type2 tendencies_1, argument_type3 tendencies_1_shift, argument_type4 phaseshift) const
     {
-      typedef double __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
-      typedef __type3 __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type6>())) __type7;
-      typedef decltype(pythonic::operator_::add(std::declval<__type2>(), std::declval<__type7>())) __type8;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type8>())) __type9;
-      typedef __type9 __type10;
-      typedef pythonic::types::none_type __type11;
-      typedef typename pythonic::returnable<__type11>::type __type12;
-      typedef __type10 __ptype6;
-      typedef __type12 result_type;
-    }  
-    ;
+      pythonic::numpy::functor::copyto{}(tendencies_d, pythonic::operator_::mul(0.5, pythonic::operator_::add(tendencies_d0, pythonic::operator_::mul(0.5, pythonic::operator_::add(tendencies_1, pythonic::operator_::div(tendencies_1_shift, phaseshift))))));
+      return pythonic::builtins::None;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& tendencies_d, argument_type1&& tendencies_0, argument_type2&& tendencies_1_shift, argument_type3&& phaseshift) const
-    ;
-  }  ;
-  struct exact_lin_compute
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    typename rk2_tendencies_d::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type rk2_tendencies_d::operator()(argument_type0 tendencies_d, argument_type1 tendencies_0, argument_type2 tendencies_1_shift, argument_type3 phaseshift) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::exp{})>::type>::type __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef decltype(pythonic::operator_::neg(std::declval<__type2>())) __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type4;
-      typedef __type4 __type5;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type5>())) __type6;
-      typedef decltype(std::declval<__type0>()(std::declval<__type6>())) __type7;
-      typedef __type7 __type8;
-      typedef long __type11;
-      typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type11>())) __type12;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type12>(), std::declval<__type5>())) __type14;
-      typedef decltype(std::declval<__type0>()(std::declval<__type14>())) __type15;
-      typedef __type15 __type16;
-      typedef pythonic::types::none_type __type17;
-      typedef typename pythonic::returnable<__type17>::type __type18;
-      typedef __type8 __ptype7;
-      typedef __type16 __ptype8;
-      typedef __type18 result_type;
-    }  
-    ;
+      pythonic::numpy::functor::copyto{}(tendencies_d, pythonic::operator_::mul(0.5, pythonic::operator_::add(tendencies_0, pythonic::operator_::div(tendencies_1_shift, phaseshift))));
+      return pythonic::builtins::None;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& f_lin, argument_type1&& exact, argument_type2&& exact2, argument_type3&& dt) const
-    ;
-  }  ;
-  struct compute_phaseshift_terms
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    typename exact_lin_compute::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type exact_lin_compute::operator()(argument_type0 f_lin, argument_type1 exact, argument_type2 exact2, argument_type3 dt) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::exp{})>::type>::type __type0;
-      typedef std::complex<double> __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type3>())) __type4;
-      typedef decltype(std::declval<__type0>()(std::declval<__type4>())) __type5;
-      typedef __type5 __type6;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type7;
-      typedef __type7 __type8;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type8>())) __type9;
-      typedef decltype(std::declval<__type0>()(std::declval<__type9>())) __type10;
-      typedef __type10 __type11;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type12;
-      typedef typename __combined<__type12,__type5>::type __type13;
-      typedef __type13 __type14;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type15;
-      typedef typename __combined<__type15,__type10>::type __type16;
-      typedef __type16 __type17;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type14>(), std::declval<__type17>())) __type18;
-      typedef typename pythonic::returnable<__type18>::type __type19;
-      typedef __type6 __ptype9;
-      typedef __type11 __ptype10;
-      typedef __type19 result_type;
-    }  
-    ;
+      pythonic::numpy::functor::copyto{}(exact, pythonic::numpy::functor::exp{}(pythonic::operator_::mul(pythonic::operator_::neg(dt), f_lin)));
+      pythonic::numpy::functor::copyto{}(exact2, pythonic::numpy::functor::exp{}(pythonic::operator_::mul(pythonic::operator_::div(pythonic::operator_::neg(dt), 2L), f_lin)));
+      return pythonic::builtins::None;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& phase_alpha, argument_type1&& phase_beta, argument_type2&& phaseshift_alpha, argument_type3&& phaseshift_beta) const
-    ;
-  }  ;
-  struct div_inplace
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 >
-    struct type
+    typename compute_phaseshift_terms::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type compute_phaseshift_terms::operator()(argument_type0 phase_alpha, argument_type1 phase_beta, argument_type2 phaseshift_alpha, argument_type3 phaseshift_beta) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef __type1 __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type3;
-      typedef __type3 __type4;
-      typedef __type4 __type5;
-      typedef typename pythonic::assignable<__type1>::type __type6;
-      typedef typename __combined<__type6,__type4>::type __type7;
-      typedef __type7 __type8;
-      typedef typename pythonic::returnable<__type8>::type __type9;
-      typedef __type2 __ptype11;
-      typedef __type5 __ptype12;
-      typedef __type9 result_type;
-    }  
-    ;
+      pythonic::numpy::functor::copyto{}(phaseshift_alpha, pythonic::numpy::functor::exp{}(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), phase_alpha)));
+      pythonic::numpy::functor::copyto{}(phaseshift_beta, pythonic::numpy::functor::exp{}(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), phase_beta)));
+      return pythonic::types::make_tuple(phaseshift_alpha, phaseshift_beta);
+    }
     template <typename argument_type0 , typename argument_type1 >
     inline
-    typename type<argument_type0, argument_type1>::result_type operator()(argument_type0&& arr, argument_type1&& phaseshift) const
-    ;
-  }  ;
-  struct mul
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    struct type
+    typename div_inplace::type<argument_type0, argument_type1>::result_type div_inplace::operator()(argument_type0 arr, argument_type1 phaseshift) const
     {
       typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
       typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type3>())) __type4;
-      typedef __type4 __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type6;
-      typedef typename __combined<__type6,__type4>::type __type7;
-      typedef __type7 __type8;
-      typedef typename pythonic::returnable<__type8>::type __type9;
-      typedef __type5 __ptype13;
-      typedef __type9 result_type;
-    }  
-    ;
+      typedef typename pythonic::assignable<__type1>::type __type2;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type3;
+      typedef __type3 __type4;
+      typedef typename __combined<__type2,__type4>::type __type5;
+      typedef typename pythonic::assignable<__type5>::type __type6;
+      __type6 arr_ = arr;
+      pythonic::operator_::idiv(arr_, phaseshift);
+      return arr_;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0&& phaseshift, argument_type1&& state_spect, argument_type2&& output) const
-    ;
-  }  ;
-  struct mean_with_phaseshift
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    typename mul::type<argument_type0, argument_type1, argument_type2>::result_type mul::operator()(argument_type0 phaseshift, argument_type1 state_spect, argument_type2 output) const
     {
-      typedef double __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type3;
-      typedef __type3 __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type6>())) __type7;
-      typedef decltype(pythonic::operator_::add(std::declval<__type2>(), std::declval<__type7>())) __type8;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type8>())) __type9;
-      typedef __type9 __type10;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type11;
-      typedef typename __combined<__type11,__type9>::type __type12;
-      typedef __type12 __type13;
-      typedef typename pythonic::returnable<__type13>::type __type14;
-      typedef __type10 __ptype14;
-      typedef __type14 result_type;
-    }  
-    ;
+      pythonic::numpy::functor::copyto{}(output, pythonic::operator_::mul(phaseshift, state_spect));
+      return output;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& tendencies_0, argument_type1&& tendencies_1_shift, argument_type2&& phaseshift, argument_type3&& output) const
-    ;
-  }  ;
-  struct step_like_RK2
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-    struct type
+    typename mean_with_phaseshift::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type mean_with_phaseshift::operator()(argument_type0 tendencies_0, argument_type1 tendencies_1_shift, argument_type2 phaseshift, argument_type3 output) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type3>())) __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type7;
-      typedef __type7 __type8;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type8>())) __type9;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type10;
-      typedef __type10 __type11;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type9>(), std::declval<__type11>())) __type12;
-      typedef decltype(pythonic::operator_::add(std::declval<__type4>(), std::declval<__type12>())) __type13;
-      typedef typename __combined<__type0,__type13>::type __type14;
-      typedef __type13 __type15;
-      typedef pythonic::types::none_type __type16;
-      typedef typename pythonic::returnable<__type16>::type __type17;
-      typedef __type15 __ptype15;
-      typedef __type17 result_type;
-    }  
-    ;
+      pythonic::numpy::functor::copyto{}(output, pythonic::operator_::mul(0.5, pythonic::operator_::add(tendencies_0, pythonic::operator_::div(tendencies_1_shift, phaseshift))));
+      return output;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0&& state_spect, argument_type1&& dt, argument_type2&& tendencies, argument_type3&& diss, argument_type4&& diss2) const
-    ;
-  }  ;
-  struct step_Euler
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-    struct type
+    typename step_like_RK2::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type step_like_RK2::operator()(argument_type0 state_spect, argument_type1 dt, argument_type2 tendencies, argument_type3 diss, argument_type4 diss2) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type4;
-      typedef __type4 __type5;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type5>())) __type6;
-      typedef decltype(pythonic::operator_::add(std::declval<__type1>(), std::declval<__type6>())) __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type9>())) __type10;
-      typedef __type10 __type11;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type12;
-      typedef typename __combined<__type12,__type10>::type __type13;
-      typedef __type13 __type14;
-      typedef typename pythonic::returnable<__type14>::type __type15;
-      typedef __type11 __ptype16;
-      typedef __type15 result_type;
-    }  
-    ;
+      pythonic::numpy::functor::copyto{}(state_spect, pythonic::operator_::add(pythonic::operator_::mul(state_spect, diss), pythonic::operator_::mul(pythonic::operator_::mul(dt, diss2), tendencies)));
+      return pythonic::builtins::None;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0&& state_spect, argument_type1&& dt, argument_type2&& tendencies, argument_type3&& diss, argument_type4&& output) const
-    ;
-  }  ;
-  struct step_Euler_inplace
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    typename step_Euler::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type step_Euler::operator()(argument_type0 state_spect, argument_type1 dt, argument_type2 tendencies, argument_type3 diss, argument_type4 output) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename __combined<__type0,__type1>::type __type2;
-      typedef __type2 __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-      typedef __type4 __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type8;
-      typedef __type8 __type9;
-      typedef typename step_Euler::type<__type3, __type5, __type7, __type9, __type1>::__ptype16 __type10;
-      typedef __type10 __type11;
-      typedef pythonic::types::none_type __type13;
-      typedef typename pythonic::returnable<__type13>::type __type14;
-      typedef __type11 __ptype17;
-      typedef __type11 __ptype18;
-      typedef __type14 result_type;
-    }  
-    ;
+      pythonic::numpy::functor::copyto{}(output, pythonic::operator_::mul(pythonic::operator_::add(state_spect, pythonic::operator_::mul(dt, tendencies)), diss));
+      return output;
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& state_spect, argument_type1&& dt, argument_type2&& tendencies, argument_type3&& diss) const
-    ;
-  }  ;
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
-    {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.0"));
-      return tmp_global;
-    }
-  }
-  inline
-  typename arguments_blocks::type::result_type arguments_blocks::operator()() const
-  {
+    typename step_Euler_inplace::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type step_Euler_inplace::operator()(argument_type0 state_spect, argument_type1 dt, argument_type2 tendencies, argument_type3 diss) const
     {
-      static typename arguments_blocks::type::result_type tmp_global = typename pythonic::assignable<typename __combined<typename __combined<typename __combined<pythonic::types::dict<pythonic::types::str,decltype(std::declval<typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::static_list{})>::type>::type>()(std::declval<decltype(pythonic::types::make_tuple(std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>()))>()))>,pythonic::types::dict<pythonic::types::str,decltype(std::declval<typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::static_list{})>::type>::type>()(std::declval<decltype(pythonic::types::make_tuple(std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>()))>()))>>::type,pythonic::types::dict<pythonic::types::str,decltype(std::declval<typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::static_list{})>::type>::type>()(std::declval<decltype(pythonic::types::make_tuple(std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>()))>()))>>::type,pythonic::types::dict<pythonic::types::str,decltype(std::declval<typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::static_list{})>::type>::type>()(std::declval<decltype(pythonic::types::make_tuple(std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>(), std::declval<pythonic::types::str>()))>()))>>::type>::type{{{ pythonic::types::str("exact_lin_compute"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("f_lin"), pythonic::types::str("exact"), pythonic::types::str("exact2"), pythonic::types::str("dt"))) }, { pythonic::types::str("rk2_tendencies_d"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("tendencies_d"), pythonic::types::str("tendencies_0"), pythonic::types::str("tendencies_1_shift"), pythonic::types::str("phaseshift"))) }, { pythonic::types::str("rk2_exact"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("tendencies_d"), pythonic::types::str("tendencies_d0"), pythonic::types::str("tendencies_1"), pythonic::types::str("tendencies_1_shift"), pythonic::types::str("phaseshift"))) }, { pythonic::types::str("rk4_step1"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("state_spect"), pythonic::types::str("state_spect_tmp"), pythonic::types::str("state_spect_12_approx2"), pythonic::types::str("tendencies_1"), pythonic::types::str("diss2"), pythonic::types::str("dt"))) }, { pythonic::types::str("rk4_step2"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("state_spect"), pythonic::types::str("state_spect_tmp"), pythonic::types::str("state_spect_1_approx"), pythonic::types::str("tendencies_2"), pythonic::types::str("diss"), pythonic::types::str("diss2"), pythonic::types::str("dt"))) }, { pythonic::types::str("rk4_step3"), pythonic::builtins::pythran::functor::static_list{}(pythonic::types::make_tuple(pythonic::types::str("state_spect"), pythonic::types::str("state_spect_tmp"), pythonic::types::str("tendencies_3"), pythonic::types::str("dt"))) }}};
-      return tmp_global;
+      pythonic::types::call(step_Euler(), state_spect, dt, tendencies, diss, state_spect);
+      return pythonic::builtins::None;
     }
   }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename rk4_step3::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type rk4_step3::operator()(argument_type0&& state_spect, argument_type1&& state_spect_tmp, argument_type2&& tendencies_3, argument_type3&& dt) const
-  {
-    state_spect[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::add(state_spect_tmp, pythonic::operator_::mul(pythonic::operator_::div(dt, 6L), tendencies_3));
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 , typename argument_type6 >
-  inline
-  typename rk4_step2::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5, argument_type6>::result_type rk4_step2::operator()(argument_type0&& state_spect, argument_type1&& state_spect_tmp, argument_type2&& state_spect_1_approx, argument_type3&& tendencies_2, argument_type4&& diss, argument_type5&& diss2, argument_type6&& dt) const
-  {
-    state_spect_tmp[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] += pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::div(dt, 3L), diss2), tendencies_2);
-    state_spect_1_approx[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::add(pythonic::operator_::mul(state_spect, diss), pythonic::operator_::mul(pythonic::operator_::mul(dt, diss2), tendencies_2));
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-  inline
-  typename rk4_step1::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type rk4_step1::operator()(argument_type0&& state_spect, argument_type1&& state_spect_tmp, argument_type2&& state_spect_12_approx2, argument_type3&& tendencies_1, argument_type4&& diss2, argument_type5&& dt) const
-  {
-    state_spect_tmp[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] += pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::div(dt, 3L), diss2), tendencies_1);
-    state_spect_12_approx2[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::add(pythonic::operator_::mul(state_spect, diss2), pythonic::operator_::mul(pythonic::operator_::div(dt, 2L), tendencies_1));
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-  inline
-  typename rk2_exact::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type rk2_exact::operator()(argument_type0&& tendencies_d, argument_type1&& tendencies_d0, argument_type2&& tendencies_1, argument_type3&& tendencies_1_shift, argument_type4&& phaseshift) const
-  {
-    tendencies_d[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::mul(0.5, pythonic::operator_::add(tendencies_d0, pythonic::operator_::mul(0.5, pythonic::operator_::add(tendencies_1, pythonic::operator_::div(tendencies_1_shift, phaseshift)))));
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename rk2_tendencies_d::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type rk2_tendencies_d::operator()(argument_type0&& tendencies_d, argument_type1&& tendencies_0, argument_type2&& tendencies_1_shift, argument_type3&& phaseshift) const
-  {
-    tendencies_d[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::mul(0.5, pythonic::operator_::add(tendencies_0, pythonic::operator_::div(tendencies_1_shift, phaseshift)));
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename exact_lin_compute::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type exact_lin_compute::operator()(argument_type0&& f_lin, argument_type1&& exact, argument_type2&& exact2, argument_type3&& dt) const
-  {
-    exact[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::numpy::functor::exp{}(pythonic::operator_::mul(pythonic::operator_::neg(dt), f_lin));
-    exact2[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::numpy::functor::exp{}(pythonic::operator_::mul(pythonic::operator_::div(pythonic::operator_::neg(dt), 2L), f_lin));
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename compute_phaseshift_terms::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type compute_phaseshift_terms::operator()(argument_type0&& phase_alpha, argument_type1&& phase_beta, argument_type2&& phaseshift_alpha, argument_type3&& phaseshift_beta) const
-  {
-    phaseshift_alpha[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::numpy::functor::exp{}(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), phase_alpha));
-    phaseshift_beta[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::numpy::functor::exp{}(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), phase_beta));
-    return pythonic::types::make_tuple(phaseshift_alpha, phaseshift_beta);
-  }
-  template <typename argument_type0 , typename argument_type1 >
-  inline
-  typename div_inplace::type<argument_type0, argument_type1>::result_type div_inplace::operator()(argument_type0&& arr, argument_type1&& phaseshift) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-    typedef __type0 __type1;
-    typedef typename pythonic::assignable<__type1>::type __type2;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type3;
-    typedef __type3 __type4;
-    typedef typename __combined<__type2,__type4>::type __type5;
-    typedef typename pythonic::assignable<__type5>::type __type6;
-    __type6 arr_ = arr;
-    pythonic::operator_::idiv(arr_, phaseshift);
-    return arr_;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-  inline
-  typename mul::type<argument_type0, argument_type1, argument_type2>::result_type mul::operator()(argument_type0&& phaseshift, argument_type1&& state_spect, argument_type2&& output) const
-  {
-    output[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::mul(phaseshift, state_spect);
-    return output;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename mean_with_phaseshift::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type mean_with_phaseshift::operator()(argument_type0&& tendencies_0, argument_type1&& tendencies_1_shift, argument_type2&& phaseshift, argument_type3&& output) const
-  {
-    output[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::mul(0.5, pythonic::operator_::add(tendencies_0, pythonic::operator_::div(tendencies_1_shift, phaseshift)));
-    return output;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-  inline
-  typename step_like_RK2::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type step_like_RK2::operator()(argument_type0&& state_spect, argument_type1&& dt, argument_type2&& tendencies, argument_type3&& diss, argument_type4&& diss2) const
-  {
-    state_spect[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::add(pythonic::operator_::mul(state_spect, diss), pythonic::operator_::mul(pythonic::operator_::mul(dt, diss2), tendencies));
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-  inline
-  typename step_Euler::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type step_Euler::operator()(argument_type0&& state_spect, argument_type1&& dt, argument_type2&& tendencies, argument_type3&& diss, argument_type4&& output) const
-  {
-    output[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::mul(pythonic::operator_::add(state_spect, pythonic::operator_::mul(dt, tendencies)), diss);
-    return output;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename step_Euler_inplace::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type step_Euler_inplace::operator()(argument_type0&& state_spect, argument_type1&& dt, argument_type2&& tendencies, argument_type3&& diss) const
-  {
-    step_Euler()(state_spect, dt, tendencies, diss, state_spect);
-    return pythonic::builtins::None;
-  }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_pseudo_spect::__transonic__()());
 static PyObject* arguments_blocks = to_python(__pythran_pseudo_spect::arguments_blocks()());
 inline
 typename __pythran_pseudo_spect::rk4_step3::type<pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long>>, double>::result_type rk4_step30(pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long>>&& state_spect, pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long>>&& state_spect_tmp, pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long>>&& tendencies_3, double&& dt) 
@@ -4159,17 +3999,17 @@
                                                      Methods,
                                                      ""
                 );
                 #endif
                 if(! theModule)
                     PYTHRAN_RETURN;
                 PyObject * theDoc = Py_BuildValue("(sss)",
-                                                  "0.11.0",
-                                                  "2022-09-02 03:40:11.100410",
-                                                  "cb7436d7c3619066765509f9b752bf5961bf64a31a62b05298e269d8e87877e8");
+                                                  "0.13.1",
+                                                  "2023-05-24 11:29:39.673636",
+                                                  "64db197e1ee7a6ad83afb96feba7544d1aeb672fbd358e4d210236df5931c870");
                 if(! theDoc)
                     PYTHRAN_RETURN;
                 PyModule_AddObject(theModule,
                                    "__pythran__",
                                    theDoc);
 
                 PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/base/time_stepping/base.py` & `fluidsim-0.7.3/fluidsim/base/time_stepping/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,14 @@
         self.one_time_step_computation()
         self.t += self.deltat
         self.it += 1
 
 
 class TimeSteppingBase(TimeSteppingBase0):
     def _init_compute_time_step(self):
-
         params_ts = self.params.time_stepping
 
         if params_ts.USE_CFL:
             if params_ts.cfl_coef is not None:
                 self.CFL = params_ts.cfl_coef
             elif any(
                 params_ts.type_time_scheme.startswith(scheme)
@@ -294,15 +293,14 @@
             self.compute_time_increment_CLF = self._compute_time_increment_CLF_U
         elif params_ts.USE_CFL:
             raise ValueError("params_ts.USE_CFL but no velocity.")
 
         self.deltat_max = params_ts.deltat_max
 
     def _init_time_scheme(self):
-
         params_ts = self.params.time_stepping
 
         if params_ts.type_time_scheme == "RK2":
             self._time_step_RK = self._time_step_RK2
         elif params_ts.type_time_scheme == "RK4":
             self._time_step_RK = self._time_step_RK4
         else:
@@ -337,15 +335,14 @@
             )
         else:
             tmp = 0.0
 
         self._compute_time_increment_CLF_from_tmp(tmp)
 
     def _compute_time_increment_CLF_from_tmp(self, tmp):
-
         if mpi.nb_proc > 1:
             tmp = mpi.comm.allreduce(tmp, op=mpi.MPI.MAX)
 
         if tmp > 0:
             deltat_CFL = self.CFL / tmp
         else:
             deltat_CFL = self.deltat_max
```

### Comparing `fluidsim-0.7.2/fluidsim/base/time_stepping/finite_diff.py` & `fluidsim-0.7.3/fluidsim/base/time_stepping/finite_diff.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/time_stepping/pseudo_spect.py` & `fluidsim-0.7.3/fluidsim/base/time_stepping/pseudo_spect.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,14 @@
             self.freq_lin = freq_dissip + freq_complex
             freq_max = freq_complex.imag.max()
             self.deltat_max = 0.78 * np.pi / freq_max
         else:
             self.freq_lin = freq_dissip
 
     def _init_time_scheme(self):
-
         type_time_scheme = self.params.time_stepping.type_time_scheme
 
         if type_time_scheme.startswith("RK"):
             self._state_spect_tmp = np.empty_like(self.sim.state.state_spect)
 
         if type_time_scheme.endswith("_random"):
             self._init_phaseshift_random()
@@ -296,15 +295,14 @@
             )
         else:
             raise NotImplementedError
         self._phaseshift = np.exp(1j * phase)
         return self._phaseshift
 
     def _init_phaseshift_random(self):
-
         params_phaseshift = self.params.time_stepping.phaseshift_random
         if params_phaseshift.nb_steps_compute_new_pair is None:
             if params_phaseshift.nb_pairs == 1:
                 params_phaseshift.nb_steps_compute_new_pair = 2
             else:
                 params_phaseshift.nb_steps_compute_new_pair = (
                     4 * params_phaseshift.nb_pairs
```

### Comparing `fluidsim-0.7.2/fluidsim/base/time_stepping/simple.py` & `fluidsim-0.7.3/fluidsim/base/time_stepping/simple.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/turb_model/__init__.py` & `fluidsim-0.7.3/fluidsim/base/turb_model/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/base/turb_model/base.py` & `fluidsim-0.7.3/fluidsim/base/turb_model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from fluidsim_core.params import iter_complete_params
 from fluidsim.extend_simul import SimulExtender
 from fluidsim.base.setofvariables import SetOfVariables
 
 
 def modif_infosolver_turb_model(info_solver):
-
     try:
         classes_TurbModel = getattr(info_solver.classes, "TurbModel")
     except AttributeError:
         classes_TurbModel = info_solver.classes._set_child(
             "TurbModel",
             attribs={
                 "class_name": "TurbModel",
@@ -101,15 +100,14 @@
         not yet been created (and cannot yet be modified)! This is why one
         needs to create a function that will be called later to modify
         ``info_solver``.
 
         """
 
         def modif_info_solver(info_solver):
-
             from fluidsim.base.turb_model.base import modif_infosolver_turb_model
 
             modif_infosolver_turb_model(info_solver)
 
             info_solver.classes.TurbModel.classes._set_child(
                 cls.tag,
                 attribs={
```

### Comparing `fluidsim-0.7.2/fluidsim/base/turb_model/smagorinsky.py` & `fluidsim-0.7.3/fluidsim/base/turb_model/smagorinsky.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
         C = sim.params.turb_model.smagorinsky.C
         delta = sim.params.oper.Lx / sim.params.oper.nx
 
         self.C_nu_T = C * delta**2 * sqrt(2)
 
     def get_forcing(self, **kwargs):
-
         ux_fft = kwargs["vx_fft"]
         uy_fft = kwargs["vy_fft"]
         uz_fft = kwargs["vz_fft"]
 
         Sxx, Syy, Szz, Syx, Szx, Szy = self.stress_tensor.compute_stress_tensor(
             ux_fft, uy_fft, uz_fft
         )
```

### Comparing `fluidsim-0.7.2/fluidsim/base/turb_model/stress_tensor.py` & `fluidsim-0.7.3/fluidsim/base/turb_model/stress_tensor.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         dx_arr_fft, dy_arr_fft, dz_arr_fft = self.oper.grad_fft_from_arr_fft(
             arr_fft
         )
         ifft = self.oper.ifft
         return ifft(dx_arr_fft), ifft(dy_arr_fft), ifft(dz_arr_fft)
 
     def compute_stress_tensor(self, ux_fft, uy_fft, uz_fft):
-
         dx_ux, dy_ux, dz_ux = self.grad_from_arr_fft(ux_fft)
         dx_uy, dy_uy, dz_uy = self.grad_from_arr_fft(uy_fft)
         dx_uz, dy_uz, dz_uz = self.grad_from_arr_fft(uz_fft)
 
         Sxx = dx_ux
         Syy = dy_uy
         Szz = dz_uz
```

### Comparing `fluidsim-0.7.2/fluidsim/base/turb_model/test_turb_model.py` & `fluidsim-0.7.3/fluidsim/base/turb_model/test_turb_model.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/extend_simul/spatial_means_regions_milestone.py` & `fluidsim-0.7.3/fluidsim/extend_simul/spatial_means_regions_milestone.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
     """
 
     _tag = "spatial_means_regions"
     _module_name = "fluidsim.extend_simul.spatial_means_regions_milestone"
 
     def __init__(self, output):
-
         params = output.sim.params
 
         params_cls = params.output.spatial_means_regions
         self.xmin_given = params_cls.xmin
         self.xmax_given = params_cls.xmax
 
         if isinstance(self.xmin_given, numbers.Number):
@@ -116,15 +115,14 @@
 
         self.info_regions = []
 
         _, _, ix_seq_start = oper.seq_indices_first_X
         nx_loc = oper.shapeX_loc[2]
 
         for xmin, xmax in zip(self.xmin_given, self.xmax_given):
-
             xmin, xmax = Lx * xmin, Lx * xmax
 
             ixmin = np.argmin(abs(x_seq - xmin))
             xmin = x_seq[ixmin]
 
             ixmin_loc = ixmin - ix_seq_start
             if ixmin_loc < 0 or ixmin_loc > nx_loc - 1:
```

### Comparing `fluidsim-0.7.2/fluidsim/magic.py` & `fluidsim-0.7.3/fluidsim/magic.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/operators/__pythran__/operators2d.cpp` & `fluidsim-0.7.3/fluidsim/operators/__pythran__/operators2d.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #include <pythonic/core.hpp>
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
-#include <pythonic/include/types/uint8.hpp>
-#include <pythonic/include/types/complex128.hpp>
 #include <pythonic/include/types/float64.hpp>
-#include <pythonic/include/types/numpy_texpr.hpp>
+#include <pythonic/include/types/uint8.hpp>
 #include <pythonic/include/types/bool.hpp>
-#include <pythonic/include/types/int.hpp>
+#include <pythonic/include/types/numpy_texpr.hpp>
 #include <pythonic/include/types/ndarray.hpp>
+#include <pythonic/include/types/complex128.hpp>
+#include <pythonic/include/types/int.hpp>
+#include <pythonic/types/bool.hpp>
 #include <pythonic/types/ndarray.hpp>
-#include <pythonic/types/uint8.hpp>
-#include <pythonic/types/numpy_texpr.hpp>
 #include <pythonic/types/int.hpp>
+#include <pythonic/types/numpy_texpr.hpp>
 #include <pythonic/types/complex128.hpp>
 #include <pythonic/types/float64.hpp>
-#include <pythonic/types/bool.hpp>
+#include <pythonic/types/uint8.hpp>
 #include <pythonic/include/builtins/None.hpp>
 #include <pythonic/include/builtins/getattr.hpp>
 #include <pythonic/include/builtins/map.hpp>
 #include <pythonic/include/builtins/range.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
 #include <pythonic/include/operator_/add.hpp>
 #include <pythonic/include/operator_/div.hpp>
@@ -43,389 +43,398 @@
 #include <pythonic/operator_/eq.hpp>
 #include <pythonic/operator_/lt.hpp>
 #include <pythonic/operator_/mul.hpp>
 #include <pythonic/operator_/sub.hpp>
 #include <pythonic/random/uniform.hpp>
 #include <pythonic/types/slice.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_operators2d
+namespace 
 {
-  struct __for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0
+  namespace __pythran_operators2d
   {
-    typedef void callable;
-    ;
-    template <typename argument_type0 >
-    struct type
+    struct __for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::random::functor::uniform{})>::type>::type __type0;
+        typedef double __type1;
+        typedef decltype(std::declval<__type0>()(std::declval<__type1>(), std::declval<__type1>())) __type2;
+        typedef typename pythonic::returnable<__type2>::type __type3;
+        typedef __type3 result_type;
+      }  
+      ;
+      template <typename argument_type0 >
+      inline
+      typename type<argument_type0>::result_type operator()(argument_type0 _) const
+      ;
+    }  ;
+    struct __transonic__
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct __code_new_method__OperatorsPseudoSpectral2D__get_phases_random
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct __code_new_method__OperatorsPseudoSpectral2D__dealiasing_setofvar
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct __for_method__OperatorsPseudoSpectral2D__dealiasing_setofvar
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      struct type
+      {
+        typedef double __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
+        typedef container<typename std::remove_reference<__type0>::type> __type4;
+        typedef __type3 __type5;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
+        typedef decltype(pythonic::types::as_const(std::declval<__type6>())) __type7;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type7>::type>::type __type8;
+        typedef typename pythonic::lazy<__type8>::type __type9;
+        typedef __type9 __type10;
+        typedef decltype(std::declval<__type2>()(std::declval<__type10>())) __type11;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type11>::type::iterator>::value_type>::type __type12;
+        typedef __type12 __type13;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type7>::type>::type __type14;
+        typedef typename pythonic::lazy<__type14>::type __type15;
+        typedef __type15 __type16;
+        typedef decltype(std::declval<__type2>()(std::declval<__type16>())) __type17;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type17>::type::iterator>::value_type>::type __type18;
+        typedef __type18 __type19;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type7>::type>::type __type20;
+        typedef typename pythonic::lazy<__type20>::type __type21;
+        typedef __type21 __type22;
+        typedef decltype(std::declval<__type2>()(std::declval<__type22>())) __type23;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type23>::type::iterator>::value_type>::type __type24;
+        typedef __type24 __type25;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type13>(), std::declval<__type19>(), std::declval<__type25>())) __type26;
+        typedef indexable<__type26> __type27;
+        typedef typename __combined<__type3,__type4,__type27>::type __type28;
+        typedef __type26 __type29;
+        typedef pythonic::types::none_type __type30;
+        typedef typename pythonic::returnable<__type30>::type __type31;
+        typedef __type1 __ptype0;
+        typedef __type29 __ptype1;
+        typedef __type31 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0 self__has_to_dealiase, argument_type1 self_where_dealiased, argument_type2 sov) const
+      ;
+    }  ;
+    struct compute_increments_dim1
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef decltype(pythonic::types::as_const(std::declval<__type1>())) __type2;
+        typedef pythonic::types::contiguous_slice __type3;
+        typedef decltype(std::declval<__type2>()(std::declval<__type3>(), std::declval<__type3>())) __type4;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type4>(), std::declval<__type4>())) __type8;
+        typedef typename pythonic::returnable<__type8>::type __type9;
+        typedef __type9 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      inline
+      typename type<argument_type0, argument_type1>::result_type operator()(argument_type0 var, argument_type1 irx) const
+      ;
+    }  ;
+    struct invlaplacian_fft
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type2;
+        typedef __type2 __type3;
+        typedef decltype(pythonic::operator_::div(std::declval<__type1>(), std::declval<__type3>())) __type4;
+        typedef typename pythonic::assignable<__type4>::type __type5;
+        typedef long __type6;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type6>(), std::declval<__type6>())) __type7;
+        typedef indexable<__type7> __type8;
+        typedef double __type9;
+        typedef container<typename std::remove_reference<__type9>::type> __type10;
+        typedef typename __combined<__type5,__type8,__type10>::type __type11;
+        typedef __type11 __type12;
+        typedef typename pythonic::returnable<__type12>::type __type13;
+        typedef __type13 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0 a_fft, argument_type1 Kn_not0, argument_type2 rank) const
+      ;
+    }  ;
+    struct laplacian_fft
     {
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::random::functor::uniform{})>::type>::type __type0;
-      typedef double __type1;
-      typedef decltype(std::declval<__type0>()(std::declval<__type1>(), std::declval<__type1>())) __type2;
-      typedef typename pythonic::returnable<__type2>::type __type3;
-      typedef __type3 result_type;
-    }  
-    ;
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type2;
+        typedef __type2 __type3;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type3>())) __type4;
+        typedef typename pythonic::returnable<__type4>::type __type5;
+        typedef __type5 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      inline
+      typename type<argument_type0, argument_type1>::result_type operator()(argument_type0 a_fft, argument_type1 Kn) const
+      ;
+    }  ;
+    struct __for_method__OperatorsPseudoSpectral2D__get_phases_random
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::tuple{})>::type>::type __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::map{})>::type>::type __type1;
+        typedef __for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0 __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type3;
+        typedef long __type4;
+        typedef decltype(std::declval<__type3>()(std::declval<__type4>())) __type5;
+        typedef decltype(std::declval<__type1>()(std::declval<__type2>(), std::declval<__type5>())) __type6;
+        typedef decltype(std::declval<__type0>()(std::declval<__type6>())) __type7;
+        typedef typename pythonic::assignable<__type7>::type __type8;
+        typedef __type8 __type9;
+        typedef decltype(pythonic::types::as_const(std::declval<__type9>())) __type10;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type10>::type>::type __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef __type12 __type13;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type14;
+        typedef __type14 __type15;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type15>())) __type16;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type17;
+        typedef __type17 __type18;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type16>(), std::declval<__type18>())) __type19;
+        typedef std::integral_constant<long,0> __type20;
+        typedef indexable_container<__type20, typename std::remove_reference<__type11>::type> __type21;
+        typedef typename __combined<__type8,__type21>::type __type22;
+        typedef __type22 __type23;
+        typedef decltype(pythonic::types::as_const(std::declval<__type23>())) __type24;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type24>::type>::type __type25;
+        typedef typename pythonic::assignable<__type25>::type __type26;
+        typedef __type26 __type27;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type28;
+        typedef __type28 __type29;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type27>(), std::declval<__type29>())) __type30;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type31;
+        typedef __type31 __type32;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type30>(), std::declval<__type32>())) __type33;
+        typedef decltype(pythonic::operator_::add(std::declval<__type19>(), std::declval<__type33>())) __type34;
+        typedef double __type36;
+        typedef decltype(pythonic::operator_::add(std::declval<__type13>(), std::declval<__type36>())) __type37;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type13>(), std::declval<__type36>())) __type39;
+        typedef typename __combined<__type37,__type39>::type __type40;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type40>(), std::declval<__type15>())) __type42;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type42>(), std::declval<__type18>())) __type44;
+        typedef decltype(pythonic::operator_::add(std::declval<__type27>(), std::declval<__type36>())) __type46;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type27>(), std::declval<__type36>())) __type48;
+        typedef typename __combined<__type46,__type48>::type __type49;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type49>(), std::declval<__type29>())) __type51;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type51>(), std::declval<__type32>())) __type53;
+        typedef decltype(pythonic::operator_::add(std::declval<__type44>(), std::declval<__type53>())) __type54;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type34>(), std::declval<__type54>())) __type55;
+        typedef typename pythonic::returnable<__type55>::type __type56;
+        typedef __type56 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 self_KX, argument_type1 self_KY, argument_type2 self_deltax, argument_type3 self_deltay) const
+      ;
+    }  ;
     template <typename argument_type0 >
     inline
-    typename type<argument_type0>::result_type operator()(argument_type0&& _) const
-    ;
-  }  ;
-  struct __transonic__
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    typename __for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0::type<argument_type0>::result_type __for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0::operator()(argument_type0 _) const
     {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
-    }  ;
+      return pythonic::random::functor::uniform{}(-0.5, 0.5);
+    }
     inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral2D__get_phases_random
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    typename __transonic__::type::result_type __transonic__::operator()() const
     {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
-    }  ;
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
+    }
     inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral2D__dealiasing_setofvar
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    typename __code_new_method__OperatorsPseudoSpectral2D__get_phases_random::type::result_type __code_new_method__OperatorsPseudoSpectral2D__get_phases_random::operator()() const
     {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
-    }  ;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral2D__get_phases_random::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, ):\n    return backend_func(self.KX, self.KY, self.deltax, self.deltay, )\n\n");
+        return tmp_global;
+      }
+    }
     inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral2D__dealiasing_setofvar
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    struct type
+    typename __code_new_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::type::result_type __code_new_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::operator()() const
     {
-      typedef double __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
-      typedef container<typename std::remove_reference<__type0>::type> __type4;
-      typedef __type3 __type5;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type6>::type>::type __type7;
-      typedef typename pythonic::lazy<__type7>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(std::declval<__type2>()(std::declval<__type9>())) __type10;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type10>::type::iterator>::value_type>::type __type11;
-      typedef __type11 __type12;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type6>::type>::type __type13;
-      typedef typename pythonic::lazy<__type13>::type __type14;
-      typedef __type14 __type15;
-      typedef decltype(std::declval<__type2>()(std::declval<__type15>())) __type16;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type16>::type::iterator>::value_type>::type __type17;
-      typedef __type17 __type18;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type6>::type>::type __type19;
-      typedef typename pythonic::lazy<__type19>::type __type20;
-      typedef __type20 __type21;
-      typedef decltype(std::declval<__type2>()(std::declval<__type21>())) __type22;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type22>::type::iterator>::value_type>::type __type23;
-      typedef __type23 __type24;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type12>(), std::declval<__type18>(), std::declval<__type24>())) __type25;
-      typedef indexable<__type25> __type26;
-      typedef typename __combined<__type3,__type4,__type26>::type __type27;
-      typedef __type25 __type28;
-      typedef pythonic::types::none_type __type29;
-      typedef typename pythonic::returnable<__type29>::type __type30;
-      typedef __type1 __ptype0;
-      typedef __type28 __ptype1;
-      typedef __type30 result_type;
-    }  
-    ;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, sov):\n    return backend_func(self._has_to_dealiase, self.where_dealiased, sov)\n\n");
+        return tmp_global;
+      }
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0&& self__has_to_dealiase, argument_type1&& self_where_dealiased, argument_type2&& sov) const
-    ;
-  }  ;
-  struct compute_increments_dim1
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 >
-    struct type
+    typename __for_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::type<argument_type0, argument_type1, argument_type2>::result_type __for_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::operator()(argument_type0 self__has_to_dealiase, argument_type1 self_where_dealiased, argument_type2 sov) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef pythonic::types::contiguous_slice __type2;
-      typedef decltype(std::declval<__type1>()(std::declval<__type2>(), std::declval<__type2>())) __type3;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type3>(), std::declval<__type3>())) __type6;
-      typedef typename pythonic::returnable<__type6>::type __type7;
-      typedef __type7 result_type;
-    }  
-    ;
+      if (self__has_to_dealiase)
+      {
+        typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov))))>::type nk = std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)));
+        typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov))))>::type n0 = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)));
+        typename pythonic::lazy<decltype(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov))))>::type n1 = std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)));
+        {
+          long  __target139658368690352 = n0;
+          for (long  i0=0L; i0 < __target139658368690352; i0 += 1L)
+          {
+            {
+              long  __target139658368688864 = n1;
+              for (long  i1=0L; i1 < __target139658368688864; i1 += 1L)
+              {
+                if (pythonic::types::as_const(self_where_dealiased)[pythonic::types::make_tuple(i0, i1)])
+                {
+                  {
+                    long  __target139658368385328 = nk;
+                    for (long  ik=0L; ik < __target139658368385328; ik += 1L)
+                    {
+                      sov[pythonic::types::make_tuple(ik, i0, i1)] = 0.0;
+                    }
+                  }
+                }
+              }
+            }
+          }
+        }
+      }
+      return pythonic::builtins::None;
+    }
     template <typename argument_type0 , typename argument_type1 >
     inline
-    typename type<argument_type0, argument_type1>::result_type operator()(argument_type0&& var, argument_type1&& irx) const
-    ;
-  }  ;
-  struct invlaplacian_fft
-  {
-    typedef void callable;
-    typedef void pure;
+    typename compute_increments_dim1::type<argument_type0, argument_type1>::result_type compute_increments_dim1::operator()(argument_type0 var, argument_type1 irx) const
+    {
+      typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, var))))>::type n1 = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, var)));
+      return pythonic::operator_::sub(pythonic::types::as_const(var)(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(irx,n1)), pythonic::types::as_const(var)(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(0L,pythonic::operator_::sub(n1, irx))));
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    struct type
+    inline
+    typename invlaplacian_fft::type<argument_type0, argument_type1, argument_type2>::result_type invlaplacian_fft::operator()(argument_type0 a_fft, argument_type1 Kn_not0, argument_type2 rank) const
     {
       typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
       typedef __type0 __type1;
       typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type2;
       typedef __type2 __type3;
       typedef decltype(pythonic::operator_::div(std::declval<__type1>(), std::declval<__type3>())) __type4;
       typedef typename pythonic::assignable<__type4>::type __type5;
       typedef long __type6;
       typedef decltype(pythonic::types::make_tuple(std::declval<__type6>(), std::declval<__type6>())) __type7;
       typedef indexable<__type7> __type8;
       typedef double __type9;
       typedef container<typename std::remove_reference<__type9>::type> __type10;
       typedef typename __combined<__type5,__type8,__type10>::type __type11;
-      typedef __type11 __type12;
-      typedef typename pythonic::returnable<__type12>::type __type13;
-      typedef __type13 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0&& a_fft, argument_type1&& Kn_not0, argument_type2&& rank) const
-    ;
-  }  ;
-  struct laplacian_fft
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 >
-    struct type
-    {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type3>())) __type4;
-      typedef typename pythonic::returnable<__type4>::type __type5;
-      typedef __type5 result_type;
-    }  
-    ;
+      typedef typename pythonic::assignable<__type11>::type __type12;
+      __type12 invlap_afft = pythonic::operator_::div(a_fft, Kn_not0);
+      if (pythonic::operator_::eq(rank, 0L))
+      {
+        invlap_afft.fast(pythonic::types::make_tuple(0L, 0L)) = 0.0;
+      }
+      return invlap_afft;
+    }
     template <typename argument_type0 , typename argument_type1 >
     inline
-    typename type<argument_type0, argument_type1>::result_type operator()(argument_type0&& a_fft, argument_type1&& Kn) const
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral2D__get_phases_random
-  {
-    typedef void callable;
-    typedef void pure;
+    typename laplacian_fft::type<argument_type0, argument_type1>::result_type laplacian_fft::operator()(argument_type0 a_fft, argument_type1 Kn) const
+    {
+      return pythonic::operator_::mul(a_fft, Kn);
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    inline
+    typename __for_method__OperatorsPseudoSpectral2D__get_phases_random::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral2D__get_phases_random::operator()(argument_type0 self_KX, argument_type1 self_KY, argument_type2 self_deltax, argument_type3 self_deltay) const
     {
       typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::tuple{})>::type>::type __type0;
       typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::map{})>::type>::type __type1;
       typedef __for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0 __type2;
       typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type3;
       typedef long __type4;
       typedef decltype(std::declval<__type3>()(std::declval<__type4>())) __type5;
       typedef decltype(std::declval<__type1>()(std::declval<__type2>(), std::declval<__type5>())) __type6;
       typedef decltype(std::declval<__type0>()(std::declval<__type6>())) __type7;
       typedef typename pythonic::assignable<__type7>::type __type8;
-      typedef __type8 __type9;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type9>::type>::type __type10;
-      typedef typename pythonic::assignable<__type10>::type __type11;
-      typedef __type11 __type12;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type13;
-      typedef __type13 __type14;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type12>(), std::declval<__type14>())) __type15;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type16;
-      typedef __type16 __type17;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type15>(), std::declval<__type17>())) __type18;
-      typedef std::integral_constant<long,0> __type19;
-      typedef indexable_container<__type19, typename std::remove_reference<__type10>::type> __type20;
-      typedef typename __combined<__type8,__type20>::type __type21;
-      typedef __type21 __type22;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type22>::type>::type __type23;
-      typedef typename pythonic::assignable<__type23>::type __type24;
-      typedef __type24 __type25;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type26;
-      typedef __type26 __type27;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type25>(), std::declval<__type27>())) __type28;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type29;
-      typedef __type29 __type30;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type28>(), std::declval<__type30>())) __type31;
-      typedef decltype(pythonic::operator_::add(std::declval<__type18>(), std::declval<__type31>())) __type32;
-      typedef double __type34;
-      typedef decltype(pythonic::operator_::add(std::declval<__type12>(), std::declval<__type34>())) __type35;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type12>(), std::declval<__type34>())) __type37;
-      typedef typename __combined<__type35,__type37>::type __type38;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type38>(), std::declval<__type14>())) __type40;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type40>(), std::declval<__type17>())) __type42;
-      typedef decltype(pythonic::operator_::add(std::declval<__type25>(), std::declval<__type34>())) __type44;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type25>(), std::declval<__type34>())) __type46;
-      typedef typename __combined<__type44,__type46>::type __type47;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type47>(), std::declval<__type27>())) __type49;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type49>(), std::declval<__type30>())) __type51;
-      typedef decltype(pythonic::operator_::add(std::declval<__type42>(), std::declval<__type51>())) __type52;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type32>(), std::declval<__type52>())) __type53;
-      typedef typename pythonic::returnable<__type53>::type __type54;
-      typedef __type54 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& self_KX, argument_type1&& self_KY, argument_type2&& self_deltax, argument_type3&& self_deltay) const
-    ;
-  }  ;
-  template <typename argument_type0 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0::type<argument_type0>::result_type __for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0::operator()(argument_type0&& _) const
-  {
-    return pythonic::random::functor::uniform{}(-0.5, 0.5);
-  }
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
-    {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.1"));
-      return tmp_global;
-    }
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral2D__get_phases_random::type::result_type __code_new_method__OperatorsPseudoSpectral2D__get_phases_random::operator()() const
-  {
-    {
-      static typename __code_new_method__OperatorsPseudoSpectral2D__get_phases_random::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, ):\n    return backend_func(self.KX, self.KY, self.deltax, self.deltay, )\n\n");
-      return tmp_global;
+      typedef std::integral_constant<long,0> __type9;
+      typedef __type8 __type10;
+      typedef decltype(pythonic::types::as_const(std::declval<__type10>())) __type11;
+      typedef typename std::tuple_element<0,typename std::remove_reference<__type11>::type>::type __type12;
+      typedef indexable_container<__type9, typename std::remove_reference<__type12>::type> __type13;
+      typedef std::integral_constant<long,1> __type14;
+      typedef typename __combined<__type8,__type13>::type __type15;
+      typedef __type15 __type16;
+      typedef decltype(pythonic::types::as_const(std::declval<__type16>())) __type17;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type17>::type>::type __type18;
+      typedef indexable_container<__type14, typename std::remove_reference<__type18>::type> __type19;
+      typedef typename __combined<__type8,__type13,__type19>::type __type20;
+      typedef typename pythonic::assignable<__type20>::type __type21;
+      __type21 __tuple0 = pythonic::builtins::functor::tuple{}(pythonic::builtins::functor::map{}(__for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0(), pythonic::builtins::functor::range{}(2L)));
+      typename pythonic::assignable_noescape<decltype(std::get<0>(pythonic::types::as_const(__tuple0)))>::type alpha_x = std::get<0>(pythonic::types::as_const(__tuple0));
+      typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(__tuple0)))>::type alpha_y = std::get<1>(pythonic::types::as_const(__tuple0));
+      return pythonic::types::make_tuple(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(alpha_x, self_deltax), self_KX), pythonic::operator_::mul(pythonic::operator_::mul(alpha_y, self_deltay), self_KY)), pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_x, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_x, 0.5)), decltype(pythonic::operator_::sub(alpha_x, 0.5))>::type(pythonic::operator_::add(alpha_x, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_x, 0.5)), decltype(pythonic::operator_::sub(alpha_x, 0.5))>::type(pythonic::operator_::sub(alpha_x, 0.5))), self_deltax), self_KX), pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_y, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_y, 0.5)), decltype(pythonic::operator_::sub(alpha_y, 0.5))>::type(pythonic::operator_::add(alpha_y, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_y, 0.5)), decltype(pythonic::operator_::sub(alpha_y, 0.5))>::type(pythonic::operator_::sub(alpha_y, 0.5))), self_deltay), self_KY)));
     }
   }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::type::result_type __code_new_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::operator()() const
-  {
-    {
-      static typename __code_new_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, sov):\n    return backend_func(self._has_to_dealiase, self.where_dealiased, sov)\n\n");
-      return tmp_global;
-    }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::type<argument_type0, argument_type1, argument_type2>::result_type __for_method__OperatorsPseudoSpectral2D__dealiasing_setofvar::operator()(argument_type0&& self__has_to_dealiase, argument_type1&& self_where_dealiased, argument_type2&& sov) const
-  {
-    if (self__has_to_dealiase)
-    {
-      typename pythonic::lazy<decltype(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)))>::type nk = std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov));
-      typename pythonic::lazy<decltype(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)))>::type n0 = std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov));
-      typename pythonic::lazy<decltype(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)))>::type n1 = std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov));
-      {
-        long  __target140028821374096 = n0;
-        for (long  i0=0L; i0 < __target140028821374096; i0 += 1L)
-        {
-          {
-            long  __target140028818906016 = n1;
-            for (long  i1=0L; i1 < __target140028818906016; i1 += 1L)
-            {
-              if (self_where_dealiased[pythonic::types::make_tuple(i0, i1)])
-              {
-                {
-                  long  __target140028818906160 = nk;
-                  for (long  ik=0L; ik < __target140028818906160; ik += 1L)
-                  {
-                    sov[pythonic::types::make_tuple(ik, i0, i1)] = 0.0;
-                  }
-                }
-              }
-            }
-          }
-        }
-      }
-    }
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 >
-  inline
-  typename compute_increments_dim1::type<argument_type0, argument_type1>::result_type compute_increments_dim1::operator()(argument_type0&& var, argument_type1&& irx) const
-  {
-    typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, var)))>::type n1 = std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, var));
-    return pythonic::operator_::sub(var(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(irx,n1)), var(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(0L,pythonic::operator_::sub(n1, irx))));
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-  inline
-  typename invlaplacian_fft::type<argument_type0, argument_type1, argument_type2>::result_type invlaplacian_fft::operator()(argument_type0&& a_fft, argument_type1&& Kn_not0, argument_type2&& rank) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-    typedef __type0 __type1;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type2;
-    typedef __type2 __type3;
-    typedef decltype(pythonic::operator_::div(std::declval<__type1>(), std::declval<__type3>())) __type4;
-    typedef typename pythonic::assignable<__type4>::type __type5;
-    typedef long __type6;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type6>(), std::declval<__type6>())) __type7;
-    typedef indexable<__type7> __type8;
-    typedef double __type9;
-    typedef container<typename std::remove_reference<__type9>::type> __type10;
-    typedef typename __combined<__type5,__type8,__type10>::type __type11;
-    typedef typename pythonic::assignable<__type11>::type __type12;
-    __type12 invlap_afft = pythonic::operator_::div(a_fft, Kn_not0);
-    if (pythonic::operator_::eq(rank, 0L))
-    {
-      invlap_afft.fast(pythonic::types::make_tuple(0L, 0L)) = 0.0;
-    }
-    return invlap_afft;
-  }
-  template <typename argument_type0 , typename argument_type1 >
-  inline
-  typename laplacian_fft::type<argument_type0, argument_type1>::result_type laplacian_fft::operator()(argument_type0&& a_fft, argument_type1&& Kn) const
-  {
-    return pythonic::operator_::mul(a_fft, Kn);
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral2D__get_phases_random::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral2D__get_phases_random::operator()(argument_type0&& self_KX, argument_type1&& self_KY, argument_type2&& self_deltax, argument_type3&& self_deltay) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::tuple{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::map{})>::type>::type __type1;
-    typedef __for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0 __type2;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type3;
-    typedef long __type4;
-    typedef decltype(std::declval<__type3>()(std::declval<__type4>())) __type5;
-    typedef decltype(std::declval<__type1>()(std::declval<__type2>(), std::declval<__type5>())) __type6;
-    typedef decltype(std::declval<__type0>()(std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef std::integral_constant<long,0> __type9;
-    typedef __type8 __type10;
-    typedef typename std::tuple_element<0,typename std::remove_reference<__type10>::type>::type __type11;
-    typedef indexable_container<__type9, typename std::remove_reference<__type11>::type> __type12;
-    typedef std::integral_constant<long,1> __type13;
-    typedef typename __combined<__type8,__type12>::type __type14;
-    typedef __type14 __type15;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type15>::type>::type __type16;
-    typedef indexable_container<__type13, typename std::remove_reference<__type16>::type> __type17;
-    typedef typename __combined<__type8,__type12,__type17>::type __type18;
-    typedef typename pythonic::assignable<__type18>::type __type19;
-    __type19 __tuple0 = pythonic::builtins::functor::tuple{}(pythonic::builtins::functor::map{}(__for_method__OperatorsPseudoSpectral2D__get_phases_random_lambda0(), pythonic::builtins::functor::range{}(2L)));
-    typename pythonic::assignable_noescape<decltype(std::get<0>(__tuple0))>::type alpha_x = std::get<0>(__tuple0);
-    typename pythonic::assignable_noescape<decltype(std::get<1>(__tuple0))>::type alpha_y = std::get<1>(__tuple0);
-    return pythonic::types::make_tuple(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(alpha_x, self_deltax), self_KX), pythonic::operator_::mul(pythonic::operator_::mul(alpha_y, self_deltay), self_KY)), pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_x, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_x, 0.5)), decltype(pythonic::operator_::sub(alpha_x, 0.5))>::type(pythonic::operator_::add(alpha_x, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_x, 0.5)), decltype(pythonic::operator_::sub(alpha_x, 0.5))>::type(pythonic::operator_::sub(alpha_x, 0.5))), self_deltax), self_KX), pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_y, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_y, 0.5)), decltype(pythonic::operator_::sub(alpha_y, 0.5))>::type(pythonic::operator_::add(alpha_y, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_y, 0.5)), decltype(pythonic::operator_::sub(alpha_y, 0.5))>::type(pythonic::operator_::sub(alpha_y, 0.5))), self_deltay), self_KY)));
-  }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_operators2d::__transonic__()());
 static PyObject* __code_new_method__OperatorsPseudoSpectral2D__get_phases_random = to_python(__pythran_operators2d::__code_new_method__OperatorsPseudoSpectral2D__get_phases_random()());
 inline
 typename __pythran_operators2d::__for_method__OperatorsPseudoSpectral2D__get_phases_random::type<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, double, double>::result_type __for_method__OperatorsPseudoSpectral2D__get_phases_random0(pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& self_KX, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& self_KY, double&& self_deltax, double&& self_deltay) 
@@ -1139,17 +1148,17 @@
                                                      Methods,
                                                      ""
                 );
                 #endif
                 if(! theModule)
                     PYTHRAN_RETURN;
                 PyObject * theDoc = Py_BuildValue("(sss)",
-                                                  "0.12.0",
-                                                  "2022-10-28 09:10:29.789589",
-                                                  "d763011fd0acaef00e80fba50db5c858f0a893a207a3554bbf114a1f0fbcbbf4");
+                                                  "0.13.1",
+                                                  "2023-05-24 11:29:39.975885",
+                                                  "6836ea80017072922f20c1f41ddb3ae52d9106d3b02323070cf65af78d5f0adb");
                 if(! theDoc)
                     PYTHRAN_RETURN;
                 PyModule_AddObject(theModule,
                                    "__pythran__",
                                    theDoc);
 
                 PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/operators/__pythran__/operators3d.cpp` & `fluidsim-0.7.3/fluidsim/operators/__pythran__/operators3d.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #include <pythonic/core.hpp>
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
-#include <pythonic/include/types/uint8.hpp>
-#include <pythonic/include/types/complex128.hpp>
 #include <pythonic/include/types/float64.hpp>
+#include <pythonic/include/types/complex128.hpp>
+#include <pythonic/include/types/uint8.hpp>
 #include <pythonic/include/types/ndarray.hpp>
+#include <pythonic/types/float64.hpp>
+#include <pythonic/types/uint8.hpp>
 #include <pythonic/types/ndarray.hpp>
 #include <pythonic/types/complex128.hpp>
-#include <pythonic/types/uint8.hpp>
-#include <pythonic/types/float64.hpp>
 #include <pythonic/include/__dispatch__/copy.hpp>
 #include <pythonic/include/builtins/None.hpp>
 #include <pythonic/include/builtins/enumerate.hpp>
 #include <pythonic/include/builtins/getattr.hpp>
 #include <pythonic/include/builtins/map.hpp>
 #include <pythonic/include/builtins/pythran/abssqr.hpp>
 #include <pythonic/include/builtins/range.hpp>
@@ -55,2058 +55,2088 @@
 #include <pythonic/operator_/lt.hpp>
 #include <pythonic/operator_/mul.hpp>
 #include <pythonic/operator_/neg.hpp>
 #include <pythonic/operator_/sub.hpp>
 #include <pythonic/random/uniform.hpp>
 #include <pythonic/types/complex.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_operators3d
+namespace 
 {
-  struct __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0
+  namespace __pythran_operators3d
   {
-    typedef void callable;
-    ;
-    template <typename argument_type0 >
-    struct type
+    struct __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0
     {
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::random::functor::uniform{})>::type>::type __type0;
-      typedef double __type1;
-      typedef decltype(std::declval<__type0>()(std::declval<__type1>(), std::declval<__type1>())) __type2;
-      typedef typename pythonic::returnable<__type2>::type __type3;
-      typedef __type3 result_type;
-    }  
-    ;
-    template <typename argument_type0 >
-    inline
-    typename type<argument_type0>::result_type operator()(argument_type0&& _) const
-    ;
-  }  ;
-  struct __transonic__
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
+      typedef void callable;
+      ;
+      template <typename argument_type0 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::random::functor::uniform{})>::type>::type __type0;
+        typedef double __type1;
+        typedef decltype(std::declval<__type0>()(std::declval<__type1>(), std::declval<__type1>())) __type2;
+        typedef typename pythonic::returnable<__type2>::type __type3;
+        typedef __type3 result_type;
+      }  
+      ;
+      template <typename argument_type0 >
+      inline
+      typename type<argument_type0>::result_type operator()(argument_type0 _) const
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__get_phases_random
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+    struct __transonic__
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+    struct __code_new_method__OperatorsPseudoSpectral3D__get_phases_random
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    struct __code_new_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft
     {
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::empty_like{})>::type>::type __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-      typedef typename pythonic::assignable<__type3>::type __type4;
-      typedef __type4 __type5;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type5>(), std::declval<__type5>(), std::declval<__type5>())) __type14;
-      typedef typename pythonic::returnable<__type14>::type __type15;
-      typedef __type15 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& arr_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    struct type
+    struct __for_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft
     {
-      typedef std::complex<double> __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type2>())) __type3;
-      typedef long __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type5;
-      typedef decltype(std::declval<__type5>()(std::declval<__type2>())) __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(std::declval<__type5>()(std::declval<__type9>())) __type10;
-      typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
-      typedef typename pythonic::assignable<__type11>::type __type12;
-      typedef double __type13;
-      typedef container<typename std::remove_reference<__type13>::type> __type14;
-      typedef typename __combined<__type12,__type14>::type __type15;
-      typedef __type15 __type16;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type16>(), std::declval<__type4>())) __type17;
-      typedef indexable<__type17> __type18;
-      typedef typename __combined<__type12,__type18,__type14>::type __type19;
-      typedef __type19 __type20;
-      typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type20>())) __type21;
-      typedef typename pythonic::assignable<__type21>::type __type22;
-      typedef __type22 __type23;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type23>())) __type24;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type25;
-      typedef __type25 __type26;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type24>(), std::declval<__type26>())) __type27;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type9>())) __type29;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type29>(), std::declval<__type23>())) __type31;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type31>(), std::declval<__type26>())) __type33;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type27>(), std::declval<__type33>())) __type34;
-      typedef typename pythonic::returnable<__type34>::type __type35;
-      typedef __type35 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& divh_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::empty_like{})>::type>::type __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type1;
+        typedef __type1 __type2;
+        typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+        typedef typename pythonic::assignable<__type3>::type __type4;
+        typedef __type4 __type5;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type5>(), std::declval<__type5>(), std::declval<__type5>())) __type14;
+        typedef typename pythonic::returnable<__type14>::type __type15;
+        typedef __type15 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 arr_fft) const
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    struct type
+    struct __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft
     {
-      typedef std::complex<double> __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type2>())) __type3;
-      typedef long __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef decltype(std::declval<__type5>()(std::declval<__type7>())) __type8;
-      typedef decltype(std::declval<__type5>()(std::declval<__type2>())) __type10;
-      typedef decltype(pythonic::operator_::add(std::declval<__type8>(), std::declval<__type10>())) __type11;
-      typedef typename pythonic::assignable<__type11>::type __type12;
-      typedef double __type13;
-      typedef container<typename std::remove_reference<__type13>::type> __type14;
-      typedef typename __combined<__type12,__type14>::type __type15;
-      typedef __type15 __type16;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type16>(), std::declval<__type4>())) __type17;
-      typedef indexable<__type17> __type18;
-      typedef typename __combined<__type12,__type18,__type14>::type __type19;
-      typedef __type19 __type20;
-      typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type20>())) __type21;
-      typedef typename pythonic::assignable<__type21>::type __type22;
-      typedef __type22 __type23;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type23>())) __type24;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type25;
-      typedef __type25 __type26;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type24>(), std::declval<__type26>())) __type27;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type7>())) __type29;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type29>(), std::declval<__type23>())) __type31;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type31>(), std::declval<__type26>())) __type33;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type27>(), std::declval<__type33>())) __type34;
-      typedef typename pythonic::returnable<__type34>::type __type35;
-      typedef __type35 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& rotz_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    struct __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft
     {
-      typedef std::complex<double> __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
-      typedef __type3 __type4;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type2>(), std::declval<__type4>())) __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type9>())) __type10;
-      typedef decltype(pythonic::operator_::add(std::declval<__type5>(), std::declval<__type10>())) __type11;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type11>())) __type12;
-      typedef typename pythonic::returnable<__type12>::type __type13;
-      typedef __type13 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vx_fft, argument_type3&& vy_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      struct type
+      {
+        typedef std::complex<double> __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+        typedef __type1 __type2;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type2>())) __type3;
+        typedef long __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type5;
+        typedef decltype(std::declval<__type5>()(std::declval<__type2>())) __type7;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type8;
+        typedef __type8 __type9;
+        typedef decltype(std::declval<__type5>()(std::declval<__type9>())) __type10;
+        typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef double __type13;
+        typedef container<typename std::remove_reference<__type13>::type> __type14;
+        typedef typename __combined<__type12,__type14>::type __type15;
+        typedef __type15 __type16;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type16>(), std::declval<__type4>())) __type17;
+        typedef indexable<__type17> __type18;
+        typedef typename __combined<__type12,__type18,__type14>::type __type19;
+        typedef __type19 __type20;
+        typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type20>())) __type21;
+        typedef typename pythonic::assignable<__type21>::type __type22;
+        typedef __type22 __type23;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type23>())) __type24;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type25;
+        typedef __type25 __type26;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type24>(), std::declval<__type26>())) __type27;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type9>())) __type29;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type29>(), std::declval<__type23>())) __type31;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type31>(), std::declval<__type26>())) __type33;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type27>(), std::declval<__type33>())) __type34;
+        typedef typename pythonic::returnable<__type34>::type __type35;
+        typedef __type35 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 divh_fft) const
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    struct type
+    struct __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft
     {
-      typedef std::complex<double> __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type3;
-      typedef double __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef decltype(std::declval<__type5>()(std::declval<__type7>())) __type8;
-      typedef decltype(std::declval<__type5>()(std::declval<__type2>())) __type10;
-      typedef decltype(pythonic::operator_::add(std::declval<__type8>(), std::declval<__type10>())) __type11;
-      typedef typename pythonic::assignable<__type11>::type __type12;
-      typedef container<typename std::remove_reference<__type4>::type> __type13;
-      typedef typename __combined<__type12,__type13>::type __type14;
-      typedef __type14 __type15;
-      typedef long __type16;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type15>(), std::declval<__type16>())) __type17;
-      typedef indexable<__type17> __type18;
-      typedef typename __combined<__type12,__type18,__type13>::type __type19;
-      typedef __type19 __type20;
-      typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type20>())) __type21;
-      typedef decltype(std::declval<__type3>()(std::declval<__type21>())) __type22;
-      typedef typename pythonic::assignable<__type22>::type __type23;
-      typedef __type23 __type24;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type2>(), std::declval<__type24>())) __type25;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type25>())) __type26;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type27;
-      typedef __type27 __type28;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type26>(), std::declval<__type28>())) __type29;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type24>())) __type32;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type32>())) __type33;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type33>(), std::declval<__type28>())) __type35;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros_like{})>::type>::type __type36;
-      typedef decltype(std::declval<__type36>()(std::declval<__type28>())) __type38;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type29>(), std::declval<__type35>(), std::declval<__type38>())) __type39;
-      typedef typename pythonic::returnable<__type39>::type __type40;
-      typedef __type40 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vt_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-    struct type
+    struct __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft
     {
-      typedef std::complex<double> __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type3;
-      typedef double __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef decltype(std::declval<__type5>()(std::declval<__type7>())) __type8;
-      typedef decltype(std::declval<__type5>()(std::declval<__type2>())) __type10;
-      typedef decltype(pythonic::operator_::add(std::declval<__type8>(), std::declval<__type10>())) __type11;
-      typedef typename pythonic::assignable<__type11>::type __type12;
-      typedef container<typename std::remove_reference<__type4>::type> __type13;
-      typedef typename __combined<__type12,__type13>::type __type14;
-      typedef __type14 __type15;
-      typedef long __type16;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type15>(), std::declval<__type16>())) __type17;
-      typedef indexable<__type17> __type18;
-      typedef typename __combined<__type12,__type18,__type13>::type __type19;
-      typedef __type19 __type20;
-      typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type20>())) __type21;
-      typedef decltype(std::declval<__type3>()(std::declval<__type21>())) __type22;
-      typedef typename pythonic::assignable<__type22>::type __type23;
-      typedef __type23 __type24;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type2>(), std::declval<__type24>())) __type25;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type25>())) __type26;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type27;
-      typedef __type27 __type28;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type26>(), std::declval<__type28>())) __type29;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type24>())) __type32;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type32>())) __type33;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type34;
-      typedef __type34 __type35;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type33>(), std::declval<__type35>())) __type36;
-      typedef decltype(pythonic::operator_::add(std::declval<__type29>(), std::declval<__type36>())) __type37;
-      typedef typename pythonic::returnable<__type37>::type __type38;
-      typedef __type38 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vx_fft, argument_type3&& vy_fft, argument_type4&& vz_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__project_toroidal
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      struct type
+      {
+        typedef std::complex<double> __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
+        typedef __type1 __type2;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type2>())) __type3;
+        typedef long __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type5;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type6;
+        typedef __type6 __type7;
+        typedef decltype(std::declval<__type5>()(std::declval<__type7>())) __type8;
+        typedef decltype(std::declval<__type5>()(std::declval<__type2>())) __type10;
+        typedef decltype(pythonic::operator_::add(std::declval<__type8>(), std::declval<__type10>())) __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef double __type13;
+        typedef container<typename std::remove_reference<__type13>::type> __type14;
+        typedef typename __combined<__type12,__type14>::type __type15;
+        typedef __type15 __type16;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type16>(), std::declval<__type4>())) __type17;
+        typedef indexable<__type17> __type18;
+        typedef typename __combined<__type12,__type18,__type14>::type __type19;
+        typedef __type19 __type20;
+        typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type20>())) __type21;
+        typedef typename pythonic::assignable<__type21>::type __type22;
+        typedef __type22 __type23;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type23>())) __type24;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type25;
+        typedef __type25 __type26;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type24>(), std::declval<__type26>())) __type27;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type7>())) __type29;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type29>(), std::declval<__type23>())) __type31;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type31>(), std::declval<__type26>())) __type33;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type27>(), std::declval<__type33>())) __type34;
+        typedef typename pythonic::returnable<__type34>::type __type35;
+        typedef __type35 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 rotz_fft) const
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__project_toroidal
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-    struct type
+    struct __code_new_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type2;
-      typedef double __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
-      typedef decltype(std::declval<__type4>()(std::declval<__type1>())) __type9;
-      typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type9>())) __type10;
-      typedef typename pythonic::assignable<__type10>::type __type11;
-      typedef container<typename std::remove_reference<__type3>::type> __type12;
-      typedef typename __combined<__type11,__type12>::type __type13;
-      typedef __type13 __type14;
-      typedef long __type15;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type14>(), std::declval<__type15>())) __type16;
-      typedef indexable<__type16> __type17;
-      typedef typename __combined<__type11,__type17,__type12>::type __type18;
-      typedef __type18 __type19;
-      typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type19>())) __type20;
-      typedef decltype(std::declval<__type2>()(std::declval<__type20>())) __type21;
-      typedef typename pythonic::assignable<__type21>::type __type22;
-      typedef __type22 __type23;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type23>())) __type24;
-      typedef typename pythonic::assignable<__type24>::type __type25;
-      typedef __type25 __type26;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type27;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type28;
-      typedef __type28 __type29;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type29>())) __type30;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type30>::type>::type __type31;
-      typedef typename pythonic::lazy<__type31>::type __type32;
-      typedef __type32 __type33;
-      typedef decltype(std::declval<__type27>()(std::declval<__type33>())) __type34;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type34>::type::iterator>::value_type>::type __type35;
-      typedef __type35 __type36;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type30>::type>::type __type37;
-      typedef typename pythonic::lazy<__type37>::type __type38;
-      typedef __type38 __type39;
-      typedef decltype(std::declval<__type27>()(std::declval<__type39>())) __type40;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type40>::type::iterator>::value_type>::type __type41;
-      typedef __type41 __type42;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type30>::type>::type __type43;
-      typedef typename pythonic::lazy<__type43>::type __type44;
-      typedef __type44 __type45;
-      typedef decltype(std::declval<__type27>()(std::declval<__type45>())) __type46;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type46>::type::iterator>::value_type>::type __type47;
-      typedef __type47 __type48;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type36>(), std::declval<__type42>(), std::declval<__type48>())) __type49;
-      typedef decltype(std::declval<__type26>()[std::declval<__type49>()]) __type50;
-      typedef decltype(pythonic::operator_::neg(std::declval<__type50>())) __type51;
-      typedef decltype(pythonic::operator_::neg(std::declval<__type26>())) __type53;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type53>(), std::declval<__type29>())) __type55;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type23>())) __type58;
-      typedef typename pythonic::assignable<__type58>::type __type59;
-      typedef __type59 __type60;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type61;
-      typedef decltype(std::declval<__type60>()[std::declval<__type49>()]) __type67;
-      typedef __type61 __type68;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type60>(), std::declval<__type68>())) __type69;
-      typedef decltype(pythonic::operator_::add(std::declval<__type55>(), std::declval<__type69>())) __type70;
-      typedef typename pythonic::assignable<__type70>::type __type71;
-      typedef __type71 __type72;
-      typedef decltype(std::declval<__type72>()[std::declval<__type49>()]) __type77;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type67>(), std::declval<__type77>())) __type78;
-      typedef container<typename std::remove_reference<__type78>::type> __type79;
-      typedef indexable<__type49> __type84;
-      typedef typename __combined<__type61,__type79,__type84>::type __type85;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type51>(), std::declval<__type77>())) __type92;
-      typedef container<typename std::remove_reference<__type92>::type> __type93;
-      typedef typename __combined<__type28,__type93,__type84>::type __type99;
-      typedef __type92 __type100;
-      typedef __type49 __type101;
-      typedef __type78 __type102;
-      typedef __type3 __type104;
-      typedef pythonic::types::none_type __type110;
-      typedef typename pythonic::returnable<__type110>::type __type111;
-      typedef __type100 __ptype0;
-      typedef __type101 __ptype1;
-      typedef __type102 __ptype4;
-      typedef __type101 __ptype5;
-      typedef __type104 __ptype8;
-      typedef __type101 __ptype9;
-      typedef __type111 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vx_fft, argument_type3&& vy_fft, argument_type4&& vz_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    struct __for_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type2;
-      typedef double __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(std::declval<__type4>()(std::declval<__type9>())) __type10;
-      typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
-      typedef typename pythonic::assignable<__type11>::type __type12;
-      typedef __type12 __type13;
-      typedef decltype(std::declval<__type4>()(std::declval<__type1>())) __type15;
-      typedef decltype(pythonic::operator_::add(std::declval<__type13>(), std::declval<__type15>())) __type16;
-      typedef typename pythonic::assignable<__type16>::type __type17;
-      typedef container<typename std::remove_reference<__type3>::type> __type18;
-      typedef typename __combined<__type17,__type18>::type __type19;
-      typedef __type19 __type20;
-      typedef long __type21;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type20>(), std::declval<__type21>())) __type22;
-      typedef indexable<__type22> __type23;
-      typedef typename __combined<__type17,__type23,__type18>::type __type24;
-      typedef __type24 __type25;
-      typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type25>())) __type26;
-      typedef typename pythonic::assignable<__type26>::type __type27;
-      typedef __type27 __type28;
-      typedef decltype(std::declval<__type2>()(std::declval<__type28>())) __type29;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type29>())) __type30;
-      typedef typename pythonic::assignable<__type30>::type __type31;
-      typedef __type31 __type32;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type34;
-      typedef decltype(std::declval<__type34>()(std::declval<__type13>())) __type36;
-      typedef typename pythonic::assignable<__type36>::type __type37;
-      typedef typename __combined<__type37,__type18>::type __type38;
-      typedef __type38 __type39;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type39>(), std::declval<__type21>())) __type40;
-      typedef indexable<__type40> __type41;
-      typedef typename __combined<__type37,__type41,__type18>::type __type42;
-      typedef __type42 __type43;
-      typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type43>())) __type44;
-      typedef typename pythonic::assignable<__type44>::type __type45;
-      typedef __type45 __type46;
-      typedef decltype(std::declval<__type2>()(std::declval<__type46>())) __type47;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type47>())) __type48;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type48>())) __type49;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type50;
-      typedef __type50 __type51;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type49>(), std::declval<__type51>())) __type52;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type9>(), std::declval<__type47>())) __type57;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type57>())) __type58;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type58>(), std::declval<__type51>())) __type60;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type28>())) __type63;
-      typedef decltype(std::declval<__type2>()(std::declval<__type63>())) __type64;
-      typedef decltype(pythonic::operator_::neg(std::declval<__type64>())) __type65;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type65>(), std::declval<__type51>())) __type67;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type52>(), std::declval<__type60>(), std::declval<__type67>())) __type68;
-      typedef typename pythonic::returnable<__type68>::type __type69;
-      typedef __type69 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& vp_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef std::complex<double> __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+        typedef __type1 __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
+        typedef __type3 __type4;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type2>(), std::declval<__type4>())) __type5;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type6;
+        typedef __type6 __type7;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type8;
+        typedef __type8 __type9;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type9>())) __type10;
+        typedef decltype(pythonic::operator_::add(std::declval<__type5>(), std::declval<__type10>())) __type11;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type11>())) __type12;
+        typedef typename pythonic::returnable<__type12>::type __type13;
+        typedef __type13 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vx_fft, argument_type3 vy_fft) const
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    struct type
+    struct __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type2;
-      typedef double __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(std::declval<__type4>()(std::declval<__type9>())) __type10;
-      typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
-      typedef typename pythonic::assignable<__type11>::type __type12;
-      typedef __type12 __type13;
-      typedef decltype(std::declval<__type4>()(std::declval<__type1>())) __type15;
-      typedef decltype(pythonic::operator_::add(std::declval<__type13>(), std::declval<__type15>())) __type16;
-      typedef typename pythonic::assignable<__type16>::type __type17;
-      typedef container<typename std::remove_reference<__type3>::type> __type18;
-      typedef typename __combined<__type17,__type18>::type __type19;
-      typedef __type19 __type20;
-      typedef long __type21;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type20>(), std::declval<__type21>())) __type22;
-      typedef indexable<__type22> __type23;
-      typedef typename __combined<__type17,__type23,__type18>::type __type24;
-      typedef __type24 __type25;
-      typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type25>())) __type26;
-      typedef typename pythonic::assignable<__type26>::type __type27;
-      typedef __type27 __type28;
-      typedef decltype(std::declval<__type2>()(std::declval<__type28>())) __type29;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type29>())) __type30;
-      typedef typename pythonic::assignable<__type30>::type __type31;
-      typedef __type31 __type32;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type34;
-      typedef decltype(std::declval<__type34>()(std::declval<__type13>())) __type36;
-      typedef typename pythonic::assignable<__type36>::type __type37;
-      typedef typename __combined<__type37,__type18>::type __type38;
-      typedef __type38 __type39;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type39>(), std::declval<__type21>())) __type40;
-      typedef indexable<__type40> __type41;
-      typedef typename __combined<__type37,__type41,__type18>::type __type42;
-      typedef __type42 __type43;
-      typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type43>())) __type44;
-      typedef typename pythonic::assignable<__type44>::type __type45;
-      typedef __type45 __type46;
-      typedef decltype(std::declval<__type2>()(std::declval<__type46>())) __type47;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type47>())) __type48;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type48>())) __type49;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type50;
-      typedef __type50 __type51;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type49>(), std::declval<__type51>())) __type52;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type9>(), std::declval<__type47>())) __type57;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type57>())) __type58;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type59;
-      typedef __type59 __type60;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type58>(), std::declval<__type60>())) __type61;
-      typedef decltype(pythonic::operator_::add(std::declval<__type52>(), std::declval<__type61>())) __type62;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type28>())) __type65;
-      typedef decltype(std::declval<__type2>()(std::declval<__type65>())) __type66;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type67;
-      typedef __type67 __type68;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type66>(), std::declval<__type68>())) __type69;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type62>(), std::declval<__type69>())) __type70;
-      typedef typename pythonic::returnable<__type70>::type __type71;
-      typedef __type71 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& vx_fft, argument_type4&& vy_fft, argument_type5&& vz_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__project_poloidal
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__project_poloidal
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    struct type
+    struct __for_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type2;
-      typedef double __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(std::declval<__type4>()(std::declval<__type9>())) __type10;
-      typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
-      typedef typename pythonic::assignable<__type11>::type __type12;
-      typedef __type12 __type13;
-      typedef decltype(std::declval<__type4>()(std::declval<__type1>())) __type15;
-      typedef decltype(pythonic::operator_::add(std::declval<__type13>(), std::declval<__type15>())) __type16;
-      typedef typename pythonic::assignable<__type16>::type __type17;
-      typedef container<typename std::remove_reference<__type3>::type> __type18;
-      typedef typename __combined<__type17,__type18>::type __type19;
-      typedef __type19 __type20;
-      typedef long __type21;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type20>(), std::declval<__type21>())) __type22;
-      typedef indexable<__type22> __type23;
-      typedef typename __combined<__type17,__type23,__type18>::type __type24;
-      typedef __type24 __type25;
-      typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type25>())) __type26;
-      typedef typename pythonic::assignable<__type26>::type __type27;
-      typedef __type27 __type28;
-      typedef decltype(std::declval<__type2>()(std::declval<__type28>())) __type29;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type29>())) __type30;
-      typedef typename pythonic::assignable<__type30>::type __type31;
-      typedef __type31 __type32;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type33;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type34;
-      typedef __type34 __type35;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type35>())) __type36;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type36>::type>::type __type37;
-      typedef typename pythonic::lazy<__type37>::type __type38;
-      typedef __type38 __type39;
-      typedef decltype(std::declval<__type33>()(std::declval<__type39>())) __type40;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type40>::type::iterator>::value_type>::type __type41;
-      typedef __type41 __type42;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type36>::type>::type __type43;
-      typedef typename pythonic::lazy<__type43>::type __type44;
-      typedef __type44 __type45;
-      typedef decltype(std::declval<__type33>()(std::declval<__type45>())) __type46;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type46>::type::iterator>::value_type>::type __type47;
-      typedef __type47 __type48;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type36>::type>::type __type49;
-      typedef typename pythonic::lazy<__type49>::type __type50;
-      typedef __type50 __type51;
-      typedef decltype(std::declval<__type33>()(std::declval<__type51>())) __type52;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type52>::type::iterator>::value_type>::type __type53;
-      typedef __type53 __type54;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type42>(), std::declval<__type48>(), std::declval<__type54>())) __type55;
-      typedef decltype(std::declval<__type32>()[std::declval<__type55>()]) __type56;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type58;
-      typedef decltype(std::declval<__type58>()(std::declval<__type13>())) __type60;
-      typedef typename pythonic::assignable<__type60>::type __type61;
-      typedef typename __combined<__type61,__type18>::type __type62;
-      typedef __type62 __type63;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type63>(), std::declval<__type21>())) __type64;
-      typedef indexable<__type64> __type65;
-      typedef typename __combined<__type61,__type65,__type18>::type __type66;
-      typedef __type66 __type67;
-      typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type67>())) __type68;
-      typedef typename pythonic::assignable<__type68>::type __type69;
-      typedef __type69 __type70;
-      typedef decltype(std::declval<__type2>()(std::declval<__type70>())) __type71;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type71>())) __type72;
-      typedef typename pythonic::assignable<__type72>::type __type73;
-      typedef __type73 __type74;
-      typedef decltype(std::declval<__type74>()[std::declval<__type55>()]) __type79;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type56>(), std::declval<__type79>())) __type80;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type74>())) __type83;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type83>(), std::declval<__type35>())) __type85;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type9>(), std::declval<__type71>())) __type90;
-      typedef typename pythonic::assignable<__type90>::type __type91;
-      typedef __type91 __type92;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type92>())) __type93;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type94;
-      typedef decltype(std::declval<__type92>()[std::declval<__type55>()]) __type106;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type56>(), std::declval<__type106>())) __type107;
-      typedef __type94 __type108;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type93>(), std::declval<__type108>())) __type109;
-      typedef decltype(pythonic::operator_::add(std::declval<__type85>(), std::declval<__type109>())) __type110;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type28>())) __type113;
-      typedef decltype(std::declval<__type2>()(std::declval<__type113>())) __type114;
-      typedef typename pythonic::assignable<__type114>::type __type115;
-      typedef __type115 __type116;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type117;
-      typedef decltype(std::declval<__type116>()[std::declval<__type55>()]) __type123;
-      typedef decltype(pythonic::operator_::neg(std::declval<__type123>())) __type124;
-      typedef __type117 __type125;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type116>(), std::declval<__type125>())) __type126;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type110>(), std::declval<__type126>())) __type127;
-      typedef typename pythonic::assignable<__type127>::type __type128;
-      typedef __type128 __type129;
-      typedef decltype(std::declval<__type129>()[std::declval<__type55>()]) __type134;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type124>(), std::declval<__type134>())) __type135;
-      typedef container<typename std::remove_reference<__type135>::type> __type136;
-      typedef indexable<__type55> __type141;
-      typedef typename __combined<__type117,__type136,__type141>::type __type142;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type107>(), std::declval<__type134>())) __type149;
-      typedef container<typename std::remove_reference<__type149>::type> __type150;
-      typedef typename __combined<__type94,__type150,__type141>::type __type156;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type80>(), std::declval<__type134>())) __type163;
-      typedef container<typename std::remove_reference<__type163>::type> __type164;
-      typedef typename __combined<__type34,__type164,__type141>::type __type170;
-      typedef __type163 __type171;
-      typedef __type55 __type172;
-      typedef __type149 __type173;
-      typedef __type135 __type175;
-      typedef pythonic::types::none_type __type177;
-      typedef typename pythonic::returnable<__type177>::type __type178;
-      typedef __type171 __ptype12;
-      typedef __type172 __ptype13;
-      typedef __type173 __ptype16;
-      typedef __type172 __ptype17;
-      typedef __type175 __ptype20;
-      typedef __type172 __ptype21;
-      typedef __type178 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& vx_fft, argument_type4&& vy_fft, argument_type5&& vz_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__project_kradial3d
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      struct type
+      {
+        typedef std::complex<double> __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
+        typedef __type1 __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type3;
+        typedef double __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type5;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type6;
+        typedef __type6 __type7;
+        typedef decltype(std::declval<__type5>()(std::declval<__type7>())) __type8;
+        typedef decltype(std::declval<__type5>()(std::declval<__type2>())) __type10;
+        typedef decltype(pythonic::operator_::add(std::declval<__type8>(), std::declval<__type10>())) __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef container<typename std::remove_reference<__type4>::type> __type13;
+        typedef typename __combined<__type12,__type13>::type __type14;
+        typedef __type14 __type15;
+        typedef long __type16;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type15>(), std::declval<__type16>())) __type17;
+        typedef indexable<__type17> __type18;
+        typedef typename __combined<__type12,__type18,__type13>::type __type19;
+        typedef __type19 __type20;
+        typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type20>())) __type21;
+        typedef decltype(std::declval<__type3>()(std::declval<__type21>())) __type22;
+        typedef typename pythonic::assignable<__type22>::type __type23;
+        typedef __type23 __type24;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type2>(), std::declval<__type24>())) __type25;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type25>())) __type26;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type27;
+        typedef __type27 __type28;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type26>(), std::declval<__type28>())) __type29;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type24>())) __type32;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type32>())) __type33;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type33>(), std::declval<__type28>())) __type35;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros_like{})>::type>::type __type36;
+        typedef decltype(std::declval<__type36>()(std::declval<__type28>())) __type38;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type29>(), std::declval<__type35>(), std::declval<__type38>())) __type39;
+        typedef typename pythonic::returnable<__type39>::type __type40;
+        typedef __type40 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vt_fft) const
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__project_kradial3d
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    struct type
+    struct __code_new_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type3;
-      typedef __type3 __type4;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type4>())) __type5;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type5>::type>::type __type6;
-      typedef typename pythonic::lazy<__type6>::type __type7;
-      typedef __type7 __type8;
-      typedef decltype(std::declval<__type2>()(std::declval<__type8>())) __type9;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type9>::type::iterator>::value_type>::type __type10;
-      typedef __type10 __type11;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type5>::type>::type __type12;
-      typedef typename pythonic::lazy<__type12>::type __type13;
-      typedef __type13 __type14;
-      typedef decltype(std::declval<__type2>()(std::declval<__type14>())) __type15;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type15>::type::iterator>::value_type>::type __type16;
-      typedef __type16 __type17;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type5>::type>::type __type18;
-      typedef typename pythonic::lazy<__type18>::type __type19;
-      typedef __type19 __type20;
-      typedef decltype(std::declval<__type2>()(std::declval<__type20>())) __type21;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type21>::type::iterator>::value_type>::type __type22;
-      typedef __type22 __type23;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type11>(), std::declval<__type17>(), std::declval<__type23>())) __type24;
-      typedef decltype(std::declval<__type1>()[std::declval<__type24>()]) __type25;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type4>())) __type28;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type29;
-      typedef __type29 __type30;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type31;
-      typedef decltype(std::declval<__type30>()[std::declval<__type24>()]) __type37;
-      typedef __type31 __type38;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type30>(), std::declval<__type38>())) __type39;
-      typedef decltype(pythonic::operator_::add(std::declval<__type28>(), std::declval<__type39>())) __type40;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type41;
-      typedef __type41 __type42;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type43;
-      typedef decltype(std::declval<__type42>()[std::declval<__type24>()]) __type49;
-      typedef __type43 __type50;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type42>(), std::declval<__type50>())) __type51;
-      typedef decltype(pythonic::operator_::add(std::declval<__type40>(), std::declval<__type51>())) __type52;
-      typedef double __type53;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type54;
-      typedef decltype(std::declval<__type54>()(std::declval<__type1>())) __type56;
-      typedef decltype(std::declval<__type54>()(std::declval<__type30>())) __type58;
-      typedef decltype(pythonic::operator_::add(std::declval<__type56>(), std::declval<__type58>())) __type59;
-      typedef decltype(std::declval<__type54>()(std::declval<__type42>())) __type61;
-      typedef decltype(pythonic::operator_::add(std::declval<__type59>(), std::declval<__type61>())) __type62;
-      typedef typename pythonic::assignable<__type62>::type __type63;
-      typedef container<typename std::remove_reference<__type53>::type> __type64;
-      typedef typename __combined<__type63,__type64>::type __type65;
-      typedef __type65 __type66;
-      typedef long __type67;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type66>(), std::declval<__type67>())) __type68;
-      typedef indexable<__type68> __type69;
-      typedef typename __combined<__type63,__type69,__type64>::type __type70;
-      typedef __type70 __type71;
-      typedef decltype(pythonic::operator_::div(std::declval<__type53>(), std::declval<__type71>())) __type72;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type52>(), std::declval<__type72>())) __type73;
-      typedef typename pythonic::assignable<__type73>::type __type74;
-      typedef __type74 __type75;
-      typedef decltype(std::declval<__type75>()[std::declval<__type24>()]) __type80;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type49>(), std::declval<__type80>())) __type81;
-      typedef container<typename std::remove_reference<__type81>::type> __type82;
-      typedef indexable<__type24> __type87;
-      typedef typename __combined<__type43,__type82,__type87>::type __type88;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type37>(), std::declval<__type80>())) __type95;
-      typedef container<typename std::remove_reference<__type95>::type> __type96;
-      typedef typename __combined<__type31,__type96,__type87>::type __type102;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type25>(), std::declval<__type80>())) __type109;
-      typedef container<typename std::remove_reference<__type109>::type> __type110;
-      typedef typename __combined<__type3,__type110,__type87>::type __type116;
-      typedef __type109 __type117;
-      typedef __type24 __type118;
-      typedef __type95 __type119;
-      typedef __type81 __type121;
-      typedef pythonic::types::none_type __type123;
-      typedef typename pythonic::returnable<__type123>::type __type124;
-      typedef __type117 __ptype24;
-      typedef __type118 __ptype25;
-      typedef __type119 __ptype28;
-      typedef __type118 __ptype29;
-      typedef __type121 __ptype32;
-      typedef __type118 __ptype33;
-      typedef __type124 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& vx_fft, argument_type4&& vy_fft, argument_type5&& vz_fft) const
-    ;
-  }  ;
-  struct __code_new_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft
-  {
-    typedef void callable;
-    typedef void pure;
-    struct type
-    {
-      typedef pythonic::types::str __type0;
-      typedef typename pythonic::returnable<__type0>::type __type1;
-      typedef __type1 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    struct type
+    struct __for_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type1>())) __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type9>())) __type10;
-      typedef decltype(pythonic::operator_::add(std::declval<__type5>(), std::declval<__type10>())) __type11;
-      typedef typename pythonic::assignable<__type11>::type __type12;
-      typedef __type12 __type13;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type3>())) __type15;
-      typedef long __type16;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type17;
-      typedef decltype(std::declval<__type17>()(std::declval<__type3>())) __type19;
-      typedef decltype(std::declval<__type17>()(std::declval<__type7>())) __type21;
-      typedef decltype(pythonic::operator_::add(std::declval<__type19>(), std::declval<__type21>())) __type22;
-      typedef typename pythonic::assignable<__type22>::type __type23;
-      typedef double __type24;
-      typedef container<typename std::remove_reference<__type24>::type> __type25;
-      typedef typename __combined<__type23,__type25>::type __type26;
-      typedef __type26 __type27;
-      typedef decltype(pythonic::operator_::eq(std::declval<__type27>(), std::declval<__type16>())) __type28;
-      typedef indexable<__type28> __type29;
-      typedef typename __combined<__type23,__type29,__type25>::type __type30;
-      typedef __type30 __type31;
-      typedef decltype(pythonic::operator_::div(std::declval<__type16>(), std::declval<__type31>())) __type32;
-      typedef typename pythonic::assignable<__type32>::type __type33;
-      typedef __type33 __type34;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type15>(), std::declval<__type34>())) __type35;
-      typedef typename pythonic::assignable<__type35>::type __type36;
-      typedef __type36 __type37;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type1>(), std::declval<__type37>())) __type38;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type7>())) __type42;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type42>(), std::declval<__type34>())) __type44;
-      typedef typename pythonic::assignable<__type44>::type __type45;
-      typedef __type45 __type46;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type9>(), std::declval<__type46>())) __type47;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type38>(), std::declval<__type47>(), std::declval<__type37>(), std::declval<__type46>())) __type50;
-      typedef typename pythonic::returnable<__type50>::type __type51;
-      typedef __type51 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vx_fft, argument_type3&& vy_fft) const
-    ;
-  }  ;
-  struct compute_energy_from_3fields
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    struct type
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      struct type
+      {
+        typedef std::complex<double> __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
+        typedef __type1 __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type3;
+        typedef double __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type5;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type6;
+        typedef __type6 __type7;
+        typedef decltype(std::declval<__type5>()(std::declval<__type7>())) __type8;
+        typedef decltype(std::declval<__type5>()(std::declval<__type2>())) __type10;
+        typedef decltype(pythonic::operator_::add(std::declval<__type8>(), std::declval<__type10>())) __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef container<typename std::remove_reference<__type4>::type> __type13;
+        typedef typename __combined<__type12,__type13>::type __type14;
+        typedef __type14 __type15;
+        typedef long __type16;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type15>(), std::declval<__type16>())) __type17;
+        typedef indexable<__type17> __type18;
+        typedef typename __combined<__type12,__type18,__type13>::type __type19;
+        typedef __type19 __type20;
+        typedef decltype(pythonic::operator_::div(std::declval<__type4>(), std::declval<__type20>())) __type21;
+        typedef decltype(std::declval<__type3>()(std::declval<__type21>())) __type22;
+        typedef typename pythonic::assignable<__type22>::type __type23;
+        typedef __type23 __type24;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type2>(), std::declval<__type24>())) __type25;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type25>())) __type26;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type27;
+        typedef __type27 __type28;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type26>(), std::declval<__type28>())) __type29;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type24>())) __type32;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type32>())) __type33;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type34;
+        typedef __type34 __type35;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type33>(), std::declval<__type35>())) __type36;
+        typedef decltype(pythonic::operator_::add(std::declval<__type29>(), std::declval<__type36>())) __type37;
+        typedef typename pythonic::returnable<__type37>::type __type38;
+        typedef __type38 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vx_fft, argument_type3 vy_fft, argument_type4 vz_fft) const
+      ;
+    }  ;
+    struct __code_new_method__OperatorsPseudoSpectral3D__project_toroidal
     {
-      typedef double __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::abssqr{})>::type>::type __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef decltype(std::declval<__type1>()(std::declval<__type3>())) __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef decltype(std::declval<__type1>()(std::declval<__type6>())) __type7;
-      typedef decltype(pythonic::operator_::add(std::declval<__type4>(), std::declval<__type7>())) __type8;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type9;
-      typedef __type9 __type10;
-      typedef decltype(std::declval<__type1>()(std::declval<__type10>())) __type11;
-      typedef decltype(pythonic::operator_::add(std::declval<__type8>(), std::declval<__type11>())) __type12;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type12>())) __type13;
-      typedef typename pythonic::returnable<__type13>::type __type14;
-      typedef __type14 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0&& vx, argument_type1&& vy, argument_type2&& vz) const
-    ;
-  }  ;
-  struct compute_energy_from_2fields
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 >
-    struct type
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct __for_method__OperatorsPseudoSpectral3D__project_toroidal
     {
-      typedef double __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::abssqr{})>::type>::type __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef decltype(std::declval<__type1>()(std::declval<__type3>())) __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef decltype(std::declval<__type1>()(std::declval<__type6>())) __type7;
-      typedef decltype(pythonic::operator_::add(std::declval<__type4>(), std::declval<__type7>())) __type8;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type8>())) __type9;
-      typedef typename pythonic::returnable<__type9>::type __type10;
-      typedef __type10 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 >
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type2;
+        typedef double __type3;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
+        typedef decltype(std::declval<__type4>()(std::declval<__type1>())) __type9;
+        typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type9>())) __type10;
+        typedef typename pythonic::assignable<__type10>::type __type11;
+        typedef container<typename std::remove_reference<__type3>::type> __type12;
+        typedef typename __combined<__type11,__type12>::type __type13;
+        typedef __type13 __type14;
+        typedef long __type15;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type14>(), std::declval<__type15>())) __type16;
+        typedef indexable<__type16> __type17;
+        typedef typename __combined<__type11,__type17,__type12>::type __type18;
+        typedef __type18 __type19;
+        typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type19>())) __type20;
+        typedef decltype(std::declval<__type2>()(std::declval<__type20>())) __type21;
+        typedef typename pythonic::assignable<__type21>::type __type22;
+        typedef __type22 __type23;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type23>())) __type24;
+        typedef typename pythonic::assignable<__type24>::type __type25;
+        typedef __type25 __type26;
+        typedef decltype(pythonic::types::as_const(std::declval<__type26>())) __type27;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type28;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type29;
+        typedef __type29 __type30;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type30>())) __type31;
+        typedef decltype(pythonic::types::as_const(std::declval<__type31>())) __type32;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type32>::type>::type __type33;
+        typedef typename pythonic::lazy<__type33>::type __type34;
+        typedef __type34 __type35;
+        typedef decltype(std::declval<__type28>()(std::declval<__type35>())) __type36;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type36>::type::iterator>::value_type>::type __type37;
+        typedef __type37 __type38;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type32>::type>::type __type39;
+        typedef typename pythonic::lazy<__type39>::type __type40;
+        typedef __type40 __type41;
+        typedef decltype(std::declval<__type28>()(std::declval<__type41>())) __type42;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type42>::type::iterator>::value_type>::type __type43;
+        typedef __type43 __type44;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type32>::type>::type __type45;
+        typedef typename pythonic::lazy<__type45>::type __type46;
+        typedef __type46 __type47;
+        typedef decltype(std::declval<__type28>()(std::declval<__type47>())) __type48;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type48>::type::iterator>::value_type>::type __type49;
+        typedef __type49 __type50;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type38>(), std::declval<__type44>(), std::declval<__type50>())) __type51;
+        typedef decltype(std::declval<__type27>()[std::declval<__type51>()]) __type52;
+        typedef decltype(pythonic::operator_::neg(std::declval<__type52>())) __type53;
+        typedef decltype(pythonic::operator_::neg(std::declval<__type26>())) __type55;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type55>(), std::declval<__type30>())) __type57;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type23>())) __type60;
+        typedef typename pythonic::assignable<__type60>::type __type61;
+        typedef __type61 __type62;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type63;
+        typedef decltype(pythonic::types::as_const(std::declval<__type62>())) __type65;
+        typedef decltype(std::declval<__type65>()[std::declval<__type51>()]) __type70;
+        typedef __type63 __type71;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type62>(), std::declval<__type71>())) __type72;
+        typedef decltype(pythonic::operator_::add(std::declval<__type57>(), std::declval<__type72>())) __type73;
+        typedef typename pythonic::assignable<__type73>::type __type74;
+        typedef __type74 __type75;
+        typedef decltype(pythonic::types::as_const(std::declval<__type75>())) __type76;
+        typedef decltype(std::declval<__type76>()[std::declval<__type51>()]) __type81;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type70>(), std::declval<__type81>())) __type82;
+        typedef container<typename std::remove_reference<__type82>::type> __type83;
+        typedef indexable<__type51> __type88;
+        typedef typename __combined<__type63,__type83,__type88>::type __type89;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type53>(), std::declval<__type81>())) __type97;
+        typedef container<typename std::remove_reference<__type97>::type> __type98;
+        typedef typename __combined<__type29,__type98,__type88>::type __type104;
+        typedef __type97 __type105;
+        typedef __type51 __type106;
+        typedef __type82 __type107;
+        typedef __type3 __type109;
+        typedef pythonic::types::none_type __type115;
+        typedef typename pythonic::returnable<__type115>::type __type116;
+        typedef __type105 __ptype0;
+        typedef __type106 __ptype1;
+        typedef __type107 __ptype4;
+        typedef __type106 __ptype5;
+        typedef __type109 __ptype8;
+        typedef __type106 __ptype9;
+        typedef __type116 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vx_fft, argument_type3 vy_fft, argument_type4 vz_fft) const
+      ;
+    }  ;
+    struct __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct __for_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type2;
+        typedef double __type3;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type8;
+        typedef __type8 __type9;
+        typedef decltype(std::declval<__type4>()(std::declval<__type9>())) __type10;
+        typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef __type12 __type13;
+        typedef decltype(std::declval<__type4>()(std::declval<__type1>())) __type15;
+        typedef decltype(pythonic::operator_::add(std::declval<__type13>(), std::declval<__type15>())) __type16;
+        typedef typename pythonic::assignable<__type16>::type __type17;
+        typedef container<typename std::remove_reference<__type3>::type> __type18;
+        typedef typename __combined<__type17,__type18>::type __type19;
+        typedef __type19 __type20;
+        typedef long __type21;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type20>(), std::declval<__type21>())) __type22;
+        typedef indexable<__type22> __type23;
+        typedef typename __combined<__type17,__type23,__type18>::type __type24;
+        typedef __type24 __type25;
+        typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type25>())) __type26;
+        typedef typename pythonic::assignable<__type26>::type __type27;
+        typedef __type27 __type28;
+        typedef decltype(std::declval<__type2>()(std::declval<__type28>())) __type29;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type29>())) __type30;
+        typedef typename pythonic::assignable<__type30>::type __type31;
+        typedef __type31 __type32;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type34;
+        typedef decltype(std::declval<__type34>()(std::declval<__type13>())) __type36;
+        typedef typename pythonic::assignable<__type36>::type __type37;
+        typedef typename __combined<__type37,__type18>::type __type38;
+        typedef __type38 __type39;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type39>(), std::declval<__type21>())) __type40;
+        typedef indexable<__type40> __type41;
+        typedef typename __combined<__type37,__type41,__type18>::type __type42;
+        typedef __type42 __type43;
+        typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type43>())) __type44;
+        typedef typename pythonic::assignable<__type44>::type __type45;
+        typedef __type45 __type46;
+        typedef decltype(std::declval<__type2>()(std::declval<__type46>())) __type47;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type47>())) __type48;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type48>())) __type49;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type50;
+        typedef __type50 __type51;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type49>(), std::declval<__type51>())) __type52;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type9>(), std::declval<__type47>())) __type57;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type57>())) __type58;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type58>(), std::declval<__type51>())) __type60;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type28>())) __type63;
+        typedef decltype(std::declval<__type2>()(std::declval<__type63>())) __type64;
+        typedef decltype(pythonic::operator_::neg(std::declval<__type64>())) __type65;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type65>(), std::declval<__type51>())) __type67;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type52>(), std::declval<__type60>(), std::declval<__type67>())) __type68;
+        typedef typename pythonic::returnable<__type68>::type __type69;
+        typedef __type69 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 vp_fft) const
+      ;
+    }  ;
+    struct __code_new_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct __for_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type2;
+        typedef double __type3;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type8;
+        typedef __type8 __type9;
+        typedef decltype(std::declval<__type4>()(std::declval<__type9>())) __type10;
+        typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef __type12 __type13;
+        typedef decltype(std::declval<__type4>()(std::declval<__type1>())) __type15;
+        typedef decltype(pythonic::operator_::add(std::declval<__type13>(), std::declval<__type15>())) __type16;
+        typedef typename pythonic::assignable<__type16>::type __type17;
+        typedef container<typename std::remove_reference<__type3>::type> __type18;
+        typedef typename __combined<__type17,__type18>::type __type19;
+        typedef __type19 __type20;
+        typedef long __type21;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type20>(), std::declval<__type21>())) __type22;
+        typedef indexable<__type22> __type23;
+        typedef typename __combined<__type17,__type23,__type18>::type __type24;
+        typedef __type24 __type25;
+        typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type25>())) __type26;
+        typedef typename pythonic::assignable<__type26>::type __type27;
+        typedef __type27 __type28;
+        typedef decltype(std::declval<__type2>()(std::declval<__type28>())) __type29;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type29>())) __type30;
+        typedef typename pythonic::assignable<__type30>::type __type31;
+        typedef __type31 __type32;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type34;
+        typedef decltype(std::declval<__type34>()(std::declval<__type13>())) __type36;
+        typedef typename pythonic::assignable<__type36>::type __type37;
+        typedef typename __combined<__type37,__type18>::type __type38;
+        typedef __type38 __type39;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type39>(), std::declval<__type21>())) __type40;
+        typedef indexable<__type40> __type41;
+        typedef typename __combined<__type37,__type41,__type18>::type __type42;
+        typedef __type42 __type43;
+        typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type43>())) __type44;
+        typedef typename pythonic::assignable<__type44>::type __type45;
+        typedef __type45 __type46;
+        typedef decltype(std::declval<__type2>()(std::declval<__type46>())) __type47;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type47>())) __type48;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type48>())) __type49;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type50;
+        typedef __type50 __type51;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type49>(), std::declval<__type51>())) __type52;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type9>(), std::declval<__type47>())) __type57;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type57>())) __type58;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type59;
+        typedef __type59 __type60;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type58>(), std::declval<__type60>())) __type61;
+        typedef decltype(pythonic::operator_::add(std::declval<__type52>(), std::declval<__type61>())) __type62;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type28>())) __type65;
+        typedef decltype(std::declval<__type2>()(std::declval<__type65>())) __type66;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type67;
+        typedef __type67 __type68;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type66>(), std::declval<__type68>())) __type69;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type62>(), std::declval<__type69>())) __type70;
+        typedef typename pythonic::returnable<__type70>::type __type71;
+        typedef __type71 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 vx_fft, argument_type4 vy_fft, argument_type5 vz_fft) const
+      ;
+    }  ;
+    struct __code_new_method__OperatorsPseudoSpectral3D__project_poloidal
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct __for_method__OperatorsPseudoSpectral3D__project_poloidal
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::sqrt{})>::type>::type __type2;
+        typedef double __type3;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type8;
+        typedef __type8 __type9;
+        typedef decltype(std::declval<__type4>()(std::declval<__type9>())) __type10;
+        typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef __type12 __type13;
+        typedef decltype(std::declval<__type4>()(std::declval<__type1>())) __type15;
+        typedef decltype(pythonic::operator_::add(std::declval<__type13>(), std::declval<__type15>())) __type16;
+        typedef typename pythonic::assignable<__type16>::type __type17;
+        typedef container<typename std::remove_reference<__type3>::type> __type18;
+        typedef typename __combined<__type17,__type18>::type __type19;
+        typedef __type19 __type20;
+        typedef long __type21;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type20>(), std::declval<__type21>())) __type22;
+        typedef indexable<__type22> __type23;
+        typedef typename __combined<__type17,__type23,__type18>::type __type24;
+        typedef __type24 __type25;
+        typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type25>())) __type26;
+        typedef typename pythonic::assignable<__type26>::type __type27;
+        typedef __type27 __type28;
+        typedef decltype(std::declval<__type2>()(std::declval<__type28>())) __type29;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type29>())) __type30;
+        typedef typename pythonic::assignable<__type30>::type __type31;
+        typedef __type31 __type32;
+        typedef decltype(pythonic::types::as_const(std::declval<__type32>())) __type33;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type34;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type35;
+        typedef __type35 __type36;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type36>())) __type37;
+        typedef decltype(pythonic::types::as_const(std::declval<__type37>())) __type38;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type38>::type>::type __type39;
+        typedef typename pythonic::lazy<__type39>::type __type40;
+        typedef __type40 __type41;
+        typedef decltype(std::declval<__type34>()(std::declval<__type41>())) __type42;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type42>::type::iterator>::value_type>::type __type43;
+        typedef __type43 __type44;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type38>::type>::type __type45;
+        typedef typename pythonic::lazy<__type45>::type __type46;
+        typedef __type46 __type47;
+        typedef decltype(std::declval<__type34>()(std::declval<__type47>())) __type48;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type48>::type::iterator>::value_type>::type __type49;
+        typedef __type49 __type50;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type38>::type>::type __type51;
+        typedef typename pythonic::lazy<__type51>::type __type52;
+        typedef __type52 __type53;
+        typedef decltype(std::declval<__type34>()(std::declval<__type53>())) __type54;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type54>::type::iterator>::value_type>::type __type55;
+        typedef __type55 __type56;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type44>(), std::declval<__type50>(), std::declval<__type56>())) __type57;
+        typedef decltype(std::declval<__type33>()[std::declval<__type57>()]) __type58;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type60;
+        typedef decltype(std::declval<__type60>()(std::declval<__type13>())) __type62;
+        typedef typename pythonic::assignable<__type62>::type __type63;
+        typedef typename __combined<__type63,__type18>::type __type64;
+        typedef __type64 __type65;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type65>(), std::declval<__type21>())) __type66;
+        typedef indexable<__type66> __type67;
+        typedef typename __combined<__type63,__type67,__type18>::type __type68;
+        typedef __type68 __type69;
+        typedef decltype(pythonic::operator_::div(std::declval<__type3>(), std::declval<__type69>())) __type70;
+        typedef typename pythonic::assignable<__type70>::type __type71;
+        typedef __type71 __type72;
+        typedef decltype(std::declval<__type2>()(std::declval<__type72>())) __type73;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type73>())) __type74;
+        typedef typename pythonic::assignable<__type74>::type __type75;
+        typedef __type75 __type76;
+        typedef decltype(pythonic::types::as_const(std::declval<__type76>())) __type77;
+        typedef decltype(std::declval<__type77>()[std::declval<__type57>()]) __type82;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type58>(), std::declval<__type82>())) __type83;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type76>())) __type86;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type86>(), std::declval<__type36>())) __type88;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type9>(), std::declval<__type73>())) __type93;
+        typedef typename pythonic::assignable<__type93>::type __type94;
+        typedef __type94 __type95;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type95>())) __type96;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type97;
+        typedef decltype(pythonic::types::as_const(std::declval<__type95>())) __type106;
+        typedef decltype(std::declval<__type106>()[std::declval<__type57>()]) __type111;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type58>(), std::declval<__type111>())) __type112;
+        typedef __type97 __type113;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type96>(), std::declval<__type113>())) __type114;
+        typedef decltype(pythonic::operator_::add(std::declval<__type88>(), std::declval<__type114>())) __type115;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type28>())) __type118;
+        typedef decltype(std::declval<__type2>()(std::declval<__type118>())) __type119;
+        typedef typename pythonic::assignable<__type119>::type __type120;
+        typedef __type120 __type121;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type122;
+        typedef decltype(pythonic::types::as_const(std::declval<__type121>())) __type124;
+        typedef decltype(std::declval<__type124>()[std::declval<__type57>()]) __type129;
+        typedef decltype(pythonic::operator_::neg(std::declval<__type129>())) __type130;
+        typedef __type122 __type131;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type121>(), std::declval<__type131>())) __type132;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type115>(), std::declval<__type132>())) __type133;
+        typedef typename pythonic::assignable<__type133>::type __type134;
+        typedef __type134 __type135;
+        typedef decltype(pythonic::types::as_const(std::declval<__type135>())) __type136;
+        typedef decltype(std::declval<__type136>()[std::declval<__type57>()]) __type141;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type130>(), std::declval<__type141>())) __type142;
+        typedef container<typename std::remove_reference<__type142>::type> __type143;
+        typedef indexable<__type57> __type148;
+        typedef typename __combined<__type122,__type143,__type148>::type __type149;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type112>(), std::declval<__type141>())) __type157;
+        typedef container<typename std::remove_reference<__type157>::type> __type158;
+        typedef typename __combined<__type97,__type158,__type148>::type __type164;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type83>(), std::declval<__type141>())) __type172;
+        typedef container<typename std::remove_reference<__type172>::type> __type173;
+        typedef typename __combined<__type35,__type173,__type148>::type __type179;
+        typedef __type172 __type180;
+        typedef __type57 __type181;
+        typedef __type157 __type182;
+        typedef __type142 __type184;
+        typedef pythonic::types::none_type __type186;
+        typedef typename pythonic::returnable<__type186>::type __type187;
+        typedef __type180 __ptype12;
+        typedef __type181 __ptype13;
+        typedef __type182 __ptype16;
+        typedef __type181 __ptype17;
+        typedef __type184 __ptype20;
+        typedef __type181 __ptype21;
+        typedef __type187 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 vx_fft, argument_type4 vy_fft, argument_type5 vz_fft) const
+      ;
+    }  ;
+    struct __code_new_method__OperatorsPseudoSpectral3D__project_kradial3d
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct __for_method__OperatorsPseudoSpectral3D__project_kradial3d
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef decltype(pythonic::types::as_const(std::declval<__type1>())) __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type3;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type4;
+        typedef __type4 __type5;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
+        typedef decltype(pythonic::types::as_const(std::declval<__type6>())) __type7;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type7>::type>::type __type8;
+        typedef typename pythonic::lazy<__type8>::type __type9;
+        typedef __type9 __type10;
+        typedef decltype(std::declval<__type3>()(std::declval<__type10>())) __type11;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type11>::type::iterator>::value_type>::type __type12;
+        typedef __type12 __type13;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type7>::type>::type __type14;
+        typedef typename pythonic::lazy<__type14>::type __type15;
+        typedef __type15 __type16;
+        typedef decltype(std::declval<__type3>()(std::declval<__type16>())) __type17;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type17>::type::iterator>::value_type>::type __type18;
+        typedef __type18 __type19;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type7>::type>::type __type20;
+        typedef typename pythonic::lazy<__type20>::type __type21;
+        typedef __type21 __type22;
+        typedef decltype(std::declval<__type3>()(std::declval<__type22>())) __type23;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type23>::type::iterator>::value_type>::type __type24;
+        typedef __type24 __type25;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type13>(), std::declval<__type19>(), std::declval<__type25>())) __type26;
+        typedef decltype(std::declval<__type2>()[std::declval<__type26>()]) __type27;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type5>())) __type30;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type31;
+        typedef __type31 __type32;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type33;
+        typedef decltype(pythonic::types::as_const(std::declval<__type32>())) __type35;
+        typedef decltype(std::declval<__type35>()[std::declval<__type26>()]) __type40;
+        typedef __type33 __type41;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type32>(), std::declval<__type41>())) __type42;
+        typedef decltype(pythonic::operator_::add(std::declval<__type30>(), std::declval<__type42>())) __type43;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type44;
+        typedef __type44 __type45;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type46;
+        typedef decltype(pythonic::types::as_const(std::declval<__type45>())) __type48;
+        typedef decltype(std::declval<__type48>()[std::declval<__type26>()]) __type53;
+        typedef __type46 __type54;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type45>(), std::declval<__type54>())) __type55;
+        typedef decltype(pythonic::operator_::add(std::declval<__type43>(), std::declval<__type55>())) __type56;
+        typedef double __type57;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type58;
+        typedef decltype(std::declval<__type58>()(std::declval<__type1>())) __type60;
+        typedef decltype(std::declval<__type58>()(std::declval<__type32>())) __type62;
+        typedef decltype(pythonic::operator_::add(std::declval<__type60>(), std::declval<__type62>())) __type63;
+        typedef decltype(std::declval<__type58>()(std::declval<__type45>())) __type65;
+        typedef decltype(pythonic::operator_::add(std::declval<__type63>(), std::declval<__type65>())) __type66;
+        typedef typename pythonic::assignable<__type66>::type __type67;
+        typedef container<typename std::remove_reference<__type57>::type> __type68;
+        typedef typename __combined<__type67,__type68>::type __type69;
+        typedef __type69 __type70;
+        typedef long __type71;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type70>(), std::declval<__type71>())) __type72;
+        typedef indexable<__type72> __type73;
+        typedef typename __combined<__type67,__type73,__type68>::type __type74;
+        typedef __type74 __type75;
+        typedef decltype(pythonic::operator_::div(std::declval<__type57>(), std::declval<__type75>())) __type76;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type56>(), std::declval<__type76>())) __type77;
+        typedef typename pythonic::assignable<__type77>::type __type78;
+        typedef __type78 __type79;
+        typedef decltype(pythonic::types::as_const(std::declval<__type79>())) __type80;
+        typedef decltype(std::declval<__type80>()[std::declval<__type26>()]) __type85;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type53>(), std::declval<__type85>())) __type86;
+        typedef container<typename std::remove_reference<__type86>::type> __type87;
+        typedef indexable<__type26> __type92;
+        typedef typename __combined<__type46,__type87,__type92>::type __type93;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type40>(), std::declval<__type85>())) __type101;
+        typedef container<typename std::remove_reference<__type101>::type> __type102;
+        typedef typename __combined<__type33,__type102,__type92>::type __type108;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type27>(), std::declval<__type85>())) __type116;
+        typedef container<typename std::remove_reference<__type116>::type> __type117;
+        typedef typename __combined<__type4,__type117,__type92>::type __type123;
+        typedef __type116 __type124;
+        typedef __type26 __type125;
+        typedef __type101 __type126;
+        typedef __type86 __type128;
+        typedef pythonic::types::none_type __type130;
+        typedef typename pythonic::returnable<__type130>::type __type131;
+        typedef __type124 __ptype24;
+        typedef __type125 __ptype25;
+        typedef __type126 __ptype28;
+        typedef __type125 __ptype29;
+        typedef __type128 __ptype32;
+        typedef __type125 __ptype33;
+        typedef __type131 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 vx_fft, argument_type4 vy_fft, argument_type5 vz_fft) const
+      ;
+    }  ;
+    struct __code_new_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft
+    {
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef typename pythonic::returnable<__type0>::type __type1;
+        typedef __type1 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct __for_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type2;
+        typedef __type2 __type3;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type1>())) __type5;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type6;
+        typedef __type6 __type7;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type8;
+        typedef __type8 __type9;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type9>())) __type10;
+        typedef decltype(pythonic::operator_::add(std::declval<__type5>(), std::declval<__type10>())) __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef __type12 __type13;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type3>())) __type15;
+        typedef long __type16;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type17;
+        typedef decltype(std::declval<__type17>()(std::declval<__type3>())) __type19;
+        typedef decltype(std::declval<__type17>()(std::declval<__type7>())) __type21;
+        typedef decltype(pythonic::operator_::add(std::declval<__type19>(), std::declval<__type21>())) __type22;
+        typedef typename pythonic::assignable<__type22>::type __type23;
+        typedef double __type24;
+        typedef container<typename std::remove_reference<__type24>::type> __type25;
+        typedef typename __combined<__type23,__type25>::type __type26;
+        typedef __type26 __type27;
+        typedef decltype(pythonic::operator_::eq(std::declval<__type27>(), std::declval<__type16>())) __type28;
+        typedef indexable<__type28> __type29;
+        typedef typename __combined<__type23,__type29,__type25>::type __type30;
+        typedef __type30 __type31;
+        typedef decltype(pythonic::operator_::div(std::declval<__type16>(), std::declval<__type31>())) __type32;
+        typedef typename pythonic::assignable<__type32>::type __type33;
+        typedef __type33 __type34;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type15>(), std::declval<__type34>())) __type35;
+        typedef typename pythonic::assignable<__type35>::type __type36;
+        typedef __type36 __type37;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type1>(), std::declval<__type37>())) __type38;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type7>())) __type42;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type42>(), std::declval<__type34>())) __type44;
+        typedef typename pythonic::assignable<__type44>::type __type45;
+        typedef __type45 __type46;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type9>(), std::declval<__type46>())) __type47;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type38>(), std::declval<__type47>(), std::declval<__type37>(), std::declval<__type46>())) __type50;
+        typedef typename pythonic::returnable<__type50>::type __type51;
+        typedef __type51 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vx_fft, argument_type3 vy_fft) const
+      ;
+    }  ;
+    struct compute_energy_from_3fields
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      struct type
+      {
+        typedef double __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::abssqr{})>::type>::type __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type2;
+        typedef __type2 __type3;
+        typedef decltype(std::declval<__type1>()(std::declval<__type3>())) __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(std::declval<__type1>()(std::declval<__type6>())) __type7;
+        typedef decltype(pythonic::operator_::add(std::declval<__type4>(), std::declval<__type7>())) __type8;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type9;
+        typedef __type9 __type10;
+        typedef decltype(std::declval<__type1>()(std::declval<__type10>())) __type11;
+        typedef decltype(pythonic::operator_::add(std::declval<__type8>(), std::declval<__type11>())) __type12;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type12>())) __type13;
+        typedef typename pythonic::returnable<__type13>::type __type14;
+        typedef __type14 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0 vx, argument_type1 vy, argument_type2 vz) const
+      ;
+    }  ;
+    struct compute_energy_from_2fields
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 >
+      struct type
+      {
+        typedef double __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::abssqr{})>::type>::type __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type2;
+        typedef __type2 __type3;
+        typedef decltype(std::declval<__type1>()(std::declval<__type3>())) __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(std::declval<__type1>()(std::declval<__type6>())) __type7;
+        typedef decltype(pythonic::operator_::add(std::declval<__type4>(), std::declval<__type7>())) __type8;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type8>())) __type9;
+        typedef typename pythonic::returnable<__type9>::type __type10;
+        typedef __type10 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      inline
+      typename type<argument_type0, argument_type1>::result_type operator()(argument_type0 vx, argument_type1 vy) const
+      ;
+    }  ;
+    struct compute_energy_from_1field_with_coef
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 >
+      struct type
+      {
+        typedef double __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
+        typedef __type1 __type2;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type2>())) __type3;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::abssqr{})>::type>::type __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type7>())) __type8;
+        typedef typename pythonic::returnable<__type8>::type __type9;
+        typedef __type9 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      inline
+      typename type<argument_type0, argument_type1>::result_type operator()(argument_type0 arr, argument_type1 coef) const
+      ;
+    }  ;
+    struct compute_energy_from_1field
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 >
+      struct type
+      {
+        typedef double __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::abssqr{})>::type>::type __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type2;
+        typedef __type2 __type3;
+        typedef decltype(std::declval<__type1>()(std::declval<__type3>())) __type4;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type4>())) __type5;
+        typedef typename pythonic::returnable<__type5>::type __type6;
+        typedef __type6 result_type;
+      }  
+      ;
+      template <typename argument_type0 >
+      inline
+      typename type<argument_type0>::result_type operator()(argument_type0 arr) const
+      ;
+    }  ;
+    struct dealiasing_variable
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      struct type
+      {
+        typedef double __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type3;
+        typedef container<typename std::remove_reference<__type0>::type> __type4;
+        typedef __type3 __type5;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
+        typedef decltype(pythonic::types::as_const(std::declval<__type6>())) __type7;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type7>::type>::type __type8;
+        typedef typename pythonic::lazy<__type8>::type __type9;
+        typedef __type9 __type10;
+        typedef decltype(std::declval<__type2>()(std::declval<__type10>())) __type11;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type11>::type::iterator>::value_type>::type __type12;
+        typedef __type12 __type13;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type7>::type>::type __type14;
+        typedef typename pythonic::lazy<__type14>::type __type15;
+        typedef __type15 __type16;
+        typedef decltype(std::declval<__type2>()(std::declval<__type16>())) __type17;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type17>::type::iterator>::value_type>::type __type18;
+        typedef __type18 __type19;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type7>::type>::type __type20;
+        typedef typename pythonic::lazy<__type20>::type __type21;
+        typedef __type21 __type22;
+        typedef decltype(std::declval<__type2>()(std::declval<__type22>())) __type23;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type23>::type::iterator>::value_type>::type __type24;
+        typedef __type24 __type25;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type13>(), std::declval<__type19>(), std::declval<__type25>())) __type26;
+        typedef indexable<__type26> __type27;
+        typedef typename __combined<__type3,__type4,__type27>::type __type28;
+        typedef __type26 __type29;
+        typedef pythonic::types::none_type __type30;
+        typedef typename pythonic::returnable<__type30>::type __type31;
+        typedef __type1 __ptype36;
+        typedef __type29 __ptype37;
+        typedef __type31 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      inline
+      typename type<argument_type0, argument_type1>::result_type operator()(argument_type0 ff_fft, argument_type1 where_dealiased) const
+      ;
+    }  ;
+    struct dealiasing_setofvar
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      struct type
+      {
+        typedef double __type0;
+        typedef __type0 __type1;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type3;
+        typedef container<typename std::remove_reference<__type0>::type> __type4;
+        typedef __type3 __type5;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
+        typedef decltype(pythonic::types::as_const(std::declval<__type6>())) __type7;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type7>::type>::type __type8;
+        typedef typename pythonic::lazy<__type8>::type __type9;
+        typedef __type9 __type10;
+        typedef decltype(std::declval<__type2>()(std::declval<__type10>())) __type11;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type11>::type::iterator>::value_type>::type __type12;
+        typedef __type12 __type13;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type7>::type>::type __type14;
+        typedef typename pythonic::lazy<__type14>::type __type15;
+        typedef __type15 __type16;
+        typedef decltype(std::declval<__type2>()(std::declval<__type16>())) __type17;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type17>::type::iterator>::value_type>::type __type18;
+        typedef __type18 __type19;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type7>::type>::type __type20;
+        typedef typename pythonic::lazy<__type20>::type __type21;
+        typedef __type21 __type22;
+        typedef decltype(std::declval<__type2>()(std::declval<__type22>())) __type23;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type23>::type::iterator>::value_type>::type __type24;
+        typedef __type24 __type25;
+        typedef typename std::tuple_element<3,typename std::remove_reference<__type7>::type>::type __type26;
+        typedef typename pythonic::lazy<__type26>::type __type27;
+        typedef __type27 __type28;
+        typedef decltype(std::declval<__type2>()(std::declval<__type28>())) __type29;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type29>::type::iterator>::value_type>::type __type30;
+        typedef __type30 __type31;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type13>(), std::declval<__type19>(), std::declval<__type25>(), std::declval<__type31>())) __type32;
+        typedef indexable<__type32> __type33;
+        typedef typename __combined<__type3,__type4,__type33>::type __type34;
+        typedef __type32 __type35;
+        typedef pythonic::types::none_type __type36;
+        typedef typename pythonic::returnable<__type36>::type __type37;
+        typedef __type1 __ptype40;
+        typedef __type35 __ptype41;
+        typedef __type37 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      inline
+      typename type<argument_type0, argument_type1>::result_type operator()(argument_type0 sov, argument_type1 where_dealiased) const
+      ;
+    }  ;
+    struct __for_method__OperatorsPseudoSpectral3D__get_phases_random
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::tuple{})>::type>::type __type0;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::map{})>::type>::type __type1;
+        typedef __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0 __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type3;
+        typedef long __type4;
+        typedef decltype(std::declval<__type3>()(std::declval<__type4>())) __type5;
+        typedef decltype(std::declval<__type1>()(std::declval<__type2>(), std::declval<__type5>())) __type6;
+        typedef decltype(std::declval<__type0>()(std::declval<__type6>())) __type7;
+        typedef typename pythonic::assignable<__type7>::type __type8;
+        typedef __type8 __type9;
+        typedef decltype(pythonic::types::as_const(std::declval<__type9>())) __type10;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type10>::type>::type __type11;
+        typedef typename pythonic::assignable<__type11>::type __type12;
+        typedef __type12 __type13;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type14;
+        typedef __type14 __type15;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type13>(), std::declval<__type15>())) __type16;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type17;
+        typedef __type17 __type18;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type16>(), std::declval<__type18>())) __type19;
+        typedef std::integral_constant<long,0> __type20;
+        typedef indexable_container<__type20, typename std::remove_reference<__type11>::type> __type21;
+        typedef typename __combined<__type8,__type21>::type __type22;
+        typedef __type22 __type23;
+        typedef decltype(pythonic::types::as_const(std::declval<__type23>())) __type24;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type24>::type>::type __type25;
+        typedef typename pythonic::assignable<__type25>::type __type26;
+        typedef __type26 __type27;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type28;
+        typedef __type28 __type29;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type27>(), std::declval<__type29>())) __type30;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type31;
+        typedef __type31 __type32;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type30>(), std::declval<__type32>())) __type33;
+        typedef decltype(pythonic::operator_::add(std::declval<__type19>(), std::declval<__type33>())) __type34;
+        typedef std::integral_constant<long,1> __type35;
+        typedef indexable_container<__type35, typename std::remove_reference<__type25>::type> __type36;
+        typedef typename __combined<__type8,__type21,__type36>::type __type37;
+        typedef __type37 __type38;
+        typedef decltype(pythonic::types::as_const(std::declval<__type38>())) __type39;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type39>::type>::type __type40;
+        typedef typename pythonic::assignable<__type40>::type __type41;
+        typedef __type41 __type42;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type43;
+        typedef __type43 __type44;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type42>(), std::declval<__type44>())) __type45;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type46;
+        typedef __type46 __type47;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type45>(), std::declval<__type47>())) __type48;
+        typedef decltype(pythonic::operator_::add(std::declval<__type34>(), std::declval<__type48>())) __type49;
+        typedef double __type51;
+        typedef decltype(pythonic::operator_::add(std::declval<__type13>(), std::declval<__type51>())) __type52;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type13>(), std::declval<__type51>())) __type54;
+        typedef typename __combined<__type52,__type54>::type __type55;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type55>(), std::declval<__type15>())) __type57;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type57>(), std::declval<__type18>())) __type59;
+        typedef decltype(pythonic::operator_::add(std::declval<__type27>(), std::declval<__type51>())) __type61;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type27>(), std::declval<__type51>())) __type63;
+        typedef typename __combined<__type61,__type63>::type __type64;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type64>(), std::declval<__type29>())) __type66;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type66>(), std::declval<__type32>())) __type68;
+        typedef decltype(pythonic::operator_::add(std::declval<__type59>(), std::declval<__type68>())) __type69;
+        typedef decltype(pythonic::operator_::add(std::declval<__type42>(), std::declval<__type51>())) __type71;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type42>(), std::declval<__type51>())) __type73;
+        typedef typename __combined<__type71,__type73>::type __type74;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type74>(), std::declval<__type44>())) __type76;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type76>(), std::declval<__type47>())) __type78;
+        typedef decltype(pythonic::operator_::add(std::declval<__type69>(), std::declval<__type78>())) __type79;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type49>(), std::declval<__type79>())) __type80;
+        typedef typename pythonic::returnable<__type80>::type __type81;
+        typedef __type81 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 self_deltax, argument_type4 self_deltay, argument_type5 self_deltaz) const
+      ;
+    }  ;
+    template <typename argument_type0 >
     inline
-    typename type<argument_type0, argument_type1>::result_type operator()(argument_type0&& vx, argument_type1&& vy) const
-    ;
-  }  ;
-  struct compute_energy_from_1field_with_coef
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 >
-    struct type
+    typename __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0::type<argument_type0>::result_type __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0::operator()(argument_type0 _) const
     {
-      typedef double __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type1;
-      typedef __type1 __type2;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type2>())) __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::abssqr{})>::type>::type __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef decltype(std::declval<__type4>()(std::declval<__type6>())) __type7;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type3>(), std::declval<__type7>())) __type8;
-      typedef typename pythonic::returnable<__type8>::type __type9;
-      typedef __type9 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 >
+      return pythonic::random::functor::uniform{}(-0.5, 0.5);
+    }
     inline
-    typename type<argument_type0, argument_type1>::result_type operator()(argument_type0&& arr, argument_type1&& coef) const
-    ;
-  }  ;
-  struct compute_energy_from_1field
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 >
-    struct type
+    typename __transonic__::type::result_type __transonic__::operator()() const
     {
-      typedef double __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::abssqr{})>::type>::type __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef decltype(std::declval<__type1>()(std::declval<__type3>())) __type4;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type0>(), std::declval<__type4>())) __type5;
-      typedef typename pythonic::returnable<__type5>::type __type6;
-      typedef __type6 result_type;
-    }  
-    ;
-    template <typename argument_type0 >
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
+    }
     inline
-    typename type<argument_type0>::result_type operator()(argument_type0&& arr) const
-    ;
-  }  ;
-  struct dealiasing_variable
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 >
-    struct type
+    typename __code_new_method__OperatorsPseudoSpectral3D__get_phases_random::type::result_type __code_new_method__OperatorsPseudoSpectral3D__get_phases_random::operator()() const
     {
-      typedef double __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type3;
-      typedef container<typename std::remove_reference<__type0>::type> __type4;
-      typedef __type3 __type5;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type6>::type>::type __type7;
-      typedef typename pythonic::lazy<__type7>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(std::declval<__type2>()(std::declval<__type9>())) __type10;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type10>::type::iterator>::value_type>::type __type11;
-      typedef __type11 __type12;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type6>::type>::type __type13;
-      typedef typename pythonic::lazy<__type13>::type __type14;
-      typedef __type14 __type15;
-      typedef decltype(std::declval<__type2>()(std::declval<__type15>())) __type16;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type16>::type::iterator>::value_type>::type __type17;
-      typedef __type17 __type18;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type6>::type>::type __type19;
-      typedef typename pythonic::lazy<__type19>::type __type20;
-      typedef __type20 __type21;
-      typedef decltype(std::declval<__type2>()(std::declval<__type21>())) __type22;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type22>::type::iterator>::value_type>::type __type23;
-      typedef __type23 __type24;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type12>(), std::declval<__type18>(), std::declval<__type24>())) __type25;
-      typedef indexable<__type25> __type26;
-      typedef typename __combined<__type3,__type4,__type26>::type __type27;
-      typedef __type25 __type28;
-      typedef pythonic::types::none_type __type29;
-      typedef typename pythonic::returnable<__type29>::type __type30;
-      typedef __type1 __ptype36;
-      typedef __type28 __ptype37;
-      typedef __type30 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 >
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__get_phases_random::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, ):\n    return backend_func(self.Kx, self.Ky, self.Kz, self.deltax, self.deltay, self.deltaz, )\n\n");
+        return tmp_global;
+      }
+    }
     inline
-    typename type<argument_type0, argument_type1>::result_type operator()(argument_type0&& ff_fft, argument_type1&& where_dealiased) const
-    ;
-  }  ;
-  struct dealiasing_setofvar
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 >
-    struct type
+    typename __code_new_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::operator()() const
     {
-      typedef double __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type3;
-      typedef container<typename std::remove_reference<__type0>::type> __type4;
-      typedef __type3 __type5;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type6>::type>::type __type7;
-      typedef typename pythonic::lazy<__type7>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(std::declval<__type2>()(std::declval<__type9>())) __type10;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type10>::type::iterator>::value_type>::type __type11;
-      typedef __type11 __type12;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type6>::type>::type __type13;
-      typedef typename pythonic::lazy<__type13>::type __type14;
-      typedef __type14 __type15;
-      typedef decltype(std::declval<__type2>()(std::declval<__type15>())) __type16;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type16>::type::iterator>::value_type>::type __type17;
-      typedef __type17 __type18;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type6>::type>::type __type19;
-      typedef typename pythonic::lazy<__type19>::type __type20;
-      typedef __type20 __type21;
-      typedef decltype(std::declval<__type2>()(std::declval<__type21>())) __type22;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type22>::type::iterator>::value_type>::type __type23;
-      typedef __type23 __type24;
-      typedef typename std::tuple_element<3,typename std::remove_reference<__type6>::type>::type __type25;
-      typedef typename pythonic::lazy<__type25>::type __type26;
-      typedef __type26 __type27;
-      typedef decltype(std::declval<__type2>()(std::declval<__type27>())) __type28;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type28>::type::iterator>::value_type>::type __type29;
-      typedef __type29 __type30;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type12>(), std::declval<__type18>(), std::declval<__type24>(), std::declval<__type30>())) __type31;
-      typedef indexable<__type31> __type32;
-      typedef typename __combined<__type3,__type4,__type32>::type __type33;
-      typedef __type31 __type34;
-      typedef pythonic::types::none_type __type35;
-      typedef typename pythonic::returnable<__type35>::type __type36;
-      typedef __type1 __ptype40;
-      typedef __type34 __ptype41;
-      typedef __type36 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 >
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, arr_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, arr_fft)\n\n");
+        return tmp_global;
+      }
+    }
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
     inline
-    typename type<argument_type0, argument_type1>::result_type operator()(argument_type0&& sov, argument_type1&& where_dealiased) const
-    ;
-  }  ;
-  struct __for_method__OperatorsPseudoSpectral3D__get_phases_random
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    struct type
+    typename __for_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 arr_fft) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::tuple{})>::type>::type __type0;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::map{})>::type>::type __type1;
-      typedef __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0 __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type3;
-      typedef long __type4;
-      typedef decltype(std::declval<__type3>()(std::declval<__type4>())) __type5;
-      typedef decltype(std::declval<__type1>()(std::declval<__type2>(), std::declval<__type5>())) __type6;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::ravel{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::empty_like{})>::type>::type __type1;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type2;
+      typedef __type2 __type3;
+      typedef decltype(std::declval<__type1>()(std::declval<__type3>())) __type4;
+      typedef typename pythonic::assignable<__type4>::type __type5;
+      typedef __type5 __type6;
       typedef decltype(std::declval<__type0>()(std::declval<__type6>())) __type7;
       typedef typename pythonic::assignable<__type7>::type __type8;
-      typedef __type8 __type9;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type9>::type>::type __type10;
-      typedef typename pythonic::assignable<__type10>::type __type11;
-      typedef __type11 __type12;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type13;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type9;
+      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::FLAT{}, std::declval<__type3>())) __type11;
+      typedef decltype(std::declval<__type9>()(std::declval<__type11>())) __type12;
+      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type12>::type::iterator>::value_type>::type __type13;
       typedef __type13 __type14;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type12>(), std::declval<__type14>())) __type15;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type16;
-      typedef __type16 __type17;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type15>(), std::declval<__type17>())) __type18;
-      typedef std::integral_constant<long,0> __type19;
-      typedef indexable_container<__type19, typename std::remove_reference<__type10>::type> __type20;
-      typedef typename __combined<__type8,__type20>::type __type21;
+      typedef decltype(pythonic::types::as_const(std::declval<__type14>())) __type15;
+      typedef typename std::tuple_element<0,typename std::remove_reference<__type15>::type>::type __type16;
+      typedef typename pythonic::assignable<__type16>::type __type17;
+      typedef __type17 __type18;
+      typedef indexable<__type18> __type19;
+      typedef std::complex<double> __type20;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type21;
       typedef __type21 __type22;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type22>::type>::type __type23;
+      typedef decltype(std::declval<__type0>()(std::declval<__type22>())) __type23;
       typedef typename pythonic::assignable<__type23>::type __type24;
       typedef __type24 __type25;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type26;
-      typedef __type26 __type27;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type25>(), std::declval<__type27>())) __type28;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type29;
-      typedef __type29 __type30;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type28>(), std::declval<__type30>())) __type31;
-      typedef decltype(pythonic::operator_::add(std::declval<__type18>(), std::declval<__type31>())) __type32;
-      typedef std::integral_constant<long,1> __type33;
-      typedef indexable_container<__type33, typename std::remove_reference<__type23>::type> __type34;
-      typedef typename __combined<__type8,__type20,__type34>::type __type35;
-      typedef __type35 __type36;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type36>::type>::type __type37;
+      typedef decltype(pythonic::types::as_const(std::declval<__type25>())) __type26;
+      typedef decltype(std::declval<__type26>()[std::declval<__type18>()]) __type28;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type20>(), std::declval<__type28>())) __type29;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type15>::type>::type __type32;
+      typedef typename pythonic::assignable<__type32>::type __type33;
+      typedef __type33 __type34;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type29>(), std::declval<__type34>())) __type35;
+      typedef container<typename std::remove_reference<__type35>::type> __type36;
+      typedef typename __combined<__type8,__type19,__type36>::type __type37;
       typedef typename pythonic::assignable<__type37>::type __type38;
-      typedef __type38 __type39;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type40;
-      typedef __type40 __type41;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type39>(), std::declval<__type41>())) __type42;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type43;
-      typedef __type43 __type44;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type42>(), std::declval<__type44>())) __type45;
-      typedef decltype(pythonic::operator_::add(std::declval<__type32>(), std::declval<__type45>())) __type46;
-      typedef double __type48;
-      typedef decltype(pythonic::operator_::add(std::declval<__type12>(), std::declval<__type48>())) __type49;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type12>(), std::declval<__type48>())) __type51;
-      typedef typename __combined<__type49,__type51>::type __type52;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type52>(), std::declval<__type14>())) __type54;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type54>(), std::declval<__type17>())) __type56;
-      typedef decltype(pythonic::operator_::add(std::declval<__type25>(), std::declval<__type48>())) __type58;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type25>(), std::declval<__type48>())) __type60;
-      typedef typename __combined<__type58,__type60>::type __type61;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type61>(), std::declval<__type27>())) __type63;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type63>(), std::declval<__type30>())) __type65;
-      typedef decltype(pythonic::operator_::add(std::declval<__type56>(), std::declval<__type65>())) __type66;
-      typedef decltype(pythonic::operator_::add(std::declval<__type39>(), std::declval<__type48>())) __type68;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type39>(), std::declval<__type48>())) __type70;
-      typedef typename __combined<__type68,__type70>::type __type71;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type71>(), std::declval<__type41>())) __type73;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type73>(), std::declval<__type44>())) __type75;
-      typedef decltype(pythonic::operator_::add(std::declval<__type66>(), std::declval<__type75>())) __type76;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type46>(), std::declval<__type76>())) __type77;
-      typedef typename pythonic::returnable<__type77>::type __type78;
-      typedef __type78 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type47;
+      typedef __type47 __type48;
+      typedef decltype(std::declval<__type0>()(std::declval<__type48>())) __type49;
+      typedef typename pythonic::assignable<__type49>::type __type50;
+      typedef __type50 __type51;
+      typedef decltype(pythonic::types::as_const(std::declval<__type51>())) __type52;
+      typedef decltype(std::declval<__type52>()[std::declval<__type18>()]) __type54;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type20>(), std::declval<__type54>())) __type55;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type55>(), std::declval<__type34>())) __type57;
+      typedef container<typename std::remove_reference<__type57>::type> __type58;
+      typedef typename __combined<__type8,__type19,__type58>::type __type59;
+      typedef typename pythonic::assignable<__type59>::type __type60;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type69;
+      typedef __type69 __type70;
+      typedef decltype(std::declval<__type0>()(std::declval<__type70>())) __type71;
+      typedef typename pythonic::assignable<__type71>::type __type72;
+      typedef __type72 __type73;
+      typedef decltype(pythonic::types::as_const(std::declval<__type73>())) __type74;
+      typedef decltype(std::declval<__type74>()[std::declval<__type18>()]) __type76;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type20>(), std::declval<__type76>())) __type77;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type77>(), std::declval<__type34>())) __type79;
+      typedef container<typename std::remove_reference<__type79>::type> __type80;
+      typedef typename __combined<__type8,__type19,__type80>::type __type81;
+      typedef typename pythonic::assignable<__type81>::type __type82;
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::empty_like{}(arr_fft))>::type dx_arr_fft = pythonic::numpy::functor::empty_like{}(arr_fft);
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::empty_like{}(arr_fft))>::type dy_arr_fft = pythonic::numpy::functor::empty_like{}(arr_fft);
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::empty_like{}(arr_fft))>::type dz_arr_fft = pythonic::numpy::functor::empty_like{}(arr_fft);
+      __type38 dx_arr_fft_flat = pythonic::numpy::functor::ravel{}(dx_arr_fft);
+      __type60 dy_arr_fft_flat = pythonic::numpy::functor::ravel{}(dy_arr_fft);
+      __type82 dz_arr_fft_flat = pythonic::numpy::functor::ravel{}(dz_arr_fft);
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::ravel{}(self_Kx))>::type Kx = pythonic::numpy::functor::ravel{}(self_Kx);
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::ravel{}(self_Ky))>::type Ky = pythonic::numpy::functor::ravel{}(self_Ky);
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::ravel{}(self_Kz))>::type Kz = pythonic::numpy::functor::ravel{}(self_Kz);
+      {
+        for (auto&& __tuple0: pythonic::builtins::functor::enumerate{}(pythonic::builtins::getattr(pythonic::types::attr::FLAT{}, arr_fft)))
+        {
+          typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(__tuple0)))>::type value = std::get<1>(pythonic::types::as_const(__tuple0));
+          typename pythonic::assignable_noescape<decltype(std::get<0>(pythonic::types::as_const(__tuple0)))>::type i = std::get<0>(pythonic::types::as_const(__tuple0));
+          dx_arr_fft_flat[i] = pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), pythonic::types::as_const(Kx)[i]), value);
+          dy_arr_fft_flat[i] = pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), pythonic::types::as_const(Ky)[i]), value);
+          dz_arr_fft_flat[i] = pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), pythonic::types::as_const(Kz)[i]), value);
+        }
+      }
+      return pythonic::types::make_tuple(dx_arr_fft, dy_arr_fft, dz_arr_fft);
+    }
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& self_deltax, argument_type4&& self_deltay, argument_type5&& self_deltaz) const
-    ;
-  }  ;
-  template <typename argument_type0 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0::type<argument_type0>::result_type __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0::operator()(argument_type0&& _) const
-  {
-    return pythonic::random::functor::uniform{}(-0.5, 0.5);
-  }
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
+    typename __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::operator()() const
     {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.1"));
-      return tmp_global;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, divh_fft):\n    return backend_func(self.Kx, self.Ky, divh_fft)\n\n");
+        return tmp_global;
+      }
     }
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__get_phases_random::type::result_type __code_new_method__OperatorsPseudoSpectral3D__get_phases_random::operator()() const
-  {
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::type<argument_type0, argument_type1, argument_type2>::result_type __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 divh_fft) const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__get_phases_random::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, ):\n    return backend_func(self.Kx, self.Ky, self.Kz, self.deltax, self.deltay, self.deltaz, )\n\n");
-      return tmp_global;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef double __type9;
+      typedef container<typename std::remove_reference<__type9>::type> __type10;
+      typedef typename __combined<__type8,__type10>::type __type11;
+      typedef __type11 __type12;
+      typedef long __type13;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
+      typedef indexable<__type14> __type15;
+      typedef typename __combined<__type8,__type15,__type10>::type __type16;
+      typedef typename pythonic::assignable<__type16>::type __type17;
+      __type17 inv_Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
+      inv_Kh_square_nozero.fast(pythonic::operator_::eq(inv_Kh_square_nozero, 0L)) = 1e-14;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1L, inv_Kh_square_nozero))>::type inv_Kh_square_nozero_ = pythonic::operator_::div(1L, inv_Kh_square_nozero);
+      return pythonic::types::make_tuple(pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), self_Kx), inv_Kh_square_nozero_), divh_fft), pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), self_Ky), inv_Kh_square_nozero_), divh_fft));
     }
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::operator()() const
-  {
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::operator()() const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, arr_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, arr_fft)\n\n");
-      return tmp_global;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, rotz_fft):\n    return backend_func(self.Kx, self.Ky, rotz_fft)\n\n");
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral3D__grad_fft_from_arr_fft::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& arr_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::ravel{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::empty_like{})>::type>::type __type1;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type2;
-    typedef __type2 __type3;
-    typedef decltype(std::declval<__type1>()(std::declval<__type3>())) __type4;
-    typedef typename pythonic::assignable<__type4>::type __type5;
-    typedef __type5 __type6;
-    typedef decltype(std::declval<__type0>()(std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type9;
-    typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::FLAT{}, std::declval<__type3>())) __type11;
-    typedef decltype(std::declval<__type9>()(std::declval<__type11>())) __type12;
-    typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type12>::type::iterator>::value_type>::type __type13;
-    typedef __type13 __type14;
-    typedef typename std::tuple_element<0,typename std::remove_reference<__type14>::type>::type __type15;
-    typedef typename pythonic::assignable<__type15>::type __type16;
-    typedef __type16 __type17;
-    typedef indexable<__type17> __type18;
-    typedef std::complex<double> __type19;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type20;
-    typedef __type20 __type21;
-    typedef decltype(std::declval<__type0>()(std::declval<__type21>())) __type22;
-    typedef typename pythonic::assignable<__type22>::type __type23;
-    typedef __type23 __type24;
-    typedef decltype(std::declval<__type24>()[std::declval<__type17>()]) __type26;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type19>(), std::declval<__type26>())) __type27;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type14>::type>::type __type29;
-    typedef typename pythonic::assignable<__type29>::type __type30;
-    typedef __type30 __type31;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type27>(), std::declval<__type31>())) __type32;
-    typedef container<typename std::remove_reference<__type32>::type> __type33;
-    typedef typename __combined<__type8,__type18,__type33>::type __type34;
-    typedef typename pythonic::assignable<__type34>::type __type35;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type44;
-    typedef __type44 __type45;
-    typedef decltype(std::declval<__type0>()(std::declval<__type45>())) __type46;
-    typedef typename pythonic::assignable<__type46>::type __type47;
-    typedef __type47 __type48;
-    typedef decltype(std::declval<__type48>()[std::declval<__type17>()]) __type50;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type19>(), std::declval<__type50>())) __type51;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type51>(), std::declval<__type31>())) __type53;
-    typedef container<typename std::remove_reference<__type53>::type> __type54;
-    typedef typename __combined<__type8,__type18,__type54>::type __type55;
-    typedef typename pythonic::assignable<__type55>::type __type56;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type65;
-    typedef __type65 __type66;
-    typedef decltype(std::declval<__type0>()(std::declval<__type66>())) __type67;
-    typedef typename pythonic::assignable<__type67>::type __type68;
-    typedef __type68 __type69;
-    typedef decltype(std::declval<__type69>()[std::declval<__type17>()]) __type71;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type19>(), std::declval<__type71>())) __type72;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type72>(), std::declval<__type31>())) __type74;
-    typedef container<typename std::remove_reference<__type74>::type> __type75;
-    typedef typename __combined<__type8,__type18,__type75>::type __type76;
-    typedef typename pythonic::assignable<__type76>::type __type77;
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::empty_like{}(arr_fft))>::type dx_arr_fft = pythonic::numpy::functor::empty_like{}(arr_fft);
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::empty_like{}(arr_fft))>::type dy_arr_fft = pythonic::numpy::functor::empty_like{}(arr_fft);
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::empty_like{}(arr_fft))>::type dz_arr_fft = pythonic::numpy::functor::empty_like{}(arr_fft);
-    __type35 dx_arr_fft_flat = pythonic::numpy::functor::ravel{}(dx_arr_fft);
-    __type56 dy_arr_fft_flat = pythonic::numpy::functor::ravel{}(dy_arr_fft);
-    __type77 dz_arr_fft_flat = pythonic::numpy::functor::ravel{}(dz_arr_fft);
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::ravel{}(self_Kx))>::type Kx = pythonic::numpy::functor::ravel{}(self_Kx);
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::ravel{}(self_Ky))>::type Ky = pythonic::numpy::functor::ravel{}(self_Ky);
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::ravel{}(self_Kz))>::type Kz = pythonic::numpy::functor::ravel{}(self_Kz);
-    {
-      for (auto&& __tuple0: pythonic::builtins::functor::enumerate{}(pythonic::builtins::getattr(pythonic::types::attr::FLAT{}, arr_fft)))
-      {
-        typename pythonic::assignable_noescape<decltype(std::get<1>(__tuple0))>::type value = std::get<1>(__tuple0);
-        typename pythonic::assignable_noescape<decltype(std::get<0>(__tuple0))>::type i = std::get<0>(__tuple0);
-        dx_arr_fft_flat[i] = pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), Kx[i]), value);
-        dy_arr_fft_flat[i] = pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), Ky[i]), value);
-        dz_arr_fft_flat[i] = pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), Kz[i]), value);
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::type<argument_type0, argument_type1, argument_type2>::result_type __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 rotz_fft) const
+    {
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef double __type9;
+      typedef container<typename std::remove_reference<__type9>::type> __type10;
+      typedef typename __combined<__type8,__type10>::type __type11;
+      typedef __type11 __type12;
+      typedef long __type13;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
+      typedef indexable<__type14> __type15;
+      typedef typename __combined<__type8,__type15,__type10>::type __type16;
+      typedef typename pythonic::assignable<__type16>::type __type17;
+      __type17 inv_Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
+      inv_Kh_square_nozero.fast(pythonic::operator_::eq(inv_Kh_square_nozero, 0L)) = 1e-14;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1L, inv_Kh_square_nozero))>::type inv_Kh_square_nozero_ = pythonic::operator_::div(1L, inv_Kh_square_nozero);
+      return pythonic::types::make_tuple(pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), self_Ky), inv_Kh_square_nozero_), rotz_fft), pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), self_Kx), inv_Kh_square_nozero_), rotz_fft));
+    }
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::operator()() const
+    {
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft):\n    return backend_func(self.Kx, self.Ky, vx_fft, vy_fft)\n\n");
+        return tmp_global;
       }
     }
-    return pythonic::types::make_tuple(dx_arr_fft, dy_arr_fft, dz_arr_fft);
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::operator()() const
-  {
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vx_fft, argument_type3 vy_fft) const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, divh_fft):\n    return backend_func(self.Kx, self.Ky, divh_fft)\n\n");
-      return tmp_global;
+      return pythonic::operator_::mul(std::complex<double>(0.0, 1.0), pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft)));
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::type<argument_type0, argument_type1, argument_type2>::result_type __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_divhfft::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& divh_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef double __type9;
-    typedef container<typename std::remove_reference<__type9>::type> __type10;
-    typedef typename __combined<__type8,__type10>::type __type11;
-    typedef __type11 __type12;
-    typedef long __type13;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
-    typedef indexable<__type14> __type15;
-    typedef typename __combined<__type8,__type15,__type10>::type __type16;
-    typedef typename pythonic::assignable<__type16>::type __type17;
-    __type17 inv_Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
-    inv_Kh_square_nozero.fast(pythonic::operator_::eq(inv_Kh_square_nozero, 0L)) = 1e-14;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1L, inv_Kh_square_nozero))>::type inv_Kh_square_nozero_ = pythonic::operator_::div(1L, inv_Kh_square_nozero);
-    return pythonic::types::make_tuple(pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), self_Kx), inv_Kh_square_nozero_), divh_fft), pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), self_Ky), inv_Kh_square_nozero_), divh_fft));
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::operator()() const
-  {
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::operator()() const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, rotz_fft):\n    return backend_func(self.Kx, self.Ky, rotz_fft)\n\n");
-      return tmp_global;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vt_fft):\n    return backend_func(self.Kx, self.Ky, vt_fft)\n\n");
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::type<argument_type0, argument_type1, argument_type2>::result_type __for_method__OperatorsPseudoSpectral3D__vxvyfft_from_rotzfft::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& rotz_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef double __type9;
-    typedef container<typename std::remove_reference<__type9>::type> __type10;
-    typedef typename __combined<__type8,__type10>::type __type11;
-    typedef __type11 __type12;
-    typedef long __type13;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
-    typedef indexable<__type14> __type15;
-    typedef typename __combined<__type8,__type15,__type10>::type __type16;
-    typedef typename pythonic::assignable<__type16>::type __type17;
-    __type17 inv_Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
-    inv_Kh_square_nozero.fast(pythonic::operator_::eq(inv_Kh_square_nozero, 0L)) = 1e-14;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1L, inv_Kh_square_nozero))>::type inv_Kh_square_nozero_ = pythonic::operator_::div(1L, inv_Kh_square_nozero);
-    return pythonic::types::make_tuple(pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), self_Ky), inv_Kh_square_nozero_), rotz_fft), pythonic::operator_::mul(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), self_Kx), inv_Kh_square_nozero_), rotz_fft));
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::operator()() const
-  {
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::type<argument_type0, argument_type1, argument_type2>::result_type __for_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vt_fft) const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft):\n    return backend_func(self.Kx, self.Ky, vx_fft, vy_fft)\n\n");
-      return tmp_global;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef double __type9;
+      typedef container<typename std::remove_reference<__type9>::type> __type10;
+      typedef typename __combined<__type8,__type10>::type __type11;
+      typedef __type11 __type12;
+      typedef long __type13;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
+      typedef indexable<__type14> __type15;
+      typedef typename __combined<__type8,__type15,__type10>::type __type16;
+      typedef typename pythonic::assignable<__type16>::type __type17;
+      __type17 Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
+      Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero)))>::type tmp = pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero));
+      return pythonic::types::make_tuple(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), pythonic::operator_::mul(self_Ky, tmp)), vt_fft), pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), pythonic::operator_::mul(self_Kx, tmp)), vt_fft), pythonic::numpy::functor::zeros_like{}(vt_fft));
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral3D__divhfft_from_vxvyfft::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vx_fft, argument_type3&& vy_fft) const
-  {
-    return pythonic::operator_::mul(std::complex<double>(0.0, 1.0), pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft)));
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::operator()() const
-  {
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::operator()() const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vt_fft):\n    return backend_func(self.Kx, self.Ky, vt_fft)\n\n");
-      return tmp_global;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, vx_fft, vy_fft, vz_fft)\n\n");
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::type<argument_type0, argument_type1, argument_type2>::result_type __for_method__OperatorsPseudoSpectral3D__vecfft_from_vtfft::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vt_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef double __type9;
-    typedef container<typename std::remove_reference<__type9>::type> __type10;
-    typedef typename __combined<__type8,__type10>::type __type11;
-    typedef __type11 __type12;
-    typedef long __type13;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
-    typedef indexable<__type14> __type15;
-    typedef typename __combined<__type8,__type15,__type10>::type __type16;
-    typedef typename pythonic::assignable<__type16>::type __type17;
-    __type17 Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
-    Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero)))>::type tmp = pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero));
-    return pythonic::types::make_tuple(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), pythonic::operator_::mul(self_Ky, tmp)), vt_fft), pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), pythonic::operator_::mul(self_Kx, tmp)), vt_fft), pythonic::numpy::functor::zeros_like{}(vt_fft));
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::operator()() const
-  {
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type __for_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vx_fft, argument_type3 vy_fft, argument_type4 vz_fft) const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, vx_fft, vy_fft, vz_fft)\n\n");
-      return tmp_global;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef double __type9;
+      typedef container<typename std::remove_reference<__type9>::type> __type10;
+      typedef typename __combined<__type8,__type10>::type __type11;
+      typedef __type11 __type12;
+      typedef long __type13;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
+      typedef indexable<__type14> __type15;
+      typedef typename __combined<__type8,__type15,__type10>::type __type16;
+      typedef typename pythonic::assignable<__type16>::type __type17;
+      __type17 Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
+      Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
+      
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero)))>::type tmp = pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero));
+      return pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), pythonic::operator_::mul(self_Ky, tmp)), vx_fft), pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), pythonic::operator_::mul(self_Kx, tmp)), vy_fft));
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type __for_method__OperatorsPseudoSpectral3D__vtfft_from_vecfft::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vx_fft, argument_type3&& vy_fft, argument_type4&& vz_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef double __type9;
-    typedef container<typename std::remove_reference<__type9>::type> __type10;
-    typedef typename __combined<__type8,__type10>::type __type11;
-    typedef __type11 __type12;
-    typedef long __type13;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
-    typedef indexable<__type14> __type15;
-    typedef typename __combined<__type8,__type15,__type10>::type __type16;
-    typedef typename pythonic::assignable<__type16>::type __type17;
-    __type17 Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
-    Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
-    
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero)))>::type tmp = pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero));
-    return pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(-0.0, -1.0), pythonic::operator_::mul(self_Ky, tmp)), vx_fft), pythonic::operator_::mul(pythonic::operator_::mul(std::complex<double>(0.0, 1.0), pythonic::operator_::mul(self_Kx, tmp)), vy_fft));
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__project_toroidal::type::result_type __code_new_method__OperatorsPseudoSpectral3D__project_toroidal::operator()() const
-  {
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__project_toroidal::type::result_type __code_new_method__OperatorsPseudoSpectral3D__project_toroidal::operator()() const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__project_toroidal::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, vx_fft, vy_fft, vz_fft)\n\n");
-      return tmp_global;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__project_toroidal::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, vx_fft, vy_fft, vz_fft)\n\n");
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__project_toroidal::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type __for_method__OperatorsPseudoSpectral3D__project_toroidal::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vx_fft, argument_type3&& vy_fft, argument_type4&& vz_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef double __type9;
-    typedef container<typename std::remove_reference<__type9>::type> __type10;
-    typedef typename __combined<__type8,__type10>::type __type11;
-    typedef __type11 __type12;
-    typedef long __type13;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
-    typedef indexable<__type14> __type15;
-    typedef typename __combined<__type8,__type15,__type10>::type __type16;
-    typedef typename pythonic::assignable<__type16>::type __type17;
-    __type17 Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
-    Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
-    
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero)))>::type tmp = pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero));
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kx, tmp))>::type cos_phi_k = pythonic::operator_::mul(self_Kx, tmp);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Ky, tmp))>::type sin_phi_k = pythonic::operator_::mul(self_Ky, tmp);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::neg(sin_phi_k), vx_fft), pythonic::operator_::mul(cos_phi_k, vy_fft)))>::type tmp_ = pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::neg(sin_phi_k), vx_fft), pythonic::operator_::mul(cos_phi_k, vy_fft));
-    typename pythonic::lazy<decltype(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)))>::type n0 = std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft));
-    typename pythonic::lazy<decltype(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)))>::type n1 = std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft));
-    typename pythonic::lazy<decltype(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)))>::type n2 = std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft));
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__project_toroidal::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type __for_method__OperatorsPseudoSpectral3D__project_toroidal::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vx_fft, argument_type3 vy_fft, argument_type4 vz_fft) const
     {
-      long  __target140028818307776 = n0;
-      for (long  i0=0L; i0 < __target140028818307776; i0 += 1L)
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef double __type9;
+      typedef container<typename std::remove_reference<__type9>::type> __type10;
+      typedef typename __combined<__type8,__type10>::type __type11;
+      typedef __type11 __type12;
+      typedef long __type13;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
+      typedef indexable<__type14> __type15;
+      typedef typename __combined<__type8,__type15,__type10>::type __type16;
+      typedef typename pythonic::assignable<__type16>::type __type17;
+      __type17 Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
+      Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
+      
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero)))>::type tmp = pythonic::numpy::functor::sqrt{}(pythonic::operator_::div(1.0, Kh_square_nozero));
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kx, tmp))>::type cos_phi_k = pythonic::operator_::mul(self_Kx, tmp);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Ky, tmp))>::type sin_phi_k = pythonic::operator_::mul(self_Ky, tmp);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::neg(sin_phi_k), vx_fft), pythonic::operator_::mul(cos_phi_k, vy_fft)))>::type tmp_ = pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::neg(sin_phi_k), vx_fft), pythonic::operator_::mul(cos_phi_k, vy_fft));
+      typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft))))>::type n0 = std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)));
+      typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft))))>::type n1 = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)));
+      typename pythonic::lazy<decltype(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft))))>::type n2 = std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)));
       {
+        long  __target139658367247168 = n0;
+        for (long  i0=0L; i0 < __target139658367247168; i0 += 1L)
         {
-          long  __target140028817949648 = n1;
-          for (long  i1=0L; i1 < __target140028817949648; i1 += 1L)
           {
+            long  __target139658367187072 = n1;
+            for (long  i1=0L; i1 < __target139658367187072; i1 += 1L)
             {
-              long  __target140028817950224 = n2;
-              for (long  i2=0L; i2 < __target140028817950224; i2 += 1L)
               {
-                vx_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::operator_::neg(sin_phi_k.fast(pythonic::types::make_tuple(i0, i1, i2))), tmp_.fast(pythonic::types::make_tuple(i0, i1, i2)));
-                vy_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(cos_phi_k.fast(pythonic::types::make_tuple(i0, i1, i2)), tmp_.fast(pythonic::types::make_tuple(i0, i1, i2)));
-                vz_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = 0.0;
+                long  __target139658367187648 = n2;
+                for (long  i2=0L; i2 < __target139658367187648; i2 += 1L)
+                {
+                  vx_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::operator_::neg(pythonic::types::as_const(sin_phi_k).fast(pythonic::types::make_tuple(i0, i1, i2))), pythonic::types::as_const(tmp_).fast(pythonic::types::make_tuple(i0, i1, i2)));
+                  vy_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::types::as_const(cos_phi_k).fast(pythonic::types::make_tuple(i0, i1, i2)), pythonic::types::as_const(tmp_).fast(pythonic::types::make_tuple(i0, i1, i2)));
+                  vz_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = 0.0;
+                }
               }
             }
           }
         }
       }
+      return pythonic::builtins::None;
     }
-    return pythonic::builtins::None;
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::operator()() const
-  {
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::operator()() const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vp_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, vp_fft)\n\n");
-      return tmp_global;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vp_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, vp_fft)\n\n");
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& vp_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef __type8 __type9;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type10;
-    typedef __type10 __type11;
-    typedef decltype(std::declval<__type0>()(std::declval<__type11>())) __type12;
-    typedef decltype(pythonic::operator_::add(std::declval<__type9>(), std::declval<__type12>())) __type13;
-    typedef typename pythonic::assignable<__type13>::type __type14;
-    typedef double __type15;
-    typedef container<typename std::remove_reference<__type15>::type> __type16;
-    typedef typename __combined<__type14,__type16>::type __type17;
-    typedef __type17 __type18;
-    typedef long __type19;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type18>(), std::declval<__type19>())) __type20;
-    typedef indexable<__type20> __type21;
-    typedef typename __combined<__type14,__type21,__type16>::type __type22;
-    typedef typename pythonic::assignable<__type22>::type __type23;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type24;
-    typedef decltype(std::declval<__type24>()(std::declval<__type9>())) __type26;
-    typedef typename pythonic::assignable<__type26>::type __type27;
-    typedef typename __combined<__type27,__type16>::type __type28;
-    typedef __type28 __type29;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type29>(), std::declval<__type19>())) __type30;
-    typedef indexable<__type30> __type31;
-    typedef typename __combined<__type27,__type31,__type16>::type __type32;
-    typedef typename pythonic::assignable<__type32>::type __type33;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky)))>::type Kh_square = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
-    __type23 K_square_nozero = pythonic::operator_::add(Kh_square, pythonic::numpy::functor::square{}(self_Kz));
-    __type33 Kh_square_nozero = pythonic::__dispatch__::functor::copy{}(Kh_square);
-    Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
-    K_square_nozero.fast(pythonic::operator_::eq(K_square_nozero, 0L)) = 1e-14;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, Kh_square_nozero))>::type inv_Kh_square_nozero = pythonic::operator_::div(1.0, Kh_square_nozero);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, K_square_nozero))>::type inv_K_square_nozero = pythonic::operator_::div(1.0, K_square_nozero);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero)))>::type cos_theta_k = pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero));
-    return pythonic::types::make_tuple(pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, pythonic::operator_::mul(self_Kx, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero))), vp_fft), pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, pythonic::operator_::mul(self_Ky, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero))), vp_fft), pythonic::operator_::mul(pythonic::operator_::neg(pythonic::numpy::functor::sqrt{}(pythonic::operator_::mul(Kh_square, inv_K_square_nozero))), vp_fft));
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::operator()() const
-  {
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral3D__vecfft_from_vpfft::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 vp_fft) const
+    {
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef __type8 __type9;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type10;
+      typedef __type10 __type11;
+      typedef decltype(std::declval<__type0>()(std::declval<__type11>())) __type12;
+      typedef decltype(pythonic::operator_::add(std::declval<__type9>(), std::declval<__type12>())) __type13;
+      typedef typename pythonic::assignable<__type13>::type __type14;
+      typedef double __type15;
+      typedef container<typename std::remove_reference<__type15>::type> __type16;
+      typedef typename __combined<__type14,__type16>::type __type17;
+      typedef __type17 __type18;
+      typedef long __type19;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type18>(), std::declval<__type19>())) __type20;
+      typedef indexable<__type20> __type21;
+      typedef typename __combined<__type14,__type21,__type16>::type __type22;
+      typedef typename pythonic::assignable<__type22>::type __type23;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type24;
+      typedef decltype(std::declval<__type24>()(std::declval<__type9>())) __type26;
+      typedef typename pythonic::assignable<__type26>::type __type27;
+      typedef typename __combined<__type27,__type16>::type __type28;
+      typedef __type28 __type29;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type29>(), std::declval<__type19>())) __type30;
+      typedef indexable<__type30> __type31;
+      typedef typename __combined<__type27,__type31,__type16>::type __type32;
+      typedef typename pythonic::assignable<__type32>::type __type33;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky)))>::type Kh_square = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
+      __type23 K_square_nozero = pythonic::operator_::add(Kh_square, pythonic::numpy::functor::square{}(self_Kz));
+      __type33 Kh_square_nozero = pythonic::__dispatch__::functor::copy{}(Kh_square);
+      Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
+      K_square_nozero.fast(pythonic::operator_::eq(K_square_nozero, 0L)) = 1e-14;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, Kh_square_nozero))>::type inv_Kh_square_nozero = pythonic::operator_::div(1.0, Kh_square_nozero);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, K_square_nozero))>::type inv_K_square_nozero = pythonic::operator_::div(1.0, K_square_nozero);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero)))>::type cos_theta_k = pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero));
+      return pythonic::types::make_tuple(pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, pythonic::operator_::mul(self_Kx, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero))), vp_fft), pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, pythonic::operator_::mul(self_Ky, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero))), vp_fft), pythonic::operator_::mul(pythonic::operator_::neg(pythonic::numpy::functor::sqrt{}(pythonic::operator_::mul(Kh_square, inv_K_square_nozero))), vp_fft));
+    }
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::operator()() const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, vx_fft, vy_fft, vz_fft)\n\n");
-      return tmp_global;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, vx_fft, vy_fft, vz_fft)\n\n");
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type __for_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& vx_fft, argument_type4&& vy_fft, argument_type5&& vz_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef __type8 __type9;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type10;
-    typedef __type10 __type11;
-    typedef decltype(std::declval<__type0>()(std::declval<__type11>())) __type12;
-    typedef decltype(pythonic::operator_::add(std::declval<__type9>(), std::declval<__type12>())) __type13;
-    typedef typename pythonic::assignable<__type13>::type __type14;
-    typedef double __type15;
-    typedef container<typename std::remove_reference<__type15>::type> __type16;
-    typedef typename __combined<__type14,__type16>::type __type17;
-    typedef __type17 __type18;
-    typedef long __type19;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type18>(), std::declval<__type19>())) __type20;
-    typedef indexable<__type20> __type21;
-    typedef typename __combined<__type14,__type21,__type16>::type __type22;
-    typedef typename pythonic::assignable<__type22>::type __type23;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type24;
-    typedef decltype(std::declval<__type24>()(std::declval<__type9>())) __type26;
-    typedef typename pythonic::assignable<__type26>::type __type27;
-    typedef typename __combined<__type27,__type16>::type __type28;
-    typedef __type28 __type29;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type29>(), std::declval<__type19>())) __type30;
-    typedef indexable<__type30> __type31;
-    typedef typename __combined<__type27,__type31,__type16>::type __type32;
-    typedef typename pythonic::assignable<__type32>::type __type33;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky)))>::type Kh_square = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
-    __type23 K_square_nozero = pythonic::operator_::add(Kh_square, pythonic::numpy::functor::square{}(self_Kz));
-    __type33 Kh_square_nozero = pythonic::__dispatch__::functor::copy{}(Kh_square);
-    Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
-    K_square_nozero.fast(pythonic::operator_::eq(K_square_nozero, 0L)) = 1e-14;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, Kh_square_nozero))>::type inv_Kh_square_nozero = pythonic::operator_::div(1.0, Kh_square_nozero);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, K_square_nozero))>::type inv_K_square_nozero = pythonic::operator_::div(1.0, K_square_nozero);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero)))>::type cos_theta_k = pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero));
-    return pythonic::operator_::sub(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, pythonic::operator_::mul(self_Kx, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero))), vx_fft), pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, pythonic::operator_::mul(self_Ky, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero))), vy_fft)), pythonic::operator_::mul(pythonic::numpy::functor::sqrt{}(pythonic::operator_::mul(Kh_square, inv_K_square_nozero)), vz_fft));
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__project_poloidal::type::result_type __code_new_method__OperatorsPseudoSpectral3D__project_poloidal::operator()() const
-  {
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type __for_method__OperatorsPseudoSpectral3D__vpfft_from_vecfft::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 vx_fft, argument_type4 vy_fft, argument_type5 vz_fft) const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__project_poloidal::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, vx_fft, vy_fft, vz_fft)\n\n");
-      return tmp_global;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef __type8 __type9;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type10;
+      typedef __type10 __type11;
+      typedef decltype(std::declval<__type0>()(std::declval<__type11>())) __type12;
+      typedef decltype(pythonic::operator_::add(std::declval<__type9>(), std::declval<__type12>())) __type13;
+      typedef typename pythonic::assignable<__type13>::type __type14;
+      typedef double __type15;
+      typedef container<typename std::remove_reference<__type15>::type> __type16;
+      typedef typename __combined<__type14,__type16>::type __type17;
+      typedef __type17 __type18;
+      typedef long __type19;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type18>(), std::declval<__type19>())) __type20;
+      typedef indexable<__type20> __type21;
+      typedef typename __combined<__type14,__type21,__type16>::type __type22;
+      typedef typename pythonic::assignable<__type22>::type __type23;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type24;
+      typedef decltype(std::declval<__type24>()(std::declval<__type9>())) __type26;
+      typedef typename pythonic::assignable<__type26>::type __type27;
+      typedef typename __combined<__type27,__type16>::type __type28;
+      typedef __type28 __type29;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type29>(), std::declval<__type19>())) __type30;
+      typedef indexable<__type30> __type31;
+      typedef typename __combined<__type27,__type31,__type16>::type __type32;
+      typedef typename pythonic::assignable<__type32>::type __type33;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky)))>::type Kh_square = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
+      __type23 K_square_nozero = pythonic::operator_::add(Kh_square, pythonic::numpy::functor::square{}(self_Kz));
+      __type33 Kh_square_nozero = pythonic::__dispatch__::functor::copy{}(Kh_square);
+      Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
+      K_square_nozero.fast(pythonic::operator_::eq(K_square_nozero, 0L)) = 1e-14;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, Kh_square_nozero))>::type inv_Kh_square_nozero = pythonic::operator_::div(1.0, Kh_square_nozero);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, K_square_nozero))>::type inv_K_square_nozero = pythonic::operator_::div(1.0, K_square_nozero);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero)))>::type cos_theta_k = pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero));
+      return pythonic::operator_::sub(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, pythonic::operator_::mul(self_Kx, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero))), vx_fft), pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, pythonic::operator_::mul(self_Ky, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero))), vy_fft)), pythonic::operator_::mul(pythonic::numpy::functor::sqrt{}(pythonic::operator_::mul(Kh_square, inv_K_square_nozero)), vz_fft));
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__project_poloidal::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type __for_method__OperatorsPseudoSpectral3D__project_poloidal::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& vx_fft, argument_type4&& vy_fft, argument_type5&& vz_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef __type8 __type9;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type10;
-    typedef __type10 __type11;
-    typedef decltype(std::declval<__type0>()(std::declval<__type11>())) __type12;
-    typedef decltype(pythonic::operator_::add(std::declval<__type9>(), std::declval<__type12>())) __type13;
-    typedef typename pythonic::assignable<__type13>::type __type14;
-    typedef double __type15;
-    typedef container<typename std::remove_reference<__type15>::type> __type16;
-    typedef typename __combined<__type14,__type16>::type __type17;
-    typedef __type17 __type18;
-    typedef long __type19;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type18>(), std::declval<__type19>())) __type20;
-    typedef indexable<__type20> __type21;
-    typedef typename __combined<__type14,__type21,__type16>::type __type22;
-    typedef typename pythonic::assignable<__type22>::type __type23;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type24;
-    typedef decltype(std::declval<__type24>()(std::declval<__type9>())) __type26;
-    typedef typename pythonic::assignable<__type26>::type __type27;
-    typedef typename __combined<__type27,__type16>::type __type28;
-    typedef __type28 __type29;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type29>(), std::declval<__type19>())) __type30;
-    typedef indexable<__type30> __type31;
-    typedef typename __combined<__type27,__type31,__type16>::type __type32;
-    typedef typename pythonic::assignable<__type32>::type __type33;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky)))>::type Kh_square = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
-    __type23 K_square_nozero = pythonic::operator_::add(Kh_square, pythonic::numpy::functor::square{}(self_Kz));
-    __type33 Kh_square_nozero = pythonic::__dispatch__::functor::copy{}(Kh_square);
-    Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
-    K_square_nozero.fast(pythonic::operator_::eq(K_square_nozero, 0L)) = 1e-14;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, Kh_square_nozero))>::type inv_Kh_square_nozero = pythonic::operator_::div(1.0, Kh_square_nozero);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, K_square_nozero))>::type inv_K_square_nozero = pythonic::operator_::div(1.0, K_square_nozero);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero)))>::type cos_theta_k = pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero));
-    typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::sqrt{}(pythonic::operator_::mul(Kh_square, inv_K_square_nozero)))>::type sin_theta_k = pythonic::numpy::functor::sqrt{}(pythonic::operator_::mul(Kh_square, inv_K_square_nozero));
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kx, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero)))>::type cos_phi_k = pythonic::operator_::mul(self_Kx, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero));
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Ky, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero)))>::type sin_phi_k = pythonic::operator_::mul(self_Ky, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero));
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::sub(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, cos_phi_k), vx_fft), pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, sin_phi_k), vy_fft)), pythonic::operator_::mul(sin_theta_k, vz_fft)))>::type tmp = pythonic::operator_::sub(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, cos_phi_k), vx_fft), pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, sin_phi_k), vy_fft)), pythonic::operator_::mul(sin_theta_k, vz_fft));
-    typename pythonic::lazy<decltype(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)))>::type n0 = std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft));
-    typename pythonic::lazy<decltype(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)))>::type n1 = std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft));
-    typename pythonic::lazy<decltype(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)))>::type n2 = std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft));
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__project_poloidal::type::result_type __code_new_method__OperatorsPseudoSpectral3D__project_poloidal::operator()() const
     {
-      long  __target140028821273376 = n0;
-      for (long  i0=0L; i0 < __target140028821273376; i0 += 1L)
       {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__project_poloidal::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, vx_fft, vy_fft, vz_fft)\n\n");
+        return tmp_global;
+      }
+    }
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__project_poloidal::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type __for_method__OperatorsPseudoSpectral3D__project_poloidal::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 vx_fft, argument_type4 vy_fft, argument_type5 vz_fft) const
+    {
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef __type8 __type9;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type10;
+      typedef __type10 __type11;
+      typedef decltype(std::declval<__type0>()(std::declval<__type11>())) __type12;
+      typedef decltype(pythonic::operator_::add(std::declval<__type9>(), std::declval<__type12>())) __type13;
+      typedef typename pythonic::assignable<__type13>::type __type14;
+      typedef double __type15;
+      typedef container<typename std::remove_reference<__type15>::type> __type16;
+      typedef typename __combined<__type14,__type16>::type __type17;
+      typedef __type17 __type18;
+      typedef long __type19;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type18>(), std::declval<__type19>())) __type20;
+      typedef indexable<__type20> __type21;
+      typedef typename __combined<__type14,__type21,__type16>::type __type22;
+      typedef typename pythonic::assignable<__type22>::type __type23;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::__dispatch__::functor::copy{})>::type>::type __type24;
+      typedef decltype(std::declval<__type24>()(std::declval<__type9>())) __type26;
+      typedef typename pythonic::assignable<__type26>::type __type27;
+      typedef typename __combined<__type27,__type16>::type __type28;
+      typedef __type28 __type29;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type29>(), std::declval<__type19>())) __type30;
+      typedef indexable<__type30> __type31;
+      typedef typename __combined<__type27,__type31,__type16>::type __type32;
+      typedef typename pythonic::assignable<__type32>::type __type33;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky)))>::type Kh_square = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
+      __type23 K_square_nozero = pythonic::operator_::add(Kh_square, pythonic::numpy::functor::square{}(self_Kz));
+      __type33 Kh_square_nozero = pythonic::__dispatch__::functor::copy{}(Kh_square);
+      Kh_square_nozero.fast(pythonic::operator_::eq(Kh_square_nozero, 0L)) = 1e-14;
+      K_square_nozero.fast(pythonic::operator_::eq(K_square_nozero, 0L)) = 1e-14;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, Kh_square_nozero))>::type inv_Kh_square_nozero = pythonic::operator_::div(1.0, Kh_square_nozero);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1.0, K_square_nozero))>::type inv_K_square_nozero = pythonic::operator_::div(1.0, K_square_nozero);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero)))>::type cos_theta_k = pythonic::operator_::mul(self_Kz, pythonic::numpy::functor::sqrt{}(inv_K_square_nozero));
+      typename pythonic::assignable_noescape<decltype(pythonic::numpy::functor::sqrt{}(pythonic::operator_::mul(Kh_square, inv_K_square_nozero)))>::type sin_theta_k = pythonic::numpy::functor::sqrt{}(pythonic::operator_::mul(Kh_square, inv_K_square_nozero));
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Kx, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero)))>::type cos_phi_k = pythonic::operator_::mul(self_Kx, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero));
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(self_Ky, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero)))>::type sin_phi_k = pythonic::operator_::mul(self_Ky, pythonic::numpy::functor::sqrt{}(inv_Kh_square_nozero));
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::sub(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, cos_phi_k), vx_fft), pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, sin_phi_k), vy_fft)), pythonic::operator_::mul(sin_theta_k, vz_fft)))>::type tmp = pythonic::operator_::sub(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, cos_phi_k), vx_fft), pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k, sin_phi_k), vy_fft)), pythonic::operator_::mul(sin_theta_k, vz_fft));
+      typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft))))>::type n0 = std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)));
+      typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft))))>::type n1 = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)));
+      typename pythonic::lazy<decltype(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft))))>::type n2 = std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)));
+      {
+        long  __target139658368853040 = n0;
+        for (long  i0=0L; i0 < __target139658368853040; i0 += 1L)
         {
-          long  __target140028821849712 = n1;
-          for (long  i1=0L; i1 < __target140028821849712; i1 += 1L)
           {
+            long  __target139658368883104 = n1;
+            for (long  i1=0L; i1 < __target139658368883104; i1 += 1L)
             {
-              long  __target140028821850288 = n2;
-              for (long  i2=0L; i2 < __target140028821850288; i2 += 1L)
               {
-                vx_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k.fast(pythonic::types::make_tuple(i0, i1, i2)), cos_phi_k.fast(pythonic::types::make_tuple(i0, i1, i2))), tmp.fast(pythonic::types::make_tuple(i0, i1, i2)));
-                vy_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::operator_::mul(cos_theta_k.fast(pythonic::types::make_tuple(i0, i1, i2)), sin_phi_k.fast(pythonic::types::make_tuple(i0, i1, i2))), tmp.fast(pythonic::types::make_tuple(i0, i1, i2)));
-                vz_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::operator_::neg(sin_theta_k.fast(pythonic::types::make_tuple(i0, i1, i2))), tmp.fast(pythonic::types::make_tuple(i0, i1, i2)));
+                long  __target139658368883680 = n2;
+                for (long  i2=0L; i2 < __target139658368883680; i2 += 1L)
+                {
+                  vx_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::operator_::mul(pythonic::types::as_const(cos_theta_k).fast(pythonic::types::make_tuple(i0, i1, i2)), pythonic::types::as_const(cos_phi_k).fast(pythonic::types::make_tuple(i0, i1, i2))), pythonic::types::as_const(tmp).fast(pythonic::types::make_tuple(i0, i1, i2)));
+                  vy_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::operator_::mul(pythonic::types::as_const(cos_theta_k).fast(pythonic::types::make_tuple(i0, i1, i2)), pythonic::types::as_const(sin_phi_k).fast(pythonic::types::make_tuple(i0, i1, i2))), pythonic::types::as_const(tmp).fast(pythonic::types::make_tuple(i0, i1, i2)));
+                  vz_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::operator_::neg(pythonic::types::as_const(sin_theta_k).fast(pythonic::types::make_tuple(i0, i1, i2))), pythonic::types::as_const(tmp).fast(pythonic::types::make_tuple(i0, i1, i2)));
+                }
               }
             }
           }
         }
       }
+      return pythonic::builtins::None;
     }
-    return pythonic::builtins::None;
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__project_kradial3d::type::result_type __code_new_method__OperatorsPseudoSpectral3D__project_kradial3d::operator()() const
-  {
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__project_kradial3d::type::result_type __code_new_method__OperatorsPseudoSpectral3D__project_kradial3d::operator()() const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__project_kradial3d::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, vx_fft, vy_fft, vz_fft)\n\n");
-      return tmp_global;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__project_kradial3d::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft, vz_fft):\n    return backend_func(self.Kx, self.Ky, self.Kz, vx_fft, vy_fft, vz_fft)\n\n");
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__project_kradial3d::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type __for_method__OperatorsPseudoSpectral3D__project_kradial3d::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& vx_fft, argument_type4&& vy_fft, argument_type5&& vz_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type8;
-    typedef __type8 __type9;
-    typedef decltype(std::declval<__type0>()(std::declval<__type9>())) __type10;
-    typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
-    typedef typename pythonic::assignable<__type11>::type __type12;
-    typedef double __type13;
-    typedef container<typename std::remove_reference<__type13>::type> __type14;
-    typedef typename __combined<__type12,__type14>::type __type15;
-    typedef __type15 __type16;
-    typedef long __type17;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type16>(), std::declval<__type17>())) __type18;
-    typedef indexable<__type18> __type19;
-    typedef typename __combined<__type12,__type19,__type14>::type __type20;
-    typedef typename pythonic::assignable<__type20>::type __type21;
-    __type21 K_square_nozero = pythonic::operator_::add(pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky)), pythonic::numpy::functor::square{}(self_Kz));
-    K_square_nozero.fast(pythonic::operator_::eq(K_square_nozero, 0L)) = 1e-14;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(pythonic::operator_::add(pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft)), pythonic::operator_::mul(self_Kz, vz_fft)), pythonic::operator_::div(1.0, K_square_nozero)))>::type tmp = pythonic::operator_::mul(pythonic::operator_::add(pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft)), pythonic::operator_::mul(self_Kz, vz_fft)), pythonic::operator_::div(1.0, K_square_nozero));
-    typename pythonic::lazy<decltype(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)))>::type n0 = std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft));
-    typename pythonic::lazy<decltype(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)))>::type n1 = std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft));
-    typename pythonic::lazy<decltype(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)))>::type n2 = std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft));
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__project_kradial3d::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type __for_method__OperatorsPseudoSpectral3D__project_kradial3d::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 vx_fft, argument_type4 vy_fft, argument_type5 vz_fft) const
     {
-      long  __target140028821370192 = n0;
-      for (long  i0=0L; i0 < __target140028821370192; i0 += 1L)
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type8;
+      typedef __type8 __type9;
+      typedef decltype(std::declval<__type0>()(std::declval<__type9>())) __type10;
+      typedef decltype(pythonic::operator_::add(std::declval<__type7>(), std::declval<__type10>())) __type11;
+      typedef typename pythonic::assignable<__type11>::type __type12;
+      typedef double __type13;
+      typedef container<typename std::remove_reference<__type13>::type> __type14;
+      typedef typename __combined<__type12,__type14>::type __type15;
+      typedef __type15 __type16;
+      typedef long __type17;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type16>(), std::declval<__type17>())) __type18;
+      typedef indexable<__type18> __type19;
+      typedef typename __combined<__type12,__type19,__type14>::type __type20;
+      typedef typename pythonic::assignable<__type20>::type __type21;
+      __type21 K_square_nozero = pythonic::operator_::add(pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky)), pythonic::numpy::functor::square{}(self_Kz));
+      K_square_nozero.fast(pythonic::operator_::eq(K_square_nozero, 0L)) = 1e-14;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(pythonic::operator_::add(pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft)), pythonic::operator_::mul(self_Kz, vz_fft)), pythonic::operator_::div(1.0, K_square_nozero)))>::type tmp = pythonic::operator_::mul(pythonic::operator_::add(pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft)), pythonic::operator_::mul(self_Kz, vz_fft)), pythonic::operator_::div(1.0, K_square_nozero));
+      typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft))))>::type n0 = std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)));
+      typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft))))>::type n1 = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)));
+      typename pythonic::lazy<decltype(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft))))>::type n2 = std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, vx_fft)));
       {
+        long  __target139658371415344 = n0;
+        for (long  i0=0L; i0 < __target139658371415344; i0 += 1L)
         {
-          long  __target140028821471632 = n1;
-          for (long  i1=0L; i1 < __target140028821471632; i1 += 1L)
           {
+            long  __target139658371557744 = n1;
+            for (long  i1=0L; i1 < __target139658371557744; i1 += 1L)
             {
-              long  __target140028821472208 = n2;
-              for (long  i2=0L; i2 < __target140028821472208; i2 += 1L)
               {
-                vx_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(self_Kx.fast(pythonic::types::make_tuple(i0, i1, i2)), tmp.fast(pythonic::types::make_tuple(i0, i1, i2)));
-                vy_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(self_Ky.fast(pythonic::types::make_tuple(i0, i1, i2)), tmp.fast(pythonic::types::make_tuple(i0, i1, i2)));
-                vz_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(self_Kz.fast(pythonic::types::make_tuple(i0, i1, i2)), tmp.fast(pythonic::types::make_tuple(i0, i1, i2)));
+                long  __target139658371558320 = n2;
+                for (long  i2=0L; i2 < __target139658371558320; i2 += 1L)
+                {
+                  vx_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::types::as_const(self_Kx).fast(pythonic::types::make_tuple(i0, i1, i2)), pythonic::types::as_const(tmp).fast(pythonic::types::make_tuple(i0, i1, i2)));
+                  vy_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::types::as_const(self_Ky).fast(pythonic::types::make_tuple(i0, i1, i2)), pythonic::types::as_const(tmp).fast(pythonic::types::make_tuple(i0, i1, i2)));
+                  vz_fft.fast(pythonic::types::make_tuple(i0, i1, i2)) = pythonic::operator_::mul(pythonic::types::as_const(self_Kz).fast(pythonic::types::make_tuple(i0, i1, i2)), pythonic::types::as_const(tmp).fast(pythonic::types::make_tuple(i0, i1, i2)));
+                }
               }
             }
           }
         }
       }
+      return pythonic::builtins::None;
     }
-    return pythonic::builtins::None;
-  }
-  inline
-  typename __code_new_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::operator()() const
-  {
+    inline
+    typename __code_new_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::type::result_type __code_new_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::operator()() const
     {
-      static typename __code_new_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft):\n    return backend_func(self.Kx, self.Ky, vx_fft, vy_fft)\n\n");
-      return tmp_global;
+      {
+        static typename __code_new_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::type::result_type tmp_global = pythonic::types::str("\n\ndef new_method(self, vx_fft, vy_fft):\n    return backend_func(self.Kx, self.Ky, vx_fft, vy_fft)\n\n");
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& vx_fft, argument_type3&& vy_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
-    typedef __type1 __type2;
-    typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-    typedef __type4 __type5;
-    typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
-    typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef double __type9;
-    typedef container<typename std::remove_reference<__type9>::type> __type10;
-    typedef typename __combined<__type8,__type10>::type __type11;
-    typedef __type11 __type12;
-    typedef long __type13;
-    typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
-    typedef indexable<__type14> __type15;
-    typedef typename __combined<__type8,__type15,__type10>::type __type16;
-    typedef typename pythonic::assignable<__type16>::type __type17;
-    __type17 inv_Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
-    inv_Kh_square_nozero.fast(pythonic::operator_::eq(inv_Kh_square_nozero, 0L)) = 1e-14;
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1L, inv_Kh_square_nozero))>::type inv_Kh_square_nozero_ = pythonic::operator_::div(1L, inv_Kh_square_nozero);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft)))>::type kdotu_fft = pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft));
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(pythonic::operator_::mul(kdotu_fft, self_Kx), inv_Kh_square_nozero_))>::type udx_fft = pythonic::operator_::mul(pythonic::operator_::mul(kdotu_fft, self_Kx), inv_Kh_square_nozero_);
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(pythonic::operator_::mul(kdotu_fft, self_Ky), inv_Kh_square_nozero_))>::type udy_fft = pythonic::operator_::mul(pythonic::operator_::mul(kdotu_fft, self_Ky), inv_Kh_square_nozero_);
-    return pythonic::types::make_tuple(pythonic::operator_::sub(vx_fft, udx_fft), pythonic::operator_::sub(vy_fft, udy_fft), udx_fft, udy_fft);
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-  inline
-  typename compute_energy_from_3fields::type<argument_type0, argument_type1, argument_type2>::result_type compute_energy_from_3fields::operator()(argument_type0&& vx, argument_type1&& vy, argument_type2&& vz) const
-  {
-    return pythonic::operator_::mul(0.5, pythonic::operator_::add(pythonic::operator_::add(pythonic::builtins::pythran::functor::abssqr{}(vx), pythonic::builtins::pythran::functor::abssqr{}(vy)), pythonic::builtins::pythran::functor::abssqr{}(vz)));
-  }
-  template <typename argument_type0 , typename argument_type1 >
-  inline
-  typename compute_energy_from_2fields::type<argument_type0, argument_type1>::result_type compute_energy_from_2fields::operator()(argument_type0&& vx, argument_type1&& vy) const
-  {
-    return pythonic::operator_::mul(0.5, pythonic::operator_::add(pythonic::builtins::pythran::functor::abssqr{}(vx), pythonic::builtins::pythran::functor::abssqr{}(vy)));
-  }
-  template <typename argument_type0 , typename argument_type1 >
-  inline
-  typename compute_energy_from_1field_with_coef::type<argument_type0, argument_type1>::result_type compute_energy_from_1field_with_coef::operator()(argument_type0&& arr, argument_type1&& coef) const
-  {
-    return pythonic::operator_::mul(pythonic::operator_::mul(0.5, coef), pythonic::builtins::pythran::functor::abssqr{}(arr));
-  }
-  template <typename argument_type0 >
-  inline
-  typename compute_energy_from_1field::type<argument_type0>::result_type compute_energy_from_1field::operator()(argument_type0&& arr) const
-  {
-    return pythonic::operator_::mul(0.5, pythonic::builtins::pythran::functor::abssqr{}(arr));
-  }
-  template <typename argument_type0 , typename argument_type1 >
-  inline
-  typename dealiasing_variable::type<argument_type0, argument_type1>::result_type dealiasing_variable::operator()(argument_type0&& ff_fft, argument_type1&& where_dealiased) const
-  {
-    typename pythonic::lazy<decltype(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft)))>::type n0 = std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft));
-    typename pythonic::lazy<decltype(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft)))>::type n1 = std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft));
-    typename pythonic::lazy<decltype(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft)))>::type n2 = std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft));
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::type<argument_type0, argument_type1, argument_type2, argument_type3>::result_type __for_method__OperatorsPseudoSpectral3D__urudfft_from_vxvyfft::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 vx_fft, argument_type3 vy_fft) const
+    {
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type1;
+      typedef __type1 __type2;
+      typedef decltype(std::declval<__type0>()(std::declval<__type2>())) __type3;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
+      typedef __type4 __type5;
+      typedef decltype(std::declval<__type0>()(std::declval<__type5>())) __type6;
+      typedef decltype(pythonic::operator_::add(std::declval<__type3>(), std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef double __type9;
+      typedef container<typename std::remove_reference<__type9>::type> __type10;
+      typedef typename __combined<__type8,__type10>::type __type11;
+      typedef __type11 __type12;
+      typedef long __type13;
+      typedef decltype(pythonic::operator_::eq(std::declval<__type12>(), std::declval<__type13>())) __type14;
+      typedef indexable<__type14> __type15;
+      typedef typename __combined<__type8,__type15,__type10>::type __type16;
+      typedef typename pythonic::assignable<__type16>::type __type17;
+      __type17 inv_Kh_square_nozero = pythonic::operator_::add(pythonic::numpy::functor::square{}(self_Kx), pythonic::numpy::functor::square{}(self_Ky));
+      inv_Kh_square_nozero.fast(pythonic::operator_::eq(inv_Kh_square_nozero, 0L)) = 1e-14;
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(1L, inv_Kh_square_nozero))>::type inv_Kh_square_nozero_ = pythonic::operator_::div(1L, inv_Kh_square_nozero);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft)))>::type kdotu_fft = pythonic::operator_::add(pythonic::operator_::mul(self_Kx, vx_fft), pythonic::operator_::mul(self_Ky, vy_fft));
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(pythonic::operator_::mul(kdotu_fft, self_Kx), inv_Kh_square_nozero_))>::type udx_fft = pythonic::operator_::mul(pythonic::operator_::mul(kdotu_fft, self_Kx), inv_Kh_square_nozero_);
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::mul(pythonic::operator_::mul(kdotu_fft, self_Ky), inv_Kh_square_nozero_))>::type udy_fft = pythonic::operator_::mul(pythonic::operator_::mul(kdotu_fft, self_Ky), inv_Kh_square_nozero_);
+      return pythonic::types::make_tuple(pythonic::operator_::sub(vx_fft, udx_fft), pythonic::operator_::sub(vy_fft, udy_fft), udx_fft, udy_fft);
+    }
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+    inline
+    typename compute_energy_from_3fields::type<argument_type0, argument_type1, argument_type2>::result_type compute_energy_from_3fields::operator()(argument_type0 vx, argument_type1 vy, argument_type2 vz) const
+    {
+      return pythonic::operator_::mul(0.5, pythonic::operator_::add(pythonic::operator_::add(pythonic::builtins::pythran::functor::abssqr{}(vx), pythonic::builtins::pythran::functor::abssqr{}(vy)), pythonic::builtins::pythran::functor::abssqr{}(vz)));
+    }
+    template <typename argument_type0 , typename argument_type1 >
+    inline
+    typename compute_energy_from_2fields::type<argument_type0, argument_type1>::result_type compute_energy_from_2fields::operator()(argument_type0 vx, argument_type1 vy) const
+    {
+      return pythonic::operator_::mul(0.5, pythonic::operator_::add(pythonic::builtins::pythran::functor::abssqr{}(vx), pythonic::builtins::pythran::functor::abssqr{}(vy)));
+    }
+    template <typename argument_type0 , typename argument_type1 >
+    inline
+    typename compute_energy_from_1field_with_coef::type<argument_type0, argument_type1>::result_type compute_energy_from_1field_with_coef::operator()(argument_type0 arr, argument_type1 coef) const
+    {
+      return pythonic::operator_::mul(pythonic::operator_::mul(0.5, coef), pythonic::builtins::pythran::functor::abssqr{}(arr));
+    }
+    template <typename argument_type0 >
+    inline
+    typename compute_energy_from_1field::type<argument_type0>::result_type compute_energy_from_1field::operator()(argument_type0 arr) const
+    {
+      return pythonic::operator_::mul(0.5, pythonic::builtins::pythran::functor::abssqr{}(arr));
+    }
+    template <typename argument_type0 , typename argument_type1 >
+    inline
+    typename dealiasing_variable::type<argument_type0, argument_type1>::result_type dealiasing_variable::operator()(argument_type0 ff_fft, argument_type1 where_dealiased) const
     {
-      long  __target140028821162592 = n0;
-      for (long  i0=0L; i0 < __target140028821162592; i0 += 1L)
+      typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft))))>::type n0 = std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft)));
+      typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft))))>::type n1 = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft)));
+      typename pythonic::lazy<decltype(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft))))>::type n2 = std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, ff_fft)));
       {
+        long  __target139658375872032 = n0;
+        for (long  i0=0L; i0 < __target139658375872032; i0 += 1L)
         {
-          long  __target140028821165616 = n1;
-          for (long  i1=0L; i1 < __target140028821165616; i1 += 1L)
           {
+            long  __target139658375943600 = n1;
+            for (long  i1=0L; i1 < __target139658375943600; i1 += 1L)
             {
-              long  __target140028821166192 = n2;
-              for (long  i2=0L; i2 < __target140028821166192; i2 += 1L)
               {
-                if (where_dealiased[pythonic::types::make_tuple(i0, i1, i2)])
+                long  __target139658375944944 = n2;
+                for (long  i2=0L; i2 < __target139658375944944; i2 += 1L)
                 {
-                  ff_fft[pythonic::types::make_tuple(i0, i1, i2)] = 0.0;
+                  if (pythonic::types::as_const(where_dealiased)[pythonic::types::make_tuple(i0, i1, i2)])
+                  {
+                    ff_fft[pythonic::types::make_tuple(i0, i1, i2)] = 0.0;
+                  }
                 }
               }
             }
           }
         }
       }
+      return pythonic::builtins::None;
     }
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 >
-  inline
-  typename dealiasing_setofvar::type<argument_type0, argument_type1>::result_type dealiasing_setofvar::operator()(argument_type0&& sov, argument_type1&& where_dealiased) const
-  {
-    typename pythonic::lazy<decltype(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)))>::type nk = std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov));
-    typename pythonic::lazy<decltype(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)))>::type n0 = std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov));
-    typename pythonic::lazy<decltype(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)))>::type n1 = std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov));
-    typename pythonic::lazy<decltype(std::get<3>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)))>::type n2 = std::get<3>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov));
+    template <typename argument_type0 , typename argument_type1 >
+    inline
+    typename dealiasing_setofvar::type<argument_type0, argument_type1>::result_type dealiasing_setofvar::operator()(argument_type0 sov, argument_type1 where_dealiased) const
     {
-      long  __target140028821148128 = n0;
-      for (long  i0=0L; i0 < __target140028821148128; i0 += 1L)
+      typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov))))>::type nk = std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)));
+      typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov))))>::type n0 = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)));
+      typename pythonic::lazy<decltype(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov))))>::type n1 = std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)));
+      typename pythonic::lazy<decltype(std::get<3>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov))))>::type n2 = std::get<3>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, sov)));
       {
+        long  __target139658373581600 = n0;
+        for (long  i0=0L; i0 < __target139658373581600; i0 += 1L)
         {
-          long  __target140028821149280 = n1;
-          for (long  i1=0L; i1 < __target140028821149280; i1 += 1L)
           {
+            long  __target139658376023584 = n1;
+            for (long  i1=0L; i1 < __target139658376023584; i1 += 1L)
             {
-              long  __target140028821162208 = n2;
-              for (long  i2=0L; i2 < __target140028821162208; i2 += 1L)
               {
-                if (where_dealiased[pythonic::types::make_tuple(i0, i1, i2)])
+                long  __target139658375871648 = n2;
+                for (long  i2=0L; i2 < __target139658375871648; i2 += 1L)
                 {
+                  if (pythonic::types::as_const(where_dealiased)[pythonic::types::make_tuple(i0, i1, i2)])
                   {
-                    long  __target140028821163360 = nk;
-                    for (long  ik=0L; ik < __target140028821163360; ik += 1L)
                     {
-                      sov[pythonic::types::make_tuple(ik, i0, i1, i2)] = 0.0;
+                      long  __target139658374902112 = nk;
+                      for (long  ik=0L; ik < __target139658374902112; ik += 1L)
+                      {
+                        sov[pythonic::types::make_tuple(ik, i0, i1, i2)] = 0.0;
+                      }
                     }
                   }
                 }
               }
             }
           }
         }
       }
+      return pythonic::builtins::None;
+    }
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+    inline
+    typename __for_method__OperatorsPseudoSpectral3D__get_phases_random::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type __for_method__OperatorsPseudoSpectral3D__get_phases_random::operator()(argument_type0 self_Kx, argument_type1 self_Ky, argument_type2 self_Kz, argument_type3 self_deltax, argument_type4 self_deltay, argument_type5 self_deltaz) const
+    {
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::tuple{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::map{})>::type>::type __type1;
+      typedef __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0 __type2;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type3;
+      typedef long __type4;
+      typedef decltype(std::declval<__type3>()(std::declval<__type4>())) __type5;
+      typedef decltype(std::declval<__type1>()(std::declval<__type2>(), std::declval<__type5>())) __type6;
+      typedef decltype(std::declval<__type0>()(std::declval<__type6>())) __type7;
+      typedef typename pythonic::assignable<__type7>::type __type8;
+      typedef std::integral_constant<long,0> __type9;
+      typedef __type8 __type10;
+      typedef decltype(pythonic::types::as_const(std::declval<__type10>())) __type11;
+      typedef typename std::tuple_element<0,typename std::remove_reference<__type11>::type>::type __type12;
+      typedef indexable_container<__type9, typename std::remove_reference<__type12>::type> __type13;
+      typedef std::integral_constant<long,1> __type14;
+      typedef typename __combined<__type8,__type13>::type __type15;
+      typedef __type15 __type16;
+      typedef decltype(pythonic::types::as_const(std::declval<__type16>())) __type17;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type17>::type>::type __type18;
+      typedef indexable_container<__type14, typename std::remove_reference<__type18>::type> __type19;
+      typedef std::integral_constant<long,2> __type20;
+      typedef typename __combined<__type8,__type13,__type19>::type __type21;
+      typedef __type21 __type22;
+      typedef decltype(pythonic::types::as_const(std::declval<__type22>())) __type23;
+      typedef typename std::tuple_element<2,typename std::remove_reference<__type23>::type>::type __type24;
+      typedef indexable_container<__type20, typename std::remove_reference<__type24>::type> __type25;
+      typedef typename __combined<__type8,__type13,__type19,__type25>::type __type26;
+      typedef typename pythonic::assignable<__type26>::type __type27;
+      __type27 __tuple0 = pythonic::builtins::functor::tuple{}(pythonic::builtins::functor::map{}(__for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0(), pythonic::builtins::functor::range{}(3L)));
+      typename pythonic::assignable_noescape<decltype(std::get<0>(pythonic::types::as_const(__tuple0)))>::type alpha_x = std::get<0>(pythonic::types::as_const(__tuple0));
+      typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(__tuple0)))>::type alpha_y = std::get<1>(pythonic::types::as_const(__tuple0));
+      typename pythonic::assignable_noescape<decltype(std::get<2>(pythonic::types::as_const(__tuple0)))>::type alpha_z = std::get<2>(pythonic::types::as_const(__tuple0));
+      return pythonic::types::make_tuple(pythonic::operator_::add(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(alpha_x, self_deltax), self_Kx), pythonic::operator_::mul(pythonic::operator_::mul(alpha_y, self_deltay), self_Ky)), pythonic::operator_::mul(pythonic::operator_::mul(alpha_z, self_deltaz), self_Kz)), pythonic::operator_::add(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_x, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_x, 0.5)), decltype(pythonic::operator_::sub(alpha_x, 0.5))>::type(pythonic::operator_::add(alpha_x, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_x, 0.5)), decltype(pythonic::operator_::sub(alpha_x, 0.5))>::type(pythonic::operator_::sub(alpha_x, 0.5))), self_deltax), self_Kx), pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_y, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_y, 0.5)), decltype(pythonic::operator_::sub(alpha_y, 0.5))>::type(pythonic::operator_::add(alpha_y, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_y, 0.5)), decltype(pythonic::operator_::sub(alpha_y, 0.5))>::type(pythonic::operator_::sub(alpha_y, 0.5))), self_deltay), self_Ky)), pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_z, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_z, 0.5)), decltype(pythonic::operator_::sub(alpha_z, 0.5))>::type(pythonic::operator_::add(alpha_z, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_z, 0.5)), decltype(pythonic::operator_::sub(alpha_z, 0.5))>::type(pythonic::operator_::sub(alpha_z, 0.5))), self_deltaz), self_Kz)));
     }
-    return pythonic::builtins::None;
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-  inline
-  typename __for_method__OperatorsPseudoSpectral3D__get_phases_random::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type __for_method__OperatorsPseudoSpectral3D__get_phases_random::operator()(argument_type0&& self_Kx, argument_type1&& self_Ky, argument_type2&& self_Kz, argument_type3&& self_deltax, argument_type4&& self_deltay, argument_type5&& self_deltaz) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::tuple{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::map{})>::type>::type __type1;
-    typedef __for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0 __type2;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type3;
-    typedef long __type4;
-    typedef decltype(std::declval<__type3>()(std::declval<__type4>())) __type5;
-    typedef decltype(std::declval<__type1>()(std::declval<__type2>(), std::declval<__type5>())) __type6;
-    typedef decltype(std::declval<__type0>()(std::declval<__type6>())) __type7;
-    typedef typename pythonic::assignable<__type7>::type __type8;
-    typedef std::integral_constant<long,0> __type9;
-    typedef __type8 __type10;
-    typedef typename std::tuple_element<0,typename std::remove_reference<__type10>::type>::type __type11;
-    typedef indexable_container<__type9, typename std::remove_reference<__type11>::type> __type12;
-    typedef std::integral_constant<long,1> __type13;
-    typedef typename __combined<__type8,__type12>::type __type14;
-    typedef __type14 __type15;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type15>::type>::type __type16;
-    typedef indexable_container<__type13, typename std::remove_reference<__type16>::type> __type17;
-    typedef std::integral_constant<long,2> __type18;
-    typedef typename __combined<__type8,__type12,__type17>::type __type19;
-    typedef __type19 __type20;
-    typedef typename std::tuple_element<2,typename std::remove_reference<__type20>::type>::type __type21;
-    typedef indexable_container<__type18, typename std::remove_reference<__type21>::type> __type22;
-    typedef typename __combined<__type8,__type12,__type17,__type22>::type __type23;
-    typedef typename pythonic::assignable<__type23>::type __type24;
-    __type24 __tuple0 = pythonic::builtins::functor::tuple{}(pythonic::builtins::functor::map{}(__for_method__OperatorsPseudoSpectral3D__get_phases_random_lambda0(), pythonic::builtins::functor::range{}(3L)));
-    typename pythonic::assignable_noescape<decltype(std::get<0>(__tuple0))>::type alpha_x = std::get<0>(__tuple0);
-    typename pythonic::assignable_noescape<decltype(std::get<1>(__tuple0))>::type alpha_y = std::get<1>(__tuple0);
-    typename pythonic::assignable_noescape<decltype(std::get<2>(__tuple0))>::type alpha_z = std::get<2>(__tuple0);
-    return pythonic::types::make_tuple(pythonic::operator_::add(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul(alpha_x, self_deltax), self_Kx), pythonic::operator_::mul(pythonic::operator_::mul(alpha_y, self_deltay), self_Ky)), pythonic::operator_::mul(pythonic::operator_::mul(alpha_z, self_deltaz), self_Kz)), pythonic::operator_::add(pythonic::operator_::add(pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_x, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_x, 0.5)), decltype(pythonic::operator_::sub(alpha_x, 0.5))>::type(pythonic::operator_::add(alpha_x, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_x, 0.5)), decltype(pythonic::operator_::sub(alpha_x, 0.5))>::type(pythonic::operator_::sub(alpha_x, 0.5))), self_deltax), self_Kx), pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_y, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_y, 0.5)), decltype(pythonic::operator_::sub(alpha_y, 0.5))>::type(pythonic::operator_::add(alpha_y, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_y, 0.5)), decltype(pythonic::operator_::sub(alpha_y, 0.5))>::type(pythonic::operator_::sub(alpha_y, 0.5))), self_deltay), self_Ky)), pythonic::operator_::mul(pythonic::operator_::mul((((bool)pythonic::operator_::lt(alpha_z, 0L)) ? typename __combined<decltype(pythonic::operator_::add(alpha_z, 0.5)), decltype(pythonic::operator_::sub(alpha_z, 0.5))>::type(pythonic::operator_::add(alpha_z, 0.5)) : typename __combined<decltype(pythonic::operator_::add(alpha_z, 0.5)), decltype(pythonic::operator_::sub(alpha_z, 0.5))>::type(pythonic::operator_::sub(alpha_z, 0.5))), self_deltaz), self_Kz)));
   }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_operators3d::__transonic__()());
 static PyObject* __code_new_method__OperatorsPseudoSpectral3D__get_phases_random = to_python(__pythran_operators3d::__code_new_method__OperatorsPseudoSpectral3D__get_phases_random()());
 inline
@@ -3153,17 +3183,17 @@
                                                      Methods,
                                                      ""
                 );
                 #endif
                 if(! theModule)
                     PYTHRAN_RETURN;
                 PyObject * theDoc = Py_BuildValue("(sss)",
-                                                  "0.12.0",
-                                                  "2022-10-28 09:10:31.280598",
-                                                  "c18106bdfcd251fb565916b074ada1407ce12ad520c8a454be57c3b24b3aea65");
+                                                  "0.13.1",
+                                                  "2023-05-24 11:29:41.880503",
+                                                  "f19181467380adab9a1d2838e6b55e731a7955428aff4a33b0bf5b7ffda4b90f");
                 if(! theDoc)
                     PYTHRAN_RETURN;
                 PyModule_AddObject(theModule,
                                    "__pythran__",
                                    theDoc);
 
                 PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/operators/base.py` & `fluidsim-0.7.3/fluidsim/operators/base.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/operators/op_finitediff1d.py` & `fluidsim-0.7.3/fluidsim/operators/op_finitediff1d.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/operators/op_finitediff2d.py` & `fluidsim-0.7.3/fluidsim/operators/op_finitediff2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     def _complete_params_with_default(params):
         """This static method is used to complete the *params* container."""
 
         attribs = {"nx": 48, "ny": 48, "Lx": 8, "Ly": 8}
         params._set_child("oper", attribs=attribs)
 
     def __init__(self, params=None):
-
         Lx = float(params.oper.Lx)
         Ly = float(params.oper.Ly)
 
         if not params.ONLY_COARSE_OPER:
             nx = int(params.oper.nx)
             ny = int(params.oper.ny)
         else:
```

### Comparing `fluidsim-0.7.2/fluidsim/operators/operators0d.py` & `fluidsim-0.7.3/fluidsim/operators/operators0d.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/operators/operators1d.py` & `fluidsim-0.7.3/fluidsim/operators/operators1d.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/operators/operators2d.py` & `fluidsim-0.7.3/fluidsim/operators/operators2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 if nb_proc > 1:
     MPI = mpi.MPI
     comm = mpi.comm
 
 
 @boost
 class OperatorsPseudoSpectral2D(_Operators, OperatorBase):
-
     _has_to_dealiase: bool
     where_dealiased: "uint8[:, :]"
     KX: Af
     KY: Af
     deltax: float
     deltay: float
 
@@ -110,15 +109,14 @@
             "truncation_shape": "cubic",
             "NO_SHEAR_MODES": False,
             "NO_KY0": False,
         }
         params._set_child("oper", attribs=attribs)
 
     def __init__(self, params):
-
         self.params = params
         self.axes = ("y", "x")
         nx = int(params.oper.nx)
         ny = int(params.oper.ny)
 
         if params.oper.nx != nx:
             raise ValueError(
@@ -604,15 +602,14 @@
                     kynodim = ikyc - nKyc
                     iky = kynodim + nKy
 
                 for ikxc in range(nKxc):
                     arr[iky, ikxc] = arr_coarse[ikyc, ikxc]
 
     def get_grid1d_seq(self, axis="x"):
-
         if axis not in ("x", "y"):
             raise ValueError
 
         if self.params.ONLY_COARSE_OPER:
             number_points = getattr(self.params.oper, "n" + axis)
             length = getattr(self, "L" + axis)
             return np.linspace(0, length, number_points)
```

### Comparing `fluidsim-0.7.2/fluidsim/operators/operators3d.py` & `fluidsim-0.7.3/fluidsim/operators/operators3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,14 @@
 
     Length of the edges of the numerical domain.
 
 """
         )
 
     def __init__(self, params=None):
-
         self.params = params
         self.axes = ("z", "y", "x")
 
         params.oper.nx = int(params.oper.nx)
         params.oper.ny = int(params.oper.ny)
         params.oper.nz = int(params.oper.nz)
 
@@ -555,15 +554,14 @@
             nk0c, nk1c, nk2c = nkyc, nkxc, nkzc
         else:
             raise NotImplementedError
 
         fc_fft_tmp = np.zeros([nk0c, nk1c, nk2c], np.complex128)
         nk0, nk1, nk2 = self.shapeK_seq
         if self.shapeK_seq[1:2] == self.shapeK_loc[1:2]:
-
             f1d_temp = np.empty([nk1c, nk2c], np.complex128)
 
             for ik0c in range(min(nk0c, nk0)):
                 ik1c = 0
                 ik2c = 0
                 ik0 = _ik_from_ikc(ik0c, nk0c, nk0, is_x=(position_x_K == 0))
                 rank_ik, ik0loc, ik1loc, ik1loc = self.where_is_wavenumber(
@@ -594,15 +592,14 @@
                         comm.Send(
                             [f1d_temp, MPI.DOUBLE_COMPLEX], dest=0, tag=ik0c
                         )
                 if rank == 0:
                     # copy into fc_fft
                     fc_fft_tmp[ik0c] = f1d_temp.copy()
         else:
-
             for ik0c in range(min(nk0c, nk0)):
                 ik0 = _ik_from_ikc(ik0c, nk0c, nk0, is_x=(position_x_K == 0))
                 for ik1c in range(min(nk1c, nk1)):
                     ik1 = _ik_from_ikc(ik1c, nk1c, nk1, is_x=(position_x_K == 1))
                     for ik2c in range(min(nk2c, nk2)):
                         ik2 = _ik_from_ikc(
                             ik2c, nk2c, nk2, is_x=(position_x_K == 2)
@@ -627,15 +624,14 @@
                             elif rank == 0:
                                 f0d_temp = comm.recv(source=rank_ik, tag=ik2c)
 
                         if rank == 0:
                             fc_fft_tmp[ik0c, ik1c, ik2c] = f0d_temp
 
         if rank == 0:
-
             # print(f"{fc_fft_tmp = }")
 
             fc_fft = np.zeros(shapeK_coarse, dtype=np.complex128)
             if self.dimX_K == (1, 0, 2):
                 for i0 in range(nkzc):
                     for i1 in range(nkyc):
                         fc_fft[i0, i1, :] = fc_fft_tmp[i1, i0, :]
@@ -676,15 +672,14 @@
                     if ik0 < iK0loc_start:
                         rank_k -= 1
                         break
             ik0_loc = ik0 - self.iK0loc_start_rank[rank_k]
             ik1_loc = ik1
             ik2_loc = ik2
         else:
-
             iki_first = self.seq_indices_first_K
             rank_k_equal_rank = (
                 iki_first[0] <= ik0 < iki_first[0] + self.shapeK_loc[0]
                 and iki_first[1] <= ik1 < iki_first[1] + self.shapeK_loc[1]
                 and iki_first[2] <= ik2 < iki_first[2] + self.shapeK_loc[2]
             )
             tmp = comm.allgather(rank_k_equal_rank)
@@ -999,26 +994,24 @@
     @boost
     def divhfft_from_vxvyfft(self, vx_fft: Ac, vy_fft: Ac):
         """Compute the horizontal divergence in spectral space."""
         return 1j * (self.Kx * vx_fft + self.Ky * vy_fft)
 
     @boost
     def vxvyfft_from_rotzfft(self, rotz_fft: Ac):
-
         inv_Kh_square_nozero = self.Kx**2 + self.Ky**2
         inv_Kh_square_nozero[inv_Kh_square_nozero == 0] = 1e-14
         inv_Kh_square_nozero = 1 / inv_Kh_square_nozero
 
         vx_fft = 1j * self.Ky * inv_Kh_square_nozero * rotz_fft
         vy_fft = -1j * self.Kx * inv_Kh_square_nozero * rotz_fft
         return vx_fft, vy_fft
 
     @boost
     def vxvyfft_from_divhfft(self, divh_fft: Ac):
-
         inv_Kh_square_nozero = self.Kx**2 + self.Ky**2
         inv_Kh_square_nozero[inv_Kh_square_nozero == 0] = 1e-14
         inv_Kh_square_nozero = 1 / inv_Kh_square_nozero
 
         vx_fft = -1j * self.Kx * inv_Kh_square_nozero * divh_fft
         vy_fft = -1j * self.Ky * inv_Kh_square_nozero * divh_fft
         return vx_fft, vy_fft
@@ -1041,15 +1034,14 @@
             dx_arr_fft_flat[i] = 1j * Kx[i] * value
             dy_arr_fft_flat[i] = 1j * Ky[i] * value
             dz_arr_fft_flat[i] = 1j * Kz[i] * value
 
         return dx_arr_fft, dy_arr_fft, dz_arr_fft
 
     def get_grid1d_seq(self, axis="x"):
-
         if axis not in ("x", "y", "z"):
             raise ValueError
 
         if self.params.ONLY_COARSE_OPER:
             number_points = getattr(self.params.oper, "n" + axis)
             length = getattr(self, "L" + axis)
             return np.linspace(0, length, number_points)
```

### Comparing `fluidsim-0.7.2/fluidsim/operators/sphericalharmo.py` & `fluidsim-0.7.3/fluidsim/operators/sphericalharmo.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,9 +70,8 @@
         # set_grid based on params.nlat and params.nlon and other flags
         # rebuild lats and lons
         # else:
         return getattr(self, axis + "s")
 
 
 if __name__ == "__main__":
-
     oper = OperatorsSphericalHarmonics()
```

### Comparing `fluidsim-0.7.2/fluidsim/operators/test/test_operators2d.py` & `fluidsim-0.7.3/fluidsim/operators/test/test_operators2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,14 @@
     @property
     def Oper(self):
         from fluidsim.operators.operators2d import OperatorsPseudoSpectral2D
 
         return OperatorsPseudoSpectral2D
 
     def test_coarse(self, allclose):
-
         params = self.Oper._create_default_params()
         params.oper.nx = 16
         params.oper.ny = 12
         if self.nb_dim == 3:
             params.oper.nz = 16
 
         params.oper.truncation_shape = "spherical"
```

### Comparing `fluidsim-0.7.2/fluidsim/operators/test/test_operators3d.py` & `fluidsim-0.7.3/fluidsim/operators/test/test_operators3d.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ad1d/init_fields.py` & `fluidsim-0.7.3/fluidsim/solvers/ad1d/init_fields.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ad1d/output/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/ad1d/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ad1d/pseudo_spect/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ad1d/pseudo_spect/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     @staticmethod
     def _complete_params_with_default(params):
         SimulBasePseudoSpectral._complete_params_with_default(params)
         params._set_attrib("U", 1.0)
 
     def tendencies_nonlin(self, state_spect=None, old=None):
-
         if old is None:
             tendencies_fft = SetOfVariables(
                 like=self.state.state_spect, info="tendencies_nonlin"
             )
         else:
             tendencies_fft = old
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ad1d/pseudo_spect/state.py` & `fluidsim-0.7.3/fluidsim/solvers/ad1d/pseudo_spect/state.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ad1d/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ad1d/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from fluidsim.base.solvers.base import SimulBase
 from fluidsim.base.setofvariables import SetOfVariables
 from fluidsim.base.solvers.finite_diff import InfoSolverFiniteDiff
 
 
 class InfoSolverAD1D(InfoSolverFiniteDiff):
     def _init_root(self):
-
         super()._init_root()
 
         package = "fluidsim.solvers.ad1d"
         self.module_name = package + ".solver"
         self.class_name = "Simul"
         self.short_name = "AD1D"
 
@@ -82,15 +81,14 @@
         return (
             self.params.nu_2 * (self.oper.sparse_pxx)
             - self.params.U * self.oper.sparse_px
         )
 
 
 if __name__ == "__main__":
-
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.U = 1.0
 
     params.short_name_type_run = "test"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ad1d/state.py` & `fluidsim-0.7.3/fluidsim/solvers/ad1d/state.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ad1d/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ad1d/test_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from fluidsim.solvers.ad1d.solver import Simul
 
 from fluidsim.util.testing import TestSimul
 
 
 @unittest.skipIf(not scipy_installed, "No module named scipy.sparse")
 class TestSolverAD1D(TestSimul):
-
     Simul = Simul
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
 
         # RuntimeWarnings are very common when numpy installed and numpy
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/burgers1d/skew_sym/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/burgers1d/skew_sym/solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         self.short_name = "BurgersSkewSym1D"
 
 
 class Simul(SimulBurgers):
     InfoSolver = InfoSolver
 
     def tendencies_nonlin(self, state_spect=None, old=None):
-
         if state_spect is None:
             u_fft = self.state.state_spect.get_var("u_fft")
             signal = self.state.state_phys.get_var("u")
         else:
             u_fft = state_spect.get_var("u_fft")
             signal = self.oper.ifft(u_fft)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/burgers1d/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/burgers1d/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         classes.Output.class_name = "Output"
 
 
 class Simul(SimulBasePseudoSpectral):
     InfoSolver = InfoSolver
 
     def tendencies_nonlin(self, state_spect=None, old=None):
-
         if state_spect is None:
             u_fft = self.state.state_spect.get_var("u_fft")
             signal = self.state.state_phys.get_var("u")
         else:
             u_fft = state_spect.get_var("u_fft")
             signal = self.oper.ifft(u_fft)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/burgers1d/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/burgers1d/test_solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 @skip_if_no_fluidfft
 class TestSolverSquare1D(TestSimul):
     Simul = Simul
 
     @classmethod
     def init_params(cls):
-
         params = cls.params = cls.Simul.create_default_params()
 
         params.short_name_type_run = "test"
         params.output.sub_directory = "unittests"
 
         params.oper.nx = 40
         params.oper.Lx = 1.0
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/models0d/lorenz/output/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/models0d/lorenz/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/models0d/lorenz/output/print_stdout.py` & `fluidsim-0.7.3/fluidsim/solvers/models0d/lorenz/output/print_stdout.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
     Used to print in both the stdout and the stdout.txt file, and also
     to print simple info on the current state of the simulation.
 
     """
 
     def complete_init_with_state(self):
-
         if self.period_print == 0:
             return
 
         self.t_last_print_info = -self.period_print
 
         self.print_stdout = self.__call__
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/models0d/lorenz/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/models0d/lorenz/solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/models0d/predaprey/output/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/models0d/predaprey/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/models0d/predaprey/output/print_stdout.py` & `fluidsim-0.7.3/fluidsim/solvers/models0d/predaprey/output/print_stdout.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
     Used to print in both the stdout and the stdout.txt file, and also
     to print simple info on the current state of the simulation.
 
     """
 
     def complete_init_with_state(self):
-
         self.potential0 = self.output.compute_potential()
 
         if self.period_print == 0:
             return
 
         self.potential_tmp = self.potential0
         self.t_last_print_info = -self.period_print
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/models0d/predaprey/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/models0d/predaprey/solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/models0d/test_lorenz.py` & `fluidsim-0.7.3/fluidsim/solvers/models0d/test_lorenz.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/models0d/test_predaprey.py` & `fluidsim-0.7.3/fluidsim/solvers/models0d/test_predaprey.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/nl1d/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/nl1d/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
     @staticmethod
     def _complete_params_with_default(params):
         SimulBasePseudoSpectral._complete_params_with_default(params)
         params._set_attrib("sigma", 1.0)
 
     def tendencies_nonlin(self, state_spect=None, old=None):
-
         if state_spect is None:
             signal = self.state.state_phys.get_var("s")
         else:
             s_fft = state_spect.get_var("s_fft")
             signal = self.oper.ifft(s_fft)
 
         f_signal = -np.sign(signal) * self.params.sigma * signal**2
@@ -70,15 +69,14 @@
         f_fft = tendencies_fft.get_var("s_fft")
         self.oper.fft_as_arg(f_signal, f_fft)
         self.oper.dealiasing(tendencies_fft)
         return tendencies_fft
 
 
 if __name__ == "__main__":
-
     from scipy.signal import gausspulse
 
     params = Simul.create_default_params()
     params.output.sub_directory = "examples"
 
     params.output.periods_save.phys_fields = 1.0
     params.short_name_type_run = "test"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/nl1d/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/nl1d/test_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 @skip_if_no_fluidfft
 @skip_if_mpi
 class TestSolverSquare1D(TestSimul):
     Simul = Simul
 
     @classmethod
     def init_params(cls):
-
         params = cls.params = cls.Simul.create_default_params()
 
         params.short_name_type_run = "test"
         params.output.sub_directory = "unittests"
 
         params.oper.nx = 40
         params.oper.Lx = 1.0
@@ -58,15 +57,14 @@
     Simul = Simul
     deltat = 2e-4
     k_init = 10
     amplitude = 0.7
 
     @classmethod
     def init_params(cls):
-
         params = cls.params = cls.Simul.create_default_params()
 
         params.short_name_type_run = "test"
         params.output.sub_directory = "unittests"
 
         params.oper.nx = 32
         params.oper.Lx = 2 * np.pi
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/__pythran__/solver.cpp` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/__pythran__/solver.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2,103 +2,106 @@
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 #include <pythonic/include/types/float64.hpp>
-#include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/include/types/numpy_texpr.hpp>
-#include <pythonic/types/numpy_texpr.hpp>
-#include <pythonic/types/ndarray.hpp>
+#include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/types/float64.hpp>
+#include <pythonic/types/ndarray.hpp>
+#include <pythonic/types/numpy_texpr.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
 #include <pythonic/include/operator_/add.hpp>
 #include <pythonic/include/operator_/eq.hpp>
 #include <pythonic/include/operator_/mul.hpp>
 #include <pythonic/include/operator_/neg.hpp>
 #include <pythonic/include/operator_/sub.hpp>
 #include <pythonic/include/types/str.hpp>
 #include <pythonic/builtins/tuple.hpp>
 #include <pythonic/operator_/add.hpp>
 #include <pythonic/operator_/eq.hpp>
 #include <pythonic/operator_/mul.hpp>
 #include <pythonic/operator_/neg.hpp>
 #include <pythonic/operator_/sub.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_solver
+namespace 
 {
-  struct __transonic__
+  namespace __pythran_solver
   {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    struct __transonic__
     {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct compute_Frot
-  {
-    typedef void callable;
-    typedef void pure;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 = long>
-    struct type
+    struct compute_Frot
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef decltype(pythonic::operator_::neg(std::declval<__type1>())) __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
-      typedef __type3 __type4;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type2>(), std::declval<__type4>())) __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type8;
-      typedef __type8 __type9;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type9>())) __type10;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type5>(), std::declval<__type10>())) __type11;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type18;
-      typedef __type18 __type19;
-      typedef decltype(pythonic::operator_::add(std::declval<__type9>(), std::declval<__type19>())) __type20;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type20>())) __type21;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type5>(), std::declval<__type21>())) __type22;
-      typedef typename __combined<__type11,__type22>::type __type23;
-      typedef typename pythonic::returnable<__type23>::type __type24;
-      typedef __type24 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 = long>
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 = long>
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef decltype(pythonic::operator_::neg(std::declval<__type1>())) __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
+        typedef __type3 __type4;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type2>(), std::declval<__type4>())) __type5;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type6;
+        typedef __type6 __type7;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type8;
+        typedef __type8 __type9;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type9>())) __type10;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type5>(), std::declval<__type10>())) __type11;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type18;
+        typedef __type18 __type19;
+        typedef decltype(pythonic::operator_::add(std::declval<__type9>(), std::declval<__type19>())) __type20;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type7>(), std::declval<__type20>())) __type21;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type5>(), std::declval<__type21>())) __type22;
+        typedef typename __combined<__type11,__type22>::type __type23;
+        typedef typename pythonic::returnable<__type23>::type __type24;
+        typedef __type24 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 = long>
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0 ux, argument_type1 uy, argument_type2 px_rot, argument_type3 py_rot, argument_type4 beta= 0L) const
+      ;
+    }  ;
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type operator()(argument_type0&& ux, argument_type1&& uy, argument_type2&& px_rot, argument_type3&& py_rot, argument_type4 beta= 0L) const
-    ;
-  }  ;
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
+    typename __transonic__::type::result_type __transonic__::operator()() const
     {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.0"));
-      return tmp_global;
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
-  inline
-  typename compute_Frot::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type compute_Frot::operator()(argument_type0&& ux, argument_type1&& uy, argument_type2&& px_rot, argument_type3&& py_rot, argument_type4 beta) const
-  {
-    if (pythonic::operator_::eq(beta, 0L))
-    {
-      return pythonic::operator_::sub(pythonic::operator_::mul(pythonic::operator_::neg(ux), px_rot), pythonic::operator_::mul(uy, py_rot));
-    }
-    else
+    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 >
+    inline
+    typename compute_Frot::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4>::result_type compute_Frot::operator()(argument_type0 ux, argument_type1 uy, argument_type2 px_rot, argument_type3 py_rot, argument_type4 beta) const
     {
-      return pythonic::operator_::sub(pythonic::operator_::mul(pythonic::operator_::neg(ux), px_rot), pythonic::operator_::mul(uy, pythonic::operator_::add(py_rot, beta)));
+      if (pythonic::operator_::eq(beta, 0L))
+      {
+        return pythonic::operator_::sub(pythonic::operator_::mul(pythonic::operator_::neg(ux), px_rot), pythonic::operator_::mul(uy, py_rot));
+      }
+      else
+      {
+        return pythonic::operator_::sub(pythonic::operator_::mul(pythonic::operator_::neg(ux), px_rot), pythonic::operator_::mul(uy, pythonic::operator_::add(py_rot, beta)));
+      }
     }
   }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_solver::__transonic__()());
 inline
@@ -1344,17 +1347,17 @@
                                          Methods,
                                          ""
     );
     #endif
     if(! theModule)
         PYTHRAN_RETURN;
     PyObject * theDoc = Py_BuildValue("(sss)",
-                                      "0.11.0",
-                                      "2022-09-02 03:40:17.715955",
-                                      "bd828fe06bfaa9a2468008a4a03a9dd82c63426f0f541e4bb482141235bae678");
+                                      "0.13.1",
+                                      "2023-05-24 11:29:42.367898",
+                                      "2a1ac2a4e88e1a9f4787b1559a937c9cadca577f2353acff17b685dc1a078679");
     if(! theDoc)
         PYTHRAN_RETURN;
     PyModule_AddObject(theModule,
                        "__pythran__",
                        theDoc);
 
     PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/bouss/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/bouss/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     Frot = -ux * px_rot - uy * py_rot + px_b
     Fb = -ux * px_b - uy * py_b
     return Frot, Fb
 
 
 class InfoSolverNS2DBouss(InfoSolverNS2D):
     def _init_root(self):
-
         super()._init_root()
 
         package = "fluidsim.solvers.ns2d.bouss"
         self.module_name = package + ".solver"
         self.class_name = "Simul"
         self.short_name = "ns2d.bouss"
 
@@ -210,15 +209,14 @@
 #     omega_dispersion_relation : arr
 #       Frequency dispersion relation in rad.
 #     """
 #     return self.params.N * (self.oper.KX / self.oper.K_not0)
 
 
 if __name__ == "__main__":
-
     from math import pi
 
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/bouss/state.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/bouss/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
                 "keys_computable": [],
                 "keys_phys_needed": ["rot", "b"],
                 "keys_linear_eigenmodes": ["rot_fft", "b_fft"],
             }
         )
 
     def __init__(self, sim, oper=None):
-
         super().__init__(sim, oper)
 
         self.field_tmp4 = np.empty_like(self.state_phys[0])
         self.field_tmp5 = np.empty_like(self.state_phys[0])
 
     def compute(self, key, SAVE_IN_DICT=True, RAISE_ERROR=True):
         """Compute and return a variable"""
@@ -139,14 +138,13 @@
         self.init_from_rotbfft(rot_fft, b_fft)
 
     def init_from_rotfft(self, rot_fft):
         b_fft = np.zeros(self.oper.shapeK_loc, dtype=np.complex128)
         self.init_from_rotbfft(rot_fft, b_fft)
 
     def init_statespect_from(self, **kwargs):
-
         # init_statespect_from looks if kwargs has two arguments.
         if len(kwargs) == 2:
             if "rot_fft" in kwargs and "b_fft" in kwargs:
                 self.init_from_rotbfft(kwargs["rot_fft"], kwargs["b_fft"])
         else:
             super(StateNS2D, self).init_statespect_from(**kwargs)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/bouss/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/bouss/test_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 class TestSimulBase(Base):
     Simul = Simul
 
 
 class TestForcingOutput(TestSimulBase):
     @classmethod
     def init_params(self):
-
         params = super().init_params()
         params.forcing.enable = True
         params.forcing.type = "tcrandom"
 
         # save all outputs!
         periods = params.output.periods_save
         for key in periods._key_attribs:
@@ -37,15 +36,14 @@
             if tag.startswith("periods"):
                 continue
             child = params.output[tag]
             if hasattr(child, "HAS_TO_PLOT_SAVED"):
                 child["HAS_TO_PLOT_SAVED"] = True
 
     def test_forcing_output(self):
-
         sim = self.sim
 
         sim.time_stepping.start()
 
         sim.state.compute("rot_fft")
         sim.state.compute("rot_fft")
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/forcing.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/forcing.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
             ForcingMilestone,
         ]
         ForcingBasePseudoSpectral._complete_info_solver(info_solver, classes)
 
     def compute_coef_ab_normalize(
         self, constant_rate_of, key_forced, f_fft, var_fft, deltat
     ):
-
         if constant_rate_of not in ["energy", "energyK"]:
             raise ValueError
 
         if hasattr(self.forcing_maker, "oper_coarse"):
             oper = self.forcing_maker.oper_coarse
         else:
             oper = self.sim.oper
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/init_fields.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/init_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
     def __call__(self):
         rot_fft, ux_fft, uy_fft = self.compute_rotuxuy_fft()
         # energy_fft = 0.5 * (np.abs(ux_fft) ** 2 + np.abs(uy_fft) ** 2)
         self.sim.state.init_from_rotfft(rot_fft)
 
     def compute_rotuxuy_fft(self):
-
         params = self.sim.params
         oper = self.sim.oper
 
         lambda0 = params.init_fields.noise.length
         if lambda0 == 0:
             lambda0 = min(oper.Lx, oper.Ly) / 4.0
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/output/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/output/__pythran__/spatiotemporal_spectra.cpp` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/output/__pythran__/spatiotemporal_spectra.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 #include <pythonic/include/types/float64.hpp>
-#include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/include/types/float32.hpp>
+#include <pythonic/include/types/ndarray.hpp>
+#include <pythonic/types/float64.hpp>
 #include <pythonic/types/float32.hpp>
 #include <pythonic/types/ndarray.hpp>
-#include <pythonic/types/float64.hpp>
 #include <pythonic/include/builtins/abs.hpp>
 #include <pythonic/include/builtins/enumerate.hpp>
 #include <pythonic/include/builtins/getattr.hpp>
 #include <pythonic/include/builtins/int_.hpp>
 #include <pythonic/include/builtins/len.hpp>
 #include <pythonic/include/builtins/pythran/make_shape.hpp>
 #include <pythonic/include/builtins/range.hpp>
@@ -49,432 +49,470 @@
 #include <pythonic/operator_/iadd.hpp>
 #include <pythonic/operator_/mul.hpp>
 #include <pythonic/operator_/ne.hpp>
 #include <pythonic/operator_/neg.hpp>
 #include <pythonic/operator_/sub.hpp>
 #include <pythonic/types/slice.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_spatiotemporal_spectra
+namespace 
 {
-  struct __transonic__
+  namespace __pythran_spatiotemporal_spectra
   {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    struct __transonic__
     {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct compute_spectrum_kzkhomega
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef decltype(pythonic::types::as_const(std::declval<__type1>())) __type2;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type2>::type>::type __type3;
+        typedef __type3 __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(pythonic::types::as_const(std::declval<__type6>())) __type7;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type7>::type>::type __type8;
+        typedef __type8 __type9;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros{})>::type>::type __type10;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::make_shape{})>::type>::type __type11;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::len{})>::type>::type __type12;
+        typedef std::integral_constant<long,1> __type13;
+        typedef indexable_container<__type13, typename std::remove_reference<__type8>::type> __type14;
+        typedef typename __combined<__type5,__type14>::type __type15;
+        typedef __type15 __type16;
+        typedef decltype(std::declval<__type12>()(std::declval<__type16>())) __type17;
+        typedef typename pythonic::assignable<__type17>::type __type18;
+        typedef __type18 __type19;
+        typedef indexable_container<__type13, typename std::remove_reference<__type3>::type> __type20;
+        typedef typename __combined<__type0,__type20>::type __type21;
+        typedef __type21 __type22;
+        typedef decltype(std::declval<__type12>()(std::declval<__type22>())) __type23;
+        typedef typename pythonic::assignable<__type23>::type __type24;
+        typedef __type24 __type25;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type26;
+        typedef __type26 __type27;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type27>())) __type28;
+        typedef decltype(pythonic::types::as_const(std::declval<__type28>())) __type29;
+        typedef typename std::tuple_element<3,typename std::remove_reference<__type29>::type>::type __type30;
+        typedef typename pythonic::assignable<__type30>::type __type31;
+        typedef __type31 __type32;
+        typedef long __type33;
+        typedef decltype(pythonic::operator_::add(std::declval<__type32>(), std::declval<__type33>())) __type34;
+        typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type34>(), std::declval<__type33>())) __type35;
+        typedef typename pythonic::assignable<__type35>::type __type36;
+        typedef __type36 __type37;
+        typedef decltype(std::declval<__type11>()(std::declval<__type19>(), std::declval<__type25>(), std::declval<__type37>())) __type38;
+        typedef decltype(std::declval<__type10>()(std::declval<__type38>())) __type39;
+        typedef typename pythonic::assignable<__type39>::type __type40;
+        typedef decltype(std::declval<__type11>()(std::declval<__type19>(), std::declval<__type25>(), std::declval<__type32>())) __type44;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, std::declval<__type27>())) __type46;
+        typedef decltype(std::declval<__type10>()(std::declval<__type44>(), std::declval<__type46>())) __type47;
+        typedef typename pythonic::assignable<__type47>::type __type48;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::int_{})>::type>::type __type49;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::round{})>::type>::type __type50;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type51;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type52;
+        typedef __type52 __type53;
+        typedef decltype(pythonic::types::as_const(std::declval<__type53>())) __type54;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type55;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type29>::type>::type __type56;
+        typedef typename pythonic::lazy<__type56>::type __type57;
+        typedef __type57 __type58;
+        typedef decltype(std::declval<__type55>()(std::declval<__type58>())) __type59;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type59>::type::iterator>::value_type>::type __type60;
+        typedef __type60 __type61;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type29>::type>::type __type62;
+        typedef typename pythonic::lazy<__type62>::type __type63;
+        typedef __type63 __type64;
+        typedef decltype(std::declval<__type55>()(std::declval<__type64>())) __type65;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type65>::type::iterator>::value_type>::type __type66;
+        typedef __type66 __type67;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type29>::type>::type __type68;
+        typedef typename pythonic::lazy<__type68>::type __type69;
+        typedef __type69 __type70;
+        typedef decltype(std::declval<__type55>()(std::declval<__type70>())) __type71;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type71>::type::iterator>::value_type>::type __type72;
+        typedef __type72 __type73;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type61>(), std::declval<__type67>(), std::declval<__type73>())) __type74;
+        typedef decltype(std::declval<__type54>()[std::declval<__type74>()]) __type75;
+        typedef decltype(std::declval<__type51>()(std::declval<__type75>())) __type76;
+        typedef typename pythonic::assignable<__type8>::type __type77;
+        typedef __type77 __type78;
+        typedef decltype(pythonic::operator_::div(std::declval<__type76>(), std::declval<__type78>())) __type79;
+        typedef decltype(std::declval<__type50>()(std::declval<__type79>())) __type80;
+        typedef decltype(std::declval<__type49>()(std::declval<__type80>())) __type81;
+        typedef typename pythonic::lazy<__type81>::type __type82;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type19>(), std::declval<__type33>())) __type84;
+        typedef typename pythonic::lazy<__type84>::type __type85;
+        typedef typename __combined<__type82,__type85>::type __type86;
+        typedef __type86 __type87;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type25>(), std::declval<__type33>())) __type89;
+        typedef typename pythonic::lazy<__type89>::type __type90;
+        typedef __type90 __type91;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type92;
+        typedef decltype(pythonic::types::as_const(std::declval<__type27>())) __type94;
+        typedef pythonic::types::contiguous_slice __type98;
+        typedef decltype(std::declval<__type94>()(std::declval<__type61>(), std::declval<__type67>(), std::declval<__type73>(), std::declval<__type98>())) __type99;
+        typedef typename pythonic::lazy<__type99>::type __type100;
+        typedef __type100 __type101;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type33>(), std::declval<__type101>())) __type102;
+        typedef typename pythonic::lazy<__type102>::type __type103;
+        typedef typename __combined<__type100,__type103>::type __type104;
+        typedef __type104 __type105;
+        typedef decltype(std::declval<__type92>()(std::declval<__type105>())) __type106;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type106>::type::iterator>::value_type>::type __type107;
+        typedef __type107 __type108;
+        typedef decltype(pythonic::types::as_const(std::declval<__type108>())) __type109;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type109>::type>::type __type110;
+        typedef typename pythonic::lazy<__type110>::type __type111;
+        typedef __type111 __type112;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type87>(), std::declval<__type91>(), std::declval<__type112>())) __type113;
+        typedef indexable<__type113> __type114;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type116;
+        typedef __type116 __type117;
+        typedef decltype(pythonic::types::as_const(std::declval<__type117>())) __type118;
+        typedef decltype(std::declval<__type118>()[std::declval<__type74>()]) __type123;
+        typedef typename pythonic::assignable<__type123>::type __type124;
+        typedef __type124 __type125;
+        typedef typename pythonic::assignable<__type3>::type __type126;
+        typedef __type126 __type127;
+        typedef decltype(pythonic::operator_::div(std::declval<__type125>(), std::declval<__type127>())) __type128;
+        typedef decltype(std::declval<__type49>()(std::declval<__type128>())) __type129;
+        typedef typename pythonic::assignable<__type129>::type __type130;
+        typedef __type130 __type131;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type87>(), std::declval<__type131>(), std::declval<__type112>())) __type140;
+        typedef indexable<__type140> __type141;
+        typedef decltype(pythonic::operator_::add(std::declval<__type131>(), std::declval<__type33>())) __type144;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type87>(), std::declval<__type144>(), std::declval<__type112>())) __type146;
+        typedef indexable<__type146> __type147;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type109>::type>::type __type150;
+        typedef typename pythonic::lazy<__type150>::type __type151;
+        typedef __type151 __type152;
+        typedef container<typename std::remove_reference<__type152>::type> __type153;
+        typedef decltype(pythonic::types::as_const(std::declval<__type22>())) __type156;
+        typedef decltype(std::declval<__type156>()[std::declval<__type131>()]) __type158;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type125>(), std::declval<__type158>())) __type159;
+        typedef decltype(pythonic::operator_::div(std::declval<__type159>(), std::declval<__type127>())) __type161;
+        typedef typename pythonic::assignable<__type161>::type __type162;
+        typedef __type162 __type163;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type33>(), std::declval<__type163>())) __type164;
+        typedef typename pythonic::assignable<__type150>::type __type168;
+        typedef __type168 __type169;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type164>(), std::declval<__type169>())) __type170;
+        typedef container<typename std::remove_reference<__type170>::type> __type171;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type163>(), std::declval<__type169>())) __type174;
+        typedef container<typename std::remove_reference<__type174>::type> __type175;
+        typedef typename __combined<__type48,__type114,__type141,__type147,__type153,__type171,__type175>::type __type176;
+        typedef __type176 __type177;
+        typedef decltype(pythonic::types::as_const(std::declval<__type177>())) __type178;
+        typedef decltype(std::declval<__type178>()(std::declval<__type98>(), std::declval<__type98>(), std::declval<__type33>())) __type179;
+        typedef container<typename std::remove_reference<__type179>::type> __type180;
+        typedef decltype(std::declval<__type178>()(std::declval<__type98>(), std::declval<__type98>(), std::declval<__type98>())) __type183;
+        typedef pythonic::types::slice __type186;
+        typedef decltype(std::declval<__type178>()(std::declval<__type98>(), std::declval<__type98>(), std::declval<__type186>())) __type187;
+        typedef decltype(pythonic::operator_::add(std::declval<__type183>(), std::declval<__type187>())) __type188;
+        typedef container<typename std::remove_reference<__type188>::type> __type189;
+        typedef typename __combined<__type40,__type180,__type189>::type __type190;
+        typedef __type190 __type191;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type78>(), std::declval<__type127>())) __type194;
+        typedef decltype(pythonic::operator_::div(std::declval<__type191>(), std::declval<__type194>())) __type195;
+        typedef typename pythonic::returnable<__type195>::type __type196;
+        typedef __type4 __ptype0;
+        typedef __type9 __ptype1;
+        typedef __type196 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0 field_k0k1k2omega, argument_type1 khs, argument_type2 kzs, argument_type3 KX, argument_type4 KZ, argument_type5 KH) const
+      ;
     }  ;
     inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct compute_spectrum_kzkhomega
-  {
-    typedef void callable;
-    typedef void pure;
+    typename __transonic__::type::result_type __transonic__::operator()() const
+    {
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    struct type
+    inline
+    typename compute_spectrum_kzkhomega::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type compute_spectrum_kzkhomega::operator()(argument_type0 field_k0k1k2omega, argument_type1 khs, argument_type2 kzs, argument_type3 KX, argument_type4 KZ, argument_type5 KH) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type1>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type4;
-      typedef __type4 __type5;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type5>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros{})>::type>::type __type8;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::make_shape{})>::type>::type __type9;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::len{})>::type>::type __type10;
-      typedef std::integral_constant<long,1> __type11;
-      typedef indexable_container<__type11, typename std::remove_reference<__type6>::type> __type12;
-      typedef typename __combined<__type4,__type12>::type __type13;
-      typedef __type13 __type14;
-      typedef decltype(std::declval<__type10>()(std::declval<__type14>())) __type15;
-      typedef typename pythonic::assignable<__type15>::type __type16;
-      typedef __type16 __type17;
-      typedef indexable_container<__type11, typename std::remove_reference<__type2>::type> __type18;
-      typedef typename __combined<__type0,__type18>::type __type19;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::make_shape{})>::type>::type __type1;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::len{})>::type>::type __type2;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
+      typedef std::integral_constant<long,1> __type4;
+      typedef __type3 __type5;
+      typedef decltype(pythonic::types::as_const(std::declval<__type5>())) __type6;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type6>::type>::type __type7;
+      typedef indexable_container<__type4, typename std::remove_reference<__type7>::type> __type8;
+      typedef typename __combined<__type3,__type8>::type __type9;
+      typedef __type9 __type10;
+      typedef decltype(std::declval<__type2>()(std::declval<__type10>())) __type11;
+      typedef typename pythonic::assignable<__type11>::type __type12;
+      typedef __type12 __type13;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type14;
+      typedef __type14 __type15;
+      typedef decltype(pythonic::types::as_const(std::declval<__type15>())) __type16;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type16>::type>::type __type17;
+      typedef indexable_container<__type4, typename std::remove_reference<__type17>::type> __type18;
+      typedef typename __combined<__type14,__type18>::type __type19;
       typedef __type19 __type20;
-      typedef decltype(std::declval<__type10>()(std::declval<__type20>())) __type21;
+      typedef decltype(std::declval<__type2>()(std::declval<__type20>())) __type21;
       typedef typename pythonic::assignable<__type21>::type __type22;
       typedef __type22 __type23;
       typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type24;
       typedef __type24 __type25;
       typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type25>())) __type26;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type26>::type>::type __type27;
-      typedef typename pythonic::assignable<__type27>::type __type28;
-      typedef __type28 __type29;
-      typedef long __type30;
-      typedef decltype(pythonic::operator_::add(std::declval<__type29>(), std::declval<__type30>())) __type31;
-      typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type31>(), std::declval<__type30>())) __type32;
-      typedef typename pythonic::assignable<__type32>::type __type33;
-      typedef __type33 __type34;
-      typedef decltype(std::declval<__type9>()(std::declval<__type17>(), std::declval<__type23>(), std::declval<__type34>())) __type35;
-      typedef decltype(std::declval<__type8>()(std::declval<__type35>())) __type36;
-      typedef typename pythonic::assignable<__type36>::type __type37;
-      typedef decltype(std::declval<__type9>()(std::declval<__type17>(), std::declval<__type23>(), std::declval<__type29>())) __type41;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, std::declval<__type25>())) __type43;
-      typedef decltype(std::declval<__type8>()(std::declval<__type41>(), std::declval<__type43>())) __type44;
-      typedef typename pythonic::assignable<__type44>::type __type45;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::int_{})>::type>::type __type46;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::round{})>::type>::type __type47;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type48;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type49;
-      typedef __type49 __type50;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type51;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type26>::type>::type __type52;
-      typedef typename pythonic::lazy<__type52>::type __type53;
+      typedef decltype(pythonic::types::as_const(std::declval<__type26>())) __type27;
+      typedef typename std::tuple_element<3,typename std::remove_reference<__type27>::type>::type __type28;
+      typedef typename pythonic::assignable<__type28>::type __type29;
+      typedef __type29 __type30;
+      typedef decltype(std::declval<__type1>()(std::declval<__type13>(), std::declval<__type23>(), std::declval<__type30>())) __type31;
+      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, std::declval<__type25>())) __type33;
+      typedef decltype(std::declval<__type0>()(std::declval<__type31>(), std::declval<__type33>())) __type34;
+      typedef typename pythonic::assignable<__type34>::type __type35;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::int_{})>::type>::type __type36;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::round{})>::type>::type __type37;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type38;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type39;
+      typedef __type39 __type40;
+      typedef decltype(pythonic::types::as_const(std::declval<__type40>())) __type41;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type42;
+      typedef typename std::tuple_element<0,typename std::remove_reference<__type27>::type>::type __type43;
+      typedef typename pythonic::lazy<__type43>::type __type44;
+      typedef __type44 __type45;
+      typedef decltype(std::declval<__type42>()(std::declval<__type45>())) __type46;
+      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type46>::type::iterator>::value_type>::type __type47;
+      typedef __type47 __type48;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type27>::type>::type __type49;
+      typedef typename pythonic::lazy<__type49>::type __type50;
+      typedef __type50 __type51;
+      typedef decltype(std::declval<__type42>()(std::declval<__type51>())) __type52;
+      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type52>::type::iterator>::value_type>::type __type53;
       typedef __type53 __type54;
-      typedef decltype(std::declval<__type51>()(std::declval<__type54>())) __type55;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type55>::type::iterator>::value_type>::type __type56;
+      typedef typename std::tuple_element<2,typename std::remove_reference<__type27>::type>::type __type55;
+      typedef typename pythonic::lazy<__type55>::type __type56;
       typedef __type56 __type57;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type26>::type>::type __type58;
-      typedef typename pythonic::lazy<__type58>::type __type59;
+      typedef decltype(std::declval<__type42>()(std::declval<__type57>())) __type58;
+      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type58>::type::iterator>::value_type>::type __type59;
       typedef __type59 __type60;
-      typedef decltype(std::declval<__type51>()(std::declval<__type60>())) __type61;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type61>::type::iterator>::value_type>::type __type62;
-      typedef __type62 __type63;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type57>(), std::declval<__type63>())) __type64;
-      typedef decltype(std::declval<__type50>()[std::declval<__type64>()]) __type65;
-      typedef decltype(std::declval<__type48>()(std::declval<__type65>())) __type66;
-      typedef typename pythonic::assignable<__type6>::type __type67;
-      typedef __type67 __type68;
-      typedef decltype(pythonic::operator_::div(std::declval<__type66>(), std::declval<__type68>())) __type69;
-      typedef decltype(std::declval<__type47>()(std::declval<__type69>())) __type70;
-      typedef decltype(std::declval<__type46>()(std::declval<__type70>())) __type71;
-      typedef typename pythonic::lazy<__type71>::type __type72;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type17>(), std::declval<__type30>())) __type74;
-      typedef typename pythonic::lazy<__type74>::type __type75;
-      typedef typename __combined<__type72,__type75>::type __type76;
-      typedef __type76 __type77;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type23>(), std::declval<__type30>())) __type79;
-      typedef typename pythonic::lazy<__type79>::type __type80;
-      typedef __type80 __type81;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type82;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type48>(), std::declval<__type54>(), std::declval<__type60>())) __type61;
+      typedef decltype(std::declval<__type41>()[std::declval<__type61>()]) __type62;
+      typedef decltype(std::declval<__type38>()(std::declval<__type62>())) __type63;
+      typedef typename pythonic::assignable<__type7>::type __type64;
+      typedef __type64 __type65;
+      typedef decltype(pythonic::operator_::div(std::declval<__type63>(), std::declval<__type65>())) __type66;
+      typedef decltype(std::declval<__type37>()(std::declval<__type66>())) __type67;
+      typedef decltype(std::declval<__type36>()(std::declval<__type67>())) __type68;
+      typedef typename pythonic::lazy<__type68>::type __type69;
+      typedef long __type71;
+      typedef decltype(pythonic::operator_::sub(std::declval<__type13>(), std::declval<__type71>())) __type72;
+      typedef typename pythonic::lazy<__type72>::type __type73;
+      typedef typename __combined<__type69,__type73>::type __type74;
+      typedef __type74 __type75;
+      typedef decltype(pythonic::operator_::sub(std::declval<__type23>(), std::declval<__type71>())) __type77;
+      typedef typename pythonic::lazy<__type77>::type __type78;
+      typedef __type78 __type79;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type80;
+      typedef decltype(pythonic::types::as_const(std::declval<__type25>())) __type82;
       typedef pythonic::types::contiguous_slice __type86;
-      typedef decltype(std::declval<__type25>()(std::declval<__type57>(), std::declval<__type63>(), std::declval<__type86>())) __type87;
+      typedef decltype(std::declval<__type82>()(std::declval<__type48>(), std::declval<__type54>(), std::declval<__type60>(), std::declval<__type86>())) __type87;
       typedef typename pythonic::lazy<__type87>::type __type88;
       typedef __type88 __type89;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type30>(), std::declval<__type89>())) __type90;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type71>(), std::declval<__type89>())) __type90;
       typedef typename pythonic::lazy<__type90>::type __type91;
       typedef typename __combined<__type88,__type91>::type __type92;
       typedef __type92 __type93;
-      typedef decltype(std::declval<__type82>()(std::declval<__type93>())) __type94;
+      typedef decltype(std::declval<__type80>()(std::declval<__type93>())) __type94;
       typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type94>::type::iterator>::value_type>::type __type95;
       typedef __type95 __type96;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type96>::type>::type __type97;
-      typedef typename pythonic::lazy<__type97>::type __type98;
-      typedef __type98 __type99;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type77>(), std::declval<__type81>(), std::declval<__type99>())) __type100;
-      typedef indexable<__type100> __type101;
-      typedef typename __combined<__type45,__type101>::type __type102;
+      typedef decltype(pythonic::types::as_const(std::declval<__type96>())) __type97;
+      typedef typename std::tuple_element<0,typename std::remove_reference<__type97>::type>::type __type98;
+      typedef typename pythonic::lazy<__type98>::type __type99;
+      typedef __type99 __type100;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type75>(), std::declval<__type79>(), std::declval<__type100>())) __type101;
+      typedef indexable<__type101> __type102;
       typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type104;
       typedef __type104 __type105;
-      typedef decltype(std::declval<__type105>()[std::declval<__type64>()]) __type109;
-      typedef typename pythonic::assignable<__type109>::type __type110;
-      typedef __type110 __type111;
-      typedef typename pythonic::assignable<__type2>::type __type112;
+      typedef decltype(pythonic::types::as_const(std::declval<__type105>())) __type106;
+      typedef decltype(std::declval<__type106>()[std::declval<__type61>()]) __type111;
+      typedef typename pythonic::assignable<__type111>::type __type112;
       typedef __type112 __type113;
-      typedef decltype(pythonic::operator_::div(std::declval<__type111>(), std::declval<__type113>())) __type114;
-      typedef decltype(std::declval<__type46>()(std::declval<__type114>())) __type115;
-      typedef typename pythonic::assignable<__type115>::type __type116;
-      typedef __type116 __type117;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type77>(), std::declval<__type117>(), std::declval<__type99>())) __type125;
-      typedef indexable<__type125> __type126;
-      typedef typename __combined<__type102,__type126>::type __type127;
-      typedef decltype(pythonic::operator_::add(std::declval<__type117>(), std::declval<__type30>())) __type130;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type77>(), std::declval<__type130>(), std::declval<__type99>())) __type132;
-      typedef indexable<__type132> __type133;
-      typedef typename __combined<__type127,__type133>::type __type134;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type96>::type>::type __type136;
-      typedef typename pythonic::lazy<__type136>::type __type137;
-      typedef __type137 __type138;
-      typedef container<typename std::remove_reference<__type138>::type> __type139;
-      typedef decltype(std::declval<__type20>()[std::declval<__type117>()]) __type143;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type111>(), std::declval<__type143>())) __type144;
-      typedef decltype(pythonic::operator_::div(std::declval<__type144>(), std::declval<__type113>())) __type146;
-      typedef typename pythonic::assignable<__type146>::type __type147;
-      typedef __type147 __type148;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type30>(), std::declval<__type148>())) __type149;
-      typedef typename pythonic::assignable<__type136>::type __type152;
-      typedef __type152 __type153;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type149>(), std::declval<__type153>())) __type154;
-      typedef container<typename std::remove_reference<__type154>::type> __type155;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type148>(), std::declval<__type153>())) __type158;
+      typedef typename pythonic::assignable<__type17>::type __type114;
+      typedef __type114 __type115;
+      typedef decltype(pythonic::operator_::div(std::declval<__type113>(), std::declval<__type115>())) __type116;
+      typedef decltype(std::declval<__type36>()(std::declval<__type116>())) __type117;
+      typedef typename pythonic::assignable<__type117>::type __type118;
+      typedef __type118 __type119;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type75>(), std::declval<__type119>(), std::declval<__type100>())) __type128;
+      typedef indexable<__type128> __type129;
+      typedef decltype(pythonic::operator_::add(std::declval<__type119>(), std::declval<__type71>())) __type132;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type75>(), std::declval<__type132>(), std::declval<__type100>())) __type134;
+      typedef indexable<__type134> __type135;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type97>::type>::type __type138;
+      typedef typename pythonic::lazy<__type138>::type __type139;
+      typedef __type139 __type140;
+      typedef container<typename std::remove_reference<__type140>::type> __type141;
+      typedef decltype(pythonic::types::as_const(std::declval<__type20>())) __type144;
+      typedef decltype(std::declval<__type144>()[std::declval<__type119>()]) __type146;
+      typedef decltype(pythonic::operator_::sub(std::declval<__type113>(), std::declval<__type146>())) __type147;
+      typedef decltype(pythonic::operator_::div(std::declval<__type147>(), std::declval<__type115>())) __type149;
+      typedef typename pythonic::assignable<__type149>::type __type150;
+      typedef __type150 __type151;
+      typedef decltype(pythonic::operator_::sub(std::declval<__type71>(), std::declval<__type151>())) __type152;
+      typedef typename pythonic::assignable<__type138>::type __type156;
+      typedef __type156 __type157;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type152>(), std::declval<__type157>())) __type158;
       typedef container<typename std::remove_reference<__type158>::type> __type159;
-      typedef typename __combined<__type134,__type101,__type139,__type139,__type126,__type155,__type155,__type133,__type159,__type159>::type __type160;
-      typedef __type160 __type161;
-      typedef decltype(std::declval<__type161>()(std::declval<__type86>(), std::declval<__type86>(), std::declval<__type30>())) __type162;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type151>(), std::declval<__type157>())) __type162;
       typedef container<typename std::remove_reference<__type162>::type> __type163;
-      typedef decltype(std::declval<__type161>()(std::declval<__type86>(), std::declval<__type86>(), std::declval<__type86>())) __type165;
-      typedef pythonic::types::slice __type167;
-      typedef decltype(std::declval<__type161>()(std::declval<__type86>(), std::declval<__type86>(), std::declval<__type167>())) __type168;
-      typedef decltype(pythonic::operator_::add(std::declval<__type165>(), std::declval<__type168>())) __type169;
-      typedef container<typename std::remove_reference<__type169>::type> __type170;
-      typedef typename __combined<__type37,__type163,__type170>::type __type171;
-      typedef __type171 __type172;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type68>(), std::declval<__type113>())) __type175;
-      typedef decltype(pythonic::operator_::div(std::declval<__type172>(), std::declval<__type175>())) __type176;
-      typedef typename pythonic::returnable<__type176>::type __type177;
-      typedef __type3 __ptype0;
-      typedef __type7 __ptype1;
-      typedef __type177 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0&& field_k0k1omega, argument_type1&& khs, argument_type2&& kzs, argument_type3&& KX, argument_type4&& KZ, argument_type5&& KH) const
-    ;
-  }  ;
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
-    {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.0"));
-      return tmp_global;
-    }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-  inline
-  typename compute_spectrum_kzkhomega::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type compute_spectrum_kzkhomega::operator()(argument_type0&& field_k0k1omega, argument_type1&& khs, argument_type2&& kzs, argument_type3&& KX, argument_type4&& KZ, argument_type5&& KH) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::make_shape{})>::type>::type __type1;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::len{})>::type>::type __type2;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
-    typedef std::integral_constant<long,1> __type4;
-    typedef __type3 __type5;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type5>::type>::type __type6;
-    typedef indexable_container<__type4, typename std::remove_reference<__type6>::type> __type7;
-    typedef typename __combined<__type3,__type7>::type __type8;
-    typedef __type8 __type9;
-    typedef decltype(std::declval<__type2>()(std::declval<__type9>())) __type10;
-    typedef typename pythonic::assignable<__type10>::type __type11;
-    typedef __type11 __type12;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type13;
-    typedef __type13 __type14;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type14>::type>::type __type15;
-    typedef indexable_container<__type4, typename std::remove_reference<__type15>::type> __type16;
-    typedef typename __combined<__type13,__type16>::type __type17;
-    typedef __type17 __type18;
-    typedef decltype(std::declval<__type2>()(std::declval<__type18>())) __type19;
-    typedef typename pythonic::assignable<__type19>::type __type20;
-    typedef __type20 __type21;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type22;
-    typedef __type22 __type23;
-    typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type23>())) __type24;
-    typedef typename std::tuple_element<2,typename std::remove_reference<__type24>::type>::type __type25;
-    typedef typename pythonic::assignable<__type25>::type __type26;
-    typedef __type26 __type27;
-    typedef decltype(std::declval<__type1>()(std::declval<__type12>(), std::declval<__type21>(), std::declval<__type27>())) __type28;
-    typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, std::declval<__type23>())) __type30;
-    typedef decltype(std::declval<__type0>()(std::declval<__type28>(), std::declval<__type30>())) __type31;
-    typedef typename pythonic::assignable<__type31>::type __type32;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::int_{})>::type>::type __type33;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::round{})>::type>::type __type34;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type35;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type36;
-    typedef __type36 __type37;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type38;
-    typedef typename std::tuple_element<0,typename std::remove_reference<__type24>::type>::type __type39;
-    typedef typename pythonic::lazy<__type39>::type __type40;
-    typedef __type40 __type41;
-    typedef decltype(std::declval<__type38>()(std::declval<__type41>())) __type42;
-    typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type42>::type::iterator>::value_type>::type __type43;
-    typedef __type43 __type44;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type24>::type>::type __type45;
-    typedef typename pythonic::lazy<__type45>::type __type46;
-    typedef __type46 __type47;
-    typedef decltype(std::declval<__type38>()(std::declval<__type47>())) __type48;
-    typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type48>::type::iterator>::value_type>::type __type49;
-    typedef __type49 __type50;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type44>(), std::declval<__type50>())) __type51;
-    typedef decltype(std::declval<__type37>()[std::declval<__type51>()]) __type52;
-    typedef decltype(std::declval<__type35>()(std::declval<__type52>())) __type53;
-    typedef typename pythonic::assignable<__type6>::type __type54;
-    typedef __type54 __type55;
-    typedef decltype(pythonic::operator_::div(std::declval<__type53>(), std::declval<__type55>())) __type56;
-    typedef decltype(std::declval<__type34>()(std::declval<__type56>())) __type57;
-    typedef decltype(std::declval<__type33>()(std::declval<__type57>())) __type58;
-    typedef typename pythonic::lazy<__type58>::type __type59;
-    typedef long __type61;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type12>(), std::declval<__type61>())) __type62;
-    typedef typename pythonic::lazy<__type62>::type __type63;
-    typedef typename __combined<__type59,__type63>::type __type64;
-    typedef __type64 __type65;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type21>(), std::declval<__type61>())) __type67;
-    typedef typename pythonic::lazy<__type67>::type __type68;
-    typedef __type68 __type69;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type70;
-    typedef pythonic::types::contiguous_slice __type74;
-    typedef decltype(std::declval<__type23>()(std::declval<__type44>(), std::declval<__type50>(), std::declval<__type74>())) __type75;
-    typedef typename pythonic::lazy<__type75>::type __type76;
-    typedef __type76 __type77;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type61>(), std::declval<__type77>())) __type78;
-    typedef typename pythonic::lazy<__type78>::type __type79;
-    typedef typename __combined<__type76,__type79>::type __type80;
-    typedef __type80 __type81;
-    typedef decltype(std::declval<__type70>()(std::declval<__type81>())) __type82;
-    typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type82>::type::iterator>::value_type>::type __type83;
-    typedef __type83 __type84;
-    typedef typename std::tuple_element<0,typename std::remove_reference<__type84>::type>::type __type85;
-    typedef typename pythonic::lazy<__type85>::type __type86;
-    typedef __type86 __type87;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type65>(), std::declval<__type69>(), std::declval<__type87>())) __type88;
-    typedef indexable<__type88> __type89;
-    typedef typename __combined<__type32,__type89>::type __type90;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type92;
-    typedef __type92 __type93;
-    typedef decltype(std::declval<__type93>()[std::declval<__type51>()]) __type97;
-    typedef typename pythonic::assignable<__type97>::type __type98;
-    typedef __type98 __type99;
-    typedef typename pythonic::assignable<__type15>::type __type100;
-    typedef __type100 __type101;
-    typedef decltype(pythonic::operator_::div(std::declval<__type99>(), std::declval<__type101>())) __type102;
-    typedef decltype(std::declval<__type33>()(std::declval<__type102>())) __type103;
-    typedef typename pythonic::assignable<__type103>::type __type104;
-    typedef __type104 __type105;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type65>(), std::declval<__type105>(), std::declval<__type87>())) __type113;
-    typedef indexable<__type113> __type114;
-    typedef typename __combined<__type90,__type114>::type __type115;
-    typedef decltype(pythonic::operator_::add(std::declval<__type105>(), std::declval<__type61>())) __type118;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type65>(), std::declval<__type118>(), std::declval<__type87>())) __type120;
-    typedef indexable<__type120> __type121;
-    typedef typename __combined<__type115,__type121>::type __type122;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type84>::type>::type __type124;
-    typedef typename pythonic::lazy<__type124>::type __type125;
-    typedef __type125 __type126;
-    typedef container<typename std::remove_reference<__type126>::type> __type127;
-    typedef decltype(std::declval<__type18>()[std::declval<__type105>()]) __type131;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type99>(), std::declval<__type131>())) __type132;
-    typedef decltype(pythonic::operator_::div(std::declval<__type132>(), std::declval<__type101>())) __type134;
-    typedef typename pythonic::assignable<__type134>::type __type135;
-    typedef __type135 __type136;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type61>(), std::declval<__type136>())) __type137;
-    typedef typename pythonic::assignable<__type124>::type __type140;
-    typedef __type140 __type141;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type137>(), std::declval<__type141>())) __type142;
-    typedef container<typename std::remove_reference<__type142>::type> __type143;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type136>(), std::declval<__type141>())) __type146;
-    typedef container<typename std::remove_reference<__type146>::type> __type147;
-    typedef typename __combined<__type122,__type89,__type127,__type114,__type143,__type121,__type147>::type __type148;
-    typedef typename pythonic::assignable<__type148>::type __type149;
-    typedef typename pythonic::lazy<__type80>::type __type150;
-    typedef typename pythonic::lazy<__type64>::type __type151;
-    typedef decltype(pythonic::operator_::add(std::declval<__type27>(), std::declval<__type61>())) __type155;
-    typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type155>(), std::declval<__type61>())) __type156;
-    typedef typename pythonic::assignable<__type156>::type __type157;
-    typedef __type157 __type158;
-    typedef decltype(std::declval<__type1>()(std::declval<__type12>(), std::declval<__type21>(), std::declval<__type158>())) __type159;
-    typedef decltype(std::declval<__type0>()(std::declval<__type159>())) __type160;
-    typedef typename pythonic::assignable<__type160>::type __type161;
-    typedef __type148 __type162;
-    typedef decltype(std::declval<__type162>()(std::declval<__type74>(), std::declval<__type74>(), std::declval<__type61>())) __type163;
-    typedef container<typename std::remove_reference<__type163>::type> __type164;
-    typedef decltype(std::declval<__type162>()(std::declval<__type74>(), std::declval<__type74>(), std::declval<__type74>())) __type166;
-    typedef pythonic::types::slice __type168;
-    typedef decltype(std::declval<__type162>()(std::declval<__type74>(), std::declval<__type74>(), std::declval<__type168>())) __type169;
-    typedef decltype(pythonic::operator_::add(std::declval<__type166>(), std::declval<__type169>())) __type170;
-    typedef container<typename std::remove_reference<__type170>::type> __type171;
-    typedef typename __combined<__type161,__type164,__type171>::type __type172;
-    typedef typename pythonic::assignable<__type172>::type __type173;
-    typename pythonic::assignable_noescape<decltype(std::get<1>(khs))>::type deltakh = std::get<1>(khs);
-    typename pythonic::assignable_noescape<decltype(std::get<1>(kzs))>::type deltakz = std::get<1>(kzs);
-    typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::len{}(khs))>::type nkh = pythonic::builtins::functor::len{}(khs);
-    typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::len{}(kzs))>::type nkz = pythonic::builtins::functor::len{}(kzs);
-    typename pythonic::lazy<decltype(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega)))>::type nk0 = std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega));
-    typename pythonic::lazy<decltype(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega)))>::type nk1 = std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega));
-    typename pythonic::assignable_noescape<decltype(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega)))>::type nomega = std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega));
-    __type149 spectrum_kzkhomega = pythonic::numpy::functor::zeros{}(pythonic::builtins::pythran::functor::make_shape{}(nkz, nkh, nomega), pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, field_k0k1omega));
-    {
-      long  __target140520541487312 = nk0;
-      for (long  ik0=0L; ik0 < __target140520541487312; ik0 += 1L)
+      typedef typename __combined<__type35,__type102,__type129,__type135,__type141,__type159,__type163>::type __type164;
+      typedef typename pythonic::assignable<__type164>::type __type165;
+      typedef typename pythonic::lazy<__type92>::type __type166;
+      typedef typename pythonic::lazy<__type74>::type __type167;
+      typedef typename pythonic::assignable<__type150>::type __type168;
+      typedef decltype(pythonic::operator_::add(std::declval<__type30>(), std::declval<__type71>())) __type172;
+      typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type172>(), std::declval<__type71>())) __type173;
+      typedef typename pythonic::assignable<__type173>::type __type174;
+      typedef __type174 __type175;
+      typedef decltype(std::declval<__type1>()(std::declval<__type13>(), std::declval<__type23>(), std::declval<__type175>())) __type176;
+      typedef decltype(std::declval<__type0>()(std::declval<__type176>())) __type177;
+      typedef typename pythonic::assignable<__type177>::type __type178;
+      typedef __type164 __type179;
+      typedef decltype(pythonic::types::as_const(std::declval<__type179>())) __type180;
+      typedef decltype(std::declval<__type180>()(std::declval<__type86>(), std::declval<__type86>(), std::declval<__type71>())) __type181;
+      typedef container<typename std::remove_reference<__type181>::type> __type182;
+      typedef decltype(std::declval<__type180>()(std::declval<__type86>(), std::declval<__type86>(), std::declval<__type86>())) __type185;
+      typedef pythonic::types::slice __type188;
+      typedef decltype(std::declval<__type180>()(std::declval<__type86>(), std::declval<__type86>(), std::declval<__type188>())) __type189;
+      typedef decltype(pythonic::operator_::add(std::declval<__type185>(), std::declval<__type189>())) __type190;
+      typedef container<typename std::remove_reference<__type190>::type> __type191;
+      typedef typename __combined<__type178,__type182,__type191>::type __type192;
+      typedef typename pythonic::assignable<__type192>::type __type193;
+      typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(khs)))>::type deltakh = std::get<1>(pythonic::types::as_const(khs));
+      typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(kzs)))>::type deltakz = std::get<1>(pythonic::types::as_const(kzs));
+      typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::len{}(khs))>::type nkh = pythonic::builtins::functor::len{}(khs);
+      typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::len{}(kzs))>::type nkz = pythonic::builtins::functor::len{}(kzs);
+      typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega))))>::type nk0 = std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega)));
+      typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega))))>::type nk1 = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega)));
+      typename pythonic::lazy<decltype(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega))))>::type nk2 = std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega)));
+      typename pythonic::assignable_noescape<decltype(std::get<3>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega))))>::type nomega = std::get<3>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega)));
+      __type165 spectrum_kzkhomega = pythonic::numpy::functor::zeros{}(pythonic::builtins::pythran::functor::make_shape{}(nkz, nkh, nomega), pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, field_k0k1k2omega));
       {
+        long  __target139658372192720 = nk0;
+        for (long  ik0=0L; ik0 < __target139658372192720; ik0 += 1L)
         {
-          long  __target140520535349184 = nk1;
-          for (long  ik1=0L; ik1 < __target140520535349184; ik1 += 1L)
           {
-            __type150 values = field_k0k1omega(ik0,ik1,pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None));
-            if (pythonic::operator_::ne(KX[pythonic::types::make_tuple(ik0, ik1)], 0.0))
-            {
-              values = pythonic::operator_::mul(2L, values);
-            }
-            typename pythonic::assignable_noescape<decltype(KH[pythonic::types::make_tuple(ik0, ik1)])>::type kappa = KH[pythonic::types::make_tuple(ik0, ik1)];
-            typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::int_{}(pythonic::operator_::div(kappa, deltakh)))>::type ikh = pythonic::builtins::functor::int_{}(pythonic::operator_::div(kappa, deltakh));
-            __type151 ikz = pythonic::builtins::functor::int_{}(pythonic::builtins::functor::round{}(pythonic::operator_::div(pythonic::builtins::functor::abs{}(KZ[pythonic::types::make_tuple(ik0, ik1)]), deltakz)));
-            if (pythonic::operator_::ge(ikz, pythonic::operator_::sub(nkz, 1L)))
-            {
-              ikz = pythonic::operator_::sub(nkz, 1L);
-            }
-            if (pythonic::operator_::ge(ikh, pythonic::operator_::sub(nkh, 1L)))
-            {
-              typename pythonic::lazy<decltype(pythonic::operator_::sub(nkh, 1L))>::type ikh_ = pythonic::operator_::sub(nkh, 1L);
-              {
-                for (auto&& __tuple0: pythonic::builtins::functor::enumerate{}(values))
-                {
-                  typename pythonic::lazy<decltype(std::get<1>(__tuple0))>::type value = std::get<1>(__tuple0);
-                  typename pythonic::lazy<decltype(std::get<0>(__tuple0))>::type i = std::get<0>(__tuple0);
-                  spectrum_kzkhomega[pythonic::types::make_tuple(ikz, ikh_, i)] += value;
-                }
-              }
-            }
-            else
+            long  __target139658367696512 = nk1;
+            for (long  ik1=0L; ik1 < __target139658367696512; ik1 += 1L)
             {
-              typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(pythonic::operator_::sub(kappa, khs[ikh]), deltakh))>::type coef_share = pythonic::operator_::div(pythonic::operator_::sub(kappa, khs[ikh]), deltakh);
               {
-                for (auto&& __tuple1: pythonic::builtins::functor::enumerate{}(values))
+                long  __target139658368382672 = nk2;
+                for (long  ik2=0L; ik2 < __target139658368382672; ik2 += 1L)
                 {
-                  typename pythonic::assignable_noescape<decltype(std::get<1>(__tuple1))>::type value_ = std::get<1>(__tuple1);
-                  typename pythonic::lazy<decltype(std::get<0>(__tuple1))>::type i_ = std::get<0>(__tuple1);
-                  spectrum_kzkhomega[pythonic::types::make_tuple(ikz, ikh, i_)] += pythonic::operator_::mul(pythonic::operator_::sub(1L, coef_share), value_);
-                  spectrum_kzkhomega[pythonic::types::make_tuple(ikz, pythonic::operator_::add(ikh, 1L), i_)] += pythonic::operator_::mul(coef_share, value_);
+                  __type166 values = pythonic::types::as_const(field_k0k1k2omega)(ik0,ik1,ik2,pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None));
+                  if (pythonic::operator_::ne(pythonic::types::as_const(KX)[pythonic::types::make_tuple(ik0, ik1, ik2)], 0.0))
+                  {
+                    values = pythonic::operator_::mul(2L, values);
+                  }
+                  typename pythonic::assignable_noescape<decltype(pythonic::types::as_const(KH)[pythonic::types::make_tuple(ik0, ik1, ik2)])>::type kappa = pythonic::types::as_const(KH)[pythonic::types::make_tuple(ik0, ik1, ik2)];
+                  typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::int_{}(pythonic::operator_::div(kappa, deltakh)))>::type ikh = pythonic::builtins::functor::int_{}(pythonic::operator_::div(kappa, deltakh));
+                  __type167 ikz = pythonic::builtins::functor::int_{}(pythonic::builtins::functor::round{}(pythonic::operator_::div(pythonic::builtins::functor::abs{}(pythonic::types::as_const(KZ)[pythonic::types::make_tuple(ik0, ik1, ik2)]), deltakz)));
+                  if (pythonic::operator_::ge(ikz, pythonic::operator_::sub(nkz, 1L)))
+                  {
+                    ikz = pythonic::operator_::sub(nkz, 1L);
+                  }
+                  {
+                    __type168 coef_share;
+                    if (pythonic::operator_::ge(ikh, pythonic::operator_::sub(nkh, 1L)))
+                    {
+                      typename pythonic::lazy<decltype(pythonic::operator_::sub(nkh, 1L))>::type ikh_ = pythonic::operator_::sub(nkh, 1L);
+                      {
+                        for (auto&& __tuple0: pythonic::builtins::functor::enumerate{}(values))
+                        {
+                          typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(__tuple0)))>::type value = std::get<1>(pythonic::types::as_const(__tuple0));
+                          typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(__tuple0)))>::type i = std::get<0>(pythonic::types::as_const(__tuple0));
+                          pythonic::types::as_const(spectrum_kzkhomega)[pythonic::types::make_tuple(ikz, ikh_, i)] += value;
+                        }
+                      }
+                    }
+                    else
+                    {
+                      coef_share = pythonic::operator_::div(pythonic::operator_::sub(kappa, pythonic::types::as_const(khs)[ikh]), deltakh);
+                      {
+                        for (auto&& __tuple1: pythonic::builtins::functor::enumerate{}(values))
+                        {
+                          typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(__tuple1)))>::type value_ = std::get<1>(pythonic::types::as_const(__tuple1));
+                          typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(__tuple1)))>::type i_ = std::get<0>(pythonic::types::as_const(__tuple1));
+                          pythonic::types::as_const(spectrum_kzkhomega)[pythonic::types::make_tuple(ikz, ikh, i_)] += pythonic::operator_::mul(pythonic::operator_::sub(1L, coef_share), value_);
+                          pythonic::types::as_const(spectrum_kzkhomega)[pythonic::types::make_tuple(ikz, pythonic::operator_::add(ikh, 1L), i_)] += pythonic::operator_::mul(coef_share, value_);
+                        }
+                      }
+                    }
+                  }
                 }
               }
             }
           }
         }
       }
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::functor::floordiv()(pythonic::operator_::add(nomega, 1L), 2L))>::type nomega_ = pythonic::operator_::functor::floordiv()(pythonic::operator_::add(nomega, 1L), 2L);
+      __type193 spectrum_onesided = pythonic::numpy::functor::zeros{}(pythonic::builtins::pythran::functor::make_shape{}(nkz, nkh, nomega_));
+      spectrum_onesided(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),0L) = pythonic::types::as_const(spectrum_kzkhomega)(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),0L);
+      spectrum_onesided(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(1L,pythonic::builtins::None)) = pythonic::operator_::add(pythonic::types::as_const(spectrum_kzkhomega)(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(1L,nomega_)), pythonic::types::as_const(spectrum_kzkhomega)(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::slice(-1L,pythonic::operator_::neg(nomega_),-1L)));
+      return pythonic::operator_::div(spectrum_onesided, pythonic::operator_::mul(deltakz, deltakh));
     }
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::functor::floordiv()(pythonic::operator_::add(nomega, 1L), 2L))>::type nomega_ = pythonic::operator_::functor::floordiv()(pythonic::operator_::add(nomega, 1L), 2L);
-    __type173 spectrum_onesided = pythonic::numpy::functor::zeros{}(pythonic::builtins::pythran::functor::make_shape{}(nkz, nkh, nomega_));
-    spectrum_onesided(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),0L) = spectrum_kzkhomega(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),0L);
-    spectrum_onesided(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(1L,pythonic::builtins::None)) = pythonic::operator_::add(spectrum_kzkhomega(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(1L,nomega_)), spectrum_kzkhomega(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::slice(-1L,pythonic::operator_::neg(nomega_),-1L)));
-    return pythonic::operator_::div(spectrum_onesided, pythonic::operator_::mul(deltakz, deltakh));
   }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_spatiotemporal_spectra::__transonic__()());
 inline
-typename __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega::type<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>::result_type compute_spectrum_kzkhomega0(pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& field_k0k1omega, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& khs, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& kzs, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KX, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KZ, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KH) 
+typename __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega::type<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>::result_type compute_spectrum_kzkhomega0(pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long,long>>&& field_k0k1k2omega, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& khs, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& kzs, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KX, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KZ, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KH) 
 {
   
                             PyThreadState *_save = PyEval_SaveThread();
                             try {
-                                auto res = __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega()(field_k0k1omega, khs, kzs, KX, KZ, KH);
+                                auto res = __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega()(field_k0k1k2omega, khs, kzs, KX, KZ, KH);
                                 PyEval_RestoreThread(_save);
                                 return res;
                             }
                             catch(...) {
                                 PyEval_RestoreThread(_save);
                                 throw;
                             }
                             ;
 }
 inline
-typename __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega::type<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>::result_type compute_spectrum_kzkhomega1(pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long>>&& field_k0k1omega, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& khs, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& kzs, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KX, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KZ, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KH) 
+typename __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega::type<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>::result_type compute_spectrum_kzkhomega1(pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long,long>>&& field_k0k1k2omega, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& khs, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& kzs, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KX, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KZ, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KH) 
 {
   
                             PyThreadState *_save = PyEval_SaveThread();
                             try {
-                                auto res = __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega()(field_k0k1omega, khs, kzs, KX, KZ, KH);
+                                auto res = __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega()(field_k0k1k2omega, khs, kzs, KX, KZ, KH);
                                 PyEval_RestoreThread(_save);
                                 return res;
                             }
                             catch(...) {
                                 PyEval_RestoreThread(_save);
                                 throw;
                             }
@@ -482,36 +520,36 @@
 }
 
 static PyObject *
 __pythran_wrap_compute_spectrum_kzkhomega0(PyObject *self, PyObject *args, PyObject *kw)
 {
     PyObject* args_obj[6+1];
     
-    char const* keywords[] = {"field_k0k1omega", "khs", "kzs", "KX", "KZ", "KH",  nullptr};
+    char const* keywords[] = {"field_k0k1k2omega", "khs", "kzs", "KX", "KZ", "KH",  nullptr};
     if(! PyArg_ParseTupleAndKeywords(args, kw, "OOOOOO",
                                      (char**)keywords , &args_obj[0], &args_obj[1], &args_obj[2], &args_obj[3], &args_obj[4], &args_obj[5]))
         return nullptr;
-    if(is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[0]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[3]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[4]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[5]))
-        return to_python(compute_spectrum_kzkhomega0(from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[0]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[3]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[4]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[5])));
+    if(is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long,long>>>(args_obj[0]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[3]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[4]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[5]))
+        return to_python(compute_spectrum_kzkhomega0(from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long,long>>>(args_obj[0]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[3]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[4]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[5])));
     else {
         return nullptr;
     }
 }
 
 static PyObject *
 __pythran_wrap_compute_spectrum_kzkhomega1(PyObject *self, PyObject *args, PyObject *kw)
 {
     PyObject* args_obj[6+1];
     
-    char const* keywords[] = {"field_k0k1omega", "khs", "kzs", "KX", "KZ", "KH",  nullptr};
+    char const* keywords[] = {"field_k0k1k2omega", "khs", "kzs", "KX", "KZ", "KH",  nullptr};
     if(! PyArg_ParseTupleAndKeywords(args, kw, "OOOOOO",
                                      (char**)keywords , &args_obj[0], &args_obj[1], &args_obj[2], &args_obj[3], &args_obj[4], &args_obj[5]))
         return nullptr;
-    if(is_convertible<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long>>>(args_obj[0]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[3]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[4]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[5]))
-        return to_python(compute_spectrum_kzkhomega1(from_python<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long>>>(args_obj[0]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[3]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[4]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[5])));
+    if(is_convertible<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long,long>>>(args_obj[0]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[3]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[4]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[5]))
+        return to_python(compute_spectrum_kzkhomega1(from_python<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long,long>>>(args_obj[0]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[3]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[4]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[5])));
     else {
         return nullptr;
     }
 }
 
             static PyObject *
             __pythran_wrapall_compute_spectrum_kzkhomega(PyObject *self, PyObject *args, PyObject *kw)
@@ -525,25 +563,25 @@
 
 
 if(PyObject* obj = __pythran_wrap_compute_spectrum_kzkhomega1(self, args, kw))
     return obj;
 PyErr_Clear();
 
                 return pythonic::python::raise_invalid_argument(
-                               "compute_spectrum_kzkhomega", "\n""    - compute_spectrum_kzkhomega(float64[:,:,:], float64[:], float64[:], float64[:,:], float64[:,:], float64[:,:])\n""    - compute_spectrum_kzkhomega(float32[:,:,:], float64[:], float64[:], float64[:,:], float64[:,:], float64[:,:])", args, kw);
+                               "compute_spectrum_kzkhomega", "\n""    - compute_spectrum_kzkhomega(float64[:,:,:,:], float64[:], float64[:], float64[:,:,:], float64[:,:,:], float64[:,:,:])\n""    - compute_spectrum_kzkhomega(float32[:,:,:,:], float64[:], float64[:], float64[:,:,:], float64[:,:,:], float64[:,:,:])", args, kw);
                 });
             }
 
 
 static PyMethodDef Methods[] = {
     {
     "compute_spectrum_kzkhomega",
     (PyCFunction)__pythran_wrapall_compute_spectrum_kzkhomega,
     METH_VARARGS | METH_KEYWORDS,
-    "Compute the kz-kh-omega spectrum.\n""\n""    Supported prototypes:\n""\n""    - compute_spectrum_kzkhomega(float64[:,:,:], float64[:], float64[:], float64[:,:], float64[:,:], float64[:,:])\n""    - compute_spectrum_kzkhomega(float32[:,:,:], float64[:], float64[:], float64[:,:], float64[:,:], float64[:,:])"},
+    "Compute the kz-kh-omega spectrum.\n""\n""    Supported prototypes:\n""\n""    - compute_spectrum_kzkhomega(float64[:,:,:,:], float64[:], float64[:], float64[:,:,:], float64[:,:,:], float64[:,:,:])\n""    - compute_spectrum_kzkhomega(float32[:,:,:,:], float64[:], float64[:], float64[:,:,:], float64[:,:,:], float64[:,:,:])"},
     {NULL, NULL, 0, NULL}
 };
 
 
 #if PY_MAJOR_VERSION >= 3
   static struct PyModuleDef moduledef = {
     PyModuleDef_HEAD_INIT,
@@ -581,17 +619,17 @@
                                          Methods,
                                          ""
     );
     #endif
     if(! theModule)
         PYTHRAN_RETURN;
     PyObject * theDoc = Py_BuildValue("(sss)",
-                                      "0.11.0",
-                                      "2022-09-02 03:40:16.964500",
-                                      "b43678c511914e408663a13ca06fad88649ede5a18f90100c698d09d77042f1b");
+                                      "0.13.1",
+                                      "2023-05-24 11:29:42.784068",
+                                      "042f493953b15f89acbd2c492e2acc0015a0f87c0eea68ae05a7ad60dc111af2");
     if(! theDoc)
         PYTHRAN_RETURN;
     PyModule_AddObject(theModule,
                        "__pythran__",
                        theDoc);
 
     PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/output/print_stdout.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/output/print_stdout.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spatial_means.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spatial_means.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,14 @@
                 ).format(PK1, PK2, PK1 + PK2, PZ1, PZ2, PZ1 + PZ2)
                 self.file.write(to_print)
 
             self.file.flush()
             os.fsync(self.file.fileno())
 
         if self.has_to_plot and mpi.rank == 0:
-
             self.ax_a.plot(tsim, energy, "k.")
 
             self.axe_b.plot(tsim, epsK_tot, "k.")
             if self.sim.params.forcing.enable:
                 self.axe_b.plot(tsim, PK_tot, "m.")
 
             if tsim - self.t_last_show >= self.period_show:
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spatiotemporal_spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spatiotemporal_spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,13 +84,12 @@
             if kx != 0.0 and kx != kx_max:
                 value *= 2
             result += value
     return result
 
 
 class SpatioTemporalSpectraNS2D(SpatioTemporalSpectraNS, SpatioTemporalSpectra2D):
-
     compute_spectrum_kzkhomega = staticmethod(compute_spectrum_kzkhomega)
     _sum_wavenumber = staticmethod(_sum_wavenumber2D)
 
     def save_spectra_kzkhomega(self, tmin=0, tmax=None, dtype=None):
         return super().save_spectra_kzkhomega(tmin, tmax, dtype)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spect_energy_budget.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spect_energy_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
         khE = self.oper.khE
         PiE = cumsum_inv(transfer2D_E) * self.oper.deltak
         PiZ = cumsum_inv(transfer2D_Z) * self.oper.deltak
         self.axe_a.plot(khE + khE[1], PiE, "k")
         self.axe_b.plot(khE + khE[1], PiZ, "g")
 
     def plot(self, tmin=0, tmax=1000, delta_t=2):
-
         with h5py.File(self.path_file, "r") as h5file:
             dset_times = h5file["times"]
             dset_khE = h5file["khE"]
             khE = dset_khE[...]
             khE = khE + khE[1]
 
             dset_transferE = h5file["transfer2D_E"]
@@ -141,15 +140,14 @@
             ax1.set_xlabel("$k_h$")
             ax1.set_ylabel("spectra")
             ax1.set_xscale("log")
             ax1.set_yscale("linear")
 
             if delta_t != 0.0:
                 for it in range(imin_plot, imax_plot, delta_i_plot):
-
                     transferE = dset_transferE[it]
                     transferZ = dset_transferZ[it]
 
                     PiE = cumsum_inv(transferE) * self.oper.deltak
                     PiZ = cumsum_inv(transferZ) * self.oper.deltak
 
                     ax1.plot(khE, PiE, "k", linewidth=1)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         else:
             print(
                 "you need to implement the ploting "
                 "of the spectra for this case"
             )
 
     def plot1d(self, tmin=0, tmax=1000, delta_t=2, coef_compensate=3):
-
         with h5py.File(self.path_file1D, "r") as h5file:
             dset_times = h5file["times"]
 
             dset_kxE = h5file["kxE"]
             kh = dset_kxE[...]
             kh2 = kh[:]
             kh2[kh == 0] = 1e-15
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/output/spectra_multidim.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/output/spectra_multidim.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,14 @@
         + "\n    ".join(params.__str__().split("\n\n", 1)[1].split("\n"))
         + "\n"
         + params._get_formatted_docs()
     )
 
 
 if __name__ == "__main__":
-
     from math import pi
 
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/state.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
                 "keys_computable": [],
                 "keys_phys_needed": ["rot"],
                 "keys_linear_eigenmodes": ["rot_fft"],
             }
         )
 
     def __init__(self, sim, oper=None):
-
         super().__init__(sim, oper)
 
         self.field_tmp0 = np.empty_like(self.state_phys[0])
         self.field_tmp1 = np.empty_like(self.state_phys[0])
         self.field_tmp2 = np.empty_like(self.state_phys[0])
         self.field_tmp3 = np.empty_like(self.state_phys[0])
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/forcing.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/forcing.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     .. inheritance-diagram:: ForcingNS2DStrat
 
     """
 
     def compute_coef_ab_normalize(
         self, constant_rate_of, key_forced, f_fft, var_fft, deltat
     ):
-
         if constant_rate_of not in ["energy", "energyK"]:
             raise ValueError
 
         if hasattr(self.forcing_maker, "oper_coarse"):
             oper = self.forcing_maker.oper_coarse
             state = self.forcing_maker.fstate_coarse
         else:
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/init_fields.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/init_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 
           Which eigenmode (ap_fft or am_fft)
 
         """
         )
 
     def __call__(self):
-
         params = self.sim.params
 
         linear_mode = self.put_ones_linear_mode()
 
         eigenmode = self.sim.params.init_fields.linear_mode.eigenmode
 
         if eigenmode == "ap_fft":
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/_old_miguel_frequency_spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/_old_miguel_frequency_spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,14 @@
 
         # Compute sampling frequency
         freq_sampling = 1.0 / (
             self.time_decimate * self.params.time_stepping.deltat0
         )
 
         for index, file_path in enumerate(list_files):
-
             # Generating counter
             print(
                 "Computing frequency spectra = {}/{}".format(
                     index, len(list_files) - 1
                 ),
                 end="\r",
             )
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/_old_miguel_spatio_temporal_spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/_old_miguel_spatio_temporal_spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,14 @@
         # Compute sampling frequency in Hz
         freq_sampling = 1.0 / (
             self.time_decimate * self.params.time_stepping.deltat0
         )
 
         # Compute temporal FT
         for index, time_start in enumerate(times_start):
-
             # Compute index to start and to end FT
             it0 = np.argmin(abs(times - time_start))
             it1 = it0 + windows_size
 
             # Compute spectrum
             omegas, temp_spectrum = signal.periodogram(
                 spatio_temp[:, it0:it1, :, :],
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/phys_fields.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/phys_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from fluidsim.base.output.phys_fields2d import PhysFieldsBase2D
 
 
 class PhysFields2DStrat(PhysFieldsBase2D):
     """Class physical fields of solver ns2d.strat"""
 
     def update_animation(self, frame, **fargs):
-
         super().update_animation(frame, **fargs)
 
         if hasattr(self, "ratio_omegas"):
             title = (
                 self.key_field
                 + f", $R = {self.output.ratio_omegas:.2f}$"
                 + f", $F = {self.output.froude_number:.1f}$"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/print_stdout.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/print_stdout.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/spatial_means.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/spatial_means.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,14 @@
                 )
                 self.file.write(to_print)
 
             self.file.flush()
             os.fsync(self.file.fileno())
 
         if self.has_to_plot and mpi.rank == 0:
-
             self.ax_a.plot(tsim, energy, "k.")
 
             self.axe_b.plot(tsim, epsK_tot, "k.")
             if self.sim.params.forcing.enable:
                 self.axe_b.plot(tsim, PK_tot, "m.")
 
             if tsim - self.t_last_show >= self.period_show:
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/spect_energy_budget.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/spect_energy_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
                         print("warning: (abs(v.sum()) > small_value) for " + k)
                         print("k = ", k)
                         print("abs(v.sum()) = ", abs(v.sum()))
 
         return dict_results
 
     def _online_plot_saving(self, dict_results):
-
         transfer2D_EA = dict_results["transferEA_2d"]
         transfer2D_EK = dict_results["transferEK_2d"]
         transfer2D_E = transfer2D_EA + transfer2D_EK
         transfer2D_Z = dict_results["transferZ_2d"]
         khE = self.oper.khE
         PiE = cumsum_inv(transfer2D_E) * self.oper.deltak
         PiZ = cumsum_inv(transfer2D_Z) * self.oper.deltak
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
             )
 
     def load1d_means(
         self, tmin=0, tmax=None, delta_t=2, versus_kx=True, versus_ky=True
     ):
         means = {}
         with h5py.File(self.path_file1D, "r") as h5file:
-
             # Open data from file
             dset_times = h5file["times"]
             dset_kxE = h5file["kxE"]
             dset_kyE = h5file["kyE"]
             times = dset_times[...]
             means["times"] = times
             means["kx"] = dset_kxE[...]
@@ -332,15 +331,14 @@
 
         ax.legend()
 
         # from ipdb import set_trace
         # set_trace()
 
     def load2d_means(self, tmin=0, tmax=1000, delta_t=2):
-
         means = {}
         # Load data from file
         with h5py.File(self.path_file2D, "r") as h5file:
             dset_times = h5file["times"]
             means["kh"] = h5file["khE"][...]
             times = dset_times[...]
             means["times"] = times
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/output/spectra_multidim.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/output/spectra_multidim.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     Frot = -ux * px_rot - uy * py_rot
     Fb = -ux * px_b - uy * py_b - N**2 * uy
     return Frot, Fb
 
 
 class InfoSolverNS2DStrat(InfoSolverNS2D):
     def _init_root(self):
-
         super()._init_root()
 
         package = "fluidsim.solvers.ns2d.strat"
         self.module_name = package + ".solver"
         self.class_name = "Simul"
         self.short_name = "NS2D.strat"
 
@@ -223,15 +222,14 @@
         omega_dispersion_relation : arr
           Frequency dispersion relation in rad.
         """
         return self.params.N * (self.oper.KX / self.oper.K_not0)
 
 
 if __name__ == "__main__":
-
     from math import pi
 
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/state.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
                 ],
                 "keys_phys_needed": ["rot", "b"],
                 "keys_linear_eigenmodes": ["rot_fft", "b_fft"],
             }
         )
 
     def __init__(self, sim, oper=None):
-
         super().__init__(sim, oper)
 
         self.field_tmp4 = np.empty_like(self.state_phys[0])
         self.field_tmp5 = np.empty_like(self.state_phys[0])
 
     def compute(self, key, SAVE_IN_DICT=True, RAISE_ERROR=True):
         """Compute and return a variable"""
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/test_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,14 @@
         params.forcing.key_forced = "ap_fft"
         params.forcing.tcrandom_anisotropic.kz_negative_enable = False
 
 
 class TestForcingOutput(TestSimulBase):
     @classmethod
     def init_params(self):
-
         params = super().init_params()
 
         # Time stepping parameters
         params.time_stepping.USE_CFL = False
         params.time_stepping.USE_T_END = False
         params.time_stepping.it_end = 2
         params.time_stepping.deltat0 = 0.1
@@ -168,15 +167,14 @@
             if tag.startswith("periods"):
                 continue
             child = params.output[tag]
             if hasattr(child, "HAS_TO_PLOT_SAVED"):
                 child["HAS_TO_PLOT_SAVED"] = True
 
     def test_forcing_output(self):
-
         sim = self.sim
 
         sim.time_stepping.start()
 
         sim.state.compute("rot_fft")
         sim.state.compute("rot_fft")
 
@@ -189,15 +187,14 @@
 
         sim.state.init_statespect_from(ux_fft=ux_fft)
         sim.state.init_statespect_from(uy_fft=uy_fft)
 
         sim.output.compute_enstrophy()
 
         if mpi.nb_proc == 1:
-
             plt.close("all")
 
             sim.output.plot_summary()
 
             sim.output.spectra.plot2d()
 
             sim.output.spatial_means.plot_energy()
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/strat/time_stepping.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/strat/time_stepping.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/test_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     def Simul(cls):
         from fluidsim.solvers.ns2d.solver import Simul
 
         return Simul
 
     @classmethod
     def init_params(cls):
-
         params = (
             cls.params
         ) = cls.Simul.create_default_params()  # pylint: disable=maybe-no-member
         params.short_name_type_run = "test"
         params.output.sub_directory = "unittests"
 
         nh = 32
@@ -118,15 +117,14 @@
                 means["PK_tot"], self.sim.params.forcing.forcing_rate
             )
 
 
 class TestForcingOutput(TestSimulBase):
     @classmethod
     def init_params(self):
-
         params = super().init_params()
 
         params.oper.truncation_shape = "no_multiple_aliases"
         params.oper.NO_SHEAR_MODES = True
         params.oper.NO_KY0 = True
 
         params.forcing.enable = True
@@ -152,15 +150,14 @@
             if tag.startswith("periods"):
                 continue
             child = params.output[tag]
             if hasattr(child, "HAS_TO_PLOT_SAVED"):
                 child["HAS_TO_PLOT_SAVED"] = True
 
     def test_forcing_output(self):
-
         sim = self.sim
         assert f"{sim.params.oper.nx}x{sim.params.oper.ny}" in sim.name_run
 
         sim.time_stepping.start()
         self.sim.state.check_energy_equal_phys_spect()
 
         # testing phaseshift
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/test_with_uxuy.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/test_with_uxuy.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns2d/with_uxuy.py` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/with_uxuy.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         ux_fft = self.sim.state.state_spect.get_var("ux_fft")
         uy_fft = self.sim.state.state_spect.get_var("uy_fft")
         return (np.abs(ux_fft) ** 2 + np.abs(uy_fft) ** 2) / 2.0
 
 
 class InfoSolver(InfoBase):
     def _init_root(self):
-
         super()._init_root()
 
         module = "fluidsim.solvers.ns2d.with_uxuy"
         self.module_name = module
         self.class_name = "Simul"
         self.short_name = "NS2D"
 
@@ -86,15 +85,14 @@
         classes.TimeStepping.class_name = "TimeStepping"
 
 
 class Simul(SimulBase):
     InfoSolver = InfoSolver
 
     def tendencies_nonlin(self, state_spect=None, old=None):
-
         # the operator and the fast Fourier transform
         oper = self.oper
         ifft_as_arg = oper.ifft_as_arg
 
         # get or compute rot_fft, ux and uy
         if state_spect is None:
             ux_fft = self.state.state_spect.get_var("ux_fft")
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/bouss/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/bouss/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from fluidsim.base.setofvariables import SetOfVariables
 
 from ..strat.solver import InfoSolverNS3DStrat, Simul as SimulStrat
 
 
 class InfoSolverNS3DBouss(InfoSolverNS3DStrat):
     def _init_root(self):
-
         super()._init_root()
 
         package = "fluidsim.solvers.ns3d.bouss"
         self.module_name = package + ".solver"
         self.class_name = "Simul"
         self.short_name = "ns3d.bouss"
 
@@ -172,15 +171,14 @@
 
         self.project_state_spect(tendencies_fft)
         self.oper.dealiasing(tendencies_fft)
         return tendencies_fft
 
 
 if __name__ == "__main__":
-
     import numpy as np
 
     # import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/bouss/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/bouss/test_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
         # save all outputs!
         periods = params.output.periods_save
         for key in periods._key_attribs:
             periods[key] = 0.2
 
     def test_output(self):
-
         sim = self.sim
         sim.time_stepping.start()
 
         if mpi.nb_proc > 1:
             return
 
         sim2 = fls.load_sim_for_plot(sim.output.path_run)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/__pythran__/watu.cpp` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/__pythran__/watu.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -3,93 +3,79 @@
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 #include <pythonic/include/types/float64.hpp>
 #include <pythonic/include/types/ndarray.hpp>
-#include <pythonic/types/ndarray.hpp>
 #include <pythonic/types/float64.hpp>
+#include <pythonic/types/ndarray.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
+#include <pythonic/include/numpy/copyto.hpp>
 #include <pythonic/include/operator_/mul.hpp>
 #include <pythonic/include/operator_/sub.hpp>
-#include <pythonic/include/types/slice.hpp>
 #include <pythonic/include/types/str.hpp>
 #include <pythonic/builtins/tuple.hpp>
+#include <pythonic/numpy/copyto.hpp>
 #include <pythonic/operator_/mul.hpp>
 #include <pythonic/operator_/sub.hpp>
-#include <pythonic/types/slice.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_watu
+namespace 
 {
-  struct __transonic__
+  namespace __pythran_watu
   {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    struct __transonic__
     {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct compute_watu_coriolis_forcing_component
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0 sigma, argument_type1 mask, argument_type2 coef_forcing_time, argument_type3 target, argument_type4 velocity, argument_type5 out) const
+      ;
     }  ;
     inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct compute_watu_coriolis_forcing_component
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    struct type
+    typename __transonic__::type::result_type __transonic__::operator()() const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type1>(), std::declval<__type3>())) __type4;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type5;
-      typedef __type5 __type6;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type3>::type>::type __type7;
-      typedef __type7 __type8;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type6>(), std::declval<__type8>())) __type9;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type10;
-      typedef __type10 __type11;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type9>(), std::declval<__type11>())) __type12;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type4>(), std::declval<__type12>())) __type13;
-      typedef __type13 __type14;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type15;
-      typedef typename __combined<__type15,__type13>::type __type16;
-      typedef __type16 __type17;
-      typedef typename pythonic::returnable<__type17>::type __type18;
-      typedef __type14 __ptype0;
-      typedef __type18 result_type;
-    }  
-    ;
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0&& sigma, argument_type1&& mask, argument_type2&& coef_forcing_time, argument_type3&& target, argument_type4&& velocity, argument_type5&& out) const
-    ;
-  }  ;
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
+    typename compute_watu_coriolis_forcing_component::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type compute_watu_coriolis_forcing_component::operator()(argument_type0 sigma, argument_type1 mask, argument_type2 coef_forcing_time, argument_type3 target, argument_type4 velocity, argument_type5 out) const
     {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.0"));
-      return tmp_global;
+      pythonic::numpy::functor::copyto{}(out, pythonic::operator_::mul(pythonic::operator_::mul(sigma, mask), pythonic::operator_::sub(pythonic::operator_::mul(coef_forcing_time, target), velocity)));
+      return out;
     }
   }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-  inline
-  typename compute_watu_coriolis_forcing_component::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type compute_watu_coriolis_forcing_component::operator()(argument_type0&& sigma, argument_type1&& mask, argument_type2&& coef_forcing_time, argument_type3&& target, argument_type4&& velocity, argument_type5&& out) const
-  {
-    out[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::mul(pythonic::operator_::mul(sigma, mask), pythonic::operator_::sub(pythonic::operator_::mul(coef_forcing_time, target), velocity));
-    return out;
-  }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_watu::__transonic__()());
 inline
 typename __pythran_watu::compute_watu_coriolis_forcing_component::type<double, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, double, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>::result_type compute_watu_coriolis_forcing_component0(double&& sigma, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& mask, double&& coef_forcing_time, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& target, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& velocity, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& out) 
 {
@@ -186,17 +172,17 @@
                                          Methods,
                                          ""
     );
     #endif
     if(! theModule)
         PYTHRAN_RETURN;
     PyObject * theDoc = Py_BuildValue("(sss)",
-                                      "0.11.0",
-                                      "2022-09-02 03:40:18.458202",
-                                      "6e006d54cb4ea8c14a48bfd37bc3a0e7ae5456ac4d7cd80ea684e925a550c59f");
+                                      "0.13.1",
+                                      "2023-05-24 11:29:43.005653",
+                                      "6b7b77e8d40e64dbdf0b0a21f7880fa30bbd78d5da45740e57f99fedee506f97");
     if(! theDoc)
         PYTHRAN_RETURN;
     PyModule_AddObject(theModule,
                        "__pythran__",
                        theDoc);
 
     PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/milestone.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/milestone.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
                     self.oper_coarse_shapeK_loc, root=0
                 )
 
             self.solid = self.sim.oper.create_arrayX(value=0)
             self.solid_fft = self.sim.oper.create_arrayK(value=0)
 
     def __init__(self, sim):
-
         if mpi.rank == 0:
             from fluidsim.operators.operators2d import OperatorsPseudoSpectral2D
 
             params = OperatorsPseudoSpectral2D._create_default_params()
             params.oper.Lx = sim.params.oper.Lx
             params.oper.Ly = sim.params.oper.Ly
             params.oper.nx = sim.params.oper.nx
@@ -66,15 +65,14 @@
         else:
             self.oper2d_big = "sequential"
             self.solid2d_big = None
 
         super().__init__(sim)
 
     def _full_from_coarse(self, solid):
-
         if self._is_using_coarse_oper:
             if mpi.rank == 0:
                 solid_coarse_fft = self.oper_coarse.fft(solid)
                 nKyc, nKxc = self.oper_coarse_shapeK_loc
                 solid_coarse_fft[nKyc // 2, :] = 0.0
                 solid_coarse_fft[:, nKxc - 1] = 0.0
 
@@ -96,15 +94,14 @@
         self.solid = self.sim.oper.build_invariant_arrayX_from_2d_indices12X(
             self.solid2d_big, self.oper2d_big
         )
 
         return self.solid
 
     def compute(self, time=None):
-
         sim = self.sim
 
         if time is None:
             time = sim.time_stepping.t
 
         solid, x_coors, y_coors = self.get_solid_field(time)
 
@@ -120,15 +117,14 @@
         if sim.params.oper.NO_SHEAR_MODES:
             sim.oper.dealiasing(fx_fft, fy_fft)
 
         self.fstate.init_statespect_from(vx_fft=fx_fft, vy_fft=fy_fft)
 
 
 if __name__ == "__main__":
-
     from time import perf_counter
 
     import matplotlib.pyplot as plt
 
     from fluidsim.solvers.ns3d.solver import Simul
 
     params = Simul.create_default_params()
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/forcing/watu.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/forcing/watu.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
             self.interpolents = None
         else:
             path_file = Path(sim.output.path_run) / "forcing_watu_coriolis.h5"
 
             if path_file.exists():
                 # load time signals
                 with h5netcdf.File(str(path_file), "r") as file:
-
                     times = file["/times"][...]
                     signals = file["/signals"][...]
 
             else:
                 time_signal_maker = FrequencyModulatedSignalMaker(
                     total_time=sim.params.forcing.watu_coriolis.period_forcing,
                     approximate_dt=sim.params.forcing.watu_coriolis.approximate_dt,
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/init_fields.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/init_fields.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/output/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/output/__pythran__/spatiotemporal_spectra.cpp` & `fluidsim-0.7.3/fluidsim/solvers/ns2d/output/__pythran__/spatiotemporal_spectra.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 #include <pythonic/include/types/float64.hpp>
-#include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/include/types/float32.hpp>
+#include <pythonic/include/types/ndarray.hpp>
+#include <pythonic/types/float64.hpp>
 #include <pythonic/types/float32.hpp>
 #include <pythonic/types/ndarray.hpp>
-#include <pythonic/types/float64.hpp>
 #include <pythonic/include/builtins/abs.hpp>
 #include <pythonic/include/builtins/enumerate.hpp>
 #include <pythonic/include/builtins/getattr.hpp>
 #include <pythonic/include/builtins/int_.hpp>
 #include <pythonic/include/builtins/len.hpp>
 #include <pythonic/include/builtins/pythran/make_shape.hpp>
 #include <pythonic/include/builtins/range.hpp>
@@ -49,455 +49,447 @@
 #include <pythonic/operator_/iadd.hpp>
 #include <pythonic/operator_/mul.hpp>
 #include <pythonic/operator_/ne.hpp>
 #include <pythonic/operator_/neg.hpp>
 #include <pythonic/operator_/sub.hpp>
 #include <pythonic/types/slice.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_spatiotemporal_spectra
+namespace 
 {
-  struct __transonic__
+  namespace __pythran_spatiotemporal_spectra
   {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    struct __transonic__
     {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct compute_spectrum_kzkhomega
+    {
+      typedef void callable;
+      typedef void pure;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef decltype(pythonic::types::as_const(std::declval<__type1>())) __type2;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type2>::type>::type __type3;
+        typedef __type3 __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(pythonic::types::as_const(std::declval<__type6>())) __type7;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type7>::type>::type __type8;
+        typedef __type8 __type9;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros{})>::type>::type __type10;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::make_shape{})>::type>::type __type11;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::len{})>::type>::type __type12;
+        typedef std::integral_constant<long,1> __type13;
+        typedef indexable_container<__type13, typename std::remove_reference<__type8>::type> __type14;
+        typedef typename __combined<__type5,__type14>::type __type15;
+        typedef __type15 __type16;
+        typedef decltype(std::declval<__type12>()(std::declval<__type16>())) __type17;
+        typedef typename pythonic::assignable<__type17>::type __type18;
+        typedef __type18 __type19;
+        typedef indexable_container<__type13, typename std::remove_reference<__type3>::type> __type20;
+        typedef typename __combined<__type0,__type20>::type __type21;
+        typedef __type21 __type22;
+        typedef decltype(std::declval<__type12>()(std::declval<__type22>())) __type23;
+        typedef typename pythonic::assignable<__type23>::type __type24;
+        typedef __type24 __type25;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type26;
+        typedef __type26 __type27;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type27>())) __type28;
+        typedef decltype(pythonic::types::as_const(std::declval<__type28>())) __type29;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type29>::type>::type __type30;
+        typedef typename pythonic::assignable<__type30>::type __type31;
+        typedef __type31 __type32;
+        typedef long __type33;
+        typedef decltype(pythonic::operator_::add(std::declval<__type32>(), std::declval<__type33>())) __type34;
+        typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type34>(), std::declval<__type33>())) __type35;
+        typedef typename pythonic::assignable<__type35>::type __type36;
+        typedef __type36 __type37;
+        typedef decltype(std::declval<__type11>()(std::declval<__type19>(), std::declval<__type25>(), std::declval<__type37>())) __type38;
+        typedef decltype(std::declval<__type10>()(std::declval<__type38>())) __type39;
+        typedef typename pythonic::assignable<__type39>::type __type40;
+        typedef decltype(std::declval<__type11>()(std::declval<__type19>(), std::declval<__type25>(), std::declval<__type32>())) __type44;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, std::declval<__type27>())) __type46;
+        typedef decltype(std::declval<__type10>()(std::declval<__type44>(), std::declval<__type46>())) __type47;
+        typedef typename pythonic::assignable<__type47>::type __type48;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::int_{})>::type>::type __type49;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::round{})>::type>::type __type50;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type51;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type52;
+        typedef __type52 __type53;
+        typedef decltype(pythonic::types::as_const(std::declval<__type53>())) __type54;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type55;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type29>::type>::type __type56;
+        typedef typename pythonic::lazy<__type56>::type __type57;
+        typedef __type57 __type58;
+        typedef decltype(std::declval<__type55>()(std::declval<__type58>())) __type59;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type59>::type::iterator>::value_type>::type __type60;
+        typedef __type60 __type61;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type29>::type>::type __type62;
+        typedef typename pythonic::lazy<__type62>::type __type63;
+        typedef __type63 __type64;
+        typedef decltype(std::declval<__type55>()(std::declval<__type64>())) __type65;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type65>::type::iterator>::value_type>::type __type66;
+        typedef __type66 __type67;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type61>(), std::declval<__type67>())) __type68;
+        typedef decltype(std::declval<__type54>()[std::declval<__type68>()]) __type69;
+        typedef decltype(std::declval<__type51>()(std::declval<__type69>())) __type70;
+        typedef typename pythonic::assignable<__type8>::type __type71;
+        typedef __type71 __type72;
+        typedef decltype(pythonic::operator_::div(std::declval<__type70>(), std::declval<__type72>())) __type73;
+        typedef decltype(std::declval<__type50>()(std::declval<__type73>())) __type74;
+        typedef decltype(std::declval<__type49>()(std::declval<__type74>())) __type75;
+        typedef typename pythonic::lazy<__type75>::type __type76;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type19>(), std::declval<__type33>())) __type78;
+        typedef typename pythonic::lazy<__type78>::type __type79;
+        typedef typename __combined<__type76,__type79>::type __type80;
+        typedef __type80 __type81;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type25>(), std::declval<__type33>())) __type83;
+        typedef typename pythonic::lazy<__type83>::type __type84;
+        typedef __type84 __type85;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type86;
+        typedef decltype(pythonic::types::as_const(std::declval<__type27>())) __type88;
+        typedef pythonic::types::contiguous_slice __type91;
+        typedef decltype(std::declval<__type88>()(std::declval<__type61>(), std::declval<__type67>(), std::declval<__type91>())) __type92;
+        typedef typename pythonic::lazy<__type92>::type __type93;
+        typedef __type93 __type94;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type33>(), std::declval<__type94>())) __type95;
+        typedef typename pythonic::lazy<__type95>::type __type96;
+        typedef typename __combined<__type93,__type96>::type __type97;
+        typedef __type97 __type98;
+        typedef decltype(std::declval<__type86>()(std::declval<__type98>())) __type99;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type99>::type::iterator>::value_type>::type __type100;
+        typedef __type100 __type101;
+        typedef decltype(pythonic::types::as_const(std::declval<__type101>())) __type102;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type102>::type>::type __type103;
+        typedef typename pythonic::lazy<__type103>::type __type104;
+        typedef __type104 __type105;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type81>(), std::declval<__type85>(), std::declval<__type105>())) __type106;
+        typedef indexable<__type106> __type107;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type109;
+        typedef __type109 __type110;
+        typedef decltype(pythonic::types::as_const(std::declval<__type110>())) __type111;
+        typedef decltype(std::declval<__type111>()[std::declval<__type68>()]) __type115;
+        typedef typename pythonic::assignable<__type115>::type __type116;
+        typedef __type116 __type117;
+        typedef typename pythonic::assignable<__type3>::type __type118;
+        typedef __type118 __type119;
+        typedef decltype(pythonic::operator_::div(std::declval<__type117>(), std::declval<__type119>())) __type120;
+        typedef decltype(std::declval<__type49>()(std::declval<__type120>())) __type121;
+        typedef typename pythonic::assignable<__type121>::type __type122;
+        typedef __type122 __type123;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type81>(), std::declval<__type123>(), std::declval<__type105>())) __type132;
+        typedef indexable<__type132> __type133;
+        typedef decltype(pythonic::operator_::add(std::declval<__type123>(), std::declval<__type33>())) __type136;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type81>(), std::declval<__type136>(), std::declval<__type105>())) __type138;
+        typedef indexable<__type138> __type139;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type102>::type>::type __type142;
+        typedef typename pythonic::lazy<__type142>::type __type143;
+        typedef __type143 __type144;
+        typedef container<typename std::remove_reference<__type144>::type> __type145;
+        typedef decltype(pythonic::types::as_const(std::declval<__type22>())) __type148;
+        typedef decltype(std::declval<__type148>()[std::declval<__type123>()]) __type150;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type117>(), std::declval<__type150>())) __type151;
+        typedef decltype(pythonic::operator_::div(std::declval<__type151>(), std::declval<__type119>())) __type153;
+        typedef typename pythonic::assignable<__type153>::type __type154;
+        typedef __type154 __type155;
+        typedef decltype(pythonic::operator_::sub(std::declval<__type33>(), std::declval<__type155>())) __type156;
+        typedef typename pythonic::assignable<__type142>::type __type160;
+        typedef __type160 __type161;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type156>(), std::declval<__type161>())) __type162;
+        typedef container<typename std::remove_reference<__type162>::type> __type163;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type155>(), std::declval<__type161>())) __type166;
+        typedef container<typename std::remove_reference<__type166>::type> __type167;
+        typedef typename __combined<__type48,__type107,__type133,__type139,__type145,__type163,__type167>::type __type168;
+        typedef __type168 __type169;
+        typedef decltype(pythonic::types::as_const(std::declval<__type169>())) __type170;
+        typedef decltype(std::declval<__type170>()(std::declval<__type91>(), std::declval<__type91>(), std::declval<__type33>())) __type171;
+        typedef container<typename std::remove_reference<__type171>::type> __type172;
+        typedef decltype(std::declval<__type170>()(std::declval<__type91>(), std::declval<__type91>(), std::declval<__type91>())) __type175;
+        typedef pythonic::types::slice __type178;
+        typedef decltype(std::declval<__type170>()(std::declval<__type91>(), std::declval<__type91>(), std::declval<__type178>())) __type179;
+        typedef decltype(pythonic::operator_::add(std::declval<__type175>(), std::declval<__type179>())) __type180;
+        typedef container<typename std::remove_reference<__type180>::type> __type181;
+        typedef typename __combined<__type40,__type172,__type181>::type __type182;
+        typedef __type182 __type183;
+        typedef decltype(pythonic::operator_::mul(std::declval<__type72>(), std::declval<__type119>())) __type186;
+        typedef decltype(pythonic::operator_::div(std::declval<__type183>(), std::declval<__type186>())) __type187;
+        typedef typename pythonic::returnable<__type187>::type __type188;
+        typedef __type4 __ptype0;
+        typedef __type9 __ptype1;
+        typedef __type188 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0 field_k0k1omega, argument_type1 khs, argument_type2 kzs, argument_type3 KX, argument_type4 KZ, argument_type5 KH) const
+      ;
     }  ;
     inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct compute_spectrum_kzkhomega
-  {
-    typedef void callable;
-    typedef void pure;
+    typename __transonic__::type::result_type __transonic__::operator()() const
+    {
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    struct type
+    inline
+    typename compute_spectrum_kzkhomega::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type compute_spectrum_kzkhomega::operator()(argument_type0 field_k0k1omega, argument_type1 khs, argument_type2 kzs, argument_type3 KX, argument_type4 KZ, argument_type5 KH) const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type1>::type>::type __type2;
-      typedef __type2 __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type4;
-      typedef __type4 __type5;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type5>::type>::type __type6;
-      typedef __type6 __type7;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros{})>::type>::type __type8;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::make_shape{})>::type>::type __type9;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::len{})>::type>::type __type10;
-      typedef std::integral_constant<long,1> __type11;
-      typedef indexable_container<__type11, typename std::remove_reference<__type6>::type> __type12;
-      typedef typename __combined<__type4,__type12>::type __type13;
-      typedef __type13 __type14;
-      typedef decltype(std::declval<__type10>()(std::declval<__type14>())) __type15;
-      typedef typename pythonic::assignable<__type15>::type __type16;
-      typedef __type16 __type17;
-      typedef indexable_container<__type11, typename std::remove_reference<__type2>::type> __type18;
-      typedef typename __combined<__type0,__type18>::type __type19;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros{})>::type>::type __type0;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::make_shape{})>::type>::type __type1;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::len{})>::type>::type __type2;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
+      typedef std::integral_constant<long,1> __type4;
+      typedef __type3 __type5;
+      typedef decltype(pythonic::types::as_const(std::declval<__type5>())) __type6;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type6>::type>::type __type7;
+      typedef indexable_container<__type4, typename std::remove_reference<__type7>::type> __type8;
+      typedef typename __combined<__type3,__type8>::type __type9;
+      typedef __type9 __type10;
+      typedef decltype(std::declval<__type2>()(std::declval<__type10>())) __type11;
+      typedef typename pythonic::assignable<__type11>::type __type12;
+      typedef __type12 __type13;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type14;
+      typedef __type14 __type15;
+      typedef decltype(pythonic::types::as_const(std::declval<__type15>())) __type16;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type16>::type>::type __type17;
+      typedef indexable_container<__type4, typename std::remove_reference<__type17>::type> __type18;
+      typedef typename __combined<__type14,__type18>::type __type19;
       typedef __type19 __type20;
-      typedef decltype(std::declval<__type10>()(std::declval<__type20>())) __type21;
+      typedef decltype(std::declval<__type2>()(std::declval<__type20>())) __type21;
       typedef typename pythonic::assignable<__type21>::type __type22;
       typedef __type22 __type23;
       typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type24;
       typedef __type24 __type25;
       typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type25>())) __type26;
-      typedef typename std::tuple_element<3,typename std::remove_reference<__type26>::type>::type __type27;
-      typedef typename pythonic::assignable<__type27>::type __type28;
-      typedef __type28 __type29;
-      typedef long __type30;
-      typedef decltype(pythonic::operator_::add(std::declval<__type29>(), std::declval<__type30>())) __type31;
-      typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type31>(), std::declval<__type30>())) __type32;
-      typedef typename pythonic::assignable<__type32>::type __type33;
-      typedef __type33 __type34;
-      typedef decltype(std::declval<__type9>()(std::declval<__type17>(), std::declval<__type23>(), std::declval<__type34>())) __type35;
-      typedef decltype(std::declval<__type8>()(std::declval<__type35>())) __type36;
-      typedef typename pythonic::assignable<__type36>::type __type37;
-      typedef decltype(std::declval<__type9>()(std::declval<__type17>(), std::declval<__type23>(), std::declval<__type29>())) __type41;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, std::declval<__type25>())) __type43;
-      typedef decltype(std::declval<__type8>()(std::declval<__type41>(), std::declval<__type43>())) __type44;
-      typedef typename pythonic::assignable<__type44>::type __type45;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::int_{})>::type>::type __type46;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::round{})>::type>::type __type47;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type48;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type49;
-      typedef __type49 __type50;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type51;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type26>::type>::type __type52;
-      typedef typename pythonic::lazy<__type52>::type __type53;
+      typedef decltype(pythonic::types::as_const(std::declval<__type26>())) __type27;
+      typedef typename std::tuple_element<2,typename std::remove_reference<__type27>::type>::type __type28;
+      typedef typename pythonic::assignable<__type28>::type __type29;
+      typedef __type29 __type30;
+      typedef decltype(std::declval<__type1>()(std::declval<__type13>(), std::declval<__type23>(), std::declval<__type30>())) __type31;
+      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, std::declval<__type25>())) __type33;
+      typedef decltype(std::declval<__type0>()(std::declval<__type31>(), std::declval<__type33>())) __type34;
+      typedef typename pythonic::assignable<__type34>::type __type35;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::int_{})>::type>::type __type36;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::round{})>::type>::type __type37;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type38;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type39;
+      typedef __type39 __type40;
+      typedef decltype(pythonic::types::as_const(std::declval<__type40>())) __type41;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type42;
+      typedef typename std::tuple_element<0,typename std::remove_reference<__type27>::type>::type __type43;
+      typedef typename pythonic::lazy<__type43>::type __type44;
+      typedef __type44 __type45;
+      typedef decltype(std::declval<__type42>()(std::declval<__type45>())) __type46;
+      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type46>::type::iterator>::value_type>::type __type47;
+      typedef __type47 __type48;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type27>::type>::type __type49;
+      typedef typename pythonic::lazy<__type49>::type __type50;
+      typedef __type50 __type51;
+      typedef decltype(std::declval<__type42>()(std::declval<__type51>())) __type52;
+      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type52>::type::iterator>::value_type>::type __type53;
       typedef __type53 __type54;
-      typedef decltype(std::declval<__type51>()(std::declval<__type54>())) __type55;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type55>::type::iterator>::value_type>::type __type56;
-      typedef __type56 __type57;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type26>::type>::type __type58;
-      typedef typename pythonic::lazy<__type58>::type __type59;
-      typedef __type59 __type60;
-      typedef decltype(std::declval<__type51>()(std::declval<__type60>())) __type61;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type61>::type::iterator>::value_type>::type __type62;
-      typedef __type62 __type63;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type26>::type>::type __type64;
-      typedef typename pythonic::lazy<__type64>::type __type65;
-      typedef __type65 __type66;
-      typedef decltype(std::declval<__type51>()(std::declval<__type66>())) __type67;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type67>::type::iterator>::value_type>::type __type68;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type48>(), std::declval<__type54>())) __type55;
+      typedef decltype(std::declval<__type41>()[std::declval<__type55>()]) __type56;
+      typedef decltype(std::declval<__type38>()(std::declval<__type56>())) __type57;
+      typedef typename pythonic::assignable<__type7>::type __type58;
+      typedef __type58 __type59;
+      typedef decltype(pythonic::operator_::div(std::declval<__type57>(), std::declval<__type59>())) __type60;
+      typedef decltype(std::declval<__type37>()(std::declval<__type60>())) __type61;
+      typedef decltype(std::declval<__type36>()(std::declval<__type61>())) __type62;
+      typedef typename pythonic::lazy<__type62>::type __type63;
+      typedef long __type65;
+      typedef decltype(pythonic::operator_::sub(std::declval<__type13>(), std::declval<__type65>())) __type66;
+      typedef typename pythonic::lazy<__type66>::type __type67;
+      typedef typename __combined<__type63,__type67>::type __type68;
       typedef __type68 __type69;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type57>(), std::declval<__type63>(), std::declval<__type69>())) __type70;
-      typedef decltype(std::declval<__type50>()[std::declval<__type70>()]) __type71;
-      typedef decltype(std::declval<__type48>()(std::declval<__type71>())) __type72;
-      typedef typename pythonic::assignable<__type6>::type __type73;
-      typedef __type73 __type74;
-      typedef decltype(pythonic::operator_::div(std::declval<__type72>(), std::declval<__type74>())) __type75;
-      typedef decltype(std::declval<__type47>()(std::declval<__type75>())) __type76;
-      typedef decltype(std::declval<__type46>()(std::declval<__type76>())) __type77;
-      typedef typename pythonic::lazy<__type77>::type __type78;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type17>(), std::declval<__type30>())) __type80;
+      typedef decltype(pythonic::operator_::sub(std::declval<__type23>(), std::declval<__type65>())) __type71;
+      typedef typename pythonic::lazy<__type71>::type __type72;
+      typedef __type72 __type73;
+      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type74;
+      typedef decltype(pythonic::types::as_const(std::declval<__type25>())) __type76;
+      typedef pythonic::types::contiguous_slice __type79;
+      typedef decltype(std::declval<__type76>()(std::declval<__type48>(), std::declval<__type54>(), std::declval<__type79>())) __type80;
       typedef typename pythonic::lazy<__type80>::type __type81;
-      typedef typename __combined<__type78,__type81>::type __type82;
-      typedef __type82 __type83;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type23>(), std::declval<__type30>())) __type85;
-      typedef typename pythonic::lazy<__type85>::type __type86;
-      typedef __type86 __type87;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type88;
-      typedef pythonic::types::contiguous_slice __type93;
-      typedef decltype(std::declval<__type25>()(std::declval<__type57>(), std::declval<__type63>(), std::declval<__type69>(), std::declval<__type93>())) __type94;
-      typedef typename pythonic::lazy<__type94>::type __type95;
-      typedef __type95 __type96;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type30>(), std::declval<__type96>())) __type97;
-      typedef typename pythonic::lazy<__type97>::type __type98;
-      typedef typename __combined<__type95,__type98>::type __type99;
-      typedef __type99 __type100;
-      typedef decltype(std::declval<__type88>()(std::declval<__type100>())) __type101;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type101>::type::iterator>::value_type>::type __type102;
-      typedef __type102 __type103;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type103>::type>::type __type104;
-      typedef typename pythonic::lazy<__type104>::type __type105;
-      typedef __type105 __type106;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type83>(), std::declval<__type87>(), std::declval<__type106>())) __type107;
-      typedef indexable<__type107> __type108;
-      typedef typename __combined<__type45,__type108>::type __type109;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type111;
-      typedef __type111 __type112;
-      typedef decltype(std::declval<__type112>()[std::declval<__type70>()]) __type117;
-      typedef typename pythonic::assignable<__type117>::type __type118;
-      typedef __type118 __type119;
-      typedef typename pythonic::assignable<__type2>::type __type120;
-      typedef __type120 __type121;
-      typedef decltype(pythonic::operator_::div(std::declval<__type119>(), std::declval<__type121>())) __type122;
-      typedef decltype(std::declval<__type46>()(std::declval<__type122>())) __type123;
-      typedef typename pythonic::assignable<__type123>::type __type124;
-      typedef __type124 __type125;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type83>(), std::declval<__type125>(), std::declval<__type106>())) __type133;
-      typedef indexable<__type133> __type134;
-      typedef typename __combined<__type109,__type134>::type __type135;
-      typedef decltype(pythonic::operator_::add(std::declval<__type125>(), std::declval<__type30>())) __type138;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type83>(), std::declval<__type138>(), std::declval<__type106>())) __type140;
-      typedef indexable<__type140> __type141;
-      typedef typename __combined<__type135,__type141>::type __type142;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type103>::type>::type __type144;
-      typedef typename pythonic::lazy<__type144>::type __type145;
-      typedef __type145 __type146;
-      typedef container<typename std::remove_reference<__type146>::type> __type147;
-      typedef decltype(std::declval<__type20>()[std::declval<__type125>()]) __type151;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type119>(), std::declval<__type151>())) __type152;
-      typedef decltype(pythonic::operator_::div(std::declval<__type152>(), std::declval<__type121>())) __type154;
-      typedef typename pythonic::assignable<__type154>::type __type155;
-      typedef __type155 __type156;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type30>(), std::declval<__type156>())) __type157;
-      typedef typename pythonic::assignable<__type144>::type __type160;
-      typedef __type160 __type161;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type157>(), std::declval<__type161>())) __type162;
-      typedef container<typename std::remove_reference<__type162>::type> __type163;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type156>(), std::declval<__type161>())) __type166;
-      typedef container<typename std::remove_reference<__type166>::type> __type167;
-      typedef typename __combined<__type142,__type108,__type147,__type147,__type134,__type163,__type163,__type141,__type167,__type167>::type __type168;
-      typedef __type168 __type169;
-      typedef decltype(std::declval<__type169>()(std::declval<__type93>(), std::declval<__type93>(), std::declval<__type30>())) __type170;
-      typedef container<typename std::remove_reference<__type170>::type> __type171;
-      typedef decltype(std::declval<__type169>()(std::declval<__type93>(), std::declval<__type93>(), std::declval<__type93>())) __type173;
-      typedef pythonic::types::slice __type175;
-      typedef decltype(std::declval<__type169>()(std::declval<__type93>(), std::declval<__type93>(), std::declval<__type175>())) __type176;
-      typedef decltype(pythonic::operator_::add(std::declval<__type173>(), std::declval<__type176>())) __type177;
-      typedef container<typename std::remove_reference<__type177>::type> __type178;
-      typedef typename __combined<__type37,__type171,__type178>::type __type179;
-      typedef __type179 __type180;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type74>(), std::declval<__type121>())) __type183;
-      typedef decltype(pythonic::operator_::div(std::declval<__type180>(), std::declval<__type183>())) __type184;
-      typedef typename pythonic::returnable<__type184>::type __type185;
-      typedef __type3 __ptype0;
-      typedef __type7 __ptype1;
-      typedef __type185 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-    inline
-    typename type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type operator()(argument_type0&& field_k0k1k2omega, argument_type1&& khs, argument_type2&& kzs, argument_type3&& KX, argument_type4&& KZ, argument_type5&& KH) const
-    ;
-  }  ;
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
-    {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.0"));
-      return tmp_global;
-    }
-  }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 , typename argument_type3 , typename argument_type4 , typename argument_type5 >
-  inline
-  typename compute_spectrum_kzkhomega::type<argument_type0, argument_type1, argument_type2, argument_type3, argument_type4, argument_type5>::result_type compute_spectrum_kzkhomega::operator()(argument_type0&& field_k0k1k2omega, argument_type1&& khs, argument_type2&& kzs, argument_type3&& KX, argument_type4&& KZ, argument_type5&& KH) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::zeros{})>::type>::type __type0;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::pythran::functor::make_shape{})>::type>::type __type1;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::len{})>::type>::type __type2;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type3;
-    typedef std::integral_constant<long,1> __type4;
-    typedef __type3 __type5;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type5>::type>::type __type6;
-    typedef indexable_container<__type4, typename std::remove_reference<__type6>::type> __type7;
-    typedef typename __combined<__type3,__type7>::type __type8;
-    typedef __type8 __type9;
-    typedef decltype(std::declval<__type2>()(std::declval<__type9>())) __type10;
-    typedef typename pythonic::assignable<__type10>::type __type11;
-    typedef __type11 __type12;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type13;
-    typedef __type13 __type14;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type14>::type>::type __type15;
-    typedef indexable_container<__type4, typename std::remove_reference<__type15>::type> __type16;
-    typedef typename __combined<__type13,__type16>::type __type17;
-    typedef __type17 __type18;
-    typedef decltype(std::declval<__type2>()(std::declval<__type18>())) __type19;
-    typedef typename pythonic::assignable<__type19>::type __type20;
-    typedef __type20 __type21;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type22;
-    typedef __type22 __type23;
-    typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type23>())) __type24;
-    typedef typename std::tuple_element<3,typename std::remove_reference<__type24>::type>::type __type25;
-    typedef typename pythonic::assignable<__type25>::type __type26;
-    typedef __type26 __type27;
-    typedef decltype(std::declval<__type1>()(std::declval<__type12>(), std::declval<__type21>(), std::declval<__type27>())) __type28;
-    typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, std::declval<__type23>())) __type30;
-    typedef decltype(std::declval<__type0>()(std::declval<__type28>(), std::declval<__type30>())) __type31;
-    typedef typename pythonic::assignable<__type31>::type __type32;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::int_{})>::type>::type __type33;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::round{})>::type>::type __type34;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::abs{})>::type>::type __type35;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type4>::type>::type __type36;
-    typedef __type36 __type37;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type38;
-    typedef typename std::tuple_element<0,typename std::remove_reference<__type24>::type>::type __type39;
-    typedef typename pythonic::lazy<__type39>::type __type40;
-    typedef __type40 __type41;
-    typedef decltype(std::declval<__type38>()(std::declval<__type41>())) __type42;
-    typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type42>::type::iterator>::value_type>::type __type43;
-    typedef __type43 __type44;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type24>::type>::type __type45;
-    typedef typename pythonic::lazy<__type45>::type __type46;
-    typedef __type46 __type47;
-    typedef decltype(std::declval<__type38>()(std::declval<__type47>())) __type48;
-    typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type48>::type::iterator>::value_type>::type __type49;
-    typedef __type49 __type50;
-    typedef typename std::tuple_element<2,typename std::remove_reference<__type24>::type>::type __type51;
-    typedef typename pythonic::lazy<__type51>::type __type52;
-    typedef __type52 __type53;
-    typedef decltype(std::declval<__type38>()(std::declval<__type53>())) __type54;
-    typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type54>::type::iterator>::value_type>::type __type55;
-    typedef __type55 __type56;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type44>(), std::declval<__type50>(), std::declval<__type56>())) __type57;
-    typedef decltype(std::declval<__type37>()[std::declval<__type57>()]) __type58;
-    typedef decltype(std::declval<__type35>()(std::declval<__type58>())) __type59;
-    typedef typename pythonic::assignable<__type6>::type __type60;
-    typedef __type60 __type61;
-    typedef decltype(pythonic::operator_::div(std::declval<__type59>(), std::declval<__type61>())) __type62;
-    typedef decltype(std::declval<__type34>()(std::declval<__type62>())) __type63;
-    typedef decltype(std::declval<__type33>()(std::declval<__type63>())) __type64;
-    typedef typename pythonic::lazy<__type64>::type __type65;
-    typedef long __type67;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type12>(), std::declval<__type67>())) __type68;
-    typedef typename pythonic::lazy<__type68>::type __type69;
-    typedef typename __combined<__type65,__type69>::type __type70;
-    typedef __type70 __type71;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type21>(), std::declval<__type67>())) __type73;
-    typedef typename pythonic::lazy<__type73>::type __type74;
-    typedef __type74 __type75;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::enumerate{})>::type>::type __type76;
-    typedef pythonic::types::contiguous_slice __type81;
-    typedef decltype(std::declval<__type23>()(std::declval<__type44>(), std::declval<__type50>(), std::declval<__type56>(), std::declval<__type81>())) __type82;
-    typedef typename pythonic::lazy<__type82>::type __type83;
-    typedef __type83 __type84;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type67>(), std::declval<__type84>())) __type85;
-    typedef typename pythonic::lazy<__type85>::type __type86;
-    typedef typename __combined<__type83,__type86>::type __type87;
-    typedef __type87 __type88;
-    typedef decltype(std::declval<__type76>()(std::declval<__type88>())) __type89;
-    typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type89>::type::iterator>::value_type>::type __type90;
-    typedef __type90 __type91;
-    typedef typename std::tuple_element<0,typename std::remove_reference<__type91>::type>::type __type92;
-    typedef typename pythonic::lazy<__type92>::type __type93;
-    typedef __type93 __type94;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type71>(), std::declval<__type75>(), std::declval<__type94>())) __type95;
-    typedef indexable<__type95> __type96;
-    typedef typename __combined<__type32,__type96>::type __type97;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type99;
-    typedef __type99 __type100;
-    typedef decltype(std::declval<__type100>()[std::declval<__type57>()]) __type105;
-    typedef typename pythonic::assignable<__type105>::type __type106;
-    typedef __type106 __type107;
-    typedef typename pythonic::assignable<__type15>::type __type108;
-    typedef __type108 __type109;
-    typedef decltype(pythonic::operator_::div(std::declval<__type107>(), std::declval<__type109>())) __type110;
-    typedef decltype(std::declval<__type33>()(std::declval<__type110>())) __type111;
-    typedef typename pythonic::assignable<__type111>::type __type112;
-    typedef __type112 __type113;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type71>(), std::declval<__type113>(), std::declval<__type94>())) __type121;
-    typedef indexable<__type121> __type122;
-    typedef typename __combined<__type97,__type122>::type __type123;
-    typedef decltype(pythonic::operator_::add(std::declval<__type113>(), std::declval<__type67>())) __type126;
-    typedef decltype(pythonic::types::make_tuple(std::declval<__type71>(), std::declval<__type126>(), std::declval<__type94>())) __type128;
-    typedef indexable<__type128> __type129;
-    typedef typename __combined<__type123,__type129>::type __type130;
-    typedef typename std::tuple_element<1,typename std::remove_reference<__type91>::type>::type __type132;
-    typedef typename pythonic::lazy<__type132>::type __type133;
-    typedef __type133 __type134;
-    typedef container<typename std::remove_reference<__type134>::type> __type135;
-    typedef decltype(std::declval<__type18>()[std::declval<__type113>()]) __type139;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type107>(), std::declval<__type139>())) __type140;
-    typedef decltype(pythonic::operator_::div(std::declval<__type140>(), std::declval<__type109>())) __type142;
-    typedef typename pythonic::assignable<__type142>::type __type143;
-    typedef __type143 __type144;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type67>(), std::declval<__type144>())) __type145;
-    typedef typename pythonic::assignable<__type132>::type __type148;
-    typedef __type148 __type149;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type145>(), std::declval<__type149>())) __type150;
-    typedef container<typename std::remove_reference<__type150>::type> __type151;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type144>(), std::declval<__type149>())) __type154;
-    typedef container<typename std::remove_reference<__type154>::type> __type155;
-    typedef typename __combined<__type130,__type96,__type135,__type122,__type151,__type129,__type155>::type __type156;
-    typedef typename pythonic::assignable<__type156>::type __type157;
-    typedef typename pythonic::lazy<__type87>::type __type158;
-    typedef typename pythonic::lazy<__type70>::type __type159;
-    typedef typename pythonic::assignable<__type143>::type __type160;
-    typedef decltype(pythonic::operator_::add(std::declval<__type27>(), std::declval<__type67>())) __type164;
-    typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type164>(), std::declval<__type67>())) __type165;
-    typedef typename pythonic::assignable<__type165>::type __type166;
-    typedef __type166 __type167;
-    typedef decltype(std::declval<__type1>()(std::declval<__type12>(), std::declval<__type21>(), std::declval<__type167>())) __type168;
-    typedef decltype(std::declval<__type0>()(std::declval<__type168>())) __type169;
-    typedef typename pythonic::assignable<__type169>::type __type170;
-    typedef __type156 __type171;
-    typedef decltype(std::declval<__type171>()(std::declval<__type81>(), std::declval<__type81>(), std::declval<__type67>())) __type172;
-    typedef container<typename std::remove_reference<__type172>::type> __type173;
-    typedef decltype(std::declval<__type171>()(std::declval<__type81>(), std::declval<__type81>(), std::declval<__type81>())) __type175;
-    typedef pythonic::types::slice __type177;
-    typedef decltype(std::declval<__type171>()(std::declval<__type81>(), std::declval<__type81>(), std::declval<__type177>())) __type178;
-    typedef decltype(pythonic::operator_::add(std::declval<__type175>(), std::declval<__type178>())) __type179;
-    typedef container<typename std::remove_reference<__type179>::type> __type180;
-    typedef typename __combined<__type170,__type173,__type180>::type __type181;
-    typedef typename pythonic::assignable<__type181>::type __type182;
-    typename pythonic::assignable_noescape<decltype(std::get<1>(khs))>::type deltakh = std::get<1>(khs);
-    typename pythonic::assignable_noescape<decltype(std::get<1>(kzs))>::type deltakz = std::get<1>(kzs);
-    typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::len{}(khs))>::type nkh = pythonic::builtins::functor::len{}(khs);
-    typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::len{}(kzs))>::type nkz = pythonic::builtins::functor::len{}(kzs);
-    typename pythonic::lazy<decltype(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega)))>::type nk0 = std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega));
-    typename pythonic::lazy<decltype(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega)))>::type nk1 = std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega));
-    typename pythonic::lazy<decltype(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega)))>::type nk2 = std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega));
-    typename pythonic::assignable_noescape<decltype(std::get<3>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega)))>::type nomega = std::get<3>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1k2omega));
-    __type157 spectrum_kzkhomega = pythonic::numpy::functor::zeros{}(pythonic::builtins::pythran::functor::make_shape{}(nkz, nkh, nomega), pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, field_k0k1k2omega));
-    {
-      long  __target140520536253728 = nk0;
-      for (long  ik0=0L; ik0 < __target140520536253728; ik0 += 1L)
+      typedef __type81 __type82;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type65>(), std::declval<__type82>())) __type83;
+      typedef typename pythonic::lazy<__type83>::type __type84;
+      typedef typename __combined<__type81,__type84>::type __type85;
+      typedef __type85 __type86;
+      typedef decltype(std::declval<__type74>()(std::declval<__type86>())) __type87;
+      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type87>::type::iterator>::value_type>::type __type88;
+      typedef __type88 __type89;
+      typedef decltype(pythonic::types::as_const(std::declval<__type89>())) __type90;
+      typedef typename std::tuple_element<0,typename std::remove_reference<__type90>::type>::type __type91;
+      typedef typename pythonic::lazy<__type91>::type __type92;
+      typedef __type92 __type93;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type69>(), std::declval<__type73>(), std::declval<__type93>())) __type94;
+      typedef indexable<__type94> __type95;
+      typedef typename std::remove_cv<typename std::remove_reference<argument_type5>::type>::type __type97;
+      typedef __type97 __type98;
+      typedef decltype(pythonic::types::as_const(std::declval<__type98>())) __type99;
+      typedef decltype(std::declval<__type99>()[std::declval<__type55>()]) __type103;
+      typedef typename pythonic::assignable<__type103>::type __type104;
+      typedef __type104 __type105;
+      typedef typename pythonic::assignable<__type17>::type __type106;
+      typedef __type106 __type107;
+      typedef decltype(pythonic::operator_::div(std::declval<__type105>(), std::declval<__type107>())) __type108;
+      typedef decltype(std::declval<__type36>()(std::declval<__type108>())) __type109;
+      typedef typename pythonic::assignable<__type109>::type __type110;
+      typedef __type110 __type111;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type69>(), std::declval<__type111>(), std::declval<__type93>())) __type120;
+      typedef indexable<__type120> __type121;
+      typedef decltype(pythonic::operator_::add(std::declval<__type111>(), std::declval<__type65>())) __type124;
+      typedef decltype(pythonic::types::make_tuple(std::declval<__type69>(), std::declval<__type124>(), std::declval<__type93>())) __type126;
+      typedef indexable<__type126> __type127;
+      typedef typename std::tuple_element<1,typename std::remove_reference<__type90>::type>::type __type130;
+      typedef typename pythonic::lazy<__type130>::type __type131;
+      typedef __type131 __type132;
+      typedef container<typename std::remove_reference<__type132>::type> __type133;
+      typedef decltype(pythonic::types::as_const(std::declval<__type20>())) __type136;
+      typedef decltype(std::declval<__type136>()[std::declval<__type111>()]) __type138;
+      typedef decltype(pythonic::operator_::sub(std::declval<__type105>(), std::declval<__type138>())) __type139;
+      typedef decltype(pythonic::operator_::div(std::declval<__type139>(), std::declval<__type107>())) __type141;
+      typedef typename pythonic::assignable<__type141>::type __type142;
+      typedef __type142 __type143;
+      typedef decltype(pythonic::operator_::sub(std::declval<__type65>(), std::declval<__type143>())) __type144;
+      typedef typename pythonic::assignable<__type130>::type __type148;
+      typedef __type148 __type149;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type144>(), std::declval<__type149>())) __type150;
+      typedef container<typename std::remove_reference<__type150>::type> __type151;
+      typedef decltype(pythonic::operator_::mul(std::declval<__type143>(), std::declval<__type149>())) __type154;
+      typedef container<typename std::remove_reference<__type154>::type> __type155;
+      typedef typename __combined<__type35,__type95,__type121,__type127,__type133,__type151,__type155>::type __type156;
+      typedef typename pythonic::assignable<__type156>::type __type157;
+      typedef typename pythonic::lazy<__type85>::type __type158;
+      typedef typename pythonic::lazy<__type68>::type __type159;
+      typedef decltype(pythonic::operator_::add(std::declval<__type30>(), std::declval<__type65>())) __type163;
+      typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type163>(), std::declval<__type65>())) __type164;
+      typedef typename pythonic::assignable<__type164>::type __type165;
+      typedef __type165 __type166;
+      typedef decltype(std::declval<__type1>()(std::declval<__type13>(), std::declval<__type23>(), std::declval<__type166>())) __type167;
+      typedef decltype(std::declval<__type0>()(std::declval<__type167>())) __type168;
+      typedef typename pythonic::assignable<__type168>::type __type169;
+      typedef __type156 __type170;
+      typedef decltype(pythonic::types::as_const(std::declval<__type170>())) __type171;
+      typedef decltype(std::declval<__type171>()(std::declval<__type79>(), std::declval<__type79>(), std::declval<__type65>())) __type172;
+      typedef container<typename std::remove_reference<__type172>::type> __type173;
+      typedef decltype(std::declval<__type171>()(std::declval<__type79>(), std::declval<__type79>(), std::declval<__type79>())) __type176;
+      typedef pythonic::types::slice __type179;
+      typedef decltype(std::declval<__type171>()(std::declval<__type79>(), std::declval<__type79>(), std::declval<__type179>())) __type180;
+      typedef decltype(pythonic::operator_::add(std::declval<__type176>(), std::declval<__type180>())) __type181;
+      typedef container<typename std::remove_reference<__type181>::type> __type182;
+      typedef typename __combined<__type169,__type173,__type182>::type __type183;
+      typedef typename pythonic::assignable<__type183>::type __type184;
+      typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(khs)))>::type deltakh = std::get<1>(pythonic::types::as_const(khs));
+      typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(kzs)))>::type deltakz = std::get<1>(pythonic::types::as_const(kzs));
+      typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::len{}(khs))>::type nkh = pythonic::builtins::functor::len{}(khs);
+      typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::len{}(kzs))>::type nkz = pythonic::builtins::functor::len{}(kzs);
+      typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega))))>::type nk0 = std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega)));
+      typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega))))>::type nk1 = std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega)));
+      typename pythonic::assignable_noescape<decltype(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega))))>::type nomega = std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_k0k1omega)));
+      __type157 spectrum_kzkhomega = pythonic::numpy::functor::zeros{}(pythonic::builtins::pythran::functor::make_shape{}(nkz, nkh, nomega), pythonic::builtins::getattr(pythonic::types::attr::DTYPE{}, field_k0k1omega));
       {
+        long  __target139658371146320 = nk0;
+        for (long  ik0=0L; ik0 < __target139658371146320; ik0 += 1L)
         {
-          long  __target140520536199072 = nk1;
-          for (long  ik1=0L; ik1 < __target140520536199072; ik1 += 1L)
           {
+            long  __target139658371153008 = nk1;
+            for (long  ik1=0L; ik1 < __target139658371153008; ik1 += 1L)
             {
-              long  __target140520536192384 = nk2;
-              for (long  ik2=0L; ik2 < __target140520536192384; ik2 += 1L)
+              __type158 values = pythonic::types::as_const(field_k0k1omega)(ik0,ik1,pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None));
+              if (pythonic::operator_::ne(pythonic::types::as_const(KX)[pythonic::types::make_tuple(ik0, ik1)], 0.0))
               {
-                __type158 values = field_k0k1k2omega(ik0,ik1,ik2,pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None));
-                if (pythonic::operator_::ne(KX[pythonic::types::make_tuple(ik0, ik1, ik2)], 0.0))
-                {
-                  values = pythonic::operator_::mul(2L, values);
-                }
-                typename pythonic::assignable_noescape<decltype(KH[pythonic::types::make_tuple(ik0, ik1, ik2)])>::type kappa = KH[pythonic::types::make_tuple(ik0, ik1, ik2)];
-                typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::int_{}(pythonic::operator_::div(kappa, deltakh)))>::type ikh = pythonic::builtins::functor::int_{}(pythonic::operator_::div(kappa, deltakh));
-                __type159 ikz = pythonic::builtins::functor::int_{}(pythonic::builtins::functor::round{}(pythonic::operator_::div(pythonic::builtins::functor::abs{}(KZ[pythonic::types::make_tuple(ik0, ik1, ik2)]), deltakz)));
-                if (pythonic::operator_::ge(ikz, pythonic::operator_::sub(nkz, 1L)))
-                {
-                  ikz = pythonic::operator_::sub(nkz, 1L);
-                }
+                values = pythonic::operator_::mul(2L, values);
+              }
+              typename pythonic::assignable_noescape<decltype(pythonic::types::as_const(KH)[pythonic::types::make_tuple(ik0, ik1)])>::type kappa = pythonic::types::as_const(KH)[pythonic::types::make_tuple(ik0, ik1)];
+              typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::int_{}(pythonic::operator_::div(kappa, deltakh)))>::type ikh = pythonic::builtins::functor::int_{}(pythonic::operator_::div(kappa, deltakh));
+              __type159 ikz = pythonic::builtins::functor::int_{}(pythonic::builtins::functor::round{}(pythonic::operator_::div(pythonic::builtins::functor::abs{}(pythonic::types::as_const(KZ)[pythonic::types::make_tuple(ik0, ik1)]), deltakz)));
+              if (pythonic::operator_::ge(ikz, pythonic::operator_::sub(nkz, 1L)))
+              {
+                ikz = pythonic::operator_::sub(nkz, 1L);
+              }
+              if (pythonic::operator_::ge(ikh, pythonic::operator_::sub(nkh, 1L)))
+              {
+                typename pythonic::lazy<decltype(pythonic::operator_::sub(nkh, 1L))>::type ikh_ = pythonic::operator_::sub(nkh, 1L);
                 {
-                  __type160 coef_share;
-                  if (pythonic::operator_::ge(ikh, pythonic::operator_::sub(nkh, 1L)))
+                  for (auto&& __tuple0: pythonic::builtins::functor::enumerate{}(values))
                   {
-                    typename pythonic::lazy<decltype(pythonic::operator_::sub(nkh, 1L))>::type ikh_ = pythonic::operator_::sub(nkh, 1L);
-                    {
-                      for (auto&& __tuple0: pythonic::builtins::functor::enumerate{}(values))
-                      {
-                        typename pythonic::lazy<decltype(std::get<1>(__tuple0))>::type value = std::get<1>(__tuple0);
-                        typename pythonic::lazy<decltype(std::get<0>(__tuple0))>::type i = std::get<0>(__tuple0);
-                        spectrum_kzkhomega[pythonic::types::make_tuple(ikz, ikh_, i)] += value;
-                      }
-                    }
+                    typename pythonic::lazy<decltype(std::get<1>(pythonic::types::as_const(__tuple0)))>::type value = std::get<1>(pythonic::types::as_const(__tuple0));
+                    typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(__tuple0)))>::type i = std::get<0>(pythonic::types::as_const(__tuple0));
+                    pythonic::types::as_const(spectrum_kzkhomega)[pythonic::types::make_tuple(ikz, ikh_, i)] += value;
                   }
-                  else
+                }
+              }
+              else
+              {
+                typename pythonic::assignable_noescape<decltype(pythonic::operator_::div(pythonic::operator_::sub(kappa, pythonic::types::as_const(khs)[ikh]), deltakh))>::type coef_share = pythonic::operator_::div(pythonic::operator_::sub(kappa, pythonic::types::as_const(khs)[ikh]), deltakh);
+                {
+                  for (auto&& __tuple1: pythonic::builtins::functor::enumerate{}(values))
                   {
-                    coef_share = pythonic::operator_::div(pythonic::operator_::sub(kappa, khs[ikh]), deltakh);
-                    {
-                      for (auto&& __tuple1: pythonic::builtins::functor::enumerate{}(values))
-                      {
-                        typename pythonic::assignable_noescape<decltype(std::get<1>(__tuple1))>::type value_ = std::get<1>(__tuple1);
-                        typename pythonic::lazy<decltype(std::get<0>(__tuple1))>::type i_ = std::get<0>(__tuple1);
-                        spectrum_kzkhomega[pythonic::types::make_tuple(ikz, ikh, i_)] += pythonic::operator_::mul(pythonic::operator_::sub(1L, coef_share), value_);
-                        spectrum_kzkhomega[pythonic::types::make_tuple(ikz, pythonic::operator_::add(ikh, 1L), i_)] += pythonic::operator_::mul(coef_share, value_);
-                      }
-                    }
+                    typename pythonic::assignable_noescape<decltype(std::get<1>(pythonic::types::as_const(__tuple1)))>::type value_ = std::get<1>(pythonic::types::as_const(__tuple1));
+                    typename pythonic::lazy<decltype(std::get<0>(pythonic::types::as_const(__tuple1)))>::type i_ = std::get<0>(pythonic::types::as_const(__tuple1));
+                    pythonic::types::as_const(spectrum_kzkhomega)[pythonic::types::make_tuple(ikz, ikh, i_)] += pythonic::operator_::mul(pythonic::operator_::sub(1L, coef_share), value_);
+                    pythonic::types::as_const(spectrum_kzkhomega)[pythonic::types::make_tuple(ikz, pythonic::operator_::add(ikh, 1L), i_)] += pythonic::operator_::mul(coef_share, value_);
                   }
                 }
               }
             }
           }
         }
       }
+      typename pythonic::assignable_noescape<decltype(pythonic::operator_::functor::floordiv()(pythonic::operator_::add(nomega, 1L), 2L))>::type nomega_ = pythonic::operator_::functor::floordiv()(pythonic::operator_::add(nomega, 1L), 2L);
+      __type184 spectrum_onesided = pythonic::numpy::functor::zeros{}(pythonic::builtins::pythran::functor::make_shape{}(nkz, nkh, nomega_));
+      spectrum_onesided(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),0L) = pythonic::types::as_const(spectrum_kzkhomega)(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),0L);
+      spectrum_onesided(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(1L,pythonic::builtins::None)) = pythonic::operator_::add(pythonic::types::as_const(spectrum_kzkhomega)(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(1L,nomega_)), pythonic::types::as_const(spectrum_kzkhomega)(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::slice(-1L,pythonic::operator_::neg(nomega_),-1L)));
+      return pythonic::operator_::div(spectrum_onesided, pythonic::operator_::mul(deltakz, deltakh));
     }
-    typename pythonic::assignable_noescape<decltype(pythonic::operator_::functor::floordiv()(pythonic::operator_::add(nomega, 1L), 2L))>::type nomega_ = pythonic::operator_::functor::floordiv()(pythonic::operator_::add(nomega, 1L), 2L);
-    __type182 spectrum_onesided = pythonic::numpy::functor::zeros{}(pythonic::builtins::pythran::functor::make_shape{}(nkz, nkh, nomega_));
-    spectrum_onesided(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),0L) = spectrum_kzkhomega(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),0L);
-    spectrum_onesided(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(1L,pythonic::builtins::None)) = pythonic::operator_::add(spectrum_kzkhomega(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(1L,nomega_)), spectrum_kzkhomega(pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None),pythonic::types::slice(-1L,pythonic::operator_::neg(nomega_),-1L)));
-    return pythonic::operator_::div(spectrum_onesided, pythonic::operator_::mul(deltakz, deltakh));
   }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_spatiotemporal_spectra::__transonic__()());
 inline
-typename __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega::type<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>::result_type compute_spectrum_kzkhomega0(pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long,long>>&& field_k0k1k2omega, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& khs, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& kzs, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KX, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KZ, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KH) 
+typename __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega::type<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>::result_type compute_spectrum_kzkhomega0(pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& field_k0k1omega, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& khs, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& kzs, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KX, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KZ, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KH) 
 {
   
                             PyThreadState *_save = PyEval_SaveThread();
                             try {
-                                auto res = __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega()(field_k0k1k2omega, khs, kzs, KX, KZ, KH);
+                                auto res = __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega()(field_k0k1omega, khs, kzs, KX, KZ, KH);
                                 PyEval_RestoreThread(_save);
                                 return res;
                             }
                             catch(...) {
                                 PyEval_RestoreThread(_save);
                                 throw;
                             }
                             ;
 }
 inline
-typename __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega::type<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>::result_type compute_spectrum_kzkhomega1(pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long,long>>&& field_k0k1k2omega, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& khs, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& kzs, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KX, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KZ, pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>&& KH) 
+typename __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega::type<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>::result_type compute_spectrum_kzkhomega1(pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long>>&& field_k0k1omega, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& khs, pythonic::types::ndarray<double,pythonic::types::pshape<long>>&& kzs, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KX, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KZ, pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>&& KH) 
 {
   
                             PyThreadState *_save = PyEval_SaveThread();
                             try {
-                                auto res = __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega()(field_k0k1k2omega, khs, kzs, KX, KZ, KH);
+                                auto res = __pythran_spatiotemporal_spectra::compute_spectrum_kzkhomega()(field_k0k1omega, khs, kzs, KX, KZ, KH);
                                 PyEval_RestoreThread(_save);
                                 return res;
                             }
                             catch(...) {
                                 PyEval_RestoreThread(_save);
                                 throw;
                             }
@@ -505,36 +497,36 @@
 }
 
 static PyObject *
 __pythran_wrap_compute_spectrum_kzkhomega0(PyObject *self, PyObject *args, PyObject *kw)
 {
     PyObject* args_obj[6+1];
     
-    char const* keywords[] = {"field_k0k1k2omega", "khs", "kzs", "KX", "KZ", "KH",  nullptr};
+    char const* keywords[] = {"field_k0k1omega", "khs", "kzs", "KX", "KZ", "KH",  nullptr};
     if(! PyArg_ParseTupleAndKeywords(args, kw, "OOOOOO",
                                      (char**)keywords , &args_obj[0], &args_obj[1], &args_obj[2], &args_obj[3], &args_obj[4], &args_obj[5]))
         return nullptr;
-    if(is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long,long>>>(args_obj[0]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[3]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[4]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[5]))
-        return to_python(compute_spectrum_kzkhomega0(from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long,long>>>(args_obj[0]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[3]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[4]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[5])));
+    if(is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[0]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[3]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[4]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[5]))
+        return to_python(compute_spectrum_kzkhomega0(from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[0]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[3]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[4]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[5])));
     else {
         return nullptr;
     }
 }
 
 static PyObject *
 __pythran_wrap_compute_spectrum_kzkhomega1(PyObject *self, PyObject *args, PyObject *kw)
 {
     PyObject* args_obj[6+1];
     
-    char const* keywords[] = {"field_k0k1k2omega", "khs", "kzs", "KX", "KZ", "KH",  nullptr};
+    char const* keywords[] = {"field_k0k1omega", "khs", "kzs", "KX", "KZ", "KH",  nullptr};
     if(! PyArg_ParseTupleAndKeywords(args, kw, "OOOOOO",
                                      (char**)keywords , &args_obj[0], &args_obj[1], &args_obj[2], &args_obj[3], &args_obj[4], &args_obj[5]))
         return nullptr;
-    if(is_convertible<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long,long>>>(args_obj[0]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[3]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[4]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[5]))
-        return to_python(compute_spectrum_kzkhomega1(from_python<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long,long>>>(args_obj[0]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[3]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[4]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long,long>>>(args_obj[5])));
+    if(is_convertible<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long>>>(args_obj[0]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[3]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[4]) && is_convertible<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[5]))
+        return to_python(compute_spectrum_kzkhomega1(from_python<pythonic::types::ndarray<float,pythonic::types::pshape<long,long,long>>>(args_obj[0]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[1]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long>>>(args_obj[2]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[3]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[4]), from_python<pythonic::types::ndarray<double,pythonic::types::pshape<long,long>>>(args_obj[5])));
     else {
         return nullptr;
     }
 }
 
             static PyObject *
             __pythran_wrapall_compute_spectrum_kzkhomega(PyObject *self, PyObject *args, PyObject *kw)
@@ -548,25 +540,25 @@
 
 
 if(PyObject* obj = __pythran_wrap_compute_spectrum_kzkhomega1(self, args, kw))
     return obj;
 PyErr_Clear();
 
                 return pythonic::python::raise_invalid_argument(
-                               "compute_spectrum_kzkhomega", "\n""    - compute_spectrum_kzkhomega(float64[:,:,:,:], float64[:], float64[:], float64[:,:,:], float64[:,:,:], float64[:,:,:])\n""    - compute_spectrum_kzkhomega(float32[:,:,:,:], float64[:], float64[:], float64[:,:,:], float64[:,:,:], float64[:,:,:])", args, kw);
+                               "compute_spectrum_kzkhomega", "\n""    - compute_spectrum_kzkhomega(float64[:,:,:], float64[:], float64[:], float64[:,:], float64[:,:], float64[:,:])\n""    - compute_spectrum_kzkhomega(float32[:,:,:], float64[:], float64[:], float64[:,:], float64[:,:], float64[:,:])", args, kw);
                 });
             }
 
 
 static PyMethodDef Methods[] = {
     {
     "compute_spectrum_kzkhomega",
     (PyCFunction)__pythran_wrapall_compute_spectrum_kzkhomega,
     METH_VARARGS | METH_KEYWORDS,
-    "Compute the kz-kh-omega spectrum.\n""\n""    Supported prototypes:\n""\n""    - compute_spectrum_kzkhomega(float64[:,:,:,:], float64[:], float64[:], float64[:,:,:], float64[:,:,:], float64[:,:,:])\n""    - compute_spectrum_kzkhomega(float32[:,:,:,:], float64[:], float64[:], float64[:,:,:], float64[:,:,:], float64[:,:,:])"},
+    "Compute the kz-kh-omega spectrum.\n""\n""    Supported prototypes:\n""\n""    - compute_spectrum_kzkhomega(float64[:,:,:], float64[:], float64[:], float64[:,:], float64[:,:], float64[:,:])\n""    - compute_spectrum_kzkhomega(float32[:,:,:], float64[:], float64[:], float64[:,:], float64[:,:], float64[:,:])"},
     {NULL, NULL, 0, NULL}
 };
 
 
 #if PY_MAJOR_VERSION >= 3
   static struct PyModuleDef moduledef = {
     PyModuleDef_HEAD_INIT,
@@ -604,17 +596,17 @@
                                          Methods,
                                          ""
     );
     #endif
     if(! theModule)
         PYTHRAN_RETURN;
     PyObject * theDoc = Py_BuildValue("(sss)",
-                                      "0.11.0",
-                                      "2022-09-02 03:40:20.225730",
-                                      "e8bf3e8a4801b600253028001c7ec341265a8b3ec02de09749b7bc03912fd645");
+                                      "0.13.1",
+                                      "2023-05-24 11:29:42.277444",
+                                      "737ec20eeee4d39c1fdac4c45595b38907201ee7114d1ec14ac609a32444d94f");
     if(! theDoc)
         PYTHRAN_RETURN;
     PyModule_AddObject(theModule,
                        "__pythran__",
                        theDoc);
 
     PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/output/print_stdout.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/output/print_stdout.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/output/spatial_means.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/output/spatial_means.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
                 / 2
             )
 
             PK1 = self.sum_wavenumbers(PK1_fft)
             PK2 = self.sum_wavenumbers(PK2_fft)
 
         if mpi.rank == 0:
-
             self.file.write(
                 f"####\ntime = {tsim:11.5e}\n"
                 f"E    = {energy:11.5e}\n"
                 f"Ex   = {nrj_vx:11.5e} ; Ey   = {nrj_vy:11.5e} ; Ez   = {nrj_vz:11.5e}\n"
                 f"epsK = {epsK:11.5e} ; epsK_hypo = {epsK_hypo:11.5e} ; "
                 f"epsK_tot = {epsK + epsK_hypo:11.5e} \n"
             )
@@ -94,15 +93,14 @@
                     f"PK_tot   = {PK1 + PK2:11.5e} \n"
                 )
 
             self.file.flush()
             os.fsync(self.file.fileno())
 
         if self.has_to_plot and mpi.rank == 0:
-
             self.ax_a.plot(tsim, energy, "k.")
 
             # self.axe_b.plot(tsim, epsK_tot, 'k.')
             # if self.sim.params.forcing.enable:
             #     self.axe_b.plot(tsim, PK_tot, 'm.')
 
             if tsim - self.t_last_show >= self.period_show:
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/output/spatiotemporal_spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/output/spatiotemporal_spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
                 if kx != 0.0 and kx != kx_max:
                     value *= 2
                 result += value
     return result
 
 
 class SpatioTemporalSpectraNS3D(SpatioTemporalSpectraNS, SpatioTemporalSpectra3D):
-
     compute_spectrum_kzkhomega = staticmethod(compute_spectrum_kzkhomega)
     _sum_wavenumber = staticmethod(_sum_wavenumber3D)
 
     def compute_spectra_urud(self, tmin=0, tmax=None, dtype=None):
         """compute the spectra of ur, ud from files"""
         # load time series as state_spect arrays + times
         series = self.load_time_series(
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/output/spect_energy_budget.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/output/spect_energy_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 
                       If True, some curves can be plotted during the run.
         """
             )
         )
 
     def __init__(self, output):
-
         params = output.sim.params
         self.nx = params.oper.nx
 
         self.oper = oper = output.sim.oper
 
         kx = oper.deltakx * np.arange(oper.nkx_spectra)
         ky = oper.deltaky * np.arange(oper.nky_spectra)
@@ -106,15 +105,14 @@
             name: spectrum_kzkh,
             name + "_kx": spectrum_kx,
             name + "_ky": spectrum_ky,
             name + "_kz": spectrum_kz,
         }
 
     def compute(self):
-
         results = {}
         state = self.sim.state
 
         oper = self.sim.oper
         ifft_as_arg_destroy = oper.ifft_as_arg_destroy
 
         state_spect = state.state_spect
@@ -241,15 +239,14 @@
                 spect = file[key][imin_plot : imax_plot + 1].mean(0)
                 means[key] = spect
         return means
 
     _key_plot_default_kzkh = "transfer_Kh"
 
     def plot_kzkh(self, tmin=0, tmax=None, key=None, ax=None):
-
         with h5py.File(self.path_file, "r") as file:
             keys_saved = [
                 key
                 for key in file.keys()
                 if key not in ("times", "info_simul")
                 and not key.startswith("k")
                 and not any(key.endswith("_k" + letter) for letter in "xyz")
@@ -272,15 +269,14 @@
         ax.set_xlabel(r"$\kappa_h$")
         ax.set_ylabel("$k_z$")
         ax.set_title(f"{key}\n{self.output.summary_simul}")
 
         ax.pcolormesh(kh, kz, spectrum, shading="nearest")
 
     def compute_fluxes_mean(self, tmin=None, tmax=None):
-
         with h5py.File(self.path_file, "r") as file:
             keys_saved = [
                 key
                 for key in file.keys()
                 if key not in ("times", "info_simul")
                 and not key.startswith("k")
                 and not any(key.endswith("_k" + letter) for letter in "xyz")
@@ -313,15 +309,14 @@
 
             key_flux = "zflux_" + key
             dict_results.update({key_flux: flux})
 
         return dict_results
 
     def plot_fluxes(self, tmin=None, tmax=None, key_k="kh", ax=None):
-
         data = self.compute_fluxes_mean(tmin, tmax)
 
         k_plot = data[key_k]
         deltak = k_plot[1]
         k_plot += deltak / 2
 
         key_flux = key_k[1] + "flux_"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/output/spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/output/spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,14 @@
         coef_plot_k53=None,
         coef_plot_k2=None,
         xlim=None,
         ylim=None,
         only_time_average=False,
         cmap=None,
     ):
-
         self._plot_times(
             tmin=tmin,
             tmax=tmax,
             delta_t=delta_t,
             coef_compensate=coef_compensate,
             key=key,
             key_k=key_k,
@@ -151,15 +150,14 @@
         coef_plot_k53=None,
         coef_plot_k2=None,
         xlim=None,
         ylim=None,
         only_time_average=False,
         cmap=None,
     ):
-
         self._plot_times(
             tmin=tmin,
             tmax=tmax,
             delta_t=delta_t,
             coef_compensate=coef_compensate,
             key=key,
             coef_plot_k3=coef_plot_k3,
@@ -185,15 +183,14 @@
         coef_plot_k2=None,
         xlim=None,
         ylim=None,
         only_time_average=False,
         ndim=1,
         cmap=None,
     ):
-
         if ndim not in [1, 3]:
             raise ValueError
 
         path_file = getattr(self, f"path_file{ndim}d")
 
         if ndim == 1:
             key_spectra = "spectra_" + key + "_" + key_k
@@ -298,15 +295,14 @@
         coef_plot_k2=None,
         xlim=None,
         ylim=None,
         directions=("x", "z"),
         plot_forcing_region=False,
         plot_dissipative_scales=False,
     ):
-
         ax = self._plot_ndim(
             tmin,
             tmax,
             coef_compensate=coef_compensate,
             coef_plot_k3=coef_plot_k3,
             coef_plot_k53=coef_plot_k53,
             coef_plot_k2=coef_plot_k2,
@@ -316,15 +312,14 @@
             directions=directions,
         )
 
         factor = 2
         ymin, ymax = ax.get_ybound()
 
         if plot_forcing_region:
-
             with h5py.File(self.path_file1d, "r") as h5file:
                 kx = h5file["kx"][...]
                 ky = h5file["ky"][...]
                 kz = h5file["kz"][...]
 
             if self.params.forcing.type == "tcrandom_anisotropic":
                 angle = ensure_radians(
@@ -409,15 +404,14 @@
         coef_compensate=0,
         coef_plot_k3=None,
         coef_plot_k53=None,
         coef_plot_k2=None,
         xlim=None,
         ylim=None,
     ):
-
         ax = self._plot_ndim(
             tmin,
             tmax,
             coef_compensate=coef_compensate,
             coef_plot_k3=coef_plot_k3,
             coef_plot_k53=coef_plot_k53,
             coef_plot_k2=coef_plot_k2,
@@ -527,15 +521,14 @@
             ax.legend(loc="lower left")
 
         return ax
 
     def _plot1d_direction(
         self, direction, imin_plot, imax_plot, coef_compensate, ax
     ):
-
         with h5py.File(self.path_file1d, "r") as h5file:
             ks = h5file["k" + direction][...]
             spectrum = _get_averaged_spectrum(
                 "spectra_E_k" + direction, h5file, imin_plot, imax_plot
             )
 
         ks_no0 = ks.copy()
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     SimulBasePseudoSpectral,
     InfoSolverPseudoSpectral3D,
 )
 
 
 class InfoSolverNS3D(InfoSolverPseudoSpectral3D):
     def _init_root(self):
-
         super()._init_root()
 
         package = "fluidsim.solvers.ns3d"
         self.module_name = package + ".solver"
         self.class_name = "Simul"
         self.short_name = "ns3d"
 
@@ -141,15 +140,14 @@
     If "toroidal" or "vortical", the solution and the equations are projected
     on the toroidal manifold. If "poloidal", on the poloidal one.
 
 """
         )
 
     def _init_projection(self):
-
         try:
             self.no_vz_kz0 = self.params.no_vz_kz0
         except AttributeError:
             self.no_vz_kz0 = False
 
         if self.no_vz_kz0:
             self.where_kz_0 = np.array(
@@ -274,15 +272,14 @@
         + "\n    ".join(params.__str__().split("\n\n", 1)[1].split("\n"))
         + "\n"
         + params._get_formatted_docs()
     )
 
 
 if __name__ == "__main__":
-
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
 
     n = 32
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/state.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
                     "vt_fft",
                 ],
                 "keys_linear_eigenmodes": ["vp_fft", "vt_fft"],
             }
         )
 
     def __init__(self, sim, oper=None):
-
         super().__init__(sim, oper)
 
         self.fields_tmp = tuple(
             np.empty_like(self.state_phys[0]) for n in range(6)
         )
 
         self.fields_spect_tmp = tuple(
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/__pythran__/solver.cpp` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/__pythran__/solver.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,94 @@
 #include <pythonic/core.hpp>
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
-#include <pythonic/include/types/int.hpp>
 #include <pythonic/include/types/float64.hpp>
-#include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/include/types/complex128.hpp>
-#include <pythonic/types/int.hpp>
-#include <pythonic/types/ndarray.hpp>
+#include <pythonic/include/types/ndarray.hpp>
+#include <pythonic/include/types/int.hpp>
 #include <pythonic/types/float64.hpp>
+#include <pythonic/types/ndarray.hpp>
+#include <pythonic/types/int.hpp>
 #include <pythonic/types/complex128.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
+#include <pythonic/include/numpy/copyto.hpp>
 #include <pythonic/include/numpy/square.hpp>
 #include <pythonic/include/operator_/mul.hpp>
 #include <pythonic/include/operator_/neg.hpp>
 #include <pythonic/include/operator_/sub.hpp>
-#include <pythonic/include/types/slice.hpp>
 #include <pythonic/include/types/str.hpp>
 #include <pythonic/builtins/tuple.hpp>
+#include <pythonic/numpy/copyto.hpp>
 #include <pythonic/numpy/square.hpp>
 #include <pythonic/operator_/mul.hpp>
 #include <pythonic/operator_/neg.hpp>
 #include <pythonic/operator_/sub.hpp>
-#include <pythonic/types/slice.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_solver
+namespace 
 {
-  struct __transonic__
+  namespace __pythran_solver
   {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    struct __transonic__
     {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
+    }  ;
+    struct compute_fb_fft
+    {
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef __type1 __type2;
+        typedef typename pythonic::assignable<__type1>::type __type3;
+        typedef __type3 __type4;
+        typedef typename pythonic::returnable<__type4>::type __type5;
+        typedef __type2 __ptype0;
+        typedef __type5 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
+      inline
+      typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0 div_vb_fft, argument_type1 N, argument_type2 vz_fft) const
+      ;
     }  ;
     inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct compute_fb_fft
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-    struct type
+    typename __transonic__::type::result_type __transonic__::operator()() const
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef __type1 __type2;
-      typedef typename pythonic::assignable<__type1>::type __type3;
-      typedef decltype(pythonic::operator_::neg(std::declval<__type1>())) __type5;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type6;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type7;
-      typedef __type7 __type8;
-      typedef decltype(std::declval<__type6>()(std::declval<__type8>())) __type9;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type10;
-      typedef __type10 __type11;
-      typedef decltype(pythonic::operator_::mul(std::declval<__type9>(), std::declval<__type11>())) __type12;
-      typedef decltype(pythonic::operator_::sub(std::declval<__type5>(), std::declval<__type12>())) __type13;
-      typedef typename __combined<__type3,__type13>::type __type14;
-      typedef __type14 __type15;
-      typedef typename pythonic::returnable<__type15>::type __type16;
-      typedef __type2 __ptype0;
-      typedef __type16 result_type;
-    }  
-    ;
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
+    }
     template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
     inline
-    typename type<argument_type0, argument_type1, argument_type2>::result_type operator()(argument_type0&& div_vb_fft, argument_type1&& N, argument_type2&& vz_fft) const
-    ;
-  }  ;
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
+    typename compute_fb_fft::type<argument_type0, argument_type1, argument_type2>::result_type compute_fb_fft::operator()(argument_type0 div_vb_fft, argument_type1 N, argument_type2 vz_fft) const
     {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.0"));
-      return tmp_global;
+      typename pythonic::assignable_noescape<decltype(div_vb_fft)>::type fb_fft = div_vb_fft;
+      pythonic::numpy::functor::copyto{}(fb_fft, pythonic::operator_::sub(pythonic::operator_::neg(div_vb_fft), pythonic::operator_::mul(pythonic::numpy::functor::square{}(N), vz_fft)));
+      return fb_fft;
     }
   }
-  template <typename argument_type0 , typename argument_type1 , typename argument_type2 >
-  inline
-  typename compute_fb_fft::type<argument_type0, argument_type1, argument_type2>::result_type compute_fb_fft::operator()(argument_type0&& div_vb_fft, argument_type1&& N, argument_type2&& vz_fft) const
-  {
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-    typedef __type0 __type1;
-    typedef typename pythonic::assignable<__type1>::type __type2;
-    typedef decltype(pythonic::operator_::neg(std::declval<__type1>())) __type4;
-    typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::numpy::functor::square{})>::type>::type __type5;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type6;
-    typedef __type6 __type7;
-    typedef decltype(std::declval<__type5>()(std::declval<__type7>())) __type8;
-    typedef typename std::remove_cv<typename std::remove_reference<argument_type2>::type>::type __type9;
-    typedef __type9 __type10;
-    typedef decltype(pythonic::operator_::mul(std::declval<__type8>(), std::declval<__type10>())) __type11;
-    typedef decltype(pythonic::operator_::sub(std::declval<__type4>(), std::declval<__type11>())) __type12;
-    typedef typename __combined<__type2,__type12>::type __type13;
-    typedef typename pythonic::assignable<__type13>::type __type14;
-    __type14 fb_fft = div_vb_fft;
-    fb_fft[pythonic::types::contiguous_slice(pythonic::builtins::None,pythonic::builtins::None)] = pythonic::operator_::sub(pythonic::operator_::neg(div_vb_fft), pythonic::operator_::mul(pythonic::numpy::functor::square{}(N), vz_fft));
-    return fb_fft;
-  }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_solver::__transonic__()());
 inline
 typename __pythran_solver::compute_fb_fft::type<pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long,long>>, long, pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long,long>>>::result_type compute_fb_fft0(pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long,long>>&& div_vb_fft, long&& N, pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long,long>>&& vz_fft) 
 {
@@ -243,17 +222,17 @@
                                          Methods,
                                          ""
     );
     #endif
     if(! theModule)
         PYTHRAN_RETURN;
     PyObject * theDoc = Py_BuildValue("(sss)",
-                                      "0.11.0",
-                                      "2022-09-02 03:40:21.224419",
-                                      "47c73dec4151bf00c94c99926e3866dee9837f0fb571523a3934d127da4a2408");
+                                      "0.13.1",
+                                      "2023-05-24 11:29:42.920722",
+                                      "8e32897d98adb4b6a17d322b74a902285d33494173542a75568c0969295f0f2b");
     if(! theDoc)
         PYTHRAN_RETURN;
     PyModule_AddObject(theModule,
                        "__pythran__",
                        theDoc);
 
     PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/output/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/output/spatial_means.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/output/spatial_means.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
             PA1 = self.sum_wavenumbers(np.ascontiguousarray(PA1_fft))
             PA2 = self.sum_wavenumbers(PA2_fft) * deltat / 2
 
             PA1 *= self.one_over_N2
             PA2 *= self.one_over_N2
 
         if mpi.rank == 0:
-
             self.file.write(
                 f"####\ntime = {tsim:11.5e}\n"
                 f"E    = {energy:11.5e}\n"
                 f"EA   = {nrj_A:11.5e} ; EKz   = {nrj_Kz:11.5e} ; "
                 f"EKhr   = {nrj_Khr:11.5e} ; EKhd   = {nrj_Khd:11.5e} ; "
                 f"EKhs   = {nrj_Khs:11.5e} ; EAs    = {nrj_As:11.5e}\n"
                 f"epsK = {epsK:11.5e} ; epsK_hypo = {epsK_hypo:11.5e} ; "
@@ -126,15 +125,14 @@
                     f"PA_tot   = {PA1 + PA2:11.5e} \n"
                 )
 
             self.file.flush()
             os.fsync(self.file.fileno())
 
         if self.has_to_plot and mpi.rank == 0:
-
             self.ax_a.plot(tsim, energy, "k.")
 
             # self.axe_b.plot(tsim, epsK_tot, 'k.')
             # if self.sim.params.forcing.enable:
             #     self.axe_b.plot(tsim, PK_tot, 'm.')
 
             if tsim - self.t_last_show >= self.period_show:
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/output/spect_energy_budget.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/output/spect_energy_budget.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 
     where :math:`f_{dK}(\kk)` and :math:`f_{dA}(\kk)` are the dissipation
     frequency depending of the wavenumber and the viscous coefficients.
 
     """
 
     def compute(self):
-
         results = super().compute()
 
         state = self.sim.state
         N = self.sim.params.N
 
         oper = self.sim.oper
 
@@ -117,15 +116,14 @@
             )
 
         return results
 
     def plot_fluxes(
         self, tmin=None, tmax=None, key_k="kh", ax=None, plot_conversion=True
     ):
-
         data = self.compute_fluxes_mean(tmin, tmax)
 
         k_plot = data[key_k]
         deltak = k_plot[1]
         k_plot += deltak / 2
 
         key_flux = key_k[1] + "flux_"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/output/spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/output/spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
 
     def plot_kzkh(self, tmin=0, tmax=None, key="Khd", ax=None):
         super().plot_kzkh(tmin, tmax, key, ax)
 
     def _plot1d_direction(
         self, direction, imin_plot, imax_plot, coef_compensate, ax
     ):
-
         with h5py.File(self.path_file1d, "r") as h5file:
             ks = h5file["k" + direction][...]
 
             def _get_spectrum(key):
                 return _get_averaged_spectrum(
                     key + direction, h5file, imin_plot, imax_plot
                 )
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     fb_fft = div_vb_fft
     fb_fft[:] = -div_vb_fft - N**2 * vz_fft
     return fb_fft
 
 
 class InfoSolverNS3DStrat(InfoSolverNS3D):
     def _init_root(self):
-
         super()._init_root()
 
         package = "fluidsim.solvers.ns3d.strat"
         self.module_name = package + ".solver"
         self.class_name = "Simul"
         self.short_name = "ns3d.strat"
 
@@ -228,15 +227,14 @@
         return self.params.N * np.sqrt(
             (self.oper.Kx**2 + self.oper.Ky**2)
             * self.oper.inv_K_square_nozero
         )
 
 
 if __name__ == "__main__":
-
     import numpy as np
 
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/state.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/state.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/strat/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/strat/test_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         params = super().init_params()
         cls._init_grid(params, nx=64)
 
         params.init_fields.type = "noise"
         params.output.HAS_TO_SAVE = False
 
     def test_tendency(self):
-
         sim = self.sim
 
         tend = sim.tendencies_nonlin(state_spect=sim.state.state_spect)
 
         T_tot = np.ascontiguousarray(sim.oper.create_arrayK(value=0.0).real)
 
         for axis in ("x", "y", "z"):
@@ -101,15 +100,14 @@
             params.oper.nx // 2,
             params.oper.ny // 2,
             params.oper.nz // 2,
         )
 
     @pytest.mark.filterwarnings("ignore:divide by zero encountered in log10")
     def test_output(self):
-
         sim = self.sim
 
         oper = sim.oper
         X, Y, Z = oper.get_XYZ_loc()
 
         def compute_forcing_fft_each_time(self):
             return {"vx_fft": oper.create_arrayK(value=0)}
@@ -262,15 +260,14 @@
         params.time_stepping.deltat0 = deltat = 0.08
 
         params.output.periods_save.spatial_means = deltat
         params.output.periods_save.spectra = deltat
         params.output.spectra.kzkh_periodicity = 1
 
     def test_noshearmodes(self):
-
         sim = self.sim
 
         sim.time_stepping.start()
 
         data = sim.output.spectra.load_kzkh_mean(
             tmin=0.2, key_to_load=["Khd", "Kz", "Khr", "A"]
         )
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/test_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         try:
             params.oper.nz = nx // 2
         except AttributeError:
             pass
 
     @classmethod
     def init_params(cls):
-
         params = cls.params = cls.Simul.create_default_params()
 
         params.short_name_type_run = "test"
         params.output.sub_directory = "unittests"
         cls._init_grid(params, nx=cls.nx)
 
         Lx = 6.0
@@ -75,15 +74,14 @@
     @classmethod
     def init_params(cls):
         params = super().init_params()
         cls._init_grid(params, nx=20)
         params.output.HAS_TO_SAVE = False
 
     def test_tendency(self):
-
         sim = self.sim
         tend = sim.tendencies_nonlin(state_spect=sim.state.state_spect)
 
         T_tot = np.ascontiguousarray(sim.oper.create_arrayK(value=0.0).real)
 
         for axis in ("x", "y", "z"):
             key = f"v{axis}_fft"
@@ -138,15 +136,14 @@
             ny // 2,
             nz // 2,
         )
         params.output.spatiotemporal_spectra.SAVE_AS_COMPLEX64 = False
 
     @pytest.mark.filterwarnings("ignore:divide by zero encountered in log10")
     def test_output(self):
-
         sim = self.sim
 
         # put energy in vz
         vz = sim.state.state_phys.get_var("vz")
         X, Y, Z = sim.oper.get_XYZ_loc()
         vz += 0.05 * np.cos(2 * pi * X / sim.oper.Lx)
         sim.state.statespect_from_statephys()
@@ -157,15 +154,14 @@
 
         # testing phaseshift
         phaseshift = sim.time_stepping._get_phaseshift()
         assert phaseshift.shape == sim.oper.Kx.shape
         assert sim.time_stepping._get_phaseshift() is phaseshift
 
         if mpi.nb_proc == 1:
-
             phys_fields = sim.output.phys_fields
             phys_fields.plot(equation=f"iz=0", numfig=1000)
 
             phys_fields.get_field_to_plot_from_state()
             phys_fields.get_field_to_plot_from_state(sim.state.get_var("vx"))
             phys_fields.get_field_to_plot_from_state("vx", "x=0")
             phys_fields.get_field_to_plot_from_state("vx", "ix=0")
@@ -409,15 +405,14 @@
     @classmethod
     def init_params(self):
         params = super().init_params()
         params.output.HAS_TO_SAVE = False
         params.init_fields.type = "in_script"
 
     def test_init_in_script(self):
-
         sim = self.sim
 
         # here we have to initialize the flow fields
 
         variables = {
             k: 1e-2 * sim.oper.create_arrayX_random() for k in ("vx", "vy", "vz")
         }
@@ -559,15 +554,14 @@
         watu.period_forcing = period_forcing
         watu.approximate_dt = period_N / 1e1
         watu.nb_wave_makers = 2
 
         params.output.periods_save.phys_fields = 2.0
 
     def test_forcing(self):
-
         sim = self.sim
         sim.time_stepping.start()
         sim.state.check_energy_equal_phys_spect()
 
         params, Simul = load_for_restart(sim.output.path_run)
         params.time_stepping.t_end += 2.0
         sim_restart = Simul(params)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/time_stepping.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/time_stepping.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/try_load.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/try_load.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/ns3d/try_save.py` & `fluidsim-0.7.3/fluidsim/solvers/ns3d/try_save.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/dimensional.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/dimensional.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
 
     def compute_nu4_dim(self, nu4):
         """Compute the adimensional hyper-viscosity."""
         return nu4 * self.tilde_nu4
 
 
 if __name__ == "__main__":
-
     converter = Converter(C=0.648**2, h=4e-4)
 
     amplitude_z = 0.001
     print("amplitude z: {:6.2f}".format(converter.compute_z_adim(amplitude_z)))
 
     nu_4 = 5e-7
     print("nu_4: {:8.3g}".format(converter.compute_nu4_adim(nu_4)))
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/forcing.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/forcing.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/init_fields.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/init_fields.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/operators.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/operators.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/output/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/output/correl_Mordant.m` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/output/correl_Mordant.m`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/output/correlations_freq.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/output/correlations_freq.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,14 @@
                     )
                     self.nb_means_times += 1
 
                     if (
                         self.nb_means_times % 128 == 0
                         or np.log(self.nb_means_times) / np.log(2) % 1 == 0
                     ) and self.nb_means_times != 1:
-
                         correlations = {
                             "corr4": self.corr4,
                             "corr2": self.corr2,
                             "nb_means": self.nb_means_times,
                         }
                         if not os.path.exists(self.path_file):
                             self._init_files2(correlations)
@@ -383,15 +382,14 @@
         self.ax1 = ax1
         ax1.set_xlabel("Omega")
         ax1.set_ylabel("Omega")
         pc1 = ax1.pcolormesh(fx, fy, corr[1, :, :], shading="nearest")
         fig1.colorbar(pc1)
 
     def compute_corr4_norm(self, it=-1):
-
         with h5py.File(self.path_file, "r") as file:
             corr4 = file["corr4"][it]
             corr2 = file["corr2"][it]
             nb_means = file["nb_means"][it]
 
         nb_omegas = self.nb_omegas
 
@@ -572,25 +570,23 @@
         plt.figure()
         ax = plt.gca()
         ax.loglog(nb_means, fcorr4, "x-")
         ax.set_ylabel("a kind of norm of corr4")
         ax.set_xlabel("number of averages")
 
     def plot_convergence(self):
-
         nb_means, dnormpickC4 = self._compute_dnormpickC4_over_dnbmean()
 
         fig = plt.figure()
         fig.suptitle('"convergence"')
         ax = plt.gca()
         ax.loglog(nb_means[1:], dnormpickC4, "x-")
         ax.set_xlabel("number of averages")
 
     def plot_corr2(self, nonorm=False, it=-1):
-
         with h5py.File(self.path_file, "r") as file:
             corr2_in_file = file["corr2"]
             corr2 = corr2_in_file[it]
             nb_means = file["nb_means"][it]
 
         fy, fx = np.meshgrid(self.omegas, self.omegas)
 
@@ -621,15 +617,14 @@
             vmin=log10corr2.min(),
             vmax=log10corr2.max(),
         )
         plt.colorbar()
         plt.axis([fx.min(), fx.max(), fy.min(), fy.max()])
 
     def plot_corr2_1d(self, it=-1):
-
         with h5py.File(self.path_file, "r") as file:
             corr2 = file["corr2"][it]
             nb_means = file["nb_means"][it]
 
         corr2_diag = np.empty(self.nb_omegas, dtype=np.complex128)
         for io3 in range(self.nb_omegas):
             corr2_diag[io3] = corr2[io3, io3]
@@ -640,15 +635,14 @@
         ax.set_title("abs(corr2_diag); nb_means: " + str(nb_means))
         plt.xlabel("Omega")
         plt.ylabel("abs(corr2)")
         # ax.loglog(self.omegas, abs(corr2_diag))
         ax.plot(self.omegas, np.log10(abs(corr2_diag)))
 
     def plot_corr4(self, it=-1):
-
         nb_omegas1 = self.iomegas1.shape[0]
         nb_omegas = self.nb_omegas
 
         corr_norm = np.empty((nb_omegas1, nb_omegas, nb_omegas))
         cum_norm = np.empty(corr_norm.shape)
         norm = np.empty(corr_norm.shape)
         norm, corr_norm, cum_norm, nb_means = self.compute_corr4_norm(it)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/output/spatial_means.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/output/spatial_means.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,14 @@
                 ).format(P1, P2, P1 + P2)
                 self.file.write(to_print)
 
             self.file.flush()
             os.fsync(self.file.fileno())
 
         if self.has_to_plot and mpi.rank == 0:
-
             self.ax_a.plot(tsim, energy, "k.")
             self.ax_a.plot(tsim, energy_k, "r.")
             self.ax_a.plot(tsim, energy_l, "b.")
             self.ax_a.plot(tsim, energy_e, "y.")
 
             self.axe_b.plot(tsim, epsK_tot, "k.")
             self.axe_b.plot(tsim, conversion_k_to_l, "c.")
@@ -197,15 +196,14 @@
             words = line.split()
             E[il] = float(words[2])
             E_k[il] = float(words[6])
             E_l[il] = float(words[10])
             E_e[il] = float(words[14])
 
             if self.sim.params.forcing.enable:
-
                 line = lines_P[il]
                 words = line.split()
                 P1[il] = float(words[2])
                 P2[il] = float(words[6])
                 P_tot[il] = float(words[10])
 
             line = lines_epsK[il]
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/output/spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/output/spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         else:
             print(
                 "you need to implement the ploting "
                 "of the spectra for this case"
             )
 
     def plot1d(self, tmin=0, tmax=1000, delta_t=2, coef_compensate=3):
-
         with h5py.File(self.path_file1D, "r") as h5file:
             dset_times = h5file["times"]
 
             dset_kxE = h5file["kxE"]
             # dset_kyE = h5file['kyE']
             kh = dset_kxE[...]
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,14 @@
             # print('ratio array\n', T)
             # print('(K+L)\n', (dt_E_K+dt_E_L)/norm)
             # print('NQ\n', dt_E_NQ/norm)
             return self.oper.sum_wavenumbers(T)
 
 
 if __name__ == "__main__":
-
     np.set_printoptions(precision=2)
 
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/state.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/state.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/test_dimensional.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/test_dimensional.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from .dimensional import Converter
 
 from fluidsim.util.testing import TestCase
 
 
 class TestDimensional(TestCase):
     def test_converter(self):
-
         conv = Converter(C=0.648**2, h=4e-4)
 
         time = 10.0
         time_adim = conv.compute_time_adim(time)
         self.assertEqual(time, conv.compute_time_dim(time_adim))
 
         amplitude_z = 0.001
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/plate2d/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/plate2d/test_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,14 @@
         params.output.correl_freq.HAS_TO_PLOT_SAVED = True
         params.output.correl_freq.it_start = 0
         params.output.correl_freq.nb_times_compute = 5
         params.output.correl_freq.coef_decimate = 1
         params.output.correl_freq.iomegas1 = [1, 2]
 
     def test_output(self):
-
         sim = self.sim
 
         sim.time_stepping.start()
 
         sim.output.correl_freq.compute_corr4_norm()
 
         for key in sim.info_solver.classes.State.keys_computable:
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sphere/ns2d/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sphere/ns2d/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,14 @@
 
         return tendencies_sh
 
 
 Simul = SimulSphereNS2D
 
 if __name__ == "__main__":
-
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
 
     params.init_fields.type = "noise"
 
     params.time_stepping.USE_CFL = True
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sphere/ns2d/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sphere/ns2d/test_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 class TestSimulBase(TestSimul):
     Simul = Simul
 
     @classmethod
     def init_params(cls):
-
         params = cls.params = cls.Simul.create_default_params()
         params.short_name_type_run = "test"
         params.output.sub_directory = "unittests"
 
         params.oper.lmax = 15
         params.oper.omega = 0.0
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sphere/sw1l/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sphere/sw1l/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
         return tendencies_sh
 
 
 Simul = SimulSphereSW1L
 
 
 if __name__ == "__main__":
-
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
     params.output.sub_directory = "test"
 
     params.nu_2 = 1e-2
     params.oper.radius = 10.0
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sphere/sw1l/state.py` & `fluidsim-0.7.3/fluidsim/solvers/sphere/sw1l/state.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sphere/sw1l/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sphere/sw1l/test_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 class TestSimulBase(TestSimul):
     Simul = Simul
 
     @classmethod
     def init_params(cls):
-
         params = cls.params = cls.Simul.create_default_params()
         params.short_name_type_run = "test"
         params.output.sub_directory = "unittests"
 
         params.oper.lmax = 15
         params.oper.omega = 0.0
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/modified/output.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/modified/output.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/modified/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/modified/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
     #             self.oper.sum_wavenumbers(T_tot),
     #             self.oper.sum_wavenumbers(abs(T_tot)),
     #         )
     #     )
 
 
 if __name__ == "__main__":
-
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
 
     nh = 64
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/modified/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/modified/test_solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,14 @@
     #     )
     #     A_fft = oper.fft2(A)
     #     if mpi.rank == 0:
     #         print("should be zero =", A_fft[0, 0])
 
 
 if __name__ == "__main__":
-
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
 
     nh = 64
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/state.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/state.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/exactlin/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/exactlin/test_solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/forcing.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/forcing.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/init_fields.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/init_fields.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/output.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/output.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,14 @@
         if self.params.forcing.enable:
             tendencies_fft += self.forcing.get_forcing()
 
         return tendencies_fft
 
 
 if __name__ == "__main__":
-
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
 
     nh = 64
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/state.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         if SAVE_IN_DICT:
             self.vars_computed[key] = result
             self.it_computed[key] = it
 
         return result
 
     def init_from_uxuyfft(self, ux_fft, uy_fft):
-
         oper = self.oper
         ifft2 = oper.ifft2
 
         oper.projection_perp(ux_fft, uy_fft)
         oper.dealiasing(ux_fft, uy_fft)
 
         ux = ifft2(ux_fft)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/modified/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/modified/test_solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/output.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/output.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,14 @@
     #     )
     #     A_fft = oper.fft2(A)
     #     if mpi.rank == 0:
     #         print("should be zero =", A_fft[0, 0])
 
 
 if __name__ == "__main__":
-
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
 
     nh = 64
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/state.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,14 @@
         state_phys.set_var("ux", ifft2(ux_fft))
         state_phys.set_var("uy", ifft2(uy_fft))
         state_phys.set_var("eta", ifft2(eta_fft))
 
         return state_phys
 
     def init_from_uxuyetafft(self, ux_fft, uy_fft, eta_fft):
-
         (q_fft, ap_fft, am_fft) = self.oper.qapamfft_from_uxuyetafft(
             ux_fft, uy_fft, eta_fft
         )
 
         state_spect = self.state_spect
         state_spect.set_var("ap_fft", ap_fft)
         state_spect.set_var("am_fft", am_fft)
@@ -209,15 +208,14 @@
         state_spect.set_var("ap_fft", ap_fft)
         state_spect.set_var("am_fft", am_fft)
 
         self.oper.dealiasing(state_spect)
         self.statephys_from_statespect()
 
     def init_from_uxuyfft(self, ux_fft, uy_fft):
-
         oper = self.oper
         ifft2 = oper.ifft2
 
         oper.projection_perp(ux_fft, uy_fft)
         oper.dealiasing(ux_fft, uy_fft)
 
         ux = ifft2(ux_fft)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/onlywaves/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/onlywaves/test_solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/operators.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         for i0 in range(n0):
             for i1 in range(n1):
                 if i0 == 0 and i1 == 0 and rank == 0:
                     q_fft[i0, i1] = 0
                     ap_fft[i0, i1] = ux_fft[0, 0] + 1.0j * uy_fft[0, 0]
                     am_fft[i0, i1] = ux_fft[0, 0] - 1.0j * uy_fft[0, 0]
                 else:
-
                     rot_fft = 1j * (
                         KX[i0, i1] * uy_fft[i0, i1] - KY[i0, i1] * ux_fft[i0, i1]
                     )
 
                     q_fft[i0, i1] = rot_fft - freq_Corio * eta_fft[i0, i1]
 
                     a_over2_fft = 0.5 * (
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/output/__init__.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/output/_old_spatial_means.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/output/_old_spatial_means.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/output/_old_spect_energy_budg.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/output/_old_spect_energy_budg.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     cumsum_inv,
     inner_prod,
 )
 
 
 class SpectralEnergyBudgetSW1LWaves(SpectralEnergyBudgetBase):
     def __init__(self, output):
-
         params = output.sim.params
         self.c2 = params.c2
         self.f = params.f
 
         super().__init__(output)
 
     def compute(self):
@@ -384,15 +383,14 @@
             "convP2D": convP2D,
             "convK2D": convK2D,
             "transfer2D_CPE": transfer2D_CPE,
         }
         return dict_results
 
     def _online_plot_saving(self, dict_results):
-
         transfer2D_CPE = dict_results["transfer2D_CPE"]
         transfer2D_EKr = dict_results["transfer2D_EKr"]
         transfer2D_EKd = dict_results["transfer2D_EKd"]
         transfer2D_EK = transfer2D_EKr + transfer2D_EKd
         transfer2D_EAr = dict_results["transfer2D_EAr"]
         transfer2D_EAd = dict_results["transfer2D_EAd"]
         transfer2D_EA = transfer2D_EAr + transfer2D_EAd
@@ -411,17 +409,15 @@
         self.axe_a.plot(khE + khE[1], PiEtot, "k", linewidth=2)
         self.axe_a.plot(khE + khE[1], CCP, "y")
         self.axe_a.plot(khE + khE[1], CCK, "y--")
 
         self.axe_b.plot(khE + khE[1], PiCPE, "g")
 
     def plot(self, tmin=0, tmax=1000, delta_t=2):
-
         with h5py.File(self.path_file, "r") as h5file:
-
             dset_times = h5file["times"]
             times = dset_times[...]
             # nt = len(times)
 
             dset_khE = h5file["khE"]
             khE = dset_khE[...]
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/output/increments.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/output/increments.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/output/normal_mode.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/output/normal_mode.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/output/print_stdout.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/output/print_stdout.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/output/spatial_means.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/output/spatial_means.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     Viz. total energy, K.E., A.P.E. and Charney potential enstrophy. It also
     handles the computation of forcing and dissipation rates for
     sw1l.modified solver
 
     """
 
     def __init__(self, output):
-
         params = output.sim.params
         self.c2 = params.c2
         self.f = params.f
         if mpi.rank == 0:
             self._result = {}
 
         super().__init__(output)
@@ -175,15 +174,14 @@
             if self.has_to_plot:
                 tsim = self.sim.time_stepping.t
                 self.axe_b.plot(tsim, epsK_tot + epsA_tot, "k.")
 
     def compute_dissipation_rates(
         self, f_d, f_d_hypo, energyK_fft, energyA_fft, CharneyPE_fft
     ):
-
         epsK = self.sum_wavenumbers(f_d * 2 * energyK_fft)
         epsK_hypo = self.sum_wavenumbers(f_d_hypo * 2 * energyK_fft)
         epsA = self.sum_wavenumbers(f_d * 2 * energyA_fft)
         epsA_hypo = self.sum_wavenumbers(f_d_hypo * 2 * energyA_fft)
         epsCPE = self.sum_wavenumbers(f_d * 2 * CharneyPE_fft)
         epsCPE_hypo = self.sum_wavenumbers(f_d_hypo * 2 * CharneyPE_fft)
 
@@ -438,15 +436,14 @@
             f_d, f_d_hypo, energyK_fft, dict_eps
         )
 
         dict_eps.update({"epsKsup": epsKsuppl, "epsKsup_hypo": epsKsuppl_hypo})
         return dict_eps
 
     def compute_epsK(self, f_d, f_d_hypo, energyK_fft, dict_eps):
-
         ux = self.sim.state.state_phys.get_var("ux")
         uy = self.sim.state.state_phys.get_var("uy")
 
         EKquad = 0.5 * (ux**2 + uy**2)
         EKquad_fft = self.sim.oper.fft2(EKquad)
 
         eta_fft = self.sim.state.get_var("eta_fft")
@@ -515,15 +512,14 @@
             )
         )
 
         PK1 = self.sum_wavenumbers(PK1_fft)
         PK2 = self.sum_wavenumbers(PK2_fft)
 
         if mpi.rank == 0:
-
             PK_tot = PK1 + PK2
             PA_tot = PA1 + PA2
             self._result.update(
                 {
                     "PK1": PK1,
                     "PK2": PK2,
                     "PK_tot": PK_tot,
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/output/spect_energy_budget.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/output/spect_energy_budget.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from .normal_mode import NormalModeDecomposition, NormalModeDecompositionModified
 
 
 class SpectralEnergyBudgetSW1LBase(SpectralEnergyBudgetBase):
     """Save and plot spectral energy budgets."""
 
     def __init__(self, output):
-
         params = output.sim.params
         self.c2 = params.c2
         self.f = params.f
 
         super().__init__(output)
 
     def _checksum_stdout(self, debug=False, **kwargs):
@@ -170,15 +169,14 @@
         #     EA=transfer2D_EA,
         #     Etot=transfer2D_EK + transfer2D_EA,
         #     debug=False,
         # )
         return dict_results
 
     def _online_plot_saving(self, dict_results):
-
         transfer2D_CPE = dict_results["transfer2D_CPE"]
         transfer2D_EK = dict_results["transfer2D_EK"]
         transfer2D_EA = dict_results["transfer2D_EA"]
         convA2D = dict_results["convA2D"]
         khE = self.oper.khE
         PiCPE = cumsum_inv(transfer2D_CPE) * self.oper.deltak
         PiEK = cumsum_inv(transfer2D_EK) * self.oper.deltak
@@ -186,17 +184,15 @@
         CCA = cumsum_inv(convA2D) * self.oper.deltak
         self.axe_a.plot(khE + khE[1], PiEK, "r")
         self.axe_a.plot(khE + khE[1], PiEA, "b")
         self.axe_a.plot(khE + khE[1], CCA, "y")
         self.axe_b.plot(khE + khE[1], PiCPE, "g")
 
     def plot(self, tmin=0, tmax=1000, delta_t=2):
-
         with h5py.File(self.path_file, "r") as h5file:
-
             dset_times = h5file["times"]
             dset_khE = h5file["khE"]
             khE = dset_khE[...]
             # khE = khE+khE[1]
 
             dset_transfer2D_EK = h5file["transfer2D_EK"]
             dset_transfer2D_Errr = h5file["transfer2D_Errr"]
@@ -474,15 +470,14 @@
             "Cq_AA": Cq_AA,
             "Tens": Tens,
         }
 
         return dict_results
 
     def _online_plot_saving(self, dict_results):
-
         # Tens = dict_results["Tens"]
         Tq_GGG = dict_results["Tq_GGG"]
         Tq_AGG = dict_results["Tq_AGG"]
         Tq_GAAs = dict_results["Tq_GAAs"]
         Tq_GAAd = dict_results["Tq_GAAd"]
         Tq_AAA = dict_results["Tq_AAA"]
         Tq_tot = Tq_GGG + Tq_AGG + Tq_GAAs + Tq_GAAd + Tq_AAA
@@ -545,17 +540,15 @@
                 "Spectral Energy Budget\n" + self.output.summary_simul
             )
             self.axe_a.legend()
             self.axe_b.legend()
             self.axe_b.set_ylabel(r"$\Sigma C(k_h)$")
 
     def plot(self, tmin=0, tmax=1000, delta_t=2):
-
         with h5py.File(self.path_file, "r") as h5file:
-
             dset_times = h5file["times"]
             dset_khE = h5file["khE"]
             khE = dset_khE[...] + 0.1  # Offset for semilog plots
             times = dset_times[...]
 
             delta_t_save = np.mean(times[1:] - times[0:-1])
             delta_i_plot = int(np.round(delta_t / delta_t_save))
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/output/spectra.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/output/spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,14 @@
         tmax: float = 1000,
         delta_t: float = 2,
         coef_compensate: float = 3,
         coef_norm: Optional[np.ndarray] = None,
         ax: Optional[mpl.axes.Axes] = None,
         help_lines: bool = True,
     ):
-
         with h5py.File(self.path_file1D, "r") as h5file:
             dset_times = h5file["times"]
             times = dset_times[...]
             # nb_spectra = times.shape[0]
 
             dset_kxE = h5file["kxE"]
             # dset_kyE = h5file['kyE']
@@ -257,15 +256,14 @@
         coef_norm: Optional[np.ndarray] = None,
         keys: List[str] = ["Etot", "EK", "EA", "EKr", "EKd"],
         colors: List[str] = ["k", "r", "b", "r--", "r:"],
         kh_norm: float = 1,
         ax: Optional[mpl.axes.Axes] = None,
         help_lines: bool = True,
     ):
-
         with h5py.File(self.path_file2D, "r") as h5file:
             times = h5file["times"][...]
 
             dset_khE = h5file["khE"]
             kh = dset_khE[...] / kh_norm
 
             dset_spectrumEK = h5file["spectrum2D_EK"]
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,14 @@
         if self.params.forcing.enable:
             tendencies_fft += self.forcing.get_forcing()
 
         return tendencies_fft
 
 
 if __name__ == "__main__":
-
     import numpy as np
 
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/state.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/state.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/test_operators.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/test_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import fluiddyn.util.mpi as mpi
 from fluiddyn.util.paramcontainer import ParamContainer
 
 from fluidsim.util.testing import TestCase, stdout_redirected, skip_if_no_fluidfft
 
 
 def create_oper(type_fft=None, coef_dealiasing=2.0 / 3):
-
     params = ParamContainer(tag="params")
 
     params._set_attrib("ONLY_COARSE_OPER", False)
     params._set_attrib("f", 0)
     params._set_attrib("c2", 100)
     params._set_attrib("kd2", 0)
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/sw1l/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/sw1l/test_solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/waves2d/solver.py` & `fluidsim-0.7.3/fluidsim/solvers/waves2d/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     SimulBasePseudoSpectral,
     InfoSolverPseudoSpectral,
 )
 
 
 class InfoSolverWaves2d(InfoSolverPseudoSpectral):
     def _init_root(self):
-
         super()._init_root()
 
         package = "fluidsim.solvers.waves2d"
         self.module_name = package + ".solver"
         self.class_name = "Simul"
         self.short_name = "Waves2d"
 
@@ -97,15 +96,14 @@
     def _complete_params_with_default(params):
         """This static method is used to complete the *params* container."""
         SimulBasePseudoSpectral._complete_params_with_default(params)
         attribs = {"c2": 1.0, "f": 0}
         params._set_attribs(attribs)
 
     def tendencies_nonlin(self, state_spect=None, old=None):
-
         if old is None:
             tendencies_fft = SetOfVariables(
                 like=self.state.state_spect, info="tendencies_nonlin"
             )
         else:
             tendencies_fft = old
 
@@ -121,15 +119,14 @@
             omega = 1.0j * np.sqrt(
                 self.params.f**2 + self.params.c2 * self.oper.K2
             )
         return omega
 
 
 if __name__ == "__main__":
-
     import fluiddyn as fld
 
     params = Simul.create_default_params()
 
     params.short_name_type_run = "test"
 
     nh = 32
```

### Comparing `fluidsim-0.7.2/fluidsim/solvers/waves2d/state.py` & `fluidsim-0.7.3/fluidsim/solvers/waves2d/state.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/solvers/waves2d/test_solver.py` & `fluidsim-0.7.3/fluidsim/solvers/waves2d/test_solver.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/__init__.py` & `fluidsim-0.7.3/fluidsim/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/__pythran__/mini_oper_modif_resol.cpp` & `fluidsim-0.7.3/fluidsim/util/__pythran__/mini_oper_modif_resol.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #include <pythonic/core.hpp>
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
-#include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/include/types/complex128.hpp>
+#include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/types/ndarray.hpp>
 #include <pythonic/types/complex128.hpp>
 #include <pythonic/include/builtins/None.hpp>
 #include <pythonic/include/builtins/getattr.hpp>
 #include <pythonic/include/builtins/min.hpp>
 #include <pythonic/include/builtins/pythran/and_.hpp>
 #include <pythonic/include/builtins/range.hpp>
@@ -29,155 +29,161 @@
 #include <pythonic/builtins/tuple.hpp>
 #include <pythonic/operator_/add.hpp>
 #include <pythonic/operator_/floordiv.hpp>
 #include <pythonic/operator_/gt.hpp>
 #include <pythonic/operator_/lt.hpp>
 #include <pythonic/operator_/neg.hpp>
 #include <pythonic/types/str.hpp>
-namespace __pythran_mini_oper_modif_resol
+namespace 
 {
-  struct __transonic__
+  namespace __pythran_mini_oper_modif_resol
   {
-    typedef void callable;
-    typedef void pure;
-    struct type
+    struct __transonic__
     {
-      typedef pythonic::types::str __type0;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
-      typedef typename pythonic::returnable<__type1>::type __type2;
-      typedef __type2 result_type;
+      typedef void callable;
+      typedef void pure;
+      struct type
+      {
+        typedef pythonic::types::str __type0;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type0>())) __type1;
+        typedef typename pythonic::returnable<__type1>::type __type2;
+        typedef __type2 result_type;
+      }  ;
+      inline
+      typename type::result_type operator()() const;
+      ;
     }  ;
-    inline
-    typename type::result_type operator()() const;
-    ;
-  }  ;
-  struct fill_field_fft_3d
-  {
-    typedef void callable;
-    ;
-    template <typename argument_type0 , typename argument_type1 >
-    struct type
+    struct fill_field_fft_3d
     {
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
-      typedef __type0 __type1;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type2;
-      typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::min{})>::type>::type __type3;
-      typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type4;
-      typedef __type4 __type5;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type5>())) __type6;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type6>::type>::type __type7;
-      typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type1>())) __type9;
-      typedef typename std::tuple_element<0,typename std::remove_reference<__type9>::type>::type __type10;
-      typedef decltype(std::declval<__type3>()(std::declval<__type7>(), std::declval<__type10>())) __type11;
-      typedef typename pythonic::assignable<__type11>::type __type12;
-      typedef __type12 __type13;
-      typedef long __type14;
-      typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type13>(), std::declval<__type14>())) __type15;
-      typedef decltype(pythonic::operator_::add(std::declval<__type15>(), std::declval<__type14>())) __type16;
-      typedef decltype(std::declval<__type2>()(std::declval<__type16>())) __type17;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type17>::type::iterator>::value_type>::type __type18;
-      typedef __type18 __type19;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type6>::type>::type __type20;
-      typedef typename std::tuple_element<1,typename std::remove_reference<__type9>::type>::type __type21;
-      typedef decltype(std::declval<__type3>()(std::declval<__type20>(), std::declval<__type21>())) __type22;
-      typedef typename pythonic::assignable<__type22>::type __type23;
-      typedef __type23 __type24;
-      typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type24>(), std::declval<__type14>())) __type25;
-      typedef decltype(pythonic::operator_::add(std::declval<__type25>(), std::declval<__type14>())) __type26;
-      typedef decltype(std::declval<__type2>()(std::declval<__type26>())) __type27;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type27>::type::iterator>::value_type>::type __type28;
-      typedef __type28 __type29;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type6>::type>::type __type30;
-      typedef typename std::tuple_element<2,typename std::remove_reference<__type9>::type>::type __type31;
-      typedef decltype(std::declval<__type3>()(std::declval<__type30>(), std::declval<__type31>())) __type32;
-      typedef typename pythonic::lazy<__type32>::type __type33;
-      typedef __type33 __type34;
-      typedef decltype(std::declval<__type2>()(std::declval<__type34>())) __type35;
-      typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type35>::type::iterator>::value_type>::type __type36;
-      typedef __type36 __type37;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type19>(), std::declval<__type29>(), std::declval<__type37>())) __type38;
-      typedef decltype(std::declval<__type1>()[std::declval<__type38>()]) __type39;
-      typedef container<typename std::remove_reference<__type39>::type> __type40;
-      typedef indexable<__type38> __type45;
-      typedef decltype(pythonic::operator_::neg(std::declval<__type19>())) __type48;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type48>(), std::declval<__type29>(), std::declval<__type37>())) __type51;
-      typedef decltype(std::declval<__type1>()[std::declval<__type51>()]) __type52;
-      typedef container<typename std::remove_reference<__type52>::type> __type53;
-      typedef indexable<__type51> __type59;
-      typedef decltype(pythonic::operator_::neg(std::declval<__type29>())) __type64;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type48>(), std::declval<__type64>(), std::declval<__type37>())) __type66;
-      typedef decltype(std::declval<__type1>()[std::declval<__type66>()]) __type67;
-      typedef container<typename std::remove_reference<__type67>::type> __type68;
-      typedef indexable<__type66> __type75;
-      typedef decltype(pythonic::types::make_tuple(std::declval<__type19>(), std::declval<__type64>(), std::declval<__type37>())) __type81;
-      typedef decltype(std::declval<__type1>()[std::declval<__type81>()]) __type82;
-      typedef container<typename std::remove_reference<__type82>::type> __type83;
-      typedef indexable<__type81> __type89;
-      typedef typename __combined<__type4,__type40,__type45,__type53,__type59,__type68,__type75,__type83,__type89>::type __type90;
-      typedef __type39 __type91;
-      typedef __type38 __type92;
-      typedef pythonic::types::none_type __type93;
-      typedef typename pythonic::returnable<__type93>::type __type94;
-      typedef __type91 __ptype0;
-      typedef __type92 __ptype1;
-      typedef __type94 result_type;
-    }  
-    ;
-    template <typename argument_type0 , typename argument_type1 >
+      typedef void callable;
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      struct type
+      {
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type0>::type>::type __type0;
+        typedef __type0 __type1;
+        typedef decltype(pythonic::types::as_const(std::declval<__type1>())) __type2;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::range{})>::type>::type __type3;
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(pythonic::builtins::functor::min{})>::type>::type __type4;
+        typedef typename std::remove_cv<typename std::remove_reference<argument_type1>::type>::type __type5;
+        typedef __type5 __type6;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type6>())) __type7;
+        typedef decltype(pythonic::types::as_const(std::declval<__type7>())) __type8;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type8>::type>::type __type9;
+        typedef decltype(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, std::declval<__type1>())) __type11;
+        typedef decltype(pythonic::types::as_const(std::declval<__type11>())) __type12;
+        typedef typename std::tuple_element<0,typename std::remove_reference<__type12>::type>::type __type13;
+        typedef decltype(std::declval<__type4>()(std::declval<__type9>(), std::declval<__type13>())) __type14;
+        typedef typename pythonic::assignable<__type14>::type __type15;
+        typedef __type15 __type16;
+        typedef long __type17;
+        typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type16>(), std::declval<__type17>())) __type18;
+        typedef decltype(pythonic::operator_::add(std::declval<__type18>(), std::declval<__type17>())) __type19;
+        typedef decltype(std::declval<__type3>()(std::declval<__type19>())) __type20;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type20>::type::iterator>::value_type>::type __type21;
+        typedef __type21 __type22;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type8>::type>::type __type23;
+        typedef typename std::tuple_element<1,typename std::remove_reference<__type12>::type>::type __type24;
+        typedef decltype(std::declval<__type4>()(std::declval<__type23>(), std::declval<__type24>())) __type25;
+        typedef typename pythonic::assignable<__type25>::type __type26;
+        typedef __type26 __type27;
+        typedef decltype(pythonic::operator_::functor::floordiv()(std::declval<__type27>(), std::declval<__type17>())) __type28;
+        typedef decltype(pythonic::operator_::add(std::declval<__type28>(), std::declval<__type17>())) __type29;
+        typedef decltype(std::declval<__type3>()(std::declval<__type29>())) __type30;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type30>::type::iterator>::value_type>::type __type31;
+        typedef __type31 __type32;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type8>::type>::type __type33;
+        typedef typename std::tuple_element<2,typename std::remove_reference<__type12>::type>::type __type34;
+        typedef decltype(std::declval<__type4>()(std::declval<__type33>(), std::declval<__type34>())) __type35;
+        typedef typename pythonic::lazy<__type35>::type __type36;
+        typedef __type36 __type37;
+        typedef decltype(std::declval<__type3>()(std::declval<__type37>())) __type38;
+        typedef typename std::remove_cv<typename std::iterator_traits<typename std::remove_reference<__type38>::type::iterator>::value_type>::type __type39;
+        typedef __type39 __type40;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type22>(), std::declval<__type32>(), std::declval<__type40>())) __type41;
+        typedef decltype(std::declval<__type2>()[std::declval<__type41>()]) __type42;
+        typedef container<typename std::remove_reference<__type42>::type> __type43;
+        typedef indexable<__type41> __type48;
+        typedef decltype(pythonic::operator_::neg(std::declval<__type22>())) __type52;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type52>(), std::declval<__type32>(), std::declval<__type40>())) __type55;
+        typedef decltype(std::declval<__type2>()[std::declval<__type55>()]) __type56;
+        typedef container<typename std::remove_reference<__type56>::type> __type57;
+        typedef indexable<__type55> __type63;
+        typedef decltype(pythonic::operator_::neg(std::declval<__type32>())) __type69;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type52>(), std::declval<__type69>(), std::declval<__type40>())) __type71;
+        typedef decltype(std::declval<__type2>()[std::declval<__type71>()]) __type72;
+        typedef container<typename std::remove_reference<__type72>::type> __type73;
+        typedef indexable<__type71> __type80;
+        typedef decltype(pythonic::types::make_tuple(std::declval<__type22>(), std::declval<__type69>(), std::declval<__type40>())) __type87;
+        typedef decltype(std::declval<__type2>()[std::declval<__type87>()]) __type88;
+        typedef container<typename std::remove_reference<__type88>::type> __type89;
+        typedef indexable<__type87> __type95;
+        typedef typename __combined<__type5,__type43,__type48,__type57,__type63,__type73,__type80,__type89,__type95>::type __type96;
+        typedef __type42 __type97;
+        typedef __type41 __type98;
+        typedef pythonic::types::none_type __type99;
+        typedef typename pythonic::returnable<__type99>::type __type100;
+        typedef __type97 __ptype0;
+        typedef __type98 __ptype1;
+        typedef __type100 result_type;
+      }  
+      ;
+      template <typename argument_type0 , typename argument_type1 >
+      inline
+      typename type<argument_type0, argument_type1>::result_type operator()(argument_type0 field_fft_in, argument_type1 field_fft_out) const
+      ;
+    }  ;
     inline
-    typename type<argument_type0, argument_type1>::result_type operator()(argument_type0&& field_fft_in, argument_type1&& field_fft_out) const
-    ;
-  }  ;
-  inline
-  typename __transonic__::type::result_type __transonic__::operator()() const
-  {
+    typename __transonic__::type::result_type __transonic__::operator()() const
     {
-      static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.0"));
-      return tmp_global;
+      {
+        static typename __transonic__::type::result_type tmp_global = pythonic::types::make_tuple(pythonic::types::str("0.5.2.post0"));
+        return tmp_global;
+      }
     }
-  }
-  template <typename argument_type0 , typename argument_type1 >
-  inline
-  typename fill_field_fft_3d::type<argument_type0, argument_type1>::result_type fill_field_fft_3d::operator()(argument_type0&& field_fft_in, argument_type1&& field_fft_out) const
-  {
-    typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::min{}(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out)), std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in))))>::type nk0_min = pythonic::builtins::functor::min{}(std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out)), std::get<0>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in)));
-    typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::min{}(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out)), std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in))))>::type nk1_min = pythonic::builtins::functor::min{}(std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out)), std::get<1>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in)));
-    typename pythonic::lazy<decltype(pythonic::builtins::functor::min{}(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out)), std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in))))>::type nk2_min = pythonic::builtins::functor::min{}(std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out)), std::get<2>(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in)));
+    template <typename argument_type0 , typename argument_type1 >
+    inline
+    typename fill_field_fft_3d::type<argument_type0, argument_type1>::result_type fill_field_fft_3d::operator()(argument_type0 field_fft_in, argument_type1 field_fft_out) const
     {
-      long  __target140520535896560 = pythonic::operator_::add(pythonic::operator_::functor::floordiv()(nk0_min, 2L), 1L);
-      for (long  ik0=0L; ik0 < __target140520535896560; ik0 += 1L)
+      typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::min{}(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out))), std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in)))))>::type nk0_min = pythonic::builtins::functor::min{}(std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out))), std::get<0>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in))));
+      typename pythonic::assignable_noescape<decltype(pythonic::builtins::functor::min{}(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out))), std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in)))))>::type nk1_min = pythonic::builtins::functor::min{}(std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out))), std::get<1>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in))));
+      typename pythonic::lazy<decltype(pythonic::builtins::functor::min{}(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out))), std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in)))))>::type nk2_min = pythonic::builtins::functor::min{}(std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_out))), std::get<2>(pythonic::types::as_const(pythonic::builtins::getattr(pythonic::types::attr::SHAPE{}, field_fft_in))));
       {
+        long  __target139658370120048 = pythonic::operator_::add(pythonic::operator_::functor::floordiv()(nk0_min, 2L), 1L);
+        for (long  ik0=0L; ik0 < __target139658370120048; ik0 += 1L)
         {
-          long  __target140520535897232 = pythonic::operator_::add(pythonic::operator_::functor::floordiv()(nk1_min, 2L), 1L);
-          for (long  ik1=0L; ik1 < __target140520535897232; ik1 += 1L)
           {
+            long  __target139658370148528 = pythonic::operator_::add(pythonic::operator_::functor::floordiv()(nk1_min, 2L), 1L);
+            for (long  ik1=0L; ik1 < __target139658370148528; ik1 += 1L)
             {
-              long  __target140520532500432 = nk2_min;
-              for (long  ik2=0L; ik2 < __target140520532500432; ik2 += 1L)
               {
-                field_fft_out[pythonic::types::make_tuple(ik0, ik1, ik2)] = field_fft_in[pythonic::types::make_tuple(ik0, ik1, ik2)];
-                if (pythonic::builtins::pythran::and_([&] () { return pythonic::operator_::gt(ik0, 0L); }, [&] () { return pythonic::operator_::lt(ik0, pythonic::operator_::functor::floordiv()(nk0_min, 2L)); }))
+                long  __target139658370146560 = nk2_min;
+                for (long  ik2=0L; ik2 < __target139658370146560; ik2 += 1L)
                 {
-                  field_fft_out[pythonic::types::make_tuple(pythonic::operator_::neg(ik0), ik1, ik2)] = field_fft_in[pythonic::types::make_tuple(pythonic::operator_::neg(ik0), ik1, ik2)];
+                  field_fft_out[pythonic::types::make_tuple(ik0, ik1, ik2)] = pythonic::types::as_const(field_fft_in)[pythonic::types::make_tuple(ik0, ik1, ik2)];
+                  if (pythonic::builtins::pythran::and_([&] () { return pythonic::operator_::gt(ik0, 0L); }, [&] () { return pythonic::operator_::lt(ik0, pythonic::operator_::functor::floordiv()(nk0_min, 2L)); }))
+                  {
+                    field_fft_out[pythonic::types::make_tuple(pythonic::operator_::neg(ik0), ik1, ik2)] = pythonic::types::as_const(field_fft_in)[pythonic::types::make_tuple(pythonic::operator_::neg(ik0), ik1, ik2)];
+                    if (pythonic::builtins::pythran::and_([&] () { return pythonic::operator_::gt(ik1, 0L); }, [&] () { return pythonic::operator_::lt(ik1, pythonic::operator_::functor::floordiv()(nk1_min, 2L)); }))
+                    {
+                      field_fft_out[pythonic::types::make_tuple(pythonic::operator_::neg(ik0), pythonic::operator_::neg(ik1), ik2)] = pythonic::types::as_const(field_fft_in)[pythonic::types::make_tuple(pythonic::operator_::neg(ik0), pythonic::operator_::neg(ik1), ik2)];
+                    }
+                  }
                   if (pythonic::builtins::pythran::and_([&] () { return pythonic::operator_::gt(ik1, 0L); }, [&] () { return pythonic::operator_::lt(ik1, pythonic::operator_::functor::floordiv()(nk1_min, 2L)); }))
                   {
-                    field_fft_out[pythonic::types::make_tuple(pythonic::operator_::neg(ik0), pythonic::operator_::neg(ik1), ik2)] = field_fft_in[pythonic::types::make_tuple(pythonic::operator_::neg(ik0), pythonic::operator_::neg(ik1), ik2)];
+                    field_fft_out[pythonic::types::make_tuple(ik0, pythonic::operator_::neg(ik1), ik2)] = pythonic::types::as_const(field_fft_in)[pythonic::types::make_tuple(ik0, pythonic::operator_::neg(ik1), ik2)];
                   }
                 }
-                if (pythonic::builtins::pythran::and_([&] () { return pythonic::operator_::gt(ik1, 0L); }, [&] () { return pythonic::operator_::lt(ik1, pythonic::operator_::functor::floordiv()(nk1_min, 2L)); }))
-                {
-                  field_fft_out[pythonic::types::make_tuple(ik0, pythonic::operator_::neg(ik1), ik2)] = field_fft_in[pythonic::types::make_tuple(ik0, pythonic::operator_::neg(ik1), ik2)];
-                }
               }
             }
           }
         }
       }
+      return pythonic::builtins::None;
     }
-    return pythonic::builtins::None;
   }
 }
 #include <pythonic/python/exception_handler.hpp>
 #ifdef ENABLE_PYTHON_MODULE
 static PyObject* __transonic__ = to_python(__pythran_mini_oper_modif_resol::__transonic__()());
 inline
 typename __pythran_mini_oper_modif_resol::fill_field_fft_3d::type<pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long,long>>, pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long,long>>>::result_type fill_field_fft_3d0(pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long,long>>&& field_fft_in, pythonic::types::ndarray<std::complex<double>,pythonic::types::pshape<long,long,long>>&& field_fft_out) 
@@ -275,17 +281,17 @@
                                          Methods,
                                          ""
     );
     #endif
     if(! theModule)
         PYTHRAN_RETURN;
     PyObject * theDoc = Py_BuildValue("(sss)",
-                                      "0.11.0",
-                                      "2022-09-02 03:40:15.433968",
-                                      "80c6e36b1fafe32f15fdce2ed5fb4df1750d2a02de22bab3496f9f019d4badf5");
+                                      "0.13.1",
+                                      "2023-05-24 11:29:43.223275",
+                                      "aed0a5a942d86c15c3186b3d60628d3c863c6f411067b70d2262f4d621beab2b");
     if(! theDoc)
         PYTHRAN_RETURN;
     PyModule_AddObject(theModule,
                        "__pythran__",
                        theDoc);
 
     PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `fluidsim-0.7.2/fluidsim/util/console/__main__.py` & `fluidsim-0.7.3/fluidsim/util/console/__main__.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/console/bench.py` & `fluidsim-0.7.3/fluidsim/util/console/bench.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/console/bench_analysis.py` & `fluidsim-0.7.3/fluidsim/util/console/bench_analysis.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/console/profile.py` & `fluidsim-0.7.3/fluidsim/util/console/profile.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/console/test_bench.py` & `fluidsim-0.7.3/fluidsim/util/console/test_bench.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
         command = f"fluidsim-bench 24 -d 2 -o {path_tmp} -t {type_fft}"
         sys.argv = command.split()
         run_bench()
 
         # Can plot only parallel benchmarks
         if mpi.rank == 0 and mpi.nb_proc != 1:
-
             command = f"fluidsim-bench-analysis 24 -d 2 -i {path_tmp}"
             sys.argv = command.split()
             run_bench_analysis()
 
         sys.argv = "fluidsim-bench -l -d 2".split()
         run_bench()
```

### Comparing `fluidsim-0.7.2/fluidsim/util/console/test_profile.py` & `fluidsim-0.7.3/fluidsim/util/console/test_profile.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/console/util.py` & `fluidsim-0.7.3/fluidsim/util/console/util.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/frequency_modulation.py` & `fluidsim-0.7.3/fluidsim/util/frequency_modulation.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/mini_oper_modif_resol.py` & `fluidsim-0.7.3/fluidsim/util/mini_oper_modif_resol.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
                         ]
                 if ik1 > 0 and ik1 < nk1_min // 2:
                     field_fft_out[ik0, -ik1, ik2] = field_fft_in[ik0, -ik1, ik2]
 
 
 class MiniOperModifResol:
     def __init__(self, shape):
-
         self.shape = shape
 
         dimension = self.dimension = len(shape)
 
         if dimension not in [2, 3]:
             raise NotImplementedError
 
@@ -75,12 +74,11 @@
         self.fft_as_arg = self.oper_fft.fft_as_arg
         self.ifft_as_arg = self.oper_fft.ifft_as_arg
 
         self.create_arrayX = self.oper_fft.create_arrayX
         self.create_arrayK = self.oper_fft.create_arrayK
 
     def fill_field_fft(self, field_spect, field2_spect, oper):
-
         if self.dimension == 2:
             return fill_field_fft_2d(field_spect, field2_spect)
 
         fill_field_fft_3d(field_spect, field2_spect)
```

### Comparing `fluidsim-0.7.2/fluidsim/util/output.py` & `fluidsim-0.7.3/fluidsim/util/output.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/scripts/modif_resolution.py` & `fluidsim-0.7.3/fluidsim/util/scripts/modif_resolution.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/scripts/restart.py` & `fluidsim-0.7.3/fluidsim/util/scripts/restart.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/scripts/test_modif_resolution.py` & `fluidsim-0.7.3/fluidsim/util/scripts/test_modif_resolution.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/scripts/test_restart.py` & `fluidsim-0.7.3/fluidsim/util/scripts/test_restart.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/scripts/test_turb_trandom_anisotropic.py` & `fluidsim-0.7.3/fluidsim/util/scripts/test_turb_trandom_anisotropic.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/scripts/turb_trandom_anisotropic.py` & `fluidsim-0.7.3/fluidsim/util/scripts/turb_trandom_anisotropic.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,9 +524,8 @@
 
 """ + indent(
         parser.format_help(), "    "
     )
 
 
 if __name__ == "__main__":
-
     params, sim = main()
```

### Comparing `fluidsim-0.7.2/fluidsim/util/test_util.py` & `fluidsim-0.7.3/fluidsim/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim/util/testing.py` & `fluidsim-0.7.3/fluidsim/util/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
     def getter(self, method):
         self.fget = method
         return self
 
 
 class TestCase(unittest.TestCase):
-
     # True except if pytest is used...
     has_to_redirect_stdout = not any(
         any(test_tool in arg for arg in sys.argv)
         for test_tool in ("pytest", "py.test")
     )
 
     def run(self, result=None):
```

### Comparing `fluidsim-0.7.2/fluidsim/util/util.py` & `fluidsim-0.7.3/fluidsim/util/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 """Utilities for the numerical simulations (:mod:`fluidsim.util.util`)
 ======================================================================
 
 """
 
+import json
 import os
 import time
+import warnings
 from copy import deepcopy as _deepcopy
 from datetime import timedelta
 from functools import partial
 from importlib import import_module
 from pathlib import Path
 from time import perf_counter
-from typing import Union
 from math import radians
-import warnings
-import json
-import hashlib
-import inspect
-from importlib import import_module
 
 import h5netcdf
 import h5py
 import numpy as np
-from rich.progress import track
 
 import fluiddyn as fld
 from fluiddyn.io.redirect_stdout import stdout_redirected
 from fluiddyn.util import mpi
 from fluiddyn.util import get_memory_usage
 
 from fluidsim_core import loader
+from fluidsim_core.output.dataframe_from_paths import DataframeMaker
 
-from fluidsim import path_dir_results
+from fluidsim_core.paths import find_path_result_dir
 
 from fluidsim.base.params import (
     Parameters,
     fix_old_params,
     load_info_solver,
     load_params_simul,
     merge_params,
@@ -102,41 +98,15 @@
             return str(dim)
 
     raise NotImplementedError(
         "Cannot deduce dimension of the solver from the name " + class_name
     )
 
 
-def pathdir_from_namedir(name_dir: Union[str, Path, None] = None):
-    """Return the path of a result directory.
-
-    name_dir: str, optional
-
-      Can be an absolute path, a relative path, or even simply just
-      the name of the directory under $FLUIDSIM_PATH.
-
-    """
-    if name_dir is None:
-        return Path.cwd()
-
-    if not isinstance(name_dir, Path):
-        name_dir = Path(name_dir)
-
-    name_dir = name_dir.expanduser()
-
-    if name_dir.is_dir():
-        return name_dir.absolute()
-
-    if not name_dir.is_absolute():
-        name_dir = path_dir_results / name_dir
-
-    if not name_dir.is_dir():
-        raise ValueError(str(name_dir) + " is not a directory")
-
-    return name_dir
+pathdir_from_namedir = find_path_result_dir
 
 
 class ModulesSolvers(dict):
     """Dictionary to gather imported solvers."""
 
     def __init__(self, names_solvers):
         for key in names_solvers:
@@ -640,15 +610,14 @@
 
     path_file = Path(path) / "stdout.txt"
     if not path_file.exists():
         print(f"Given path does not exist:\n{path}")
         return 666, 666
 
     with open(path_file, "r") as file_stdout:
-
         line = ""
         while not line.startswith("it ="):
             line = file_stdout.readline()
 
         words = line.split()
         t_s = float(words[6])
 
@@ -760,15 +729,14 @@
                 "Angle should be a string with \n"
                 + "the degree symbol or a float in radians"
             )
     return angle
 
 
 def get_last_time_spatial_means_from_path(path):
-
     path_file = Path(path) / "spatial_means.txt"
 
     if path_file.exists():
         with open(path_file, "rb") as file_means:
             nb_char = file_means.seek(0, os.SEEK_END)  # go to the end
             nb_char_to_read = min(nb_char, 1000)
             file_means.seek(-nb_char_to_read, 2)
@@ -791,131 +759,36 @@
             while line != b"":
                 line_prev = line
                 line = file_means.readline()
 
         return json.loads(line_prev)["t"]
 
 
-def get_mean_values_from_path(
-    path, tmin=None, tmax=None, use_cache=True, customize=None
-):
-
-    """Get a dict of scalar values characterizing the simulation
-
-    Parameters
-    ----------
-
-    tmin: float
-        Minimum time
-
-    tmax: float
-        Maximum time
-
-    use_cache: bool
-        If True, return the cached result
-
-    customize: callable
-
-        If not None, called as ``customize(result, self.sim)`` to modify the
-        returned dict.
-
-    Examples
-    --------
-
-    .. code-block:: python
-
-        def customize(result, sim):
-            result["Rb"] = float(sim.params.short_name_type_run.split("_Rb")[-1])
-        get_mean_values_from_path(path, customize=customize)
-
-    """
-
-    if (
-        tmin is None
-        or isinstance(tmin, str)
-        or tmax is None
-        or isinstance(tmax, str)
-    ):
+class _DataframeMakerFluidsim(DataframeMaker):
+    def get_time_start_from_path(self, path):
+        """ "Get first time"""
         t_start, _ = times_start_last_from_path(path)
-        t_last = get_last_time_spatial_means_from_path(path)
-
-    if tmin is None:
-        tmin = t_start
-    elif isinstance(tmin, str):
-        if tmin.startswith("t_start+"):
-            tmin = t_start + float(tmin.split("t_start+")[-1])
-        elif tmin.startswith("t_last-"):
-            tmin = t_last - float(tmin.split("t_last-")[-1])
-        else:
-            raise ValueError(
-                f"isinstance(tmin, str) and {tmin=} but tmin has to start by "
-                '"t_start+" or "t_last-"'
-            )
-    tmin = float(tmin)
-
-    if tmax is None:
-        tmax = t_last
-    elif isinstance(tmax, str):
-        if tmax.startswith("t_start+"):
-            tmax = t_start + float(tmax.split("t_start+")[-1])
-        elif tmax.startswith("t_last-"):
-            tmax = t_last - float(tmax.split("t_last-")[-1])
-        else:
-            raise ValueError(
-                f"isinstance(tmax, str) and {tmax=} but tmin has to start by "
-                '"t_start+" or "t_last-"'
-            )
-    tmax = float(tmax)
-
-    cache_dir = Path(path) / ".cache"
-    cache_dir.mkdir(exist_ok=True)
-
-    if customize is not None:
-        source = inspect.getsource(customize).encode().strip()
-        hash = hashlib.sha256(source).hexdigest()[:16]
-        part_customize = f"_customize{hash}"
-    else:
-        part_customize = ""
-
-    cache_file = cache_dir / (
-        f"mean_values_tmin{tmin}_tmax{tmax}{part_customize}.json"
-    )
-
-    if use_cache and cache_file.exists():
-        with open(cache_file, "r") as file:
-            return json.load(file)
-
-    sim = load_sim_for_plot(path, hide_stdout=True)
-
-    result = sim.output._compute_mean_values(tmin, tmax)
-    if customize is not None:
-        customize(result, sim)
-
-    print("saving", cache_file)
-    with open(cache_file, "w") as file:
-        json.dump(result, file, indent=2)
-    return result
+        return t_start
 
+    def get_time_last_from_path(self, path):
+        """ "Get last saved time"""
+        return get_last_time_spatial_means_from_path(path)
+
+    def load_sim(self, path):
+        """Load a simulation object"""
+        return load_sim_for_plot(path, hide_stdout=True)
 
-def get_dataframe_from_paths(
-    paths, tmin=None, tmax=None, use_cache=True, customize=None
-):
-    """Produce a dataframe from a set of simulations.
-
-    Uses ``sim.output.get_mean_values``
-
-    """
-
-    from pandas import DataFrame
-
-    values = []
-    for path in track(paths, "Getting the mean values"):
-        values.append(
-            get_mean_values_from_path(path, tmin, tmax, use_cache, customize)
+    def get_dataframe_from_paths(
+        self, paths, tmin=None, tmax=None, use_cache=True, customize=None
+    ):
+        df = super().get_dataframe_from_paths(
+            paths, tmin, tmax, use_cache, customize
         )
+        if "R2" in df.columns and "R4" in df.columns:
+            df["min_R"] = np.array([df.R2, df.R4]).min(axis=0)
+        return df
 
-    df = DataFrame(values)
 
-    if "R2" in df.columns and "R4" in df.columns:
-        df["min_R"] = np.array([df.R2, df.R4]).min(axis=0)
+_dataframe_maker = _DataframeMakerFluidsim()
 
-    return df
+get_mean_values_from_path = _dataframe_maker.get_mean_values_from_path
+get_dataframe_from_paths = _dataframe_maker.get_dataframe_from_paths
```

### Comparing `fluidsim-0.7.2/fluidsim.egg-info/PKG-INFO` & `fluidsim-0.7.3/fluidsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidsim
-Version: 0.7.2
+Version: 0.7.3
 Summary: Framework for studying fluid dynamics with simulations.
 Home-page: https://fluidsim.readthedocs.io
 Author: Pierre Augier
 Author-email: pierre.augier@legi.cnrs.fr
 License: CeCILL
 Project-URL: Source, https://foss.heptapod.net/fluiddyn/fluidsim
 Project-URL: Documentation, https://fluidsim.readthedocs.io
@@ -13,17 +13,17 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Provides-Extra: doc
 Provides-Extra: fft
 Provides-Extra: sphere
 Provides-Extra: mpi
 Provides-Extra: test
 Provides-Extra: dev
```

### Comparing `fluidsim-0.7.2/fluidsim.egg-info/SOURCES.txt` & `fluidsim-0.7.3/fluidsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim.egg-info/entry_points.txt` & `fluidsim-0.7.3/fluidsim.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/fluidsim.egg-info/requires.txt` & `fluidsim-0.7.3/fluidsim.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-fluidsim-core>=0.7.2
+fluidsim-core>=0.7.3
 h5py
 h5netcdf
 transonic>=0.4.3
 setuptools_scm
 xarray
 rich
 matplotlib>=3.3
@@ -25,14 +25,16 @@
 pytest-mock
 ipython
 pymech
 mpi4py
 pyfftw>=0.10.4
 fluidfft>=0.2.7
 fluidsht>=0.0.3a0
+build
+twine
 
 [doc]
 sphinx
 sphinx_rtd_theme
 numpydoc
 jupyter
 pandas
@@ -62,14 +64,16 @@
 pytest-mock
 ipython
 pymech
 mpi4py
 pyfftw>=0.10.4
 fluidfft>=0.2.7
 fluidsht>=0.0.3a0
+build
+twine
 
 [mpi]
 mpi4py
 
 [sphere]
 fluidsht>=0.0.3a0
```

### Comparing `fluidsim-0.7.2/pylintrc` & `fluidsim-0.7.3/pylintrc`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/pyproject.toml` & `fluidsim-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/setup.cfg` & `fluidsim-0.7.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 	pymech
 dev = 
 	%(doc)s
 	%(test)s
 	%(mpi)s
 	%(fft)s
 	%(sphere)s
+	build
+	twine
 full = 
 	%(dev)s
 
 [options.entry_points]
 console_scripts = 
 	fluidsim = fluidsim.util.console.__main__:run
 	fluidsim-create-xml-description = fluidsim.base.output:run
```

### Comparing `fluidsim-0.7.2/setup.py` & `fluidsim-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from time import time
 from runpy import run_path
 
 from setuptools import setup, find_packages
 
 from transonic.dist import make_backend_files, init_transonic_extensions
 
-if sys.version_info[:2] < (3, 8):
-    raise RuntimeError("Python version >= 3.8 required.")
+if sys.version_info[:2] < (3, 9):
+    raise RuntimeError("Python version >= 3.9 required.")
 
 here = Path(__file__).parent.absolute()
 
 sys.path.insert(0, ".")
 
 from setup_configure import FFTW3, logger, TRANSONIC_BACKEND, get_config
 from setup_build import FluidSimBuildExt
@@ -190,17 +190,17 @@
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         # actually CeCILL License (GPL compatible license for French laws)
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     packages=find_packages(exclude=["doc", "examples"]),
     setup_requires=setup_requires,
     install_requires=install_requires,
     cmdclass={"build_ext": FluidSimBuildExt},
     ext_modules=create_extensions(),
 )
```

### Comparing `fluidsim-0.7.2/setup_build.py` & `fluidsim-0.7.3/setup_build.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/setup_configure.py` & `fluidsim-0.7.3/setup_configure.py`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/site.cfg.default` & `fluidsim-0.7.3/site.cfg.default`

 * *Files identical despite different names*

### Comparing `fluidsim-0.7.2/tox.ini` & `fluidsim-0.7.3/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 #
 # To run tox faster, check out Detox
 # (https://pypi.python.org/pypi/detox), which runs your tox runs in
 # parallel. To use it, "pip install detox" and then run "detox" from
 # this directory.
 [tox]
 envlist =
-    py{38,39,310}-pythran-fft
+    py{38,39,310,311}-pythran-fft
     lint
     codecov
 isolated_build = True
 
 [gh-actions]
 python =
     3.8: py38-pythran-fft
     3.9: py39-pythran-fft
     3.10: py310-pythran-fft
+    3.11: py311-pythran-fft
 
 [testenv]
 setenv =
     FLUIDSIM_PATH = {toxinidir}/fluidsim_path
     FLUIDDYN_PATH_SCRATCH = {toxinidir}/scratch
     # no need to compile fluidfft files for these tests
     FLUIDFFT_TRANSONIC_BACKEND = python
```

