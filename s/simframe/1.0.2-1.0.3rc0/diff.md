# Comparing `tmp/simframe-1.0.2.tar.gz` & `tmp/simframe-1.0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simframe-1.0.2.tar", last modified: Tue Mar 29 17:44:10 2022, max compression
+gzip compressed data, was "simframe-1.0.3rc0.tar", last modified: Fri May 12 14:57:17 2023, max compression
```

## Comparing `simframe-1.0.2.tar` & `simframe-1.0.3rc0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:09.304050 simframe-1.0.2/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1532 2022-03-10 11:03:13.000000 simframe-1.0.2/LICENSE
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      198 2022-03-10 11:03:13.000000 simframe-1.0.2/MANIFEST.in
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4438 2022-03-29 17:44:09.300053 simframe-1.0.2/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3248 2022-03-10 11:03:13.000000 simframe-1.0.2/README.md
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:07.161050 simframe-1.0.2/docs/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      638 2021-12-24 09:33:56.000000 simframe-1.0.2/docs/Makefile
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      799 2021-12-24 09:33:56.000000 simframe-1.0.2/docs/make.bat
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      143 2021-12-24 09:33:56.000000 simframe-1.0.2/docs/requirements.txt
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:07.229053 simframe-1.0.2/docs/source/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      421 2021-12-24 09:33:56.000000 simframe-1.0.2/docs/source/api.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1828 2022-03-10 11:03:13.000000 simframe-1.0.2/docs/source/conf.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1032 2022-03-10 11:03:13.000000 simframe-1.0.2/docs/source/index.rst
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:07.591084 simframe-1.0.2/examples/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    99494 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/1_simple_integration.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    49496 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/2_advanced_integration.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   125207 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/3_updating.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    13834 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/4_custom_schemes.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   381957 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/5_adaptive_schemes.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    68256 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/6_implicit_integration.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1380 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/A_citation.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2648 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/B_contrib_bug_feature.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   391549 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/example_compartmental_models.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)  4006805 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/example_coupled_oscillators.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1280874 2022-03-29 12:45:07.000000 simframe-1.0.2/examples/example_double_pendulum.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2022-03-29 17:44:09.306050 simframe-1.0.2/setup.cfg
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2064 2021-12-24 09:33:56.000000 simframe-1.0.2/setup.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:07.720058 simframe-1.0.2/simframe/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      356 2022-03-29 17:37:46.000000 simframe-1.0.2/simframe/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:08.159052 simframe-1.0.2/simframe/frame/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      529 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/frame/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2074 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/frame/abstractgroup.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     9540 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/frame/field.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6707 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/frame/frame.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    13245 2022-03-29 12:45:07.000000 simframe-1.0.2/simframe/frame/group.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3897 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/frame/heartbeat.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     5516 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/frame/intvar.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      964 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/frame/updater.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:08.264050 simframe-1.0.2/simframe/integration/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      715 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2314 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/instruction.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7722 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/integrator.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3301 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/scheme.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:08.901049 simframe-1.0.2/simframe/integration/schemes/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2659 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1087 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_1_euler.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2631 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_2_fehlberg_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1232 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_2_heun.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2374 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_2_heun_euler_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1218 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_2_midpoint.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1250 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_2_ralston.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2814 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_3_bogacki_shampine_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2736 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_3_gottlieb_shu_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1340 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_3_heun.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1360 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_3_kutta.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1375 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_3_ralston.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1456 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_3_ssprk.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1499 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_4_38rule.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1818 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_4_ralston.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1531 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_4_runge_kutta.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3718 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_5_cash_karp_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4164 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/expl_5_dormand_prince_adptv.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1362 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/impl_1_euler_direct.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1614 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/impl_1_euler_gmres.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1422 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/impl_2_midpoint_direct.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      764 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/integration/schemes/update.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:09.039051 simframe-1.0.2/simframe/io/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      710 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/io/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      782 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/io/dump.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7507 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/io/progress.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4634 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/io/reader.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    10622 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/io/writer.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:09.169050 simframe-1.0.2/simframe/io/writers/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      507 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/io/writers/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6983 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/io/writers/hdf5writer.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6050 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/io/writers/namespacewriter.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:09.271052 simframe-1.0.2/simframe/utils/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      451 2022-03-29 12:45:08.000000 simframe-1.0.2/simframe/utils/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1770 2021-12-24 09:33:56.000000 simframe-1.0.2/simframe/utils/color.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1249 2022-03-29 12:45:08.000000 simframe-1.0.2/simframe/utils/format.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2022-03-29 17:44:07.946051 simframe-1.0.2/simframe.egg-info/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4438 2022-03-29 17:44:06.000000 simframe-1.0.2/simframe.egg-info/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2484 2022-03-29 17:44:07.000000 simframe-1.0.2/simframe.egg-info/SOURCES.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2022-03-29 17:44:06.000000 simframe-1.0.2/simframe.egg-info/dependency_links.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2022-03-29 17:44:06.000000 simframe-1.0.2/simframe.egg-info/not-zip-safe
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       33 2022-03-29 17:44:06.000000 simframe-1.0.2/simframe.egg-info/requires.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       15 2022-03-29 17:44:06.000000 simframe-1.0.2/simframe.egg-info/top_level.txt
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:17.571697 simframe-1.0.3rc0/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1532 2022-03-10 11:03:13.000000 simframe-1.0.3rc0/LICENSE
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      198 2022-03-10 11:03:13.000000 simframe-1.0.3rc0/MANIFEST.in
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4697 2023-05-12 14:57:17.566697 simframe-1.0.3rc0/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3524 2023-05-12 14:36:17.000000 simframe-1.0.3rc0/README.md
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:14.773544 simframe-1.0.3rc0/docs/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      638 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/docs/Makefile
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      799 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/docs/make.bat
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      129 2023-05-12 14:36:17.000000 simframe-1.0.3rc0/docs/requirements.txt
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:14.896866 simframe-1.0.3rc0/docs/source/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      421 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/docs/source/api.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1828 2022-03-10 11:03:13.000000 simframe-1.0.3rc0/docs/source/conf.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1032 2022-03-10 11:03:13.000000 simframe-1.0.3rc0/docs/source/index.rst
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:15.429207 simframe-1.0.3rc0/examples/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    71383 2023-05-12 14:36:17.000000 simframe-1.0.3rc0/examples/1_simple_integration.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    49496 2023-05-12 14:36:17.000000 simframe-1.0.3rc0/examples/2_advanced_integration.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   142872 2023-05-12 14:36:17.000000 simframe-1.0.3rc0/examples/3_updating.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    13834 2022-03-29 12:45:07.000000 simframe-1.0.3rc0/examples/4_custom_schemes.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   381957 2022-03-29 12:45:07.000000 simframe-1.0.3rc0/examples/5_adaptive_schemes.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    68256 2022-03-29 12:45:07.000000 simframe-1.0.3rc0/examples/6_implicit_integration.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1380 2022-03-29 12:45:07.000000 simframe-1.0.3rc0/examples/A_citation.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2648 2022-03-29 12:45:07.000000 simframe-1.0.3rc0/examples/B_contrib_bug_feature.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   391549 2022-03-29 12:45:07.000000 simframe-1.0.3rc0/examples/example_compartmental_models.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)  4006805 2022-03-29 12:45:07.000000 simframe-1.0.3rc0/examples/example_coupled_oscillators.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1280874 2022-03-29 12:45:07.000000 simframe-1.0.3rc0/examples/example_double_pendulum.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-05-12 14:57:17.573692 simframe-1.0.3rc0/setup.cfg
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2064 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/setup.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:15.496678 simframe-1.0.3rc0/simframe/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      360 2023-05-12 14:37:05.000000 simframe-1.0.3rc0/simframe/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:15.975765 simframe-1.0.3rc0/simframe/frame/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      529 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/frame/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2074 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/frame/abstractgroup.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    10152 2023-05-12 14:36:17.000000 simframe-1.0.3rc0/simframe/frame/field.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6707 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/frame/frame.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    13139 2023-05-12 14:54:08.000000 simframe-1.0.3rc0/simframe/frame/group.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3897 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/frame/heartbeat.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     5516 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/frame/intvar.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      964 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/frame/updater.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:16.133990 simframe-1.0.3rc0/simframe/integration/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      715 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2314 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/instruction.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7722 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/integrator.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3301 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/scheme.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:17.146691 simframe-1.0.3rc0/simframe/integration/schemes/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2659 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1087 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_1_euler.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2631 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_2_fehlberg_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1232 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_2_heun.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2374 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_2_heun_euler_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1218 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_2_midpoint.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1250 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_2_ralston.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2814 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_3_bogacki_shampine_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2736 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_3_gottlieb_shu_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1340 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_3_heun.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1360 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_3_kutta.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1375 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_3_ralston.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1456 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_3_ssprk.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1499 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_4_38rule.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1818 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_4_ralston.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1531 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_4_runge_kutta.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3718 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_5_cash_karp_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4164 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/expl_5_dormand_prince_adptv.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1362 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/impl_1_euler_direct.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1614 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/impl_1_euler_gmres.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1422 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/impl_2_midpoint_direct.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      764 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/integration/schemes/update.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:17.319691 simframe-1.0.3rc0/simframe/io/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      710 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/io/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      782 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/io/dump.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7507 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/io/progress.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4634 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/io/reader.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     9406 2023-05-12 14:36:17.000000 simframe-1.0.3rc0/simframe/io/writer.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:17.437689 simframe-1.0.3rc0/simframe/io/writers/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      507 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/io/writers/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6983 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/io/writers/hdf5writer.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     6050 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/io/writers/namespacewriter.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:17.528694 simframe-1.0.3rc0/simframe/utils/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      451 2022-03-29 12:45:08.000000 simframe-1.0.3rc0/simframe/utils/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1770 2021-12-24 09:33:56.000000 simframe-1.0.3rc0/simframe/utils/color.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1249 2022-03-29 12:45:08.000000 simframe-1.0.3rc0/simframe/utils/format.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-12 14:57:15.664494 simframe-1.0.3rc0/simframe.egg-info/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4697 2023-05-12 14:57:13.000000 simframe-1.0.3rc0/simframe.egg-info/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2484 2023-05-12 14:57:14.000000 simframe-1.0.3rc0/simframe.egg-info/SOURCES.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-05-12 14:57:13.000000 simframe-1.0.3rc0/simframe.egg-info/dependency_links.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2022-03-29 17:44:06.000000 simframe-1.0.3rc0/simframe.egg-info/not-zip-safe
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       33 2023-05-12 14:57:13.000000 simframe-1.0.3rc0/simframe.egg-info/requires.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       15 2023-05-12 14:57:13.000000 simframe-1.0.3rc0/simframe.egg-info/top_level.txt
```

### Comparing `simframe-1.0.2/LICENSE` & `simframe-1.0.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/PKG-INFO` & `simframe-1.0.3rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: simframe
-Version: 1.0.2
+Version: 1.0.3rc0
 Summary: Framework for Scientific Simulations
 Home-page: https://github.com/stammler/simframe
 Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com, til.birnstiel@lmu.de
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/simframe/
 Project-URL: Documentation, https://simframe.readthedocs.io/
 Keywords: numerical,simulation,integration,science,mathematics,physics
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -25,19 +24,17 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simframe
 
-[![Documentation Status](https://readthedocs.org/projects/simframe/badge/?version=latest)](https://simframe.readthedocs.io/en/latest/?badge=latest) 
-![GitHub](https://img.shields.io/github/license/stammler/simframe) 
-[![status](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6/status.svg)](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6) 
-![PyPI - Downloads](https://img.shields.io/pypi/dm/simframe?label=PyPI%20downloads)
-[![Fedora package](https://img.shields.io/fedora/v/python3-simframe?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-simframe)
+[![Documentation Status](https://readthedocs.org/projects/simframe/badge/?version=latest)](https://simframe.readthedocs.io/en/latest/?badge=latest) [![GitHub](https://img.shields.io/github/license/stammler/simframe) ](https://github.com/stammler/simframe/blob/master/LICENSE) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/stammler/simframe/blob/master/.github/CODE_OF_CONDUCT.md)  
+[![status](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6/status.svg)](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6)  
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/simframe?label=PyPI%20downloads)](https://pypistats.org/packages/simframe) [![Fedora package](https://img.shields.io/fedora/v/python3-simframe?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-simframe)
 
 ### Framework for scientific simulations
 
 `Simframe` is a Python framework to facilitate scientific simulations. The scope of the software is to provide a framework which can hold data fields, which can be used to integrate differential equations, and which can read and write data files.
 
 Data fields are stored in modified `numpy.ndarray`s. Therefore, `Simframe` can only work with data, that can be stored in `NumPy` arrays.
 
@@ -86,9 +83,7 @@
 ```
 
 ## Ackowledgements
 
 `simframe` has received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme under grant agreement No 714769.
 
 `simframe` was developed at the [University Observatory](https://www.usm.uni-muenchen.de/index_en.php) of the [Ludwig Maximilian University of Munich](https://www.en.uni-muenchen.de/index.html).
-
-
```

### Comparing `simframe-1.0.2/README.md` & `simframe-1.0.3rc0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Simframe
 
-[![Documentation Status](https://readthedocs.org/projects/simframe/badge/?version=latest)](https://simframe.readthedocs.io/en/latest/?badge=latest) 
-![GitHub](https://img.shields.io/github/license/stammler/simframe) 
-[![status](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6/status.svg)](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6) 
-![PyPI - Downloads](https://img.shields.io/pypi/dm/simframe?label=PyPI%20downloads)
-[![Fedora package](https://img.shields.io/fedora/v/python3-simframe?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-simframe)
+[![Documentation Status](https://readthedocs.org/projects/simframe/badge/?version=latest)](https://simframe.readthedocs.io/en/latest/?badge=latest) [![GitHub](https://img.shields.io/github/license/stammler/simframe) ](https://github.com/stammler/simframe/blob/master/LICENSE) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/stammler/simframe/blob/master/.github/CODE_OF_CONDUCT.md)  
+[![status](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6/status.svg)](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6)  
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/simframe?label=PyPI%20downloads)](https://pypistats.org/packages/simframe) [![Fedora package](https://img.shields.io/fedora/v/python3-simframe?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-simframe)
 
 ### Framework for scientific simulations
 
 `Simframe` is a Python framework to facilitate scientific simulations. The scope of the software is to provide a framework which can hold data fields, which can be used to integrate differential equations, and which can read and write data files.
 
 Data fields are stored in modified `numpy.ndarray`s. Therefore, `Simframe` can only work with data, that can be stored in `NumPy` arrays.
```

### Comparing `simframe-1.0.2/docs/Makefile` & `simframe-1.0.3rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/docs/make.bat` & `simframe-1.0.3rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/docs/source/conf.py` & `simframe-1.0.3rc0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/docs/source/index.rst` & `simframe-1.0.3rc0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/examples/2_advanced_integration.ipynb` & `simframe-1.0.3rc0/examples/2_advanced_integration.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998788759689923%*

 * *Differences: {"'cells'": "{53: {'source': {insert: [(0, '## Inspecting memory usage\\n')], delete: [0]}}}"}*

```diff
@@ -660,15 +660,15 @@
                 "sim.toc"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Inspecting Memory usage\n",
+                "## Inspecting memory usage\n",
                 "\n",
                 "It is possible to print out the memory usage in bytes of a group with the command"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 33,
```

### Comparing `simframe-1.0.2/examples/3_updating.ipynb` & `simframe-1.0.3rc0/examples/3_updating.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9799228512326917%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'In addition to the `simframe` requirements, the "*

 * *            "following packages are needed for this notebook: `astropy`, `matplotlib`.')], delete: "*

 * *            "[3]}}, 1: {'source': {insert: [(0, '# Updating Groups and Fields\\n')], delete: "*

 * *            "[0]}}, 6: {'source': ['import astropy.constants as c\\n', 'import astropy.units as "*

 * *            "u']}, 9: {'execution_count': 6}, 10: {'execution_count': 7}, 12: {'execution_count': "*

 * *            '8, \'source\ […]*

```diff
@@ -3,22 +3,22 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "**This notebook teaches how to:**  \n",
                 "update groups and fields and use heartbeats.\n",
                 "\n",
-                "[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/stammler/simframe/HEAD?labpath=examples%2F3_updating.ipynb)"
+                "In addition to the `simframe` requirements, the following packages are needed for this notebook: `astropy`, `matplotlib`."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# 3. Updating Groups and Fields\n",
+                "# Updating Groups and Fields\n",
                 "\n",
                 "In this example we revisit the orbital integration from the previous tutorial. But this time we also want to calculate the equilibrium temperature on Earth. That is not a quantity that we need to integrate. We can simply calculate it from the other quantities. But we have to tell `simframe` how to do it."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -58,46 +58,52 @@
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
-                "AU       = 1.495978707e11          # Astronomical unit [m]\n",
-                "day      = 8.64e4                  # Day [s]\n",
-                "G        = 6.6743e-11              # Gravitational constant [m\u00b3/kg/s\u00b2]\n",
-                "year     = 3.15576e7               # Year [s]\n",
-                "\n",
-                "M_earth  = 5.972167867791379e24    # Mass of the Earth [kg]\n",
-                "M_sun    = 1.988409870698051e30    # Mass of the Sun [kg]\n",
-                "\n",
-                "R_earth  = 6.3781e6                # Radius of Earth [m]\n",
-                "R_sun    = 6.957e8                 # Radius of Sun [m]\n",
-                "sigma_sb = 5.6703744191844314e-08  # Stefan-Boltzmann constant [W/m\u00b2/K^4]"
+                "import astropy.constants as c\n",
+                "import astropy.units as u"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "AU   = (1.*u.au).si.value\n",
+                "day  = (1.*u.day).si.value\n",
+                "G    = c.G.si.value\n",
+                "year = (1.*u.year).si.value\n",
+                "\n",
+                "M_earth = c.M_earth.si.value\n",
+                "M_sun   = c.M_sun.si.value"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "**Earth**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.addfield(\"M\", M_earth, description=\"Mass [kg]\", constant=True)\n",
                 "sim.Earth.addfield(\"r\", np.zeros(3), description=\"Position [m]\")\n",
                 "sim.Earth.addfield(\"v\", np.zeros(3), description=\"Velocity [m/s]\")"
             ]
@@ -107,80 +113,80 @@
             "metadata": {},
             "source": [
                 "**Sun**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sim.Sun.addfield(\"M\", M_sun, description=\"Mass [kg]\", constant=True)\n",
+                "sim.Sun.addfield(\"M\", c.M_sun.si.value, description=\"Mass [kg]\", constant=True)\n",
                 "sim.Sun.addfield(\"r\", np.zeros(3), description=\"Position [m]\")\n",
                 "sim.Sun.addfield(\"v\", np.zeros(3), description=\"Velocity [m/s]\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "**Integration variable**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.addintegrationvariable(\"t\", 0., description=\"Time [s]\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "dt = 1.*day"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def f_dt(frame):\n",
                 "    return dt"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.t.updater = f_dt"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "snapwidth = 5.*day\n",
                 "tmax = 2.*year"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.t.snapshots = np.arange(snapwidth, tmax+1, snapwidth)"
             ]
         },
         {
@@ -188,33 +194,33 @@
             "metadata": {},
             "source": [
                 "**Writer**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from simframe import writers"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.writer = writers.namespacewriter()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.writer.verbosity = 0"
             ]
         },
         {
@@ -222,54 +228,54 @@
             "metadata": {},
             "source": [
                 "**Differential equations**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def dr_Earth(frame, x, Y):\n",
                 "    return frame.Earth.v\n",
                 "\n",
                 "def dr_Sun(frame, x, Y):\n",
                 "    return frame.Sun.v"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Gravitational acceleration\n",
                 "def ag(M, r, R):\n",
                 "    direction = r-R\n",
                 "    distance = np.linalg.norm(direction)\n",
                 "    return -G * M * direction / distance**3"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def dv_Earth(frame, x, Y):\n",
                 "    return ag(frame.Sun.M, frame.Earth.r, frame.Sun.r)\n",
                 "\n",
                 "def dv_Sun(frame, x, Y):\n",
                 "    return ag(frame.Earth.M, frame.Sun.r, frame.Earth.r)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.v.differentiator = dv_Earth\n",
                 "sim.Earth.r.differentiator = dr_Earth\n",
                 "sim.Sun.v.differentiator   = dv_Sun\n",
                 "sim.Sun.r.differentiator   = dr_Sun"
@@ -280,33 +286,33 @@
             "metadata": {},
             "source": [
                 "**Integrator**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from simframe import Integrator"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [],
             "source": [
                 "integrator = Integrator(sim.t, description=\"Leapfrog integratior\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from simframe import schemes\n",
                 "from simframe.integration import Instruction"
             ]
         },
@@ -315,15 +321,15 @@
             "metadata": {},
             "source": [
                 "**Leapfrog integrator**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 25,
             "metadata": {},
             "outputs": [],
             "source": [
                 "instructions = [Instruction(schemes.expl_1_euler, sim.Sun.v,   fstep=0.5),\n",
                 "                Instruction(schemes.expl_1_euler, sim.Earth.v, fstep=0.5),\n",
                 "                Instruction(schemes.update,       sim.Sun.v             ),\n",
                 "                Instruction(schemes.update,       sim.Earth.v           ),\n",
@@ -334,24 +340,24 @@
                 "                Instruction(schemes.expl_1_euler, sim.Sun.v,   fstep=0.5),\n",
                 "                Instruction(schemes.expl_1_euler, sim.Earth.v, fstep=0.5),\n",
                 "               ]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 26,
             "metadata": {},
             "outputs": [],
             "source": [
                 "integrator.instructions = instructions"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 27,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.integrator = integrator"
             ]
         },
         {
@@ -361,52 +367,52 @@
                 "**Initial conditions**\n",
                 "\n",
                 "In this example we want to send the Earth on an eccentric orbit to have a seasonal change in the equilibrium temperature. For this we simply incline the initial velocities of Earth an Sun by an angle `alpha`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 28,
             "metadata": {},
             "outputs": [],
             "source": [
                 "r_Earth_ini = np.array([AU, 0., 0.])\n",
                 "r_Sun_ini = np.zeros(3)\n",
                 "# Center of mass\n",
                 "COM_ini = (M_earth*r_Earth_ini + M_sun*r_Sun_ini) / (M_earth+M_sun)\n",
                 "# Offset both positions\n",
                 "r_Earth_ini -= COM_ini\n",
                 "r_Sun_ini -= COM_ini"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 29,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mu = M_earth*M_sun / (M_earth+M_sun)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 30,
             "metadata": {},
             "outputs": [],
             "source": [
-                "alpha = 30. * (np.pi/180.) # 30 degrees in radians\n",
+                "alpha = 30. * u.deg\n",
                 "v_Earth_ini = np.sqrt(G*M_sun/M_earth*mu/AU)\n",
                 "v_Earth_ini = np.array([-np.sin(alpha)*v_Earth_ini, np.cos(alpha)*v_Earth_ini, 0.])\n",
                 "v_Sun_ini   = np.sqrt(G*M_earth/M_sun*mu/AU)\n",
                 "v_Sun_ini   = np.array([np.sin(alpha)*v_Sun_ini, -np.cos(alpha)*v_Sun_ini, 0.])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 31,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.r = r_Earth_ini\n",
                 "sim.Earth.v = v_Earth_ini\n",
                 "sim.Sun.r   = r_Sun_ini\n",
                 "sim.Sun.v   = v_Sun_ini"
@@ -417,22 +423,22 @@
             "metadata": {},
             "source": [
                 "**Starting**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 32,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Execution time: \u001b[94m0:00:01\u001b[0m\n"
+                        "Execution time: \u001b[94m0:00:03\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "sim.run()"
             ]
         },
@@ -441,24 +447,24 @@
             "metadata": {},
             "source": [
                 "**Reading and plotting**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 33,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data = sim.writer.read.all()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 34,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "\n",
@@ -478,24 +484,24 @@
                 "    ax.set_ylim(-1.5*AU, 1.5*AU)\n",
                 "    fig.tight_layout()\n",
                 "    plt.show()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 35,
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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\n",
                         "text/plain": [
-                            "<Figure size 900x600 with 1 Axes>"
+                            "<Figure size 960x720 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
@@ -511,33 +517,48 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "**Adding Temperature**\n",
                 "\n",
-                "To calculate the temperature Earth and Sun need additional fields for their temperatures and their radii. In additional to that, we give the Earth an additional field for the Earth-Sun distance.\n",
-                "\n",
+                "To calculate the temperature Earth and Sun need additional fields for their temperatures and their radii. In additional to that, we give the Earth an additional field for the Earth-Sun distance."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 36,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "R_Earth = c.R_earth.si.value\n",
+                "R_Sun   = c.R_sun.si.value"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "We initialize the Earth's temperature with zero and update it as soon as we have a function for it."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 37,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.addfield(\"d\", AU, description=\"Earth-Sun distance [m]\")\n",
-                "sim.Earth.addfield(\"R\", R_earth, description=\"Radius [m]\")\n",
+                "sim.Earth.addfield(\"R\", R_Earth, description=\"Radius [m]\")\n",
                 "sim.Earth.addfield(\"T\", 0., description=\"Temperature [K]\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 38,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Group\n",
                             "-----\n",
@@ -546,36 +567,36 @@
                             "    r            : Field (Position [m])\n",
                             "    R            : Field (Radius [m])\n",
                             "    T            : Field (Temperature [K])\n",
                             "    v            : Field (Velocity [m/s])\n",
                             "  -----"
                         ]
                     },
-                    "execution_count": 36,
+                    "execution_count": 38,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sim.Earth"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 39,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sim.Sun.addfield(\"R\", R_sun, description=\"Radius [m]\", constant=True)\n",
+                "sim.Sun.addfield(\"R\", R_Sun, description=\"Radius [m]\", constant=True)\n",
                 "sim.Sun.addfield(\"T\", 5778, description=\"Effective temperature [K]\", constant=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 40,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Group\n",
                             "-----\n",
@@ -583,15 +604,15 @@
                             "    r            : Field (Position [m])\n",
                             "    R            : Field (Radius [m]), \u001b[95mconstant\u001b[0m\n",
                             "    T            : Field (Effective temperature [K]), \u001b[95mconstant\u001b[0m\n",
                             "    v            : Field (Velocity [m/s])\n",
                             "  -----"
                         ]
                     },
-                    "execution_count": 38,
+                    "execution_count": 40,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sim.Sun"
             ]
@@ -603,15 +624,15 @@
                 "## Skipping Fields in Output Files\n",
                 "\n",
                 "It is possible to not write certain fields into the output. This can be especially useful if you have large fields, that consume a significant amount of memory, that you don't need for your data analysis. Simply the the `save` attribute to `False`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": 41,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Sun.T.save = False"
             ]
         },
         {
@@ -646,24 +667,24 @@
                 "$T = T_\\mathrm{eff} \\sqrt[4]{\\frac{R_\\odot^2}{4d^2}}$.\n",
                 "\n",
                 "So the equilibrium temperature on Earth depends on the Sun's effective temperature $T_\\mathrm{eff}$, the Sun's radius $R_\\odot$, and the Earth-Sun distance $d$. We can now write a function that takes the frame object as argument and returns Earth's temperature."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": 42,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sigma_sb = sigma_sb"
+                "sigma_sb = c.sigma_sb.si.value"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": 43,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def T(frame):\n",
                 "    return frame.Sun.T * (frame.Sun.R**2 / (4.*frame.Earth.d**2))**0.25"
             ]
         },
@@ -672,15 +693,15 @@
             "metadata": {},
             "source": [
                 "We can now assign this function to the updater of the temperature field"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 42,
+            "execution_count": 44,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.T.updater = T"
             ]
         },
         {
@@ -688,25 +709,25 @@
             "metadata": {},
             "source": [
                 "The function for calculating the Earth-Sun distance is pretty simple and can be simply assigned to the updater of the field."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 45,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def d(sim):\n",
                 "    return np.linalg.norm(sim.Earth.r - sim.Sun.r)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": 46,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.d.updater = d"
             ]
         },
         {
@@ -714,24 +735,24 @@
             "metadata": {},
             "source": [
                 "Right now the temperature is zero as we initialized it."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": 47,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.0"
                         ]
                     },
-                    "execution_count": 45,
+                    "execution_count": 47,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sim.Earth.T"
             ]
@@ -741,33 +762,33 @@
             "metadata": {},
             "source": [
                 "We can now use our the updater of the temperature field to calculate it's initial value"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 46,
+            "execution_count": 48,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.T.update()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
+            "execution_count": 49,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "278.6190681198289"
                         ]
                     },
-                    "execution_count": 47,
+                    "execution_count": 49,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sim.Earth.T"
             ]
@@ -783,25 +804,25 @@
                 "The only update operation that is performed once per time step is the update of the frame object `Frame.update()`. From here we have to delegate tasks down the tree structure.\n",
                 "\n",
                 "There are in principle two methods of updating groups. One is by writing a function and assigning it to the group's updater. Here we write a function that is calling Earth's updater and assign it to theupdater of the frame."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 48,
+            "execution_count": 50,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def update_Earth(frame):\n",
                 "    frame.Earth.update()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 49,
+            "execution_count": 51,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.updater = update_Earth"
             ]
         },
         {
@@ -809,15 +830,15 @@
             "metadata": {},
             "source": [
                 "The second method is by assigning a list of group attributes to an updater. The updater is then calling the updaters of these attributes in exactly that order."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 50,
+            "execution_count": 52,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.updater = [\"d\", \"T\"]    # Earth-Sun distance first, then temperature"
             ]
         },
         {
@@ -825,24 +846,24 @@
             "metadata": {},
             "source": [
                 "If the updater of a group has been set with a list, the order can be displayed. The attribute will return `None`, if no updater is set or if the updater was set with a function."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 51,
+            "execution_count": 53,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['d', 'T']"
                         ]
                     },
-                    "execution_count": 51,
+                    "execution_count": 53,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sim.Earth.updateorder"
             ]
@@ -854,36 +875,36 @@
                 "**Resetting to initial conditions**\n",
                 "\n",
                 "We can now reset to the initial conditions we have saved earlier, reset the namespace writer, and run the simulation again."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 52,
+            "execution_count": 54,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.r = r_Earth_ini\n",
                 "sim.Earth.v = v_Earth_ini\n",
                 "sim.Sun.r   = r_Sun_ini\n",
                 "sim.Sun.v   = v_Sun_ini\n",
                 "sim.t       = 0.\n",
                 "sim.writer.reset()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 53,
+            "execution_count": 55,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Execution time: \u001b[94m0:00:01\u001b[0m\n"
+                        "Execution time: \u001b[94m0:00:03\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "sim.run()"
             ]
         },
@@ -892,32 +913,32 @@
             "metadata": {},
             "source": [
                 "**Reading and plotting**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 54,
+            "execution_count": 56,
             "metadata": {},
             "outputs": [],
             "source": [
                 "data_T = sim.writer.read.all()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 55,
+            "execution_count": 57,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "def plot_temperature(data):\n",
                 "    fig, ax = plt.subplots(dpi=150)\n",
-                "    ax.plot(data.t/year, data.Earth.T-273.15, c=\"C3\", label=\"Temperature\")\n",
+                "    ax.plot(data.t/year, (data.Earth.T*u.K).to(u.Celsius, equivalencies=u.temperature()), c=\"C3\", label=\"Temperature\")\n",
                 "    ax.plot(-2., 0., label=\"Earth-Sun distance\", c=\"C0\")\n",
                 "    ax.set_xlabel(\"Time [years]\")\n",
                 "    ax.set_ylabel(\"Temperature [\u00b0C]\")\n",
                 "    ax.set_xlim(data.t[0]/year, data.t[-1]/year)\n",
                 "    ax.set_ylim(-100., 150.)\n",
                 "    axr = ax.twinx()\n",
                 "    axr.plot(data.t/year, data.Earth.d/AU, c=\"C0\")\n",
@@ -926,29 +947,27 @@
                 "    ax.legend()\n",
                 "    fig.tight_layout()\n",
                 "    plt.show()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 56,
+            "execution_count": 58,
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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\n",
                         "text/plain": [
-                            "<Figure size 900x600 with 2 Axes>"
+                            "<Figure size 960x720 with 2 Axes>"
                         ]
                     },
-                    "metadata": {
-                        "needs_background": "light"
-                    },
+                    "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "plot_temperature(data_T)"
             ]
         },
@@ -961,26 +980,26 @@
                 "Every updater is actually performing three operations. The updater operation itself, a **\"systole\"**, that is executed before the update operation and a **\"diastole\"** that is executed after the update operation.\n",
                 "\n",
                 "In this simple case we want to print Earth's temperature before and after it's calculation."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 57,
+            "execution_count": 59,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def T_sys(frame):\n",
                 "    msg = \"{:6s}: T = {:5.1f} K\".format(\"Before\", sim.Earth.T)\n",
                 "    print(msg)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 58,
+            "execution_count": 60,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def T_dia(frame):\n",
                 "    msg = \"{:6s}: T = {:5.1f} K\".format(\"After\", sim.Earth.T)\n",
                 "    print(msg)"
             ]
@@ -990,34 +1009,34 @@
             "metadata": {},
             "source": [
                 "We can assign these functions to systole and diastole of the temperature updater."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 59,
+            "execution_count": 61,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.T.updater.systole = T_sys\n",
                 "sim.Earth.T.updater.diastole = T_dia"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 60,
+            "execution_count": 62,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sim.Earth.T = 0."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 61,
+            "execution_count": 63,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Before: T =   0.0 K\n",
@@ -1035,27 +1054,27 @@
             "source": [
                 "Note: The updater of an integration variable is not directly setting its new value. Only the integrator is setting the new value of the integration variable after all integration instructions have been executed successfully. This has the consequence, that the diastole of an integration variable _DOES NOT_ have access to the updated value."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.8.11"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `simframe-1.0.2/examples/4_custom_schemes.ipynb` & `simframe-1.0.3rc0/examples/4_custom_schemes.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/examples/5_adaptive_schemes.ipynb` & `simframe-1.0.3rc0/examples/5_adaptive_schemes.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/examples/6_implicit_integration.ipynb` & `simframe-1.0.3rc0/examples/6_implicit_integration.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/examples/A_citation.ipynb` & `simframe-1.0.3rc0/examples/A_citation.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/examples/B_contrib_bug_feature.ipynb` & `simframe-1.0.3rc0/examples/B_contrib_bug_feature.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/examples/example_compartmental_models.ipynb` & `simframe-1.0.3rc0/examples/example_compartmental_models.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/examples/example_coupled_oscillators.ipynb` & `simframe-1.0.3rc0/examples/example_coupled_oscillators.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/examples/example_double_pendulum.ipynb` & `simframe-1.0.3rc0/examples/example_double_pendulum.ipynb`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/setup.py` & `simframe-1.0.3rc0/setup.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/frame/__init__.py` & `simframe-1.0.3rc0/simframe/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/frame/abstractgroup.py` & `simframe-1.0.3rc0/simframe/frame/abstractgroup.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/frame/field.py` & `simframe-1.0.3rc0/simframe/frame/field.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,31 @@
         return ret
 
     def __format__(self, format_spec):
         if self.shape == (1,):
             return self[0].__format__(format_spec)
         else:
             return super().__format__(format_spec)
+        
+    def __reduce__(self):
+        """
+        Custom ``__reduce__`` function that carries extra information about
+        custom attributes of ``Field`` class.
+        """
+        pickled_state = super(Field, self).__reduce__()
+        new_state = pickled_state[2] + (self.__dict__,)
+        return (pickled_state[0], pickled_state[1], new_state)
+
+    def __setstate__(self, state):
+        """
+        Custom ``__setstate__`` function that adds extra
+        custom attributes of ``Field`` class.
+        """
+        self.__dict__.update(state[-1])
+        super(Field, self).__setstate__(state[0:-1])
 
     @property
     def constant(self):
         '''If True, ``Field`` is immutable.'''
         return self._constant
 
     @constant.setter
```

### Comparing `simframe-1.0.2/simframe/frame/frame.py` & `simframe-1.0.3rc0/simframe/frame/frame.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/frame/group.py` & `simframe-1.0.3rc0/simframe/frame/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,36 +288,34 @@
 
 
 def _mem_tree(obj, prefix="", skip_hidden=True):
     ret = ""
     total = 0.0
     prefix = prefix + 4 * " "
     for key in sorted(obj.__dict__.keys(), key=str.casefold):
-        if key == '_owner':
+        if key == "_owner":
             continue
         if skip_hidden & key.startswith("_"):
             continue
         val = obj.__dict__[key]
         part1 = "{}- {}: ".format(prefix, colorize(key, "blue"))
         if isinstance(val, Group):
             part2, size = _mem_tree(val, prefix=prefix)
             ret += part1.ljust(56) + \
                 "total: " + byteformat(size) + "\n" + part2
-            #f'total {size:.2f} MiB'.rjust(16) + '\n' + part2
         else:
             if isinstance(val, _np.ndarray):
                 size = val.nbytes
                 shape = str(val.shape).rjust(17)
             else:
-                #size = _sys.getsizeof(val)
                 size = val.__sizeof__()
-                shape = ' ' * 17
+                shape = " " * 17
             s = byteformat(size)
             part2 = shape + " " + s
-            ret += (part1).ljust(45) + part2 + '\n'
+            ret += (part1).ljust(45) + part2 + "\n"
 
         s = byteformat(size)
         total += size
     return ret, total
 
 
 def _toc_tree(obj, prefix=""):
```

### Comparing `simframe-1.0.2/simframe/frame/heartbeat.py` & `simframe-1.0.3rc0/simframe/frame/heartbeat.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/frame/intvar.py` & `simframe-1.0.3rc0/simframe/frame/intvar.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/frame/updater.py` & `simframe-1.0.3rc0/simframe/frame/updater.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/__init__.py` & `simframe-1.0.3rc0/simframe/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/instruction.py` & `simframe-1.0.3rc0/simframe/integration/instruction.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/integrator.py` & `simframe-1.0.3rc0/simframe/integration/integrator.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/scheme.py` & `simframe-1.0.3rc0/simframe/integration/scheme.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/__init__.py` & `simframe-1.0.3rc0/simframe/integration/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_1_euler.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_1_euler.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_2_fehlberg_adptv.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_2_fehlberg_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_2_heun.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_2_heun.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_2_heun_euler_adptv.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_2_heun_euler_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_2_midpoint.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_2_midpoint.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_2_ralston.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_2_ralston.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_3_bogacki_shampine_adptv.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_3_bogacki_shampine_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_3_gottlieb_shu_adptv.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_3_gottlieb_shu_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_3_heun.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_3_heun.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_3_kutta.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_3_kutta.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_3_ralston.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_3_ralston.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_3_ssprk.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_3_ssprk.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_4_38rule.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_4_38rule.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_4_ralston.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_4_ralston.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_4_runge_kutta.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_4_runge_kutta.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_5_cash_karp_adptv.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_5_cash_karp_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/expl_5_dormand_prince_adptv.py` & `simframe-1.0.3rc0/simframe/integration/schemes/expl_5_dormand_prince_adptv.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/impl_1_euler_direct.py` & `simframe-1.0.3rc0/simframe/integration/schemes/impl_1_euler_direct.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/impl_1_euler_gmres.py` & `simframe-1.0.3rc0/simframe/integration/schemes/impl_1_euler_gmres.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/impl_2_midpoint_direct.py` & `simframe-1.0.3rc0/simframe/integration/schemes/impl_2_midpoint_direct.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/integration/schemes/update.py` & `simframe-1.0.3rc0/simframe/integration/schemes/update.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/io/__init__.py` & `simframe-1.0.3rc0/simframe/io/__init__.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/io/dump.py` & `simframe-1.0.3rc0/simframe/io/dump.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/io/progress.py` & `simframe-1.0.3rc0/simframe/io/progress.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/io/reader.py` & `simframe-1.0.3rc0/simframe/io/reader.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/io/writer.py` & `simframe-1.0.3rc0/simframe/io/writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,9 @@
-import dill
-import numpy as np
-import random
-import string
 import os
 
-from simframe.frame.field import Field
-from simframe.frame.intvar import IntVar
 from simframe.io.reader import Reader
 from simframe.io.dump import writedump
 from simframe.frame.abstractgroup import AbstractGroup
 from simframe.utils.color import colorize
 
 
 class Writer(object):
@@ -145,15 +139,14 @@
 
     @dumping.setter
     def dumping(self, value):
         if not isinstance(value, int):
             raise TypeError("<dumping> has to be of type bool.")
         if value:
             self._dumping = True
-            self._preparedump()
         else:
             self._dumping = False
 
     @property
     def verbosity(self):
         '''Verbosity of the writer.'''
         return self._verbosity
@@ -258,33 +251,14 @@
 
         if self.verbosity > 0:
             msg = "Writing dump file {}".format(colorize(filename, "blue"))
             print(msg)
 
         writedump(frame, filename)
 
-    def _preparedump(self):
-        """This function dumps a template ``<simframe.frame.Field>`` and ``<simframe.frame.IntVar>`` to file
-        and deletes the file directly afterwards. For some reason ``dill`` does not correctly save ``Field`` and ``IntVar``
-        correctly the first time. This function is called everytime ``<Writer.dumping>`` is set to ``True``
-        to make sure dumping works correctly when needed.
-
-        This is a "dirty fix". The reason why ``dill`` does not work correctly the first time is unknown.
-        """
-        while(True):
-            filename = "temp_" + "".join(random.choice(string.ascii_uppercase)
-                                         for i in range(5)) + ".dmp"
-            if not os.path.isfile(filename):    # pragma: no cover
-                break                           # Impossible to test due to randomness
-        temp = IntVar(None, 0., snapshots=[0.])
-        writedump(temp, filename)
-        temp = Field(None, 0.)
-        writedump(temp, filename)
-        os.remove(filename)
-
     def write(self, owner, i, forceoverwrite, filename=""):
         """Writes output to file
 
         Parameters
         ----------
         owner : Frame
             Parent ``Frame`` object
```

### Comparing `simframe-1.0.2/simframe/io/writers/hdf5writer.py` & `simframe-1.0.3rc0/simframe/io/writers/hdf5writer.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/io/writers/namespacewriter.py` & `simframe-1.0.3rc0/simframe/io/writers/namespacewriter.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/utils/color.py` & `simframe-1.0.3rc0/simframe/utils/color.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe/utils/format.py` & `simframe-1.0.3rc0/simframe/utils/format.py`

 * *Files identical despite different names*

### Comparing `simframe-1.0.2/simframe.egg-info/PKG-INFO` & `simframe-1.0.3rc0/simframe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: simframe
-Version: 1.0.2
+Version: 1.0.3rc0
 Summary: Framework for Scientific Simulations
 Home-page: https://github.com/stammler/simframe
 Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com, til.birnstiel@lmu.de
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/simframe/
 Project-URL: Documentation, https://simframe.readthedocs.io/
 Keywords: numerical,simulation,integration,science,mathematics,physics
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -25,19 +24,17 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simframe
 
-[![Documentation Status](https://readthedocs.org/projects/simframe/badge/?version=latest)](https://simframe.readthedocs.io/en/latest/?badge=latest) 
-![GitHub](https://img.shields.io/github/license/stammler/simframe) 
-[![status](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6/status.svg)](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6) 
-![PyPI - Downloads](https://img.shields.io/pypi/dm/simframe?label=PyPI%20downloads)
-[![Fedora package](https://img.shields.io/fedora/v/python3-simframe?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-simframe)
+[![Documentation Status](https://readthedocs.org/projects/simframe/badge/?version=latest)](https://simframe.readthedocs.io/en/latest/?badge=latest) [![GitHub](https://img.shields.io/github/license/stammler/simframe) ](https://github.com/stammler/simframe/blob/master/LICENSE) [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/stammler/simframe/blob/master/.github/CODE_OF_CONDUCT.md)  
+[![status](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6/status.svg)](https://joss.theoj.org/papers/0ef61e034c57445e846b2ec383c920a6)  
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/simframe?label=PyPI%20downloads)](https://pypistats.org/packages/simframe) [![Fedora package](https://img.shields.io/fedora/v/python3-simframe?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-simframe)
 
 ### Framework for scientific simulations
 
 `Simframe` is a Python framework to facilitate scientific simulations. The scope of the software is to provide a framework which can hold data fields, which can be used to integrate differential equations, and which can read and write data files.
 
 Data fields are stored in modified `numpy.ndarray`s. Therefore, `Simframe` can only work with data, that can be stored in `NumPy` arrays.
 
@@ -86,9 +83,7 @@
 ```
 
 ## Ackowledgements
 
 `simframe` has received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme under grant agreement No 714769.
 
 `simframe` was developed at the [University Observatory](https://www.usm.uni-muenchen.de/index_en.php) of the [Ludwig Maximilian University of Munich](https://www.en.uni-muenchen.de/index.html).
-
-
```

### Comparing `simframe-1.0.2/simframe.egg-info/SOURCES.txt` & `simframe-1.0.3rc0/simframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

