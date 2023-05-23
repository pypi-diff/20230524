# Comparing `tmp/gadapt-0.2.tar.gz` & `tmp/gadapt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.tar", last modified: Tue May 23 22:23:02 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.1.tar", last modified: Tue May 23 22:46:53 2023, max compression
```

## Comparing `gadapt-0.2.tar` & `gadapt-0.2.1.tar`

### file list

```diff
@@ -1,107 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.182916 gadapt-0.2/
--rw-rw-rw-   0        0        0      337 2023-05-23 22:23:02.182916 gadapt-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-05-20 09:05:31.000000 gadapt-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.034915 gadapt-0.2/gadapt/
--rw-rw-rw-   0        0        0      513 2023-05-23 22:00:19.000000 gadapt-0.2/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.049415 gadapt-0.2/gadapt/cost_finding/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      708 2023-05-21 09:37:48.000000 gadapt-0.2/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2078 2023-05-21 09:27:38.000000 gadapt-0.2/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.053414 gadapt-0.2/gadapt/crossover/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     6984 2023-05-22 17:45:24.000000 gadapt-0.2/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1215 2023-05-22 17:43:24.000000 gadapt-0.2/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.056415 gadapt-0.2/gadapt/execution/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3310 2023-05-22 17:43:16.000000 gadapt-0.2/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.062914 gadapt-0.2/gadapt/exit_check/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      308 2023-05-21 09:27:27.000000 gadapt-0.2/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1047 2023-05-21 09:37:54.000000 gadapt-0.2/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      298 2023-05-21 09:27:27.000000 gadapt-0.2/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      380 2023-05-18 18:36:32.000000 gadapt-0.2/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.066417 gadapt-0.2/gadapt/factory/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0    10019 2023-05-22 17:51:10.000000 gadapt-0.2/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0     7873 2023-05-22 18:10:31.000000 gadapt-0.2/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.075415 gadapt-0.2/gadapt/ga_logging/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2116 2023-05-18 19:46:16.000000 gadapt-0.2/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.089415 gadapt-0.2/gadapt/ga_model/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     6633 2023-05-22 17:39:59.000000 gadapt-0.2/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      683 2023-05-21 10:44:03.000000 gadapt-0.2/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     3711 2023-05-22 18:10:00.000000 gadapt-0.2/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     1416 2023-05-21 11:30:38.000000 gadapt-0.2/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1308 2023-05-21 09:38:09.000000 gadapt-0.2/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2533 2023-05-21 09:38:16.000000 gadapt-0.2/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    10309 2023-05-21 09:38:24.000000 gadapt-0.2/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      781 2023-05-22 13:25:31.000000 gadapt-0.2/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.092914 gadapt-0.2/gadapt/gene_combination/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      281 2023-05-22 09:58:34.000000 gadapt-0.2/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0      823 2023-05-22 17:42:12.000000 gadapt-0.2/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.093915 gadapt-0.2/gadapt/immigration/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.096915 gadapt-0.2/gadapt/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      598 2023-05-21 09:38:38.000000 gadapt-0.2/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      322 2023-05-08 07:23:26.000000 gadapt-0.2/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.100415 gadapt-0.2/gadapt/immigration/population_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      161 2023-05-21 09:38:42.000000 gadapt-0.2/gadapt/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0      817 2023-05-08 07:22:17.000000 gadapt-0.2/gadapt/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.101915 gadapt-0.2/gadapt/mutation/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.110914 gadapt-0.2/gadapt/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      828 2023-05-22 17:39:59.000000 gadapt-0.2/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     2903 2023-05-22 17:39:59.000000 gadapt-0.2/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0      915 2023-05-22 17:39:59.000000 gadapt-0.2/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.128415 gadapt-0.2/gadapt/mutation/population_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1375 2023-05-21 09:38:54.000000 gadapt-0.2/gadapt/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1255 2023-05-21 09:27:38.000000 gadapt-0.2/gadapt/mutation/population_mutation/composed_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.130915 gadapt-0.2/gadapt/mutation/population_mutation/cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/mutation/population_mutation/cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     2852 2023-05-21 09:38:59.000000 gadapt-0.2/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1954 2023-05-22 17:39:59.000000 gadapt-0.2/gadapt/mutation/population_mutation/parents_diversity_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.136916 gadapt-0.2/gadapt/mutation/population_mutation/previous_cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     3715 2023-05-22 18:09:18.000000 gadapt-0.2/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0      456 2023-05-21 09:39:09.000000 gadapt-0.2/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
--rw-rw-rw-   0        0        0     1048 2023-05-22 17:39:59.000000 gadapt-0.2/gadapt/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.139916 gadapt-0.2/gadapt/parent_selection/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      279 2023-05-21 09:39:14.000000 gadapt-0.2/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0      862 2023-05-18 07:22:58.000000 gadapt-0.2/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.147416 gadapt-0.2/gadapt/sampling/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-21 09:39:18.000000 gadapt-0.2/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      419 2023-05-22 13:38:56.000000 gadapt-0.2/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      411 2023-05-22 13:28:32.000000 gadapt-0.2/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1798 2023-05-22 14:01:48.000000 gadapt-0.2/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2608 2023-05-22 12:50:02.000000 gadapt-0.2/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.156914 gadapt-0.2/gadapt/string_operation/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3221 2023-05-21 11:30:07.000000 gadapt-0.2/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.171414 gadapt-0.2/gadapt/utils/
--rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-05-22 13:04:13.000000 gadapt-0.2/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.177915 gadapt-0.2/gadapt/validation/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      758 2023-05-21 09:39:32.000000 gadapt-0.2/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    15392 2023-05-23 19:50:24.000000 gadapt-0.2/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.181915 gadapt-0.2/gadapt/variable_update/
--rw-rw-rw-   0        0        0        0 2023-05-23 22:06:08.000000 gadapt-0.2/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-21 09:36:51.000000 gadapt-0.2/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     1981 2023-05-08 05:52:39.000000 gadapt-0.2/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-05-23 22:23:02.044915 gadapt-0.2/gadapt.egg-info/
--rw-rw-rw-   0        0        0      337 2023-05-23 22:23:01.000000 gadapt-0.2/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3461 2023-05-23 22:23:01.000000 gadapt-0.2/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 22:23:01.000000 gadapt-0.2/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 22:23:01.000000 gadapt-0.2/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-23 22:23:02.187415 gadapt-0.2/setup.cfg
--rw-rw-rw-   0        0        0      431 2023-05-23 22:20:21.000000 gadapt-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.469187 gadapt-0.2.1/
+-rw-rw-rw-   0        0        0      339 2023-05-23 22:46:53.469688 gadapt-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-05-20 09:05:31.000000 gadapt-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.339685 gadapt-0.2.1/gadapt/
+-rw-rw-rw-   0        0        0      513 2023-05-23 22:00:19.000000 gadapt-0.2.1/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.366185 gadapt-0.2.1/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0       27 2023-05-23 22:36:02.000000 gadapt-0.2.1/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0      708 2023-05-21 09:37:48.000000 gadapt-0.2.1/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2078 2023-05-21 09:27:38.000000 gadapt-0.2.1/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.376186 gadapt-0.2.1/gadapt/crossover/
+-rw-rw-rw-   0        0        0       24 2023-05-23 22:36:24.000000 gadapt-0.2.1/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     6984 2023-05-22 17:45:24.000000 gadapt-0.2.1/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1215 2023-05-22 17:43:24.000000 gadapt-0.2.1/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.379685 gadapt-0.2.1/gadapt/execution/
+-rw-rw-rw-   0        0        0       24 2023-05-23 22:37:05.000000 gadapt-0.2.1/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3310 2023-05-22 17:43:16.000000 gadapt-0.2.1/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.385186 gadapt-0.2.1/gadapt/exit_check/
+-rw-rw-rw-   0        0        0       25 2023-05-23 22:37:37.000000 gadapt-0.2.1/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-05-21 09:27:27.000000 gadapt-0.2.1/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1047 2023-05-21 09:37:54.000000 gadapt-0.2.1/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      298 2023-05-21 09:27:27.000000 gadapt-0.2.1/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      380 2023-05-18 18:36:32.000000 gadapt-0.2.1/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.388187 gadapt-0.2.1/gadapt/factory/
+-rw-rw-rw-   0        0        0       22 2023-05-23 22:37:58.000000 gadapt-0.2.1/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0    10019 2023-05-22 17:51:10.000000 gadapt-0.2.1/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0     7873 2023-05-22 18:10:31.000000 gadapt-0.2.1/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.390187 gadapt-0.2.1/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0       25 2023-05-23 22:38:17.000000 gadapt-0.2.1/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2116 2023-05-18 19:46:16.000000 gadapt-0.2.1/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.418686 gadapt-0.2.1/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       23 2023-05-23 22:38:44.000000 gadapt-0.2.1/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     6633 2023-05-22 17:39:59.000000 gadapt-0.2.1/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      683 2023-05-21 10:44:03.000000 gadapt-0.2.1/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     3711 2023-05-22 18:10:00.000000 gadapt-0.2.1/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     1416 2023-05-21 11:30:38.000000 gadapt-0.2.1/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1308 2023-05-21 09:38:09.000000 gadapt-0.2.1/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2533 2023-05-21 09:38:16.000000 gadapt-0.2.1/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.1/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    10309 2023-05-21 09:38:24.000000 gadapt-0.2.1/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      781 2023-05-22 13:25:31.000000 gadapt-0.2.1/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.424187 gadapt-0.2.1/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0       31 2023-05-23 22:39:08.000000 gadapt-0.2.1/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-05-22 09:58:34.000000 gadapt-0.2.1/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0      823 2023-05-22 17:42:12.000000 gadapt-0.2.1/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.429185 gadapt-0.2.1/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0       31 2023-05-23 22:44:18.000000 gadapt-0.2.1/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-05-21 09:39:14.000000 gadapt-0.2.1/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0      862 2023-05-18 07:22:58.000000 gadapt-0.2.1/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.444686 gadapt-0.2.1/gadapt/sampling/
+-rw-rw-rw-   0        0        0       23 2023-05-23 22:44:44.000000 gadapt-0.2.1/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-21 09:39:18.000000 gadapt-0.2.1/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      419 2023-05-22 13:38:56.000000 gadapt-0.2.1/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      411 2023-05-22 13:28:32.000000 gadapt-0.2.1/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1798 2023-05-22 14:01:48.000000 gadapt-0.2.1/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2608 2023-05-22 12:50:02.000000 gadapt-0.2.1/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.450187 gadapt-0.2.1/gadapt/string_operation/
+-rw-rw-rw-   0        0        0       31 2023-05-23 22:45:02.000000 gadapt-0.2.1/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3221 2023-05-21 11:30:07.000000 gadapt-0.2.1/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.455686 gadapt-0.2.1/gadapt/utils/
+-rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.1/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       20 2023-05-23 22:45:18.000000 gadapt-0.2.1/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1206 2023-05-22 13:04:13.000000 gadapt-0.2.1/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.460687 gadapt-0.2.1/gadapt/validation/
+-rw-rw-rw-   0        0        0       25 2023-05-23 22:45:47.000000 gadapt-0.2.1/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      758 2023-05-21 09:39:32.000000 gadapt-0.2.1/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    15392 2023-05-23 19:50:24.000000 gadapt-0.2.1/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.468186 gadapt-0.2.1/gadapt/variable_update/
+-rw-rw-rw-   0        0        0       30 2023-05-23 22:46:12.000000 gadapt-0.2.1/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-21 09:36:51.000000 gadapt-0.2.1/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     1981 2023-05-08 05:52:39.000000 gadapt-0.2.1/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-05-23 22:46:53.361686 gadapt-0.2.1/gadapt.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-23 22:46:53.000000 gadapt-0.2.1/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2002 2023-05-23 22:46:53.000000 gadapt-0.2.1/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 22:46:53.000000 gadapt-0.2.1/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 22:46:53.000000 gadapt-0.2.1/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-23 22:46:53.471686 gadapt-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      433 2023-05-23 22:46:26.000000 gadapt-0.2.1/setup.py
```

### Comparing `gadapt-0.2/gadapt/__init__.py` & `gadapt-0.2.1/gadapt/__init__.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/cost_finding/base_cost_finder.py` & `gadapt-0.2.1/gadapt/cost_finding/base_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.1/gadapt/cost_finding/common_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/crossover/base_crossover.py` & `gadapt-0.2.1/gadapt/crossover/base_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.1/gadapt/crossover/uniform_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/execution/ga_executor.py` & `gadapt-0.2.1/gadapt/execution/ga_executor.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.1/gadapt/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/factory/ga_factory.py` & `gadapt-0.2.1/gadapt/factory/ga_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga.py` & `gadapt-0.2.1/gadapt/ga.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.1/gadapt/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga_model/chromosome.py` & `gadapt-0.2.1/gadapt/ga_model/chromosome.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga_model/definitions.py` & `gadapt-0.2.1/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga_model/ga_options.py` & `gadapt-0.2.1/gadapt/ga_model/ga_options.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga_model/ga_results.py` & `gadapt-0.2.1/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga_model/gene.py` & `gadapt-0.2.1/gadapt/ga_model/gene.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.1/gadapt/ga_model/genetic_variable.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga_model/population.py` & `gadapt-0.2.1/gadapt/ga_model/population.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.1/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.1/gadapt/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.1/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/sampling/base_sampling.py` & `gadapt-0.2.1/gadapt/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.1/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.1/gadapt/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.1/gadapt/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/utils/ga_utils.py` & `gadapt-0.2.1/gadapt/utils/ga_utils.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/validation/base_options_validator.py` & `gadapt-0.2.1/gadapt/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/validation/common_options_validator.py` & `gadapt-0.2.1/gadapt/validation/common_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.1/gadapt/variable_update/common_variable_updater.py`

 * *Files identical despite different names*

