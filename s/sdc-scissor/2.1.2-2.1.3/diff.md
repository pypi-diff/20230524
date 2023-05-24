# Comparing `tmp/sdc_scissor-2.1.2.tar.gz` & `tmp/sdc_scissor-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdc_scissor-2.1.2.tar", max compression
+gzip compressed data, was "sdc_scissor-2.1.3.tar", max compression
```

## Comparing `sdc_scissor-2.1.2.tar` & `sdc_scissor-2.1.3.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0    34916 2023-01-11 13:24:47.343855 sdc_scissor-2.1.2/LICENSE.md
--rw-r--r--   0        0        0    10999 2023-01-11 13:24:47.343855 sdc_scissor-2.1.2/README.md
--rw-r--r--   0        0        0     1119 2023-01-11 13:24:47.447855 sdc_scissor-2.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/__init__.py
--rw-r--r--   0        0        0    14526 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/cli.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/__init__.py
--rw-r--r--   0        0        0     4779 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/angle_based_strategy.py
--rw-r--r--   0        0        0     3980 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/equi_distance_strategy.py
--rw-r--r--   0        0        0    10532 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/feature_extraction.py
--rw-r--r--   0        0        0     2587 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py
--rw-r--r--   0        0        0     3203 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/road_geometry_calculator.py
--rw-r--r--   0        0        0      401 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/segmentation_strategy.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/machine_learning_api/__init__.py
--rw-r--r--   0        0        0    10655 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py
--rw-r--r--   0        0        0      334 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/machine_learning_api/csv_loader.py
--rw-r--r--   0        0        0     7955 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/machine_learning_api/model_evaluator.py
--rw-r--r--   0        0        0     2447 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/machine_learning_api/predictor.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/__init__.py
--rw-r--r--   0        0        0      643 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/beamng_bump.py
--rw-r--r--   0        0        0      569 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/beamng_delineator.py
--rw-r--r--   0        0        0      764 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/beamng_obstacle_factory.py
--rw-r--r--   0        0        0      675 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/beamng_tree.py
--rw-r--r--   0        0        0      828 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/bump.py
--rw-r--r--   0        0        0      160 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/carla_bump.py
--rw-r--r--   0        0        0      190 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/carla_delineator.py
--rw-r--r--   0        0        0      753 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/carla_obstacle_factory.py
--rw-r--r--   0        0        0      159 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/carla_tree.py
--rw-r--r--   0        0        0      664 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/delineator.py
--rw-r--r--   0        0        0      522 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/obstacle_factory.py
--rw-r--r--   0        0        0      709 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/obstacle_api/tree.py
--rw-r--r--   0        0        0      965 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization
--rw-r--r--   0        0        0       94 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/README.md
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/__init__.py
--rw-r--r--   0        0        0      515 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/faultDetection.m
--rw-r--r--   0        0        0     6436 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m
--rw-r--r--   0        0        0      464 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/featureSelection.m
--rw-r--r--   0        0        0      396 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/fitness.m
--rw-r--r--   0        0        0     1084 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/initialPopulation.m
--rw-r--r--   0        0        0      577 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/main.m
--rw-r--r--   0        0        0      612 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/mainGreedy.m
--rw-r--r--   0        0        0      221 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/objectives.m
--rw-r--r--   0        0        0      760 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m
--rw-r--r--   0        0        0     1516 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/permutationMutation.m
--rw-r--r--   0        0        0      303 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/plotResults.m
--rw-r--r--   0        0        0     1367 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py
--rw-r--r--   0        0        0    10296 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R
--rw-r--r--   0        0        0     5034 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf
--rw-r--r--   0        0        0     2128 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv
--rw-r--r--   0        0        0      125 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/medians_APFDc.csv
--rw-r--r--   0        0        0     1877 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/plot.R
--rw-r--r--   0        0        0     1724 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/table.R
--rw-r--r--   0        0        0      394 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/utils.R
--rw-r--r--   0        0        0      584 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv
--rw-r--r--   0        0        0      958 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv
--rw-r--r--   0        0        0     1057 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/runGreedy.m
--rw-r--r--   0        0        0     4267 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/runMOSearch.m
--rw-r--r--   0        0        0     3489 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/runSearch.m
--rw-r--r--   0        0        0   239182 2023-01-11 13:24:47.495855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv
--rw-r--r--   0        0        0  1146691 2023-01-11 13:24:47.507855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv
--rw-r--r--   0        0        0   440097 2023-01-11 13:24:47.507855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv
--rw-r--r--   0        0        0     1070 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py
--rw-r--r--   0        0        0   353423 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv
--rw-r--r--   0        0        0      661 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md
--rw-r--r--   0        0        0  1142098 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv
--rw-r--r--   0        0        0     4434 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md
--rw-r--r--   0        0        0      650 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh
--rw-r--r--   0        0        0      724 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh
--rw-r--r--   0        0        0       64 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/requirements.txt
--rw-r--r--   0        0        0      324 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/setup.cfg
--rw-r--r--   0        0        0       38 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/setup.py
--rw-r--r--   0        0        0     2415 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/README.md
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/__init__.py
--rw-r--r--   0        0        0      779 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py
--rw-r--r--   0        0        0     1310 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py
--rw-r--r--   0        0        0      844 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py
--rw-r--r--   0        0        0     7915 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/run.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/simulator_api/__init__.py
--rw-r--r--   0        0        0     1676 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/simulator_api/abstract_simulator.py
--rw-r--r--   0        0        0     6672 2023-01-11 13:24:47.511855 sdc_scissor-2.1.2/sdc_scissor/simulator_api/beamng_simulator.py
--rw-r--r--   0        0        0      807 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/simulator_api/simulator_factory.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/__init__.py
--rw-r--r--   0        0        0      424 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/road_model.py
--rw-r--r--   0        0        0     2324 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test.py
--rw-r--r--   0        0        0     5482 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generator.py
--rw-r--r--   0        0        0    13515 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py
--rw-r--r--   0        0        0      304 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/duplicate_elimination.py
--rw-r--r--   0        0        0      862 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py
--rw-r--r--   0        0        0    13276 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py
--rw-r--r--   0        0        0     2444 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py
--rw-r--r--   0        0        0     2581 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py
--rw-r--r--   0        0        0     3787 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py
--rw-r--r--   0        0        0      587 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py
--rw-r--r--   0        0        0     8894 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/__init__.py
--rw-r--r--   0        0        0     2852 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py
--rw-r--r--   0        0        0      575 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/config.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/__init__.py
--rw-r--r--   0        0        0     1067 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/__init__.py
--rw-r--r--   0        0        0   372723 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/generators/__init__.py
--rw-r--r--   0        0        0     2656 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py
--rw-r--r--   0        0        0     5008 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py
--rw-r--r--   0        0        0    14139 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/utils/__init__.py
--rw-r--r--   0        0        0      730 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/__init__.py
--rw-r--r--   0        0        0     1067 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.515855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/__init__.py
--rw-r--r--   0        0        0   372723 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/__init__.py
--rw-r--r--   0        0        0     5706 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py
--rw-r--r--   0        0        0     5235 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py
--rw-r--r--   0        0        0    14522 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py
--rw-r--r--   0        0        0        0 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/__init__.py
--rw-r--r--   0        0        0      694 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py
--rw-r--r--   0        0        0     2787 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_loader.py
--rw-r--r--   0        0        0     6393 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_monitor.py
--rw-r--r--   0        0        0     1701 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_plotter.py
--rw-r--r--   0        0        0     6284 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_runner.py
--rw-r--r--   0        0        0     3148 2023-01-11 13:24:47.519855 sdc_scissor-2.1.2/sdc_scissor/testing_api/test_validator.py
--rw-r--r--   0        0        0    13916 1970-01-01 00:00:00.000000 sdc_scissor-2.1.2/setup.py
--rw-r--r--   0        0        0    11992 1970-01-01 00:00:00.000000 sdc_scissor-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-02-15 16:15:19.486930 sdc_scissor-2.1.3/LICENSE.md
+-rw-r--r--   0        0        0    11027 2023-02-15 16:15:19.486930 sdc_scissor-2.1.3/README.md
+-rw-r--r--   0        0        0     1119 2023-02-15 16:15:19.590929 sdc_scissor-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/__init__.py
+-rw-r--r--   0        0        0    14526 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/cli.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/__init__.py
+-rw-r--r--   0        0        0     4779 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/angle_based_strategy.py
+-rw-r--r--   0        0        0     3980 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/equi_distance_strategy.py
+-rw-r--r--   0        0        0    10532 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/feature_extraction.py
+-rw-r--r--   0        0        0     2587 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py
+-rw-r--r--   0        0        0     3203 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/road_geometry_calculator.py
+-rw-r--r--   0        0        0      401 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/segmentation_strategy.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/machine_learning_api/__init__.py
+-rw-r--r--   0        0        0    10655 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py
+-rw-r--r--   0        0        0      334 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/machine_learning_api/csv_loader.py
+-rw-r--r--   0        0        0     7955 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/machine_learning_api/model_evaluator.py
+-rw-r--r--   0        0        0     2447 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/machine_learning_api/predictor.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/__init__.py
+-rw-r--r--   0        0        0      643 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/beamng_bump.py
+-rw-r--r--   0        0        0      569 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/beamng_delineator.py
+-rw-r--r--   0        0        0      764 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/beamng_obstacle_factory.py
+-rw-r--r--   0        0        0      675 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/beamng_tree.py
+-rw-r--r--   0        0        0      828 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/bump.py
+-rw-r--r--   0        0        0      160 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/carla_bump.py
+-rw-r--r--   0        0        0      190 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/carla_delineator.py
+-rw-r--r--   0        0        0      753 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/carla_obstacle_factory.py
+-rw-r--r--   0        0        0      159 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/carla_tree.py
+-rw-r--r--   0        0        0      664 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/delineator.py
+-rw-r--r--   0        0        0      522 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/obstacle_factory.py
+-rw-r--r--   0        0        0      709 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/obstacle_api/tree.py
+-rw-r--r--   0        0        0      965 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization
+-rw-r--r--   0        0        0       94 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/README.md
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/__init__.py
+-rw-r--r--   0        0        0      515 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/faultDetection.m
+-rw-r--r--   0        0        0     6436 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m
+-rw-r--r--   0        0        0      464 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/featureSelection.m
+-rw-r--r--   0        0        0      396 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/fitness.m
+-rw-r--r--   0        0        0     1084 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/initialPopulation.m
+-rw-r--r--   0        0        0      577 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/main.m
+-rw-r--r--   0        0        0      612 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/mainGreedy.m
+-rw-r--r--   0        0        0      221 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/objectives.m
+-rw-r--r--   0        0        0      760 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m
+-rw-r--r--   0        0        0     1516 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/permutationMutation.m
+-rw-r--r--   0        0        0      303 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/plotResults.m
+-rw-r--r--   0        0        0     1367 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py
+-rw-r--r--   0        0        0    10296 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R
+-rw-r--r--   0        0        0     5034 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf
+-rw-r--r--   0        0        0     2128 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv
+-rw-r--r--   0        0        0      125 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/medians_APFDc.csv
+-rw-r--r--   0        0        0     1877 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/plot.R
+-rw-r--r--   0        0        0     1724 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/table.R
+-rw-r--r--   0        0        0      394 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/utils.R
+-rw-r--r--   0        0        0      584 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv
+-rw-r--r--   0        0        0      958 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv
+-rw-r--r--   0        0        0     1057 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/runGreedy.m
+-rw-r--r--   0        0        0     4267 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/runMOSearch.m
+-rw-r--r--   0        0        0     3489 2023-02-15 16:15:19.638929 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/runSearch.m
+-rw-r--r--   0        0        0   239182 2023-02-15 16:15:19.642928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv
+-rw-r--r--   0        0        0  1146691 2023-02-15 16:15:19.650928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv
+-rw-r--r--   0        0        0   440097 2023-02-15 16:15:19.654928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv
+-rw-r--r--   0        0        0     1070 2023-02-15 16:15:19.654928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py
+-rw-r--r--   0        0        0   353423 2023-02-15 16:15:19.654928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv
+-rw-r--r--   0        0        0      661 2023-02-15 16:15:19.654928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md
+-rw-r--r--   0        0        0  1142098 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv
+-rw-r--r--   0        0        0     4434 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md
+-rw-r--r--   0        0        0      650 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh
+-rw-r--r--   0        0        0      724 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh
+-rw-r--r--   0        0        0       64 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/requirements.txt
+-rw-r--r--   0        0        0      324 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/setup.cfg
+-rw-r--r--   0        0        0       38 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/setup.py
+-rw-r--r--   0        0        0     2415 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/README.md
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/__init__.py
+-rw-r--r--   0        0        0      779 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py
+-rw-r--r--   0        0        0     1310 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py
+-rw-r--r--   0        0        0      844 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py
+-rw-r--r--   0        0        0     7915 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/run.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/simulator_api/__init__.py
+-rw-r--r--   0        0        0     1676 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/simulator_api/abstract_simulator.py
+-rw-r--r--   0        0        0     6672 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/simulator_api/beamng_simulator.py
+-rw-r--r--   0        0        0      807 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/simulator_api/simulator_factory.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/__init__.py
+-rw-r--r--   0        0        0      424 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/road_model.py
+-rw-r--r--   0        0        0     2324 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test.py
+-rw-r--r--   0        0        0     5482 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generator.py
+-rw-r--r--   0        0        0    13515 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py
+-rw-r--r--   0        0        0      304 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/duplicate_elimination.py
+-rw-r--r--   0        0        0      862 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py
+-rw-r--r--   0        0        0    13276 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py
+-rw-r--r--   0        0        0     2444 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py
+-rw-r--r--   0        0        0     2581 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py
+-rw-r--r--   0        0        0     3787 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py
+-rw-r--r--   0        0        0      587 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py
+-rw-r--r--   0        0        0     8894 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/__init__.py
+-rw-r--r--   0        0        0     2852 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py
+-rw-r--r--   0        0        0      575 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/config.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/__init__.py
+-rw-r--r--   0        0        0     1067 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.658928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/__init__.py
+-rw-r--r--   0        0        0   372723 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/__init__.py
+-rw-r--r--   0        0        0     2656 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py
+-rw-r--r--   0        0        0     5008 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py
+-rw-r--r--   0        0        0    14139 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/utils/__init__.py
+-rw-r--r--   0        0        0      730 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/__init__.py
+-rw-r--r--   0        0        0     1067 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/__init__.py
+-rw-r--r--   0        0        0   372723 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/__init__.py
+-rw-r--r--   0        0        0     5706 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py
+-rw-r--r--   0        0        0     5235 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py
+-rw-r--r--   0        0        0    14522 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py
+-rw-r--r--   0        0        0        0 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/__init__.py
+-rw-r--r--   0        0        0      694 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py
+-rw-r--r--   0        0        0     2787 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_loader.py
+-rw-r--r--   0        0        0     6393 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_monitor.py
+-rw-r--r--   0        0        0     1843 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_plotter.py
+-rw-r--r--   0        0        0     6333 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_runner.py
+-rw-r--r--   0        0        0     3148 2023-02-15 16:15:19.662928 sdc_scissor-2.1.3/sdc_scissor/testing_api/test_validator.py
+-rw-r--r--   0        0        0    13944 1970-01-01 00:00:00.000000 sdc_scissor-2.1.3/setup.py
+-rw-r--r--   0        0        0    12020 1970-01-01 00:00:00.000000 sdc_scissor-2.1.3/PKG-INFO
```

### Comparing `sdc_scissor-2.1.2/LICENSE.md` & `sdc_scissor-2.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/README.md` & `sdc_scissor-2.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,16 @@
   journal={ACM Transactions on Software Engineering and Methodology (TOSEM)},
   doi={10.1145/3533818}
 }
 ```
 
 ## Contacts
 * Christian Birchler
-    * Zurich University of Applied Science (ZHAW), Switzerland - birc@zhaw.ch
+    * Zurich University of Applied Sciences (ZHAW), Switzerland - birc@zhaw.ch
 * Nicolas Ganz
-    * Zurich University of Applied Science (ZHAW), Switzerland - gann@zhaw.ch
+    * Zurich University of Applied Sciences (ZHAW), Switzerland - gann@zhaw.ch
 * Sajad Khatiri
-    * Zurich University of Applied Science (ZHAW), Switzerland - mazr@zhaw.ch
+    * Zurich University of Applied Sciences (ZHAW), Switzerland - mazr@zhaw.ch
 * Dr. Alessio Gambi
-    * Passau University, Germany - alessio.gambi@uni-passau.de
+    * IMC University Of Applied Sciences Krems, Austria - alessio.gambi@fh-krems.ac.at
 * Dr. Sebastiano Panichella
-    * Zurich University of Applied Science (ZHAW), Switzerland - panc@zhaw.ch
+    * Zurich University of Applied Sciences (ZHAW), Switzerland - panc@zhaw.ch
```

### Comparing `sdc_scissor-2.1.2/pyproject.toml` & `sdc_scissor-2.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SDC-Scissor"
-version = "2.1.2"
+version = "2.1.3"
 description = "A cost-effective test selection for self-driving cars in virtual environments"
 authors = ["Christian Birchler <birchler.chr@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/ChristianBirchler/sdc-scissor"
 documentation = "https://sdc-scissor.readthedocs.io/"
 packages = [
```

### Comparing `sdc_scissor-2.1.2/sdc_scissor/cli.py` & `sdc_scissor-2.1.3/sdc_scissor/cli.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/angle_based_strategy.py` & `sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/angle_based_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/equi_distance_strategy.py` & `sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/equi_distance_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/feature_extraction.py` & `sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py` & `sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/feature_extraction_api/road_geometry_calculator.py` & `sdc_scissor-2.1.3/sdc_scissor/feature_extraction_api/road_geometry_calculator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py` & `sdc_scissor-2.1.3/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/machine_learning_api/model_evaluator.py` & `sdc_scissor-2.1.3/sdc_scissor/machine_learning_api/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/machine_learning_api/predictor.py` & `sdc_scissor-2.1.3/sdc_scissor/machine_learning_api/predictor.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/obstacle_api/beamng_bump.py` & `sdc_scissor-2.1.3/sdc_scissor/obstacle_api/beamng_bump.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/obstacle_api/beamng_delineator.py` & `sdc_scissor-2.1.3/sdc_scissor/obstacle_api/beamng_delineator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/obstacle_api/beamng_obstacle_factory.py` & `sdc_scissor-2.1.3/sdc_scissor/obstacle_api/beamng_obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/obstacle_api/beamng_tree.py` & `sdc_scissor-2.1.3/sdc_scissor/obstacle_api/beamng_tree.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/obstacle_api/bump.py` & `sdc_scissor-2.1.3/sdc_scissor/obstacle_api/bump.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/obstacle_api/carla_obstacle_factory.py` & `sdc_scissor-2.1.3/sdc_scissor/obstacle_api/carla_obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/obstacle_api/delineator.py` & `sdc_scissor-2.1.3/sdc_scissor/obstacle_api/delineator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/obstacle_api/obstacle_factory.py` & `sdc_scissor-2.1.3/sdc_scissor/obstacle_api/obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/obstacle_api/tree.py` & `sdc_scissor-2.1.3/sdc_scissor/obstacle_api/tree.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/faultDetection.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/faultDetection.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/initialPopulation.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/initialPopulation.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/main.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/main.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/mainGreedy.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/mainGreedy.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/permutationMutation.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/permutationMutation.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/plot.R` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/plot.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/table.R` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/table.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/runGreedy.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/runGreedy.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/runMOSearch.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/runMOSearch.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/code/runSearch.m` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/code/runSearch.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/README.md` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/sdc_prioritizer/testPrioritization/run.py` & `sdc_scissor-2.1.3/sdc_scissor/sdc_prioritizer/testPrioritization/run.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/simulator_api/abstract_simulator.py` & `sdc_scissor-2.1.3/sdc_scissor/simulator_api/abstract_simulator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/simulator_api/beamng_simulator.py` & `sdc_scissor-2.1.3/sdc_scissor/simulator_api/beamng_simulator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/simulator_api/simulator_factory.py` & `sdc_scissor-2.1.3/sdc_scissor/simulator_api/simulator_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generator.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/ambiegen/config.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/ambiegen/config.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_loader.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_loader.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_monitor.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_runner.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 
 from beamngpy import Scenario, BNGError
 from scipy.spatial.transform import Rotation
 
 from sdc_scissor.testing_api.test import Test
-from sdc_scissor.testing_api.test_plotter import TestPlotter
+from sdc_scissor.testing_api.test_plotter import TestPlotter, NullTestPlotter
 from sdc_scissor.testing_api.test_loader import TestLoader
 from sdc_scissor.testing_api.test_monitor import TestMonitor
 from sdc_scissor.testing_api.road_model import RoadModel
 from sdc_scissor.simulator_api.abstract_simulator import AbstractSimulator
 from sdc_scissor.obstacle_api.obstacle_factory import ObstacleFactory
 from sdc_scissor.testing_api.test_validator import TestIsNotValidException
 
@@ -78,15 +78,15 @@
         self.oob: float = kwargs.get("oob", None)
         self.interrupt: bool = kwargs.get("interrupt", None)
         self.bump_dist = kwargs.get("bump_dist", None)
         self.delineator_dist = kwargs.get("delineator_dist", None)
         self.tree_dist = kwargs.get("tree_dist", None)
         self.obstacle_factory: ObstacleFactory = kwargs.get("obstacle_factory", None)
         self.fov: list = kwargs.get("fov", None)
-        self.test_plotter: TestPlotter = TestPlotter()
+        self.test_plotter: TestPlotter = kwargs.get("test_plotter", NullTestPlotter())
 
     def run_test_suite(self):
         """ """
         logging.info("* run_test_suite")
         self.simulator.open()
         has_execution_failed = False
         test = None
```

### Comparing `sdc_scissor-2.1.2/sdc_scissor/testing_api/test_validator.py` & `sdc_scissor-2.1.3/sdc_scissor/testing_api/test_validator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.1.2/setup.py` & `sdc_scissor-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
  'scikit-learn>=1.0.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['sdc-scissor = sdc_scissor.cli:cli']}
 
 setup_kwargs = {
     'name': 'sdc-scissor',
-    'version': '2.1.2',
+    'version': '2.1.3',
     'description': 'A cost-effective test selection for self-driving cars in virtual environments',
-    'long_description': '# SDC-Scissor\n```{code-block} text\n ____    ____    ____              ____                                                \n/\\  _`\\ /\\  _`\\ /\\  _`\\           /\\  _`\\           __                                 \n\\ \\,\\L\\_\\ \\ \\/\\ \\ \\ \\/\\_\\         \\ \\,\\L\\_\\    ___ /\\_\\    ____    ____    ___   _ __  \n \\/_\\__ \\\\ \\ \\ \\ \\ \\ \\/_/_  _______\\/_\\__ \\   /\'___\\/\\ \\  /\',__\\  /\',__\\  / __`\\/\\`\'__\\\n   /\\ \\L\\ \\ \\ \\_\\ \\ \\ \\L\\ \\/\\______\\ /\\ \\L\\ \\/\\ \\__/\\ \\ \\/\\__, `\\/\\__, `\\/\\ \\L\\ \\ \\ \\/ \n   \\ `\\____\\ \\____/\\ \\____/\\/______/ \\ `\\____\\ \\____\\\\ \\_\\/\\____/\\/\\____/\\ \\____/\\ \\_\\ \n    \\/_____/\\/___/  \\/___/            \\/_____/\\/____/ \\/_/\\/___/  \\/___/  \\/___/  \\/_/ \n                                                                                       \n                                                                                       \n```\n[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)\n[![GitHub issues](https://img.shields.io/github/issues/ChristianBirchler/sdc-scissor)](https://github.com/ChristianBirchler/sdc-scissor/issues)\n[![GitHub forks](https://img.shields.io/github/forks/ChristianBirchler/sdc-scissor)](https://github.com/ChristianBirchler/sdc-scissor/network)\n[![GitHub stars](https://img.shields.io/github/stars/ChristianBirchler/sdc-scissor)](https://github.com/ChristianBirchler/sdc-scissor/stargazers)\n[![](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/ci.yml/badge.svg)](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/ci.yml)\n[![CD](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/cd.yml/badge.svg)](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/cd.yml)\n[![PyPI](https://img.shields.io/pypi/v/sdc-scissor)](https://pypi.org/project/sdc-scissor/)\n[![](https://readthedocs.org/projects/sdc-scissor/badge)](https://sdc-scissor.readthedocs.io)\n[![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=alert_status)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=ncloc)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=coverage)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=sqale_index)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=reliability_rating)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=duplicated_lines_density)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=vulnerabilities)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=bugs)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=security_rating)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=sqale_rating)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=code_smells)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![DOI](https://zenodo.org/badge/363107094.svg)](https://zenodo.org/badge/latestdoi/363107094)\n<div style="text-align: center;">\n<a href="https://github.com/ChristianBirchler/sdc-scissor">\n<img src="https://raw.githubusercontent.com/ChristianBirchler/sdc-scissor/main/docs/images/github_logo_icon.png">\n</a>\n<a href="https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor">\n<img src="https://sonarcloud.io/images/project_badges/sonarcloud-black.svg">\n</a>\n</div>\n\n## A Tool for Cost-effective Simulation-based Test Selection in Self-driving Cars Software\nSDC-Scissor is a tool that let you test self-driving cars more efficiently in simulation. It uses a machine-learning\napproach to select only relevant test scenarios so that the testing process is faster. Furthermore, the selected tests\nare diverse and try to challenge the car with corner cases.\n\nFurthermore, this repository contains also code for test multi-objective test case prioritization with an evolutionary\ngenetic search algorithm. If you are interested in prioritizing test cases, then you should read the dedicated\n[README.md](https://github.com/ChristianBirchler/sdc-scissor/blob/main/sdc_scissor/sdc_prioritizer/testPrioritization/README.md)\nfor this. If you use the prioritization technique then also cite the papers from the reference section!\n\n## Support\nWe use [GitHub Discussions](https://github.com/ChristianBirchler/sdc-scissor/discussions) as a community platform. You\ncan ask questions and get support there from the community. Furthermore, new features and releases will be discussed and\nannounced there.\n\n## Documentation\nFor the documentation follow the link: [sdc-scissor.readthedocs.io](https://sdc-scissor.readthedocs.io/en/latest/)\n\n[![](https://raw.githubusercontent.com/ChristianBirchler/sdc-scissor/main/docs/images/readthedocs.png)](https://sdc-scissor.readthedocs.io/en/latest/)\n\n## License\n```{code-block} text\nSDC-Scissor tool for cost-effective simulation-based test selection\nin self-driving cars software.\nCopyright (C) 2022  Christian Birchler\n\nThis program is free software: you can redistribute it and/or modify\nit under the terms of the GNU General Public License as published by\nthe Free Software Foundation, either version 3 of the License, or\n(at your option) any later version.\n\nThis program is distributed in the hope that it will be useful,\nbut WITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\nGNU General Public License for more details.\n\nYou should have received a copy of the GNU General Public License\nalong with this program.  If not, see <https://www.gnu.org/licenses/>.\n```\n\nThe software we developed is distributed under GNU GPL license. See the\n[LICENSE.md](https://github.com/ChristianBirchler/sdc-scissor/blob/main/LICENSE.md) file.\n\n## References\nIf you use this tool in your research, please cite the following papers:\n\n- **Christian Birchler**, Nicolas Ganz, Sajad Khatiri, Alessio Gambi, and Sebastiano Panichella, "Cost-effective Simulation-based Test Selection in Self-driving Cars Software with SDC-Scissor," *In 2022 IEEE 29th International Conference on Software Analysis, Evolution and Reengineering (SANER)*, pp. 164-168, doi: 10.1109/SANER53432.2022.00030.\n  - [IEEE Xplore](https://doi.org/10.1109/SANER53432.2022.00030)\n  - [Preprint](https://doi.org/10.21256/zhaw-24017)\n  - [GitHub](https://github.com/ChristianBirchler/sdc-scissor)\n````{code-block} bibtex\n@inproceedings{Birchler2022Cost1,\n  author={Birchler, Christian and Ganz, Nicolas and Khatiri, Sajad and Gambi, Alessio, and Panichella, Sebastiano},\n  booktitle={2022 IEEE 29th International Conference on Software Analysis, Evolution and Reengineering (SANER)},\n  title={Cost-effective Simulationbased Test Selection in Self-driving Cars Software with SDC-Scissor},\n  year={2022},\n  doi={10.1109/SANER53432.2022.00030}\n}\n````\n- **Christian Birchler**, Nicolas Ganz, Sajad Khatiri, Alessio Gambi, and Sebastiano Panichella, "Cost-effective Simulation-based Test Selection in Self-driving Cars Software," *Science of Computer Programming (SCP)*, doi: to appear, 2022.\n  - [Accepted manuscript version](https://doi.org/10.48550/arXiv.2211.11409)\n````{code-block} bibtex\n@article{Birchler2022Cost2,\n  author    = {Christian Birchler and Nicolas Ganz and Sajad Khatiri and Alessio Gambi and Sebastiano Panichella},\n  title     = {Cost-effective Simulation-based Test Selection in Self-driving Cars Software},\n  journal   = {Science of Computer Programming (SCP)},\n  year      = {2022},\n  doi       = {to appear},\n  eprinttype = {arXiv},\n  eprint    = {2211.11409}\n}\n````\n- **Christian Birchler**, Sajad Khatiri, Bill Bosshard, Alessio Gambi, and Sebastiano Panichella, "Machine Learning-based Test Selection for Simulation-based Testing of Self-driving Cars Software," *Empirical Software Engineering (EMSE)*, doi: to appear, 2022.\n  - [Preprint](https://doi.org/10.48550/arXiv.2212.04769)\n````{code-block} bibtex\n@article{Birchler2022Machine,\n  author    = {Christian Birchler and Sajad Khatiri and Bill Bosshard and Alessio Gambi and Sebastiano Panichella},\n  title     = {Machine Learning-based Test Selection for Simulation-based Testing of Self-driving Cars Software},\n  journal   = {Empirical Software Engineering (EMSE)},\n  year      = {2022},\n  doi       = {to appear},\n  eprinttype = {arXiv},\n  eprint    = {2212.04769}\n}\n````\n- **Christian Birchler**, Sajad Khatiri, Pouria Derakhshanfar, Sebastiano Panichella, and Annibale Panichella, "Single and Multi-objective Test Cases Prioritization for Self-driving Cars in Virtual Environments," *ACM Transactions on Software Engineering and Methodology (TOSEM)*, doi: 10.1145/3533818, 2022.\n  - [ACM Digital Library](https://doi.org/10.1145/3533818)\n  - [Preprint](https://doi.org/10.48550/arXiv.2107.09614)\n```{code-block} bibtex\n@article{Birchler2022Single,\n  author={Birchler, Christian and Khatiri, Sajad and Derakhshanfar, Pouria and Panichella, Sebastiano and Panichella, Annibale},\n  title={Single and Multi-objective Test Cases Prioritization for Self-driving Cars in Virtual Environments},\n  year={2022},\n  publisher={Association for Computing Machinery},\n  journal={ACM Transactions on Software Engineering and Methodology (TOSEM)},\n  doi={10.1145/3533818}\n}\n```\n\n## Contacts\n* Christian Birchler\n    * Zurich University of Applied Science (ZHAW), Switzerland - birc@zhaw.ch\n* Nicolas Ganz\n    * Zurich University of Applied Science (ZHAW), Switzerland - gann@zhaw.ch\n* Sajad Khatiri\n    * Zurich University of Applied Science (ZHAW), Switzerland - mazr@zhaw.ch\n* Dr. Alessio Gambi\n    * Passau University, Germany - alessio.gambi@uni-passau.de\n* Dr. Sebastiano Panichella\n    * Zurich University of Applied Science (ZHAW), Switzerland - panc@zhaw.ch\n',
+    'long_description': '# SDC-Scissor\n```{code-block} text\n ____    ____    ____              ____                                                \n/\\  _`\\ /\\  _`\\ /\\  _`\\           /\\  _`\\           __                                 \n\\ \\,\\L\\_\\ \\ \\/\\ \\ \\ \\/\\_\\         \\ \\,\\L\\_\\    ___ /\\_\\    ____    ____    ___   _ __  \n \\/_\\__ \\\\ \\ \\ \\ \\ \\ \\/_/_  _______\\/_\\__ \\   /\'___\\/\\ \\  /\',__\\  /\',__\\  / __`\\/\\`\'__\\\n   /\\ \\L\\ \\ \\ \\_\\ \\ \\ \\L\\ \\/\\______\\ /\\ \\L\\ \\/\\ \\__/\\ \\ \\/\\__, `\\/\\__, `\\/\\ \\L\\ \\ \\ \\/ \n   \\ `\\____\\ \\____/\\ \\____/\\/______/ \\ `\\____\\ \\____\\\\ \\_\\/\\____/\\/\\____/\\ \\____/\\ \\_\\ \n    \\/_____/\\/___/  \\/___/            \\/_____/\\/____/ \\/_/\\/___/  \\/___/  \\/___/  \\/_/ \n                                                                                       \n                                                                                       \n```\n[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)\n[![GitHub issues](https://img.shields.io/github/issues/ChristianBirchler/sdc-scissor)](https://github.com/ChristianBirchler/sdc-scissor/issues)\n[![GitHub forks](https://img.shields.io/github/forks/ChristianBirchler/sdc-scissor)](https://github.com/ChristianBirchler/sdc-scissor/network)\n[![GitHub stars](https://img.shields.io/github/stars/ChristianBirchler/sdc-scissor)](https://github.com/ChristianBirchler/sdc-scissor/stargazers)\n[![](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/ci.yml/badge.svg)](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/ci.yml)\n[![CD](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/cd.yml/badge.svg)](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/cd.yml)\n[![PyPI](https://img.shields.io/pypi/v/sdc-scissor)](https://pypi.org/project/sdc-scissor/)\n[![](https://readthedocs.org/projects/sdc-scissor/badge)](https://sdc-scissor.readthedocs.io)\n[![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=alert_status)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=ncloc)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=coverage)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=sqale_index)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=reliability_rating)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=duplicated_lines_density)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=vulnerabilities)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=bugs)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=security_rating)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=sqale_rating)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=code_smells)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)\n[![DOI](https://zenodo.org/badge/363107094.svg)](https://zenodo.org/badge/latestdoi/363107094)\n<div style="text-align: center;">\n<a href="https://github.com/ChristianBirchler/sdc-scissor">\n<img src="https://raw.githubusercontent.com/ChristianBirchler/sdc-scissor/main/docs/images/github_logo_icon.png">\n</a>\n<a href="https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor">\n<img src="https://sonarcloud.io/images/project_badges/sonarcloud-black.svg">\n</a>\n</div>\n\n## A Tool for Cost-effective Simulation-based Test Selection in Self-driving Cars Software\nSDC-Scissor is a tool that let you test self-driving cars more efficiently in simulation. It uses a machine-learning\napproach to select only relevant test scenarios so that the testing process is faster. Furthermore, the selected tests\nare diverse and try to challenge the car with corner cases.\n\nFurthermore, this repository contains also code for test multi-objective test case prioritization with an evolutionary\ngenetic search algorithm. If you are interested in prioritizing test cases, then you should read the dedicated\n[README.md](https://github.com/ChristianBirchler/sdc-scissor/blob/main/sdc_scissor/sdc_prioritizer/testPrioritization/README.md)\nfor this. If you use the prioritization technique then also cite the papers from the reference section!\n\n## Support\nWe use [GitHub Discussions](https://github.com/ChristianBirchler/sdc-scissor/discussions) as a community platform. You\ncan ask questions and get support there from the community. Furthermore, new features and releases will be discussed and\nannounced there.\n\n## Documentation\nFor the documentation follow the link: [sdc-scissor.readthedocs.io](https://sdc-scissor.readthedocs.io/en/latest/)\n\n[![](https://raw.githubusercontent.com/ChristianBirchler/sdc-scissor/main/docs/images/readthedocs.png)](https://sdc-scissor.readthedocs.io/en/latest/)\n\n## License\n```{code-block} text\nSDC-Scissor tool for cost-effective simulation-based test selection\nin self-driving cars software.\nCopyright (C) 2022  Christian Birchler\n\nThis program is free software: you can redistribute it and/or modify\nit under the terms of the GNU General Public License as published by\nthe Free Software Foundation, either version 3 of the License, or\n(at your option) any later version.\n\nThis program is distributed in the hope that it will be useful,\nbut WITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\nGNU General Public License for more details.\n\nYou should have received a copy of the GNU General Public License\nalong with this program.  If not, see <https://www.gnu.org/licenses/>.\n```\n\nThe software we developed is distributed under GNU GPL license. See the\n[LICENSE.md](https://github.com/ChristianBirchler/sdc-scissor/blob/main/LICENSE.md) file.\n\n## References\nIf you use this tool in your research, please cite the following papers:\n\n- **Christian Birchler**, Nicolas Ganz, Sajad Khatiri, Alessio Gambi, and Sebastiano Panichella, "Cost-effective Simulation-based Test Selection in Self-driving Cars Software with SDC-Scissor," *In 2022 IEEE 29th International Conference on Software Analysis, Evolution and Reengineering (SANER)*, pp. 164-168, doi: 10.1109/SANER53432.2022.00030.\n  - [IEEE Xplore](https://doi.org/10.1109/SANER53432.2022.00030)\n  - [Preprint](https://doi.org/10.21256/zhaw-24017)\n  - [GitHub](https://github.com/ChristianBirchler/sdc-scissor)\n````{code-block} bibtex\n@inproceedings{Birchler2022Cost1,\n  author={Birchler, Christian and Ganz, Nicolas and Khatiri, Sajad and Gambi, Alessio, and Panichella, Sebastiano},\n  booktitle={2022 IEEE 29th International Conference on Software Analysis, Evolution and Reengineering (SANER)},\n  title={Cost-effective Simulationbased Test Selection in Self-driving Cars Software with SDC-Scissor},\n  year={2022},\n  doi={10.1109/SANER53432.2022.00030}\n}\n````\n- **Christian Birchler**, Nicolas Ganz, Sajad Khatiri, Alessio Gambi, and Sebastiano Panichella, "Cost-effective Simulation-based Test Selection in Self-driving Cars Software," *Science of Computer Programming (SCP)*, doi: to appear, 2022.\n  - [Accepted manuscript version](https://doi.org/10.48550/arXiv.2211.11409)\n````{code-block} bibtex\n@article{Birchler2022Cost2,\n  author    = {Christian Birchler and Nicolas Ganz and Sajad Khatiri and Alessio Gambi and Sebastiano Panichella},\n  title     = {Cost-effective Simulation-based Test Selection in Self-driving Cars Software},\n  journal   = {Science of Computer Programming (SCP)},\n  year      = {2022},\n  doi       = {to appear},\n  eprinttype = {arXiv},\n  eprint    = {2211.11409}\n}\n````\n- **Christian Birchler**, Sajad Khatiri, Bill Bosshard, Alessio Gambi, and Sebastiano Panichella, "Machine Learning-based Test Selection for Simulation-based Testing of Self-driving Cars Software," *Empirical Software Engineering (EMSE)*, doi: to appear, 2022.\n  - [Preprint](https://doi.org/10.48550/arXiv.2212.04769)\n````{code-block} bibtex\n@article{Birchler2022Machine,\n  author    = {Christian Birchler and Sajad Khatiri and Bill Bosshard and Alessio Gambi and Sebastiano Panichella},\n  title     = {Machine Learning-based Test Selection for Simulation-based Testing of Self-driving Cars Software},\n  journal   = {Empirical Software Engineering (EMSE)},\n  year      = {2022},\n  doi       = {to appear},\n  eprinttype = {arXiv},\n  eprint    = {2212.04769}\n}\n````\n- **Christian Birchler**, Sajad Khatiri, Pouria Derakhshanfar, Sebastiano Panichella, and Annibale Panichella, "Single and Multi-objective Test Cases Prioritization for Self-driving Cars in Virtual Environments," *ACM Transactions on Software Engineering and Methodology (TOSEM)*, doi: 10.1145/3533818, 2022.\n  - [ACM Digital Library](https://doi.org/10.1145/3533818)\n  - [Preprint](https://doi.org/10.48550/arXiv.2107.09614)\n```{code-block} bibtex\n@article{Birchler2022Single,\n  author={Birchler, Christian and Khatiri, Sajad and Derakhshanfar, Pouria and Panichella, Sebastiano and Panichella, Annibale},\n  title={Single and Multi-objective Test Cases Prioritization for Self-driving Cars in Virtual Environments},\n  year={2022},\n  publisher={Association for Computing Machinery},\n  journal={ACM Transactions on Software Engineering and Methodology (TOSEM)},\n  doi={10.1145/3533818}\n}\n```\n\n## Contacts\n* Christian Birchler\n    * Zurich University of Applied Sciences (ZHAW), Switzerland - birc@zhaw.ch\n* Nicolas Ganz\n    * Zurich University of Applied Sciences (ZHAW), Switzerland - gann@zhaw.ch\n* Sajad Khatiri\n    * Zurich University of Applied Sciences (ZHAW), Switzerland - mazr@zhaw.ch\n* Dr. Alessio Gambi\n    * IMC University Of Applied Sciences Krems, Austria - alessio.gambi@fh-krems.ac.at\n* Dr. Sebastiano Panichella\n    * Zurich University of Applied Sciences (ZHAW), Switzerland - panc@zhaw.ch\n',
     'author': 'Christian Birchler',
     'author_email': 'birchler.chr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ChristianBirchler/sdc-scissor',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sdc_scissor-2.1.2/PKG-INFO` & `sdc_scissor-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdc-scissor
-Version: 2.1.2
+Version: 2.1.3
 Summary: A cost-effective test selection for self-driving cars in virtual environments
 Home-page: https://github.com/ChristianBirchler/sdc-scissor
 License: GPL-3.0-or-later
 Author: Christian Birchler
 Author-email: birchler.chr@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -162,17 +162,17 @@
   journal={ACM Transactions on Software Engineering and Methodology (TOSEM)},
   doi={10.1145/3533818}
 }
 ```
 
 ## Contacts
 * Christian Birchler
-    * Zurich University of Applied Science (ZHAW), Switzerland - birc@zhaw.ch
+    * Zurich University of Applied Sciences (ZHAW), Switzerland - birc@zhaw.ch
 * Nicolas Ganz
-    * Zurich University of Applied Science (ZHAW), Switzerland - gann@zhaw.ch
+    * Zurich University of Applied Sciences (ZHAW), Switzerland - gann@zhaw.ch
 * Sajad Khatiri
-    * Zurich University of Applied Science (ZHAW), Switzerland - mazr@zhaw.ch
+    * Zurich University of Applied Sciences (ZHAW), Switzerland - mazr@zhaw.ch
 * Dr. Alessio Gambi
-    * Passau University, Germany - alessio.gambi@uni-passau.de
+    * IMC University Of Applied Sciences Krems, Austria - alessio.gambi@fh-krems.ac.at
 * Dr. Sebastiano Panichella
-    * Zurich University of Applied Science (ZHAW), Switzerland - panc@zhaw.ch
+    * Zurich University of Applied Sciences (ZHAW), Switzerland - panc@zhaw.ch
```

