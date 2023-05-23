# Comparing `tmp/gadapt-0.2.5.tar.gz` & `tmp/gadapt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.5.tar", last modified: Tue May 23 23:09:29 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.6.tar", last modified: Tue May 23 23:31:02 2023, max compression
```

## Comparing `gadapt-0.2.5.tar` & `gadapt-0.2.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.323030 gadapt-0.2.5/
--rw-rw-rw-   0        0        0      339 2023-05-23 23:09:29.323530 gadapt-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-05-20 09:05:31.000000 gadapt-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.031028 gadapt-0.2.5/gadapt/
--rw-rw-rw-   0        0        0       77 2023-05-23 23:09:04.000000 gadapt-0.2.5/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.049529 gadapt-0.2.5/gadapt/cost_finding/
--rw-rw-rw-   0        0        0       26 2023-05-23 22:56:38.000000 gadapt-0.2.5/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      708 2023-05-21 09:37:48.000000 gadapt-0.2.5/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2078 2023-05-21 09:27:38.000000 gadapt-0.2.5/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.054528 gadapt-0.2.5/gadapt/crossover/
--rw-rw-rw-   0        0        0       23 2023-05-23 22:57:09.000000 gadapt-0.2.5/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     6984 2023-05-22 17:45:24.000000 gadapt-0.2.5/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1215 2023-05-22 17:43:24.000000 gadapt-0.2.5/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.057529 gadapt-0.2.5/gadapt/execution/
--rw-rw-rw-   0        0        0       23 2023-05-23 22:57:21.000000 gadapt-0.2.5/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3310 2023-05-22 17:43:16.000000 gadapt-0.2.5/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.072529 gadapt-0.2.5/gadapt/exit_check/
--rw-rw-rw-   0        0        0       24 2023-05-23 22:57:26.000000 gadapt-0.2.5/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      308 2023-05-21 09:27:27.000000 gadapt-0.2.5/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1047 2023-05-21 09:37:54.000000 gadapt-0.2.5/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      298 2023-05-21 09:27:27.000000 gadapt-0.2.5/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      380 2023-05-18 18:36:32.000000 gadapt-0.2.5/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.076529 gadapt-0.2.5/gadapt/factory/
--rw-rw-rw-   0        0        0       21 2023-05-23 22:57:38.000000 gadapt-0.2.5/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0    10019 2023-05-22 17:51:10.000000 gadapt-0.2.5/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0     7873 2023-05-22 18:10:31.000000 gadapt-0.2.5/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.079528 gadapt-0.2.5/gadapt/ga_logging/
--rw-rw-rw-   0        0        0       24 2023-05-23 22:57:44.000000 gadapt-0.2.5/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2116 2023-05-18 19:46:16.000000 gadapt-0.2.5/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.215030 gadapt-0.2.5/gadapt/ga_model/
--rw-rw-rw-   0        0        0       22 2023-05-23 22:57:51.000000 gadapt-0.2.5/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     6633 2023-05-22 17:39:59.000000 gadapt-0.2.5/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      683 2023-05-21 10:44:03.000000 gadapt-0.2.5/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     3711 2023-05-22 18:10:00.000000 gadapt-0.2.5/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     1416 2023-05-21 11:30:38.000000 gadapt-0.2.5/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1308 2023-05-21 09:38:09.000000 gadapt-0.2.5/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2533 2023-05-21 09:38:16.000000 gadapt-0.2.5/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.5/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    10309 2023-05-21 09:38:24.000000 gadapt-0.2.5/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      781 2023-05-22 13:25:31.000000 gadapt-0.2.5/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.221030 gadapt-0.2.5/gadapt/gene_combination/
--rw-rw-rw-   0        0        0       30 2023-05-23 22:59:40.000000 gadapt-0.2.5/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      281 2023-05-22 09:58:34.000000 gadapt-0.2.5/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0      823 2023-05-22 17:42:12.000000 gadapt-0.2.5/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.225030 gadapt-0.2.5/gadapt/parent_selection/
--rw-rw-rw-   0        0        0       30 2023-05-23 23:00:33.000000 gadapt-0.2.5/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      279 2023-05-21 09:39:14.000000 gadapt-0.2.5/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0      862 2023-05-18 07:22:58.000000 gadapt-0.2.5/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.305529 gadapt-0.2.5/gadapt/sampling/
--rw-rw-rw-   0        0        0       22 2023-05-23 23:00:40.000000 gadapt-0.2.5/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-21 09:39:18.000000 gadapt-0.2.5/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      419 2023-05-22 13:38:56.000000 gadapt-0.2.5/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      411 2023-05-22 13:28:32.000000 gadapt-0.2.5/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1798 2023-05-22 14:01:48.000000 gadapt-0.2.5/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2608 2023-05-22 12:50:02.000000 gadapt-0.2.5/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.308030 gadapt-0.2.5/gadapt/string_operation/
--rw-rw-rw-   0        0        0       30 2023-05-23 23:00:47.000000 gadapt-0.2.5/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3221 2023-05-21 11:30:07.000000 gadapt-0.2.5/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.314531 gadapt-0.2.5/gadapt/utils/
--rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.5/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0       19 2023-05-23 23:00:55.000000 gadapt-0.2.5/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-05-22 13:04:13.000000 gadapt-0.2.5/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.319032 gadapt-0.2.5/gadapt/validation/
--rw-rw-rw-   0        0        0       24 2023-05-23 23:01:01.000000 gadapt-0.2.5/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      758 2023-05-21 09:39:32.000000 gadapt-0.2.5/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    15392 2023-05-23 19:50:24.000000 gadapt-0.2.5/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.322530 gadapt-0.2.5/gadapt/variable_update/
--rw-rw-rw-   0        0        0       29 2023-05-23 23:01:09.000000 gadapt-0.2.5/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-21 09:36:51.000000 gadapt-0.2.5/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     1981 2023-05-08 05:52:39.000000 gadapt-0.2.5/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:09:29.045029 gadapt-0.2.5/gadapt.egg-info/
--rw-rw-rw-   0        0        0      339 2023-05-23 23:09:28.000000 gadapt-0.2.5/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2002 2023-05-23 23:09:28.000000 gadapt-0.2.5/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 23:09:28.000000 gadapt-0.2.5/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 23:09:28.000000 gadapt-0.2.5/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-23 23:09:29.325532 gadapt-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      433 2023-05-23 23:09:10.000000 gadapt-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.384334 gadapt-0.2.6/
+-rw-rw-rw-   0        0        0      339 2023-05-23 23:31:02.384833 gadapt-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-05-20 09:05:31.000000 gadapt-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.285333 gadapt-0.2.6/gadapt/
+-rw-rw-rw-   0        0        0       77 2023-05-23 23:30:15.000000 gadapt-0.2.6/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.298833 gadapt-0.2.6/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0       26 2023-05-23 22:56:38.000000 gadapt-0.2.6/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0      729 2023-05-23 23:17:08.000000 gadapt-0.2.6/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2099 2023-05-23 23:29:54.000000 gadapt-0.2.6/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.301833 gadapt-0.2.6/gadapt/crossover/
+-rw-rw-rw-   0        0        0       23 2023-05-23 22:57:09.000000 gadapt-0.2.6/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7054 2023-05-23 23:29:42.000000 gadapt-0.2.6/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1229 2023-05-23 23:14:52.000000 gadapt-0.2.6/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.304833 gadapt-0.2.6/gadapt/execution/
+-rw-rw-rw-   0        0        0       23 2023-05-23 22:57:21.000000 gadapt-0.2.6/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-05-23 23:29:11.000000 gadapt-0.2.6/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.318334 gadapt-0.2.6/gadapt/exit_check/
+-rw-rw-rw-   0        0        0       24 2023-05-23 22:57:26.000000 gadapt-0.2.6/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.6/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1061 2023-05-23 23:17:08.000000 gadapt-0.2.6/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.6/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.6/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.321333 gadapt-0.2.6/gadapt/factory/
+-rw-rw-rw-   0        0        0       21 2023-05-23 22:57:38.000000 gadapt-0.2.6/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0    10425 2023-05-23 23:28:33.000000 gadapt-0.2.6/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0     7964 2023-05-23 23:16:43.000000 gadapt-0.2.6/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.323835 gadapt-0.2.6/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0       24 2023-05-23 22:57:44.000000 gadapt-0.2.6/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2116 2023-05-18 19:46:16.000000 gadapt-0.2.6/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.345334 gadapt-0.2.6/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       22 2023-05-23 22:57:51.000000 gadapt-0.2.6/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     6696 2023-05-23 23:26:15.000000 gadapt-0.2.6/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      683 2023-05-21 10:44:03.000000 gadapt-0.2.6/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     3718 2023-05-23 23:14:52.000000 gadapt-0.2.6/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     1423 2023-05-23 23:26:32.000000 gadapt-0.2.6/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1336 2023-05-23 23:16:43.000000 gadapt-0.2.6/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2547 2023-05-23 23:16:43.000000 gadapt-0.2.6/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.6/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    10378 2023-05-23 23:25:30.000000 gadapt-0.2.6/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      802 2023-05-23 23:16:43.000000 gadapt-0.2.6/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.349834 gadapt-0.2.6/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0       30 2023-05-23 22:59:40.000000 gadapt-0.2.6/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-05-23 23:17:08.000000 gadapt-0.2.6/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.6/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.353334 gadapt-0.2.6/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0       30 2023-05-23 23:00:33.000000 gadapt-0.2.6/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      300 2023-05-23 23:17:08.000000 gadapt-0.2.6/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.6/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.361833 gadapt-0.2.6/gadapt/sampling/
+-rw-rw-rw-   0        0        0       22 2023-05-23 23:00:40.000000 gadapt-0.2.6/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      708 2023-05-23 23:17:08.000000 gadapt-0.2.6/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.6/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      418 2023-05-23 23:14:52.000000 gadapt-0.2.6/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1805 2023-05-23 23:14:52.000000 gadapt-0.2.6/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2615 2023-05-23 23:14:52.000000 gadapt-0.2.6/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.367335 gadapt-0.2.6/gadapt/string_operation/
+-rw-rw-rw-   0        0        0       30 2023-05-23 23:00:47.000000 gadapt-0.2.6/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3221 2023-05-21 11:30:07.000000 gadapt-0.2.6/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.371334 gadapt-0.2.6/gadapt/utils/
+-rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.6/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       19 2023-05-23 23:00:55.000000 gadapt-0.2.6/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1213 2023-05-23 23:15:55.000000 gadapt-0.2.6/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.376334 gadapt-0.2.6/gadapt/validation/
+-rw-rw-rw-   0        0        0       24 2023-05-23 23:01:01.000000 gadapt-0.2.6/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-05-23 23:17:08.000000 gadapt-0.2.6/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    15539 2023-05-23 23:17:43.000000 gadapt-0.2.6/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.383335 gadapt-0.2.6/gadapt/variable_update/
+-rw-rw-rw-   0        0        0       29 2023-05-23 23:01:09.000000 gadapt-0.2.6/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      177 2023-05-23 23:17:08.000000 gadapt-0.2.6/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     1988 2023-05-23 23:14:52.000000 gadapt-0.2.6/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:31:02.294336 gadapt-0.2.6/gadapt.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-23 23:31:02.000000 gadapt-0.2.6/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2002 2023-05-23 23:31:02.000000 gadapt-0.2.6/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 23:31:02.000000 gadapt-0.2.6/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 23:31:02.000000 gadapt-0.2.6/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-23 23:31:02.386333 gadapt-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      433 2023-05-23 23:30:04.000000 gadapt-0.2.6/setup.py
```

### Comparing `gadapt-0.2.5/gadapt/cost_finding/base_cost_finder.py` & `gadapt-0.2.6/gadapt/cost_finding/base_cost_finder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import traceback
 from typing import List
-from ga_model.chromosome import Chromosome
-import ga_model.definitions
+from gadapt.ga_model.chromosome import Chromosome
+import gadapt.ga_model.definitions
 
 class BaseCostFinder:
     def execute_function(self, cost_function, c: Chromosome):
         dict = {}
         for g in c:
             dict[g.genetic_variable.variable_id] = g.variable_value
         try:
@@ -15,8 +15,8 @@
         except Exception:
             print(Exception)
             traceback.print_exc()
             c.succ = False
             c.cost_value = sys.float_info.max
 
     def find_costs_for_chromosome(self, population):
-        raise Exception(ga_model.definitions.NOT_IMPLEMENTED)
+        raise Exception(gadapt.ga_model.definitions.NOT_IMPLEMENTED)
```

### Comparing `gadapt-0.2.5/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.6/gadapt/cost_finding/common_cost_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import math
 from typing import List
-from cost_finding.base_cost_finder import BaseCostFinder
-from ga_model.chromosome import Chromosome
-from ga_model.population import Population
+from gadapt.cost_finding.base_cost_finder import BaseCostFinder
+from gadapt.ga_model.chromosome import Chromosome
+from gadapt.ga_model.population import Population
 import utils.ga_utils
 
 class CommonCostFinder(BaseCostFinder):
     def find_costs_for_chromosome(self, population: Population):
         if (population is None):
             raise Exception("population must not be null!")
         chromosomes_for_execution: List[Chromosome] = [
```

### Comparing `gadapt-0.2.5/gadapt/crossover/base_crossover.py` & `gadapt-0.2.6/gadapt/crossover/base_crossover.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from ga_model.chromosome import Chromosome
-from ga_model.gene import Gene
-from immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
-from mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
-from gene_combination.base_gene_combination import BaseGeneCombination
-import utils.ga_utils
-import ga_model.definitions
+from gadapt.ga_model.chromosome import Chromosome
+from gadapt.ga_model.gene import Gene
+from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
+from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
+from gadapt.gene_combination.base_gene_combination import BaseGeneCombination
+import gadapt.utils.ga_utils
+import gadapt.ga_model.definitions
 
 class BaseCrossover:
     
     def __init__(self, gene_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator):
         self._mutation_on_both_sides = True
         self.gene_combination = gene_combination
         self.mutator = mutator
@@ -66,15 +66,15 @@
                 genetic_variable_mother = next((item.genetic_variable for item in mother if item.genetic_variable == self.genetic_variable), None)
             if (genetic_variable_mother is None):
                 raise Exception("chromosomes in crossover do not have the same structure!")
             genetic_diversity.append(get_genetic_diversity(mother_gene, father_gene))
             var1, var2 = self.combine(mother_gene, father_gene)
             offspring1.add_gene(self.genetic_variable_father, var1)
             offspring2.add_gene(self.genetic_variable_father, var2)
-        parrents_diversity = round(utils.ga_utils.average(genetic_diversity), 2)
+        parrents_diversity = round(gadapt.utils.ga_utils.average(genetic_diversity), 2)
         offspring1.parents_diversity = parrents_diversity
         offspring2.parents_diversity = parrents_diversity
         offspring1.mutation_on_both_sides = self.mutation_on_both_sides
         offspring2.mutation_on_both_sides = self.mutation_on_both_sides
         offspring1.mother_id = mother.chromosome_id
         offspring2.mother_id = mother.chromosome_id
         offspring1.father_id = father.chromosome_id
@@ -82,18 +82,18 @@
         self.increase_generation(offspring1, offspring2, mother, father)
         return offspring1, offspring2
     
     def mate_init(self):
         pass
 
     def get_mother_father_genes(self, mother: Chromosome, father: Chromosome):
-        raise Exception(ga_model.definitions.NOT_IMPLEMENTED)
+        raise Exception(gadapt.ga_model.definitions.NOT_IMPLEMENTED)
 
     def combine(self, mother_gene: Gene, father_gene: Gene):
-        raise Exception(ga_model.definitions.NOT_IMPLEMENTED)
+        raise Exception(gadapt.ga_model.definitions.NOT_IMPLEMENTED)
     
     def increase_generation(self, offspring1: Chromosome, offspring2: Chromosome, mother: Chromosome, father: Chromosome):
         current_generation = mother.chromosome_generation
         if current_generation == 0 or current_generation < father.chromosome_generation:
             current_generation = father.chromosome_generation
         current_generation += 1
         offspring1.chromosome_generation = current_generation
```

### Comparing `gadapt-0.2.5/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.6/gadapt/crossover/uniform_crossover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ga_model.chromosome import Chromosome
+from gadapt.ga_model.chromosome import Chromosome
 from crossover.base_crossover import BaseCrossover
-from ga_model.gene import Gene
+from gadapt.ga_model.gene import Gene
 from immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
 from mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 from gene_combination.base_gene_combination import BaseGeneCombination
 
 class UniformCrossover(BaseCrossover):
     
     def __init__(self, var_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator):
```

### Comparing `gadapt-0.2.5/gadapt/execution/ga_executor.py` & `gadapt-0.2.6/gadapt/execution/ga_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from factory.ga_factory import GAFactory
+from gadapt.factory.ga_factory import GAFactory
 from ga_logging.logging_settings import init_logging
-from ga_model.ga_options import GAOptions
-from ga_model.ga_results import GAResults
-from ga_model.population import Population
-import ga_model.message_levels
+from gadapt.ga_model.ga_options import GAOptions
+from gadapt.ga_model.ga_results import GAResults
+from gadapt.ga_model.population import Population
+import gadapt.ga_model.message_levels
 
 class GAExecutor:
     def __init__(self, ga_options: GAOptions, factory: GAFactory) -> None:
         if (not ga_options is None):
             self.ga_options = ga_options    
         self.factory = factory          
 
 
     def execute(self) -> GAResults:
         results = GAResults()
         try: 
             init_logging(self.ga_options.logging)                           
         except Exception as ex:
-            results.messages.append((ga_model.message_levels.WARNING, "Logging failed. Error message: {exc}".format(exc=str(ex))))
+            results.messages.append((gadapt.ga_model.message_levels.WARNING, "Logging failed. Error message: {exc}".format(exc=str(ex))))
             self.ga_options.logging = False
         validator = self.factory.get_options_validator()
         validator.validate()
         if not validator.success:
             results.success = False
             results.messages = validator.validation_messages
             return results
@@ -50,18 +50,18 @@
         population.find_costs()
         while not population.exit():
             population.immigrate()
             population.mate()
             population.mutate()
             population.find_costs()            
         if population.timeout_expired:
-            results.messages.append((ga_model.message_levels.WARNING, "Timeout expired!"))
+            results.messages.append((gadapt.ga_model.message_levels.WARNING, "Timeout expired!"))
         best_individual = population.best_individual
         results.min_cost = population.min_cost
         results.number_of_iterations = population.population_generation
         for g in best_individual:
             results.result_values[g.genetic_variable.variable_id] = g.variable_value
         #except Exception as ex:
         #    results.success = False
-        #    results.messages.append((ga_model.message_levels.ERROR, str(ex)))
+        #    results.messages.append((gadapt.ga_model.message_levels.ERROR, str(ex)))
         return results
```

### Comparing `gadapt-0.2.5/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.6/gadapt/exit_check/base_exit_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from datetime import datetime
-import ga_model.definitions
+import gadapt.ga_model.definitions
 
 class BaseExitChecker:
     def __init__(self, max_attempt_no: int) -> None:
         self.max_attempt_no = max_attempt_no
         self.attempt_no = 0              
     
     @property
@@ -26,8 +26,8 @@
             self.attempt_no = 0
         if self.attempt_no >= self.max_attempt_no:
             logging.info("function exit.")
             return True
         return False
     
     def is_exit(self, population) -> bool:
-        raise Exception(ga_model.definitions.NOT_IMPLEMENTED)
+        raise Exception(gadapt.ga_model.definitions.NOT_IMPLEMENTED)
```

### Comparing `gadapt-0.2.5/gadapt/ga.py` & `gadapt-0.2.6/gadapt/ga.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import sys
-from execution.ga_executor import GAExecutor
-from factory.ga_factory import GAFactory
-from ga_model.genetic_variable import GeneticVariable
-from ga_model.ga_options import GAOptions
-from ga_model.ga_results import GAResults
-from ga_model.population import Population
+from gadapt.execution.ga_executor import GAExecutor
+from gadapt.factory.ga_factory import GAFactory
+from gadapt.ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.ga_options import GAOptions
+from gadapt.ga_model.ga_results import GAResults
+from gadapt.ga_model.population import Population
 import utils.ga_utils
-import ga_model.definitions
+import gadapt.ga_model.definitions
 
 class GA:
     def __init__(self,
                  cost_function = None,
                  population_size = 64, 
-                 exit_check = ga_model.definitions.AVG_COST,
+                 exit_check = gadapt.ga_model.definitions.AVG_COST,
                  requested_cost = sys.float_info.max,
                  max_attempt_no = 10,
-                 parent_selection = ga_model.definitions.ROULETTE_WHEEL,
-                 population_mutation = ga_model.definitions.COST_DIVERSITY, 
+                 parent_selection = gadapt.ga_model.definitions.ROULETTE_WHEEL,
+                 population_mutation = gadapt.ga_model.definitions.COST_DIVERSITY, 
                  number_of_mutation_chromosomes = 1,    
-                 parent_diversity_mutation_chromosome_selection = ga_model.definitions.ROULETTE_WHEEL, 
+                 parent_diversity_mutation_chromosome_selection = gadapt.ga_model.definitions.ROULETTE_WHEEL, 
                  must_mutate_for_same_parents = True,
-                 chromosome_mutation = ga_model.definitions.CROSS_DIVERSITY,                                        
+                 chromosome_mutation = gadapt.ga_model.definitions.CROSS_DIVERSITY,                                        
                  number_of_mutation_genes = 1,                     
-                 cross_diversity_mutation_gene_selection = ga_model.definitions.ROULETTE_WHEEL,
+                 cross_diversity_mutation_gene_selection = gadapt.ga_model.definitions.ROULETTE_WHEEL,
                  immigration_number = 0,                                                                                   
                  logging = False,                                                              
                  timeout = 120
                  ) -> None:                     
         self.cost_function = cost_function
         self.population_size = population_size
         self.exit_check = exit_check
```

### Comparing `gadapt-0.2.5/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.6/gadapt/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.5/gadapt/ga_model/chromosome.py` & `gadapt-0.2.6/gadapt/ga_model/chromosome.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List
-from ga_model.gene import Gene
-from ga_model.genetic_variable import GeneticVariable
-from ga_model.ranking_model import RankingModel
-from immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
-from mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
-import string_operation.ga_strings
-import ga_model.definitions
+from gadapt.ga_model.gene import Gene
+from gadapt.ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.ranking_model import RankingModel
+from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
+from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
+import gadapt.string_operation.ga_strings
+import gadapt.ga_model.definitions
 class Chromosome (RankingModel):
     
     def __init__(self, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator, population_generation: int):
         super().__init__()
         self._mutator = mutator
         self._immigrator = immigrator
-        self.cost_value = ga_model.definitions.FLOAT_NAN
+        self.cost_value = gadapt.ga_model.definitions.FLOAT_NAN
         self._is_immigrant = False
         self.population_generation = population_generation
         self._chromosome_id = None
         self._mutated_variables_id_list = []
         self.first_mutant_generation = 0
         self.first_immigrant_generation = 0
         self.last_mutant_generation = 0
@@ -129,15 +129,15 @@
     def father_id(self) -> int:
         return self._father_id
     
     @father_id.setter
     def father_id(self, value: int):
         self._father_id = value
 
-    def add_gene(self, gen_var: GeneticVariable, gen_var_value: float = ga_model.definitions.FLOAT_NAN):
+    def add_gene(self, gen_var: GeneticVariable, gen_var_value: float = gadapt.ga_model.definitions.FLOAT_NAN):
         g = Gene(gen_var, gen_var_value)
         self.append(g)
 
     @property
     def parents_diversity(self) -> float:
         return self._parents_diversity
```

### Comparing `gadapt-0.2.5/gadapt/ga_model/definitions.py` & `gadapt-0.2.6/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.5/gadapt/ga_model/ga_options.py` & `gadapt-0.2.6/gadapt/ga_model/ga_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from typing import List
-from ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.genetic_variable import GeneticVariable
 class GAOptions():
    
     def __init__(self, ga) -> None:
         super().__init__()           
         self._population_size = ga.population_size
         self._cost_function = ga.cost_function
         if ga._number_of_mutation_chromosomes_changed:
```

### Comparing `gadapt-0.2.5/gadapt/ga_model/ga_results.py` & `gadapt-0.2.6/gadapt/ga_model/ga_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-import string_operation.ga_strings as ga_strings
+import gadapt.string_operation.ga_strings as ga_strings
 
 class GAResults:
     def __init__(self) -> None:
         self._success = True
         self.result_values = {}
         self._messages = []
```

### Comparing `gadapt-0.2.5/gadapt/ga_model/gene.py` & `gadapt-0.2.6/gadapt/ga_model/gene.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import math
-from ga_model.genetic_variable import GeneticVariable
-from ga_model.ranking_model import RankingModel
+from gadapt.ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.ranking_model import RankingModel
 import string_operation.ga_strings
-import ga_model.definitions
+import gadapt.ga_model.definitions
 class Gene(RankingModel):
 
     def __init__(self, gen_variable, var_value = None):
         super().__init__()
         self.genetic_variable = gen_variable        
         self.variable_value = var_value
         self._rank = -1
-        self._cummulative_probability = ga_model.definitions.FLOAT_NAN
+        self._cummulative_probability = gadapt.ga_model.definitions.FLOAT_NAN
         if (self.variable_value == None or math.isnan(self.variable_value)):
             self.set_random_value()
 
     def __str__(self) -> str:
         return self.to_string()
     
     def to_string(self):
```

### Comparing `gadapt-0.2.5/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.6/gadapt/ga_model/genetic_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
-import ga_model.definitions
+import gadapt.ga_model.definitions
 class GeneticVariable:
 
     def __init__(self, id: int) -> None:
         self.variable_id = id
-        self._standard_deviation = ga_model.definitions.FLOAT_NAN
+        self._standard_deviation = gadapt.ga_model.definitions.FLOAT_NAN
     
     def __eq__(self, other):
         if not isinstance(other, GeneticVariable):
             return False
         return self.variable_id == other.variable_id
     
     def __hash__(self) -> int:
```

### Comparing `gadapt-0.2.5/gadapt/ga_model/population.py` & `gadapt-0.2.6/gadapt/ga_model/population.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from selectors import BaseSelector
 from typing import List, Tuple
-from exit_check.base_exit_checker import BaseExitChecker
-from cost_finding.base_cost_finder import BaseCostFinder
-from crossover.base_crossover import BaseCrossover
-from ga_model.chromosome import Chromosome
-from ga_model.ga_options import GAOptions
-from ga_model.gene import Gene
-from ga_model.genetic_variable import GeneticVariable
-from immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
-from immigration.population_immigration.base_population_immigrator import BasePopulationImmigrator
-from mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
-from mutation.population_mutation.base_population_mutator import BasePopulationMutator
-from mutation.population_mutation.composed_population_mutator import ComposedPopulationMutator
+from gadapt.exit_check.base_exit_checker import BaseExitChecker
+from gadapt.cost_finding.base_cost_finder import BaseCostFinder
+from gadapt.crossover.base_crossover import BaseCrossover
+from gadapt.ga_model.chromosome import Chromosome
+from gadapt.ga_model.ga_options import GAOptions
+from gadapt.ga_model.gene import Gene
+from gadapt.ga_model.genetic_variable import GeneticVariable
+from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
+from gadapt.immigration.population_immigration.base_population_immigrator import BasePopulationImmigrator
+from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
+from gadapt.mutation.population_mutation.base_population_mutator import BasePopulationMutator
+from gadapt.mutation.population_mutation.composed_population_mutator import ComposedPopulationMutator
 from sklearn.preprocessing import MinMaxScaler
-from variable_update.base_variable_updater import BaseVariableUpdater
-import string_operation.ga_strings
+from gadapt.variable_update.base_variable_updater import BaseVariableUpdater
+import gadapt.string_operation.ga_strings
 from datetime import datetime
-import ga_model.definitions
+import gadapt.ga_model.definitions
 
 class Population:
 
     def __init__(self, options: GAOptions,
                  chromosome_mutator: BaseChromosomeMutator,
                  population_mutator: BasePopulationMutator,
                  exit_checker: BaseExitChecker,
                  cost_finder: BaseCostFinder,
                  population_immigrator: BasePopulationImmigrator,
                  chromosome_immigrator: BaseChromosomeImmigrator,
-                 selector: BaseSelector,
+                 selector,
                  crossover: BaseCrossover,
                  variable_updater: BaseVariableUpdater):
         if options.population_size < 4:
             raise Exception("Population size 4 must be higher than 3")        
         self.scaler = MinMaxScaler(feature_range=(1, 2))
         self.options = options
         self.chromosome_mutator = chromosome_mutator
@@ -71,18 +70,18 @@
         self.chromosomes.append(c)
 
     def generate_initial_population(self):
         for i in range(self.options.population_size):
             self.add_new_chromosome()
 
     def to_string(self):
-        return string_operation.ga_strings.population_to_string(self)
+        return gadapt.string_operation.ga_strings.population_to_string(self)
 
     def set_init_values(self):
-        float_init_value = ga_model.definitions.FLOAT_NAN
+        float_init_value = gadapt.ga_model.definitions.FLOAT_NAN
         self.avg_cost = float_init_value
         self.previous_avg_cost = float_init_value
         self.min_cost = float_init_value
         self.previous_min_cost = float_init_value
         self.first_cost = float_init_value
 
     @property
```

### Comparing `gadapt-0.2.5/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.6/gadapt/ga_model/ranking_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import ga_model.definitions
+import gadapt.ga_model.definitions
 class RankingModel:
     def __init__(self):
         self._rank = -1
-        self._cummulative_probability = ga_model.definitions.FLOAT_NAN
+        self._cummulative_probability = gadapt.ga_model.definitions.FLOAT_NAN
     
     @property
     def rank(self):
         return self._rank
     
     @rank.setter
     def rank(self, value):
@@ -22,8 +22,8 @@
 
     def replace_rank(self, rank):
         self.rank = rank
         return self
 
     def reset_for_sampling(self):
         self._rank = -1
-        self._cummulative_probability = ga_model.definitions.FLOAT_NAN
+        self._cummulative_probability = gadapt.ga_model.definitions.FLOAT_NAN
```

### Comparing `gadapt-0.2.5/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.6/gadapt/gene_combination/blending_gene_combination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
-from ga_model.gene import Gene
-from gene_combination.base_gene_combination import BaseGeneCombination
+from gadapt.ga_model.gene import Gene
+from gadapt.gene_combination.base_gene_combination import BaseGeneCombination
 
 class BlendingGeneCombination(BaseGeneCombination):
     def combine(self, mother_gene: Gene, father_gene: Gene):
         genetic_variable = father_gene.genetic_variable
         val_father = father_gene.variable_value
         val_mother = mother_gene.variable_value
         x = 1
```

### Comparing `gadapt-0.2.5/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.6/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Tuple
-from ga_model.chromosome import Chromosome
-from parent_selection.base_parent_selector import BaseParentSelector
-from sampling.base_sampling import BaseSampling
+from gadapt.ga_model.chromosome import Chromosome
+from gadapt.parent_selection.base_parent_selector import BaseParentSelector
+from gadapt.sampling.base_sampling import BaseSampling
 
 
 class SamplingParentSelector(BaseParentSelector):
 
     def __init__(self, sampling: BaseSampling) -> None:
         super().__init__()
         self.sampling = sampling
```

### Comparing `gadapt-0.2.5/gadapt/sampling/base_sampling.py` & `gadapt-0.2.6/gadapt/sampling/base_sampling.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List
-from ga_model.ranking_model import RankingModel
-import ga_model.definitions
+from gadapt.ga_model.ranking_model import RankingModel
+import gadapt.ga_model.definitions
 class BaseSampling:
     def get_sample(self, lst: List[RankingModel], max_num, sort_key=None) -> List[RankingModel]:
         if len(lst) == 0:
             return lst
         for m in lst:
             m.reset_for_sampling()
         if max_num < 1 or max_num > len(lst):
             self.max_num = len(lst)
         else:
             self.max_num = max_num
         self.sort_key = sort_key
         return self.prepare_sample(lst)
     
     def prepare_sample(self, lst: List[RankingModel]) -> List[RankingModel]:
-        raise Exception(ga_model.definitions.NOT_IMPLEMENTED)
+        raise Exception(gadapt.ga_model.definitions.NOT_IMPLEMENTED)
```

### Comparing `gadapt-0.2.5/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.6/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 from typing import List
-from ga_model.ranking_model import RankingModel
+from gadapt.ga_model.ranking_model import RankingModel
 from sampling.base_sampling import BaseSampling
 
 class RouletteWheelSampling(BaseSampling):
     
     def prepare_sample(self, lst: List[RankingModel]) -> List[RankingModel]:
         rank_sum = sum(range(1, len(lst) + 1))
         cummultative_probability_list: List[float] = []
```

### Comparing `gadapt-0.2.5/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.6/gadapt/sampling/tournament_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 from typing import List
-from ga_model.ranking_model import RankingModel
+from gadapt.ga_model.ranking_model import RankingModel
 from sampling.base_sampling import BaseSampling
 
 class TournamentSampling(BaseSampling):
     def __init__(self, group_size = None) -> None:
         super().__init__()
         self.group_size = group_size
```

### Comparing `gadapt-0.2.5/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.6/gadapt/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.5/gadapt/utils/ga_utils.py` & `gadapt-0.2.6/gadapt/utils/ga_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from functools import reduce
 import math
 import random
 from typing import List
-import ga_model.definitions
+import gadapt.ga_model.definitions
 def get_rand_bool():
     rand_int = random.getrandbits(1)
     return bool(rand_int)
 
 def get_rand_bool_with_probability(f: float):
     r = random.uniform(0, 1)
     if r <= f:
```

### Comparing `gadapt-0.2.5/gadapt/validation/base_options_validator.py` & `gadapt-0.2.6/gadapt/validation/base_options_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import List, Tuple
-import ga_model.message_levels
-import ga_model.definitions
+import gadapt.ga_model.message_levels
+import gadapt.ga_model.definitions
 
 class BaseOptionsValidator:
     
     def __init__(self, options) -> None:
         self._validation_messages = []
         self.options = options
         self.success = True
     
     def validate(self) -> bool:
-        raise Exception(ga_model.definitions.NOT_IMPLEMENTED)
+        raise Exception(gadapt.ga_model.definitions.NOT_IMPLEMENTED)
     
     @property
     def validation_messages(self):
         return self._validation_messages
     
     @validation_messages.setter
     def validation_messages(self, value):
         self._validation_messages = value
 
-    def add_message(self, message, message_level = ga_model.message_levels.ERROR):
+    def add_message(self, message, message_level = gadapt.ga_model.message_levels.ERROR):
         self.validation_messages.append((message_level, message))
```

### Comparing `gadapt-0.2.5/gadapt/validation/common_options_validator.py` & `gadapt-0.2.6/gadapt/validation/common_options_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from validation.base_options_validator import BaseOptionsValidator
-import ga_model.definitions
-import ga_model.definitions
+from gadapt.validation.base_options_validator import BaseOptionsValidator
+import gadapt.ga_model.definitions
+import gadapt.ga_model.definitions
 class CommonOptionsValidator(BaseOptionsValidator):
 
     def __init__(self, options) -> None:
         super().__init__(options)
         self._validation_messages = []        
 
     def validate(self):        
@@ -130,27 +130,27 @@
             rslt &= False                                                           
         if self.options.chromosome_mutation is None:
             self.add_message("Chromosome Mutation must not be None!")
             rslt &= False
         elif not isinstance(self.options.chromosome_mutation, str):
             self.add_message("Chromosome Mutation must be type str!")
             rslt &= False  
-        elif  self.options.chromosome_mutation not in ga_model.definitions.CHROMOSOME_MUTATOR_STRINGS:
-            self.add_message("Invalid value of Chromosome Mutation: {0}. Allowed values: {1}".format(self.options.chromosome_mutation, self.get_allowed_values(ga_model.definitions.CHROMOSOME_MUTATOR_STRINGS)))
+        elif  self.options.chromosome_mutation not in gadapt.ga_model.definitions.CHROMOSOME_MUTATOR_STRINGS:
+            self.add_message("Invalid value of Chromosome Mutation: {0}. Allowed values: {1}".format(self.options.chromosome_mutation, self.get_allowed_values(gadapt.ga_model.definitions.CHROMOSOME_MUTATOR_STRINGS)))
             rslt &= False   
         if self.options.exit_check is None:
             self.add_message("Exit Check must not be None!")
             rslt &= False
         elif not isinstance(self.options.exit_check, str):
             self.add_message("Exit Check must be type str!")
             rslt &= False
-        elif self.options.exit_check not in ga_model.definitions.EXIT_CRITERIA_STRINGS:
-            self.add_message("Invalid value of Exit Check: {0}. Allowed values: {1}".format(self.options.exit_check, self.get_allowed_values(ga_model.definitions.EXIT_CRITERIA_STRINGS)))
+        elif self.options.exit_check not in gadapt.ga_model.definitions.EXIT_CRITERIA_STRINGS:
+            self.add_message("Invalid value of Exit Check: {0}. Allowed values: {1}".format(self.options.exit_check, self.get_allowed_values(gadapt.ga_model.definitions.EXIT_CRITERIA_STRINGS)))
             rslt &= False
-        if self.options.chromosome_mutation == ga_model.definitions.CROSS_DIVERSITY:
+        if self.options.chromosome_mutation == gadapt.ga_model.definitions.CROSS_DIVERSITY:
             if self.options.cross_diversity_mutation_gene_selection is None:
                 self.add_message("Cross Diversity Mutation Gene Selection must not be None!")
                 rslt &= False
             elif not isinstance(self.options.cross_diversity_mutation_gene_selection, str):
                 self.add_message("Cross Diversity Mutation Gene Selection must be type str!")
                 rslt &= False
             elif not self.validate_selection(self.options.cross_diversity_mutation_gene_selection, "Cross Diversity Mutation Gene Selection", self.options.number_of_mutation_genes, "Group Size for Cross Diversity Mutation Gene Selection must be below or equal than the number of mutation variables!"):
@@ -163,37 +163,37 @@
             rslt &= False        
         if self.options.must_mutate_for_same_parents is None:
             self.add_message("Must Mutate For Same Parents must not be None!")
             rslt &= False
         elif not isinstance(self.options.must_mutate_for_same_parents, bool):
             self.add_message("Must Mutate For Same Parents must be type bool!")
             rslt &= False 
-        if self.options.population_mutation == ga_model.definitions.COST_DIVERSITY or ga_model.definitions.PARENTS_DIVERSITY in self.options.population_mutation:
+        if self.options.population_mutation == gadapt.ga_model.definitions.COST_DIVERSITY or gadapt.ga_model.definitions.PARENTS_DIVERSITY in self.options.population_mutation:
             if self.options.parent_diversity_mutation_chromosome_selection is None:
                 self.add_message("Parent Diversity Mutation Chromosome Selection must not be None!")
                 rslt &= False
             elif not isinstance(self.options.parent_diversity_mutation_chromosome_selection, str):
                 self.add_message("Parent Diversity Mutation Chromosome Selection must be type str!")
                 rslt &= False
             elif not self.validate_selection(self.options.parent_diversity_mutation_chromosome_selection, "Parents Diversity Mutation Chromosome Selection", (population_size // 2) - self.options.immigration_number, "Group Size for Parents Diversity Mutation Chromosome Selection cannot have the value below half population!"):
                 rslt &= False 
         if self.options.population_mutation is None:
             self.add_message("Population Mutation must not be None!")
             rslt &= False
         elif not isinstance(self.options.population_mutation, str):
             self.add_message("Population Mutation must be type str!")
             rslt &= False
-        elif ga_model.definitions.PARAM_SEPARATOR in self.options.population_mutation:
-            mutator_strings = [ms.strip() for ms in self.options.population_mutation.split(ga_model.definitions.PARAM_SEPARATOR)]
+        elif gadapt.ga_model.definitions.PARAM_SEPARATOR in self.options.population_mutation:
+            mutator_strings = [ms.strip() for ms in self.options.population_mutation.split(gadapt.ga_model.definitions.PARAM_SEPARATOR)]
             for mutator_string in mutator_strings:
-                if mutator_string not in ga_model.definitions.POPULATION_MUTATOR_STRINGS:
-                    self.add_message("Invalid value of Population Mutation: {0}. Allowed values: {1}".format(mutator_string, self.get_allowed_values(ga_model.definitions.POPULATION_MUTATOR_STRINGS)))
+                if mutator_string not in gadapt.ga_model.definitions.POPULATION_MUTATOR_STRINGS:
+                    self.add_message("Invalid value of Population Mutation: {0}. Allowed values: {1}".format(mutator_string, self.get_allowed_values(gadapt.ga_model.definitions.POPULATION_MUTATOR_STRINGS)))
                     rslt &= False
-        elif self.options.population_mutation not in ga_model.definitions.POPULATION_MUTATOR_STRINGS:
-            self.add_message("Invalid value of Population Mutation: {0}. Allowed values: {1}".format(self.options.population_mutation, self.get_allowed_values(ga_model.definitions.POPULATION_MUTATOR_STRINGS)))
+        elif self.options.population_mutation not in gadapt.ga_model.definitions.POPULATION_MUTATOR_STRINGS:
+            self.add_message("Invalid value of Population Mutation: {0}. Allowed values: {1}".format(self.options.population_mutation, self.get_allowed_values(gadapt.ga_model.definitions.POPULATION_MUTATOR_STRINGS)))
             rslt &= False
         if self.options.parent_selection is None:
             self.add_message("Parent Selection must not be None!")
             rslt &= False
         elif not isinstance(self.options.parent_selection, str):
             self.add_message("Parent Selection must be type str!")
             rslt &= False
@@ -213,19 +213,19 @@
             rslt &= False
         elif self.options.timeout < 1:
             self.add_message("Invalid timeout value: {0}".format(str(self.options.timeout)))
             rslt &= False
         return rslt
     
     def validate_selection(self, selection_string, selection_type, comparing_number, group_size_error_message) -> bool:
-        selection_strings = selection_string.split(ga_model.definitions.PARAM_SEPARATOR)
-        if len(selection_strings) > 2 or (len(selection_strings) > 1 and selection_strings[0] != ga_model.definitions.TOURNAMENT):
+        selection_strings = selection_string.split(gadapt.ga_model.definitions.PARAM_SEPARATOR)
+        if len(selection_strings) > 2 or (len(selection_strings) > 1 and selection_strings[0] != gadapt.ga_model.definitions.TOURNAMENT):
             self.add_message("Invalid {0} value: {1}".format(selection_type, selection_string))
             return False
-        if selection_strings[0] == ga_model.definitions.TOURNAMENT and len(selection_strings) > 1:
+        if selection_strings[0] == gadapt.ga_model.definitions.TOURNAMENT and len(selection_strings) > 1:
             group_size= selection_strings[1]
             n_group_size = -1
             try:
                 n_group_size = int(group_size)
             except:
                 self.add_message("Invalid {0} value: {1}".format(selection_type, selection_string))
                 return False
@@ -234,16 +234,16 @@
                 return False
             if not isinstance(n_group_size, int):
                 self.add_message("Invalid value for {0}: {1}".format(selection_type, selection_string))
                 return False
             elif int(n_group_size) > comparing_number:
                 self.add_message(group_size_error_message)
                 return False
-        if not selection_strings[0] in ga_model.definitions.SELECTION_STRINGS:
-            self.add_message("Invalid {0} value: {1}. Allowed values: {2}".format(selection_type, selection_string, self.get_allowed_values(ga_model.definitions.SELECTION_STRINGS)))
+        if not selection_strings[0] in gadapt.ga_model.definitions.SELECTION_STRINGS:
+            self.add_message("Invalid {0} value: {1}. Allowed values: {2}".format(selection_type, selection_string, self.get_allowed_values(gadapt.ga_model.definitions.SELECTION_STRINGS)))
             return False
         return True
     
     def get_allowed_values(self, s_list):
         rslt = ""
         for s in s_list:
             rslt += s + ", "
```

### Comparing `gadapt-0.2.5/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.6/gadapt/variable_update/common_variable_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import statistics as stat
-from ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.genetic_variable import GeneticVariable
 import utils.ga_utils
 
 class CommonVariableUpdater:
     def update_variables(self, population):
         def scale_values(gv: GeneticVariable, values):
             rslt = []
             max_val = max(values)
```

### Comparing `gadapt-0.2.5/gadapt.egg-info/SOURCES.txt` & `gadapt-0.2.6/gadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

