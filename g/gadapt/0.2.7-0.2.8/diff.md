# Comparing `tmp/gadapt-0.2.7.tar.gz` & `tmp/gadapt-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.7.tar", last modified: Tue May 23 23:38:27 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.8.tar", last modified: Tue May 23 23:51:41 2023, max compression
```

## Comparing `gadapt-0.2.7.tar` & `gadapt-0.2.8.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.204599 gadapt-0.2.7/
--rw-rw-rw-   0        0        0      339 2023-05-23 23:38:27.204599 gadapt-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-05-20 09:05:31.000000 gadapt-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.028598 gadapt-0.2.7/gadapt/
--rw-rw-rw-   0        0        0       77 2023-05-23 23:37:48.000000 gadapt-0.2.7/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.055097 gadapt-0.2.7/gadapt/cost_finding/
--rw-rw-rw-   0        0        0       33 2023-05-23 23:37:03.000000 gadapt-0.2.7/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      729 2023-05-23 23:17:08.000000 gadapt-0.2.7/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2099 2023-05-23 23:29:54.000000 gadapt-0.2.7/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.065597 gadapt-0.2.7/gadapt/crossover/
--rw-rw-rw-   0        0        0       30 2023-05-23 23:36:56.000000 gadapt-0.2.7/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     7054 2023-05-23 23:29:42.000000 gadapt-0.2.7/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1229 2023-05-23 23:14:52.000000 gadapt-0.2.7/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.069097 gadapt-0.2.7/gadapt/execution/
--rw-rw-rw-   0        0        0       30 2023-05-23 23:36:51.000000 gadapt-0.2.7/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-05-23 23:29:11.000000 gadapt-0.2.7/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.084098 gadapt-0.2.7/gadapt/exit_check/
--rw-rw-rw-   0        0        0       31 2023-05-23 23:36:42.000000 gadapt-0.2.7/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.7/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1061 2023-05-23 23:17:08.000000 gadapt-0.2.7/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.7/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.7/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.095098 gadapt-0.2.7/gadapt/factory/
--rw-rw-rw-   0        0        0       28 2023-05-23 23:36:36.000000 gadapt-0.2.7/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0    10425 2023-05-23 23:28:33.000000 gadapt-0.2.7/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0     7964 2023-05-23 23:16:43.000000 gadapt-0.2.7/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.105098 gadapt-0.2.7/gadapt/ga_logging/
--rw-rw-rw-   0        0        0       31 2023-05-23 23:36:29.000000 gadapt-0.2.7/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2116 2023-05-18 19:46:16.000000 gadapt-0.2.7/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.126598 gadapt-0.2.7/gadapt/ga_model/
--rw-rw-rw-   0        0        0       29 2023-05-23 23:36:23.000000 gadapt-0.2.7/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     6696 2023-05-23 23:26:15.000000 gadapt-0.2.7/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      683 2023-05-21 10:44:03.000000 gadapt-0.2.7/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     3718 2023-05-23 23:14:52.000000 gadapt-0.2.7/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     1423 2023-05-23 23:26:32.000000 gadapt-0.2.7/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1336 2023-05-23 23:16:43.000000 gadapt-0.2.7/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2547 2023-05-23 23:16:43.000000 gadapt-0.2.7/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.7/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    10378 2023-05-23 23:25:30.000000 gadapt-0.2.7/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      802 2023-05-23 23:16:43.000000 gadapt-0.2.7/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.137098 gadapt-0.2.7/gadapt/gene_combination/
--rw-rw-rw-   0        0        0       37 2023-05-23 23:36:17.000000 gadapt-0.2.7/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      309 2023-05-23 23:17:08.000000 gadapt-0.2.7/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.7/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.148599 gadapt-0.2.7/gadapt/parent_selection/
--rw-rw-rw-   0        0        0       37 2023-05-23 23:35:32.000000 gadapt-0.2.7/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      300 2023-05-23 23:17:08.000000 gadapt-0.2.7/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.7/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.166100 gadapt-0.2.7/gadapt/sampling/
--rw-rw-rw-   0        0        0       29 2023-05-23 23:35:26.000000 gadapt-0.2.7/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      708 2023-05-23 23:17:08.000000 gadapt-0.2.7/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.7/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      418 2023-05-23 23:14:52.000000 gadapt-0.2.7/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1805 2023-05-23 23:14:52.000000 gadapt-0.2.7/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2615 2023-05-23 23:14:52.000000 gadapt-0.2.7/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.177598 gadapt-0.2.7/gadapt/string_operation/
--rw-rw-rw-   0        0        0       37 2023-05-23 23:35:18.000000 gadapt-0.2.7/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3221 2023-05-21 11:30:07.000000 gadapt-0.2.7/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.188598 gadapt-0.2.7/gadapt/utils/
--rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.7/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0       26 2023-05-23 23:35:11.000000 gadapt-0.2.7/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1213 2023-05-23 23:15:55.000000 gadapt-0.2.7/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.198599 gadapt-0.2.7/gadapt/validation/
--rw-rw-rw-   0        0        0       31 2023-05-23 23:35:05.000000 gadapt-0.2.7/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      786 2023-05-23 23:17:08.000000 gadapt-0.2.7/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    15539 2023-05-23 23:17:43.000000 gadapt-0.2.7/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.203598 gadapt-0.2.7/gadapt/variable_update/
--rw-rw-rw-   0        0        0       36 2023-05-23 23:34:20.000000 gadapt-0.2.7/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      177 2023-05-23 23:17:08.000000 gadapt-0.2.7/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     1988 2023-05-23 23:14:52.000000 gadapt-0.2.7/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:38:27.043098 gadapt-0.2.7/gadapt.egg-info/
--rw-rw-rw-   0        0        0      339 2023-05-23 23:38:26.000000 gadapt-0.2.7/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2002 2023-05-23 23:38:26.000000 gadapt-0.2.7/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 23:38:26.000000 gadapt-0.2.7/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 23:38:26.000000 gadapt-0.2.7/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-23 23:38:27.206599 gadapt-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      433 2023-05-23 23:37:27.000000 gadapt-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.398345 gadapt-0.2.8/
+-rw-rw-rw-   0        0        0      339 2023-05-23 23:51:41.398345 gadapt-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-05-20 09:05:31.000000 gadapt-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.239345 gadapt-0.2.8/gadapt/
+-rw-rw-rw-   0        0        0       77 2023-05-23 23:50:53.000000 gadapt-0.2.8/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.258345 gadapt-0.2.8/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0       33 2023-05-23 23:37:03.000000 gadapt-0.2.8/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0      729 2023-05-23 23:17:08.000000 gadapt-0.2.8/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2113 2023-05-23 23:44:34.000000 gadapt-0.2.8/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.264844 gadapt-0.2.8/gadapt/crossover/
+-rw-rw-rw-   0        0        0       30 2023-05-23 23:36:56.000000 gadapt-0.2.8/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7054 2023-05-23 23:29:42.000000 gadapt-0.2.8/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.8/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.267843 gadapt-0.2.8/gadapt/execution/
+-rw-rw-rw-   0        0        0       30 2023-05-23 23:36:51.000000 gadapt-0.2.8/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3373 2023-05-23 23:47:09.000000 gadapt-0.2.8/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.280345 gadapt-0.2.8/gadapt/exit_check/
+-rw-rw-rw-   0        0        0       31 2023-05-23 23:36:42.000000 gadapt-0.2.8/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.8/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1061 2023-05-23 23:17:08.000000 gadapt-0.2.8/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.8/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.8/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.282844 gadapt-0.2.8/gadapt/factory/
+-rw-rw-rw-   0        0        0       28 2023-05-23 23:36:36.000000 gadapt-0.2.8/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0    10425 2023-05-23 23:28:33.000000 gadapt-0.2.8/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0     8076 2023-05-23 23:48:38.000000 gadapt-0.2.8/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.286345 gadapt-0.2.8/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0       31 2023-05-23 23:36:29.000000 gadapt-0.2.8/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-05-23 23:47:24.000000 gadapt-0.2.8/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.302344 gadapt-0.2.8/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       29 2023-05-23 23:36:23.000000 gadapt-0.2.8/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     6703 2023-05-23 23:40:14.000000 gadapt-0.2.8/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      683 2023-05-21 10:44:03.000000 gadapt-0.2.8/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     3718 2023-05-23 23:14:52.000000 gadapt-0.2.8/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     1423 2023-05-23 23:26:32.000000 gadapt-0.2.8/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1350 2023-05-23 23:43:23.000000 gadapt-0.2.8/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2547 2023-05-23 23:16:43.000000 gadapt-0.2.8/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.8/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    10348 2023-05-23 23:44:09.000000 gadapt-0.2.8/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      802 2023-05-23 23:16:43.000000 gadapt-0.2.8/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.339845 gadapt-0.2.8/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0       37 2023-05-23 23:36:17.000000 gadapt-0.2.8/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-05-23 23:17:08.000000 gadapt-0.2.8/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.8/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.343845 gadapt-0.2.8/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0       37 2023-05-23 23:35:32.000000 gadapt-0.2.8/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      300 2023-05-23 23:17:08.000000 gadapt-0.2.8/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.8/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.381845 gadapt-0.2.8/gadapt/sampling/
+-rw-rw-rw-   0        0        0       29 2023-05-23 23:35:26.000000 gadapt-0.2.8/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      708 2023-05-23 23:17:08.000000 gadapt-0.2.8/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.8/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.8/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.8/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.8/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.384345 gadapt-0.2.8/gadapt/string_operation/
+-rw-rw-rw-   0        0        0       37 2023-05-23 23:40:32.000000 gadapt-0.2.8/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3221 2023-05-21 11:30:07.000000 gadapt-0.2.8/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.388346 gadapt-0.2.8/gadapt/utils/
+-rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.8/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       26 2023-05-23 23:35:11.000000 gadapt-0.2.8/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1213 2023-05-23 23:15:55.000000 gadapt-0.2.8/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.392345 gadapt-0.2.8/gadapt/validation/
+-rw-rw-rw-   0        0        0       31 2023-05-23 23:35:05.000000 gadapt-0.2.8/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-05-23 23:17:08.000000 gadapt-0.2.8/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    15539 2023-05-23 23:17:43.000000 gadapt-0.2.8/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.396845 gadapt-0.2.8/gadapt/variable_update/
+-rw-rw-rw-   0        0        0       36 2023-05-23 23:34:20.000000 gadapt-0.2.8/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      177 2023-05-23 23:17:08.000000 gadapt-0.2.8/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2002 2023-05-23 23:46:55.000000 gadapt-0.2.8/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-05-23 23:51:41.252845 gadapt-0.2.8/gadapt.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-23 23:51:40.000000 gadapt-0.2.8/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2002 2023-05-23 23:51:41.000000 gadapt-0.2.8/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 23:51:40.000000 gadapt-0.2.8/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 23:51:40.000000 gadapt-0.2.8/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-23 23:51:41.400346 gadapt-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      433 2023-05-23 23:50:29.000000 gadapt-0.2.8/setup.py
```

### Comparing `gadapt-0.2.7/gadapt/cost_finding/base_cost_finder.py` & `gadapt-0.2.8/gadapt/cost_finding/base_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.8/gadapt/cost_finding/common_cost_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import math
 from typing import List
 from gadapt.cost_finding.base_cost_finder import BaseCostFinder
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.population import Population
-import utils.ga_utils
+import gadapt.utils.ga_utils
 
 class CommonCostFinder(BaseCostFinder):
     def find_costs_for_chromosome(self, population: Population):
         if (population is None):
             raise Exception("population must not be null!")
         chromosomes_for_execution: List[Chromosome] = [
             c for c in population if (math.isnan(c.cost_value)) or (c.is_immigrant and c.population_generation == population.population_generation)]
@@ -25,13 +25,13 @@
         self.log_population(population)
         population.clear_and_add_chromosomes(better_chromosomes)
         population.update_variables()
         self.cost_found_first_time(population, better_chromosomes)
         
     def cost_found_first_time(self, population: Population, better_chromosomes: List[Chromosome] ):
         if math.isnan(population.first_cost):
-            population.first_cost = utils.ga_utils.average([c.cost_value for c in better_chromosomes])
+            population.first_cost = gadapt.utils.ga_utils.average([c.cost_value for c in better_chromosomes])
             population.population_mutator.after_first_execution(population)
 
     def log_population(self, population: Population):
         if population.options.logging:
             logging.info(str(population))
```

### Comparing `gadapt-0.2.7/gadapt/crossover/base_crossover.py` & `gadapt-0.2.8/gadapt/crossover/base_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.8/gadapt/crossover/uniform_crossover.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from gadapt.ga_model.chromosome import Chromosome
-from crossover.base_crossover import BaseCrossover
+from gadapt.crossover.base_crossover import BaseCrossover
 from gadapt.ga_model.gene import Gene
-from immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
-from mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
-from gene_combination.base_gene_combination import BaseGeneCombination
+from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
+from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
+from gadapt.gene_combination.base_gene_combination import BaseGeneCombination
 
 class UniformCrossover(BaseCrossover):
     
     def __init__(self, var_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator):
         super(UniformCrossover, self).__init__(var_combination, mutator, immigrator)
         self.gene_combination = var_combination
```

### Comparing `gadapt-0.2.7/gadapt/execution/ga_executor.py` & `gadapt-0.2.8/gadapt/execution/ga_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from gadapt.factory.ga_factory import GAFactory
-from ga_logging.logging_settings import init_logging
+from gadapt.ga_logging.logging_settings import init_logging
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.ga_results import GAResults
 from gadapt.ga_model.population import Population
 import gadapt.ga_model.message_levels
 
 class GAExecutor:
     def __init__(self, ga_options: GAOptions, factory: GAFactory) -> None:
```

### Comparing `gadapt-0.2.7/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.8/gadapt/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/factory/ga_factory.py` & `gadapt-0.2.8/gadapt/factory/ga_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/ga.py` & `gadapt-0.2.8/gadapt/ga.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from gadapt.execution.ga_executor import GAExecutor
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga_model.genetic_variable import GeneticVariable
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.ga_results import GAResults
 from gadapt.ga_model.population import Population
-import utils.ga_utils
+import gadapt.utils.ga_utils
 import gadapt.ga_model.definitions
 
 class GA:
     def __init__(self,
                  cost_function = None,
                  population_size = 64, 
                  exit_check = gadapt.ga_model.definitions.AVG_COST,
@@ -53,15 +53,15 @@
         
     @property
     def population_size(self) -> int:
         return self._population_size
     
     @population_size.setter
     def population_size(self, value: int):
-        self._population_size = utils.ga_utils.try_get_int(value)
+        self._population_size = gadapt.utils.ga_utils.try_get_int(value)
 
     def add(self, min_value: float, max_value:float, step: float=0.01):    
         if (not isinstance(min_value, float) and not isinstance(min_value, int)) or (not isinstance(max_value, float) and not isinstance(max_value, int)):
             raise Exception("min value, max value and step must be numerical values!")
         genetic_variable = GeneticVariable(self._current_gv_id)
         genetic_variable.min_value = min_value
         genetic_variable.max_value = max_value
@@ -79,116 +79,116 @@
 
     @property
     def number_of_mutation_genes(self) -> int:
         return self._number_of_mutation_genes
     
     @number_of_mutation_genes.setter
     def number_of_mutation_genes(self, value: int):
-        self._number_of_mutation_genes = utils.ga_utils.try_get_int(value)
+        self._number_of_mutation_genes = gadapt.utils.ga_utils.try_get_int(value)
 
     @property
     def number_of_mutation_chromosomes(self) -> int:
         return self._number_of_mutation_chromosomes
     
     @number_of_mutation_chromosomes.setter
     def number_of_mutation_chromosomes(self, value: int):
         first_time = self._number_of_mutation_chromosomes == -1
-        self._number_of_mutation_chromosomes = utils.ga_utils.try_get_int(value)
+        self._number_of_mutation_chromosomes = gadapt.utils.ga_utils.try_get_int(value)
         if not first_time:
             self._number_of_mutation_chromosomes_changed = True
 
     @property
     def immigration_number(self) -> int:
         return self._immigration_number
     
     @immigration_number.setter
     def immigration_number(self, value: int):
-        self._immigration_number = utils.ga_utils.try_get_int(value)
+        self._immigration_number = gadapt.utils.ga_utils.try_get_int(value)
     
     @property
     def population_mutation(self) -> str:
         return self._population_mutation
 
     @population_mutation.setter
     def population_mutation(self, value: str):
-        self._population_mutation = utils.ga_utils.prepare_string(value)
+        self._population_mutation = gadapt.utils.ga_utils.prepare_string(value)
 
     @property
     def parent_diversity_mutation_chromosome_selection(self) -> str:
         return self._parent_diversity_mutation_chromosome_selection
 
     @parent_diversity_mutation_chromosome_selection.setter
     def parent_diversity_mutation_chromosome_selection(self, value: str):
-        self._parent_diversity_mutation_chromosome_selection = utils.ga_utils.prepare_string(value)
+        self._parent_diversity_mutation_chromosome_selection = gadapt.utils.ga_utils.prepare_string(value)
 
     @property
     def chromosome_mutation(self) -> str:
         return self._chromosome_mutation
 
     @chromosome_mutation.setter
     def chromosome_mutation(self, value: str):
-        self._chromosome_mutation = utils.ga_utils.prepare_string(value)
+        self._chromosome_mutation = gadapt.utils.ga_utils.prepare_string(value)
 
     @property
     def cross_diversity_mutation_gene_selection(self) -> str:
         return self._cross_diversity_mutation_gene_selection
 
     @cross_diversity_mutation_gene_selection.setter
     def cross_diversity_mutation_gene_selection(self, value: str):
-        self._cross_diversity_mutation_gene_selection = utils.ga_utils.prepare_string(value)
+        self._cross_diversity_mutation_gene_selection = gadapt.utils.ga_utils.prepare_string(value)
 
     @property
     def max_attempt_no(self) -> int:
         return self._max_attempt_no
 
     @max_attempt_no.setter
     def max_attempt_no(self, value: int):
-        self._max_attempt_no = utils.ga_utils.try_get_int(value)
+        self._max_attempt_no = gadapt.utils.ga_utils.try_get_int(value)
 
     @property
     def exit_check(self) -> str:
         return self._exit_check
 
     @exit_check.setter
     def exit_check(self, value: str):
-        self._exit_check = utils.ga_utils.prepare_string(value)
+        self._exit_check = gadapt.utils.ga_utils.prepare_string(value)
 
     @property
     def parent_selection(self) -> str:
         return self._parent_selection
 
     @parent_selection.setter
     def parent_selection(self, value: str):
-        self._parent_selection = utils.ga_utils.prepare_string(value)
+        self._parent_selection = gadapt.utils.ga_utils.prepare_string(value)
 
     @property
     def requested_cost(self) -> float:
         return self._requested_cost
 
     @requested_cost.setter
     def requested_cost(self, value: float):
-        self._requested_cost = utils.ga_utils.try_get_float(value)
+        self._requested_cost = gadapt.utils.ga_utils.try_get_float(value)
 
     @property
     def logging(self) -> bool:
         return self._logging
     
     @logging.setter
     def logging(self, value: bool):
-        self._logging = utils.ga_utils.try_get_bool(value)
+        self._logging = gadapt.utils.ga_utils.try_get_bool(value)
 
     @property
     def must_mutate_for_same_parents(self) -> bool:
         return self._must_mutate_for_same_parents
     
     @must_mutate_for_same_parents.setter
     def must_mutate_for_same_parents(self, value: bool):
-        self._must_mutate_for_same_parents = utils.ga_utils.try_get_bool(value)
+        self._must_mutate_for_same_parents = gadapt.utils.ga_utils.try_get_bool(value)
     
     @property
     def timeout(self) -> int:
         return self._timeout
     
     @timeout.setter
     def timeout(self, value: int):
-        self._timeout = utils.ga_utils.try_get_int(value)
+        self._timeout = gadapt.utils.ga_utils.try_get_int(value)
```

### Comparing `gadapt-0.2.7/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.8/gadapt/ga_logging/logging_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from genericpath import isfile
 import logging
 import os
 from os.path import isfile, join
 import traceback
-from utils.TimeStampFormatter import TimestampFormatter
+from gadapt.utils.TimeStampFormatter import TimestampFormatter
 
 def init_logging(is_logging: bool):
     def get_last_num(s: str) -> int:
         try:
             if not s.startswith("log.log"):
                 return -1
             if s == "log.log":
```

### Comparing `gadapt-0.2.7/gadapt/ga_model/chromosome.py` & `gadapt-0.2.8/gadapt/ga_model/chromosome.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     def append(self, g: Gene):
         self.genes.append(g)
 
     def clear(self):
         self.genes.clear()
 
     def to_string(self):
-        return string_operation.ga_strings.chromosome_to_string(self)
+        return gadapt.string_operation.ga_strings.chromosome_to_string(self)
 
     def set_chromosome_string(self, value: str):
         if value is None:
            self._chromosome_string  = None 
 
     def get_chromosome_string(self):
         if self._chromosome_string is None:
```

### Comparing `gadapt-0.2.7/gadapt/ga_model/definitions.py` & `gadapt-0.2.8/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/ga_model/ga_options.py` & `gadapt-0.2.8/gadapt/ga_model/ga_options.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/ga_model/ga_results.py` & `gadapt-0.2.8/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/ga_model/gene.py` & `gadapt-0.2.8/gadapt/ga_model/gene.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from gadapt.ga_model.genetic_variable import GeneticVariable
 from gadapt.ga_model.ranking_model import RankingModel
-import string_operation.ga_strings
+import gadapt.string_operation.ga_strings
 import gadapt.ga_model.definitions
 class Gene(RankingModel):
 
     def __init__(self, gen_variable, var_value = None):
         super().__init__()
         self.genetic_variable = gen_variable        
         self.variable_value = var_value
@@ -14,15 +14,15 @@
         if (self.variable_value == None or math.isnan(self.variable_value)):
             self.set_random_value()
 
     def __str__(self) -> str:
         return self.to_string()
     
     def to_string(self):
-        return string_operation.ga_strings.gene_to_string(self)
+        return gadapt.string_operation.ga_strings.gene_to_string(self)
 
     @property
     def genetic_variable(self) -> GeneticVariable:
         return self._genetic_variable
     
     @genetic_variable.setter
     def genetic_variable(self, value: GeneticVariable):
```

### Comparing `gadapt-0.2.7/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.8/gadapt/ga_model/genetic_variable.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/ga_model/population.py` & `gadapt-0.2.8/gadapt/ga_model/population.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,19 +174,19 @@
         return self._cost_finder
 
     @cost_finder.setter
     def cost_finder(self, value: BaseCostFinder):
         self._cost_finder = value
 
     @property
-    def selector(self) -> BaseSelector:
+    def selector(self):
         return self._selector
 
     @selector.setter
-    def selector(self, value: BaseSelector):
+    def selector(self, value):
         self._selector = value
 
     @property
     def population_immigrator(self) -> BasePopulationImmigrator:
         return self._population_immigrator
 
     @population_immigrator.setter
```

### Comparing `gadapt-0.2.7/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.8/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.8/gadapt/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.8/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/sampling/base_sampling.py` & `gadapt-0.2.8/gadapt/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.8/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 from typing import List
 from gadapt.ga_model.ranking_model import RankingModel
-from sampling.base_sampling import BaseSampling
+from gadapt.sampling.base_sampling import BaseSampling
 
 class RouletteWheelSampling(BaseSampling):
     
     def prepare_sample(self, lst: List[RankingModel]) -> List[RankingModel]:
         rank_sum = sum(range(1, len(lst) + 1))
         cummultative_probability_list: List[float] = []
         cummulative_probability = 0.0
```

### Comparing `gadapt-0.2.7/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.8/gadapt/sampling/tournament_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 from typing import List
 from gadapt.ga_model.ranking_model import RankingModel
-from sampling.base_sampling import BaseSampling
+from gadapt.sampling.base_sampling import BaseSampling
 
 class TournamentSampling(BaseSampling):
     def __init__(self, group_size = None) -> None:
         super().__init__()
         self.group_size = group_size
     
     def prepare_sample(self, lst: List[RankingModel]) -> List[RankingModel]:
```

### Comparing `gadapt-0.2.7/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.8/gadapt/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/utils/ga_utils.py` & `gadapt-0.2.8/gadapt/utils/ga_utils.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/validation/base_options_validator.py` & `gadapt-0.2.8/gadapt/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/validation/common_options_validator.py` & `gadapt-0.2.8/gadapt/validation/common_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.7/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.8/gadapt/variable_update/common_variable_updater.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import statistics as stat
 from gadapt.ga_model.genetic_variable import GeneticVariable
-import utils.ga_utils
+import gadapt.utils.ga_utils
 
 class CommonVariableUpdater:
     def update_variables(self, population):
         def scale_values(gv: GeneticVariable, values):
             rslt = []
             max_val = max(values)
             diff = (gv.max_value - max_val)
@@ -37,10 +37,10 @@
                 key.stacked = False        
         for key in values_per_variables:
             if key.stacked:
                 key.relative_standard_deviation = 0.0
                 continue
             scaled_values = scale_values(key, values_per_variables[key])
             stddev = stat.stdev(scaled_values)
-            avg_val = utils.ga_utils.average(scaled_values)
+            avg_val = gadapt.utils.ga_utils.average(scaled_values)
             rel_st_dev = stddev / avg_val
             key.relative_standard_deviation = rel_st_dev
```

### Comparing `gadapt-0.2.7/gadapt.egg-info/SOURCES.txt` & `gadapt-0.2.8/gadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

