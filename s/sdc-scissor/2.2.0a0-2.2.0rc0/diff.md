# Comparing `tmp/sdc_scissor-2.2.0a0.tar.gz` & `tmp/sdc_scissor-2.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdc_scissor-2.2.0a0.tar", max compression
+gzip compressed data, was "sdc_scissor-2.2.0rc0.tar", max compression
```

## Comparing `sdc_scissor-2.2.0a0.tar` & `sdc_scissor-2.2.0rc0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0    34916 2023-05-24 04:33:22.881389 sdc_scissor-2.2.0a0/LICENSE.md
--rw-r--r--   0        0        0    10767 2023-05-24 04:33:22.881389 sdc_scissor-2.2.0a0/README.md
--rw-r--r--   0        0        0     1460 2023-05-24 04:33:22.973389 sdc_scissor-2.2.0a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/can_api/__init__.py
--rw-r--r--   0        0        0     4480 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/can_api/can_bus_handler.py
--rw-r--r--   0        0        0     1730 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/can_api/can_msg_generator.py
--rw-r--r--   0        0        0     3547 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/can_api/can_output.py
--rw-r--r--   0        0        0    18875 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/cli.py
--rw-r--r--   0        0        0     1448 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/config.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/__init__.py
--rw-r--r--   0        0        0     4763 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/angle_based_strategy.py
--rw-r--r--   0        0        0     3980 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/equi_distance_strategy.py
--rw-r--r--   0        0        0    10519 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/feature_extraction.py
--rw-r--r--   0        0        0     2587 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py
--rw-r--r--   0        0        0     3203 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/road_geometry_calculator.py
--rw-r--r--   0        0        0      401 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/segmentation_strategy.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/machine_learning_api/__init__.py
--rw-r--r--   0        0        0     9597 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py
--rw-r--r--   0        0        0      255 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/machine_learning_api/csv_loader.py
--rw-r--r--   0        0        0     7726 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/machine_learning_api/model_evaluator.py
--rw-r--r--   0        0        0     2382 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/machine_learning_api/predictor.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/__init__.py
--rw-r--r--   0        0        0      643 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/beamng_bump.py
--rw-r--r--   0        0        0      569 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/beamng_delineator.py
--rw-r--r--   0        0        0      764 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/beamng_obstacle_factory.py
--rw-r--r--   0        0        0      675 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/beamng_tree.py
--rw-r--r--   0        0        0      828 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/bump.py
--rw-r--r--   0        0        0      160 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/carla_bump.py
--rw-r--r--   0        0        0      190 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/carla_delineator.py
--rw-r--r--   0        0        0      753 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/carla_obstacle_factory.py
--rw-r--r--   0        0        0      160 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/carla_tree.py
--rw-r--r--   0        0        0      664 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/delineator.py
--rw-r--r--   0        0        0      522 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/obstacle_factory.py
--rw-r--r--   0        0        0      709 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/tree.py
--rw-r--r--   0        0        0      966 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization
--rw-r--r--   0        0        0       95 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/README.md
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/__init__.py
--rw-r--r--   0        0        0      510 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/faultDetection.m
--rw-r--r--   0        0        0     6298 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m
--rw-r--r--   0        0        0      463 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/featureSelection.m
--rw-r--r--   0        0        0      391 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/fitness.m
--rw-r--r--   0        0        0     1075 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/initialPopulation.m
--rw-r--r--   0        0        0      574 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/main.m
--rw-r--r--   0        0        0      609 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/mainGreedy.m
--rw-r--r--   0        0        0      220 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/objectives.m
--rw-r--r--   0        0        0      750 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m
--rw-r--r--   0        0        0     1501 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/permutationMutation.m
--rw-r--r--   0        0        0      302 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/plotResults.m
--rw-r--r--   0        0        0     1367 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py
--rw-r--r--   0        0        0    10251 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R
--rw-r--r--   0        0        0     5034 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf
--rw-r--r--   0        0        0     2128 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv
--rw-r--r--   0        0        0      125 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/medians_APFDc.csv
--rw-r--r--   0        0        0     1869 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/plot.R
--rw-r--r--   0        0        0     1694 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/table.R
--rw-r--r--   0        0        0      395 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/utils.R
--rw-r--r--   0        0        0      584 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv
--rw-r--r--   0        0        0      958 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv
--rw-r--r--   0        0        0     1051 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/runGreedy.m
--rw-r--r--   0        0        0     4258 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/runMOSearch.m
--rw-r--r--   0        0        0     3480 2023-05-24 04:33:23.017390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/runSearch.m
--rw-r--r--   0        0        0   239182 2023-05-24 04:33:23.021390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv
--rw-r--r--   0        0        0  1146691 2023-05-24 04:33:23.029390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv
--rw-r--r--   0        0        0   440097 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv
--rw-r--r--   0        0        0     1070 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py
--rw-r--r--   0        0        0   353423 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv
--rw-r--r--   0        0        0      660 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md
--rw-r--r--   0        0        0  1142098 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv
--rw-r--r--   0        0        0     4431 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md
--rw-r--r--   0        0        0      650 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh
--rw-r--r--   0        0        0      725 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh
--rw-r--r--   0        0        0       65 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/requirements.txt
--rw-r--r--   0        0        0      324 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/setup.cfg
--rw-r--r--   0        0        0       38 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/setup.py
--rw-r--r--   0        0        0     2413 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/README.md
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/__init__.py
--rw-r--r--   0        0        0      780 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py
--rw-r--r--   0        0        0     1306 2023-05-24 04:33:23.033390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py
--rw-r--r--   0        0        0      843 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py
--rw-r--r--   0        0        0     7798 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/run.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/simulator_api/__init__.py
--rw-r--r--   0        0        0     1661 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/simulator_api/abstract_simulator.py
--rw-r--r--   0        0        0     6672 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/simulator_api/beamng_simulator.py
--rw-r--r--   0        0        0      807 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/simulator_api/simulator_factory.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/__init__.py
--rw-r--r--   0        0        0      424 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/road_model.py
--rw-r--r--   0        0        0     2323 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test.py
--rw-r--r--   0        0        0     5482 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generator.py
--rw-r--r--   0        0        0    13513 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py
--rw-r--r--   0        0        0      304 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/duplicate_elimination.py
--rw-r--r--   0        0        0      862 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py
--rw-r--r--   0        0        0    13276 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py
--rw-r--r--   0        0        0     2443 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py
--rw-r--r--   0        0        0     2580 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py
--rw-r--r--   0        0        0     3786 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py
--rw-r--r--   0        0        0      587 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py
--rw-r--r--   0        0        0     8854 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py
--rw-r--r--   0        0        0      575 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/config.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/__init__.py
--rw-r--r--   0        0        0     1067 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/__init__.py
--rw-r--r--   0        0        0   372723 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/__init__.py
--rw-r--r--   0        0        0     2658 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py
--rw-r--r--   0        0        0     4908 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py
--rw-r--r--   0        0        0    14117 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/utils/__init__.py
--rw-r--r--   0        0        0      731 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/__init__.py
--rw-r--r--   0        0        0     1067 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.037390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/__init__.py
--rw-r--r--   0        0        0   372723 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/__init__.py
--rw-r--r--   0        0        0     5693 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py
--rw-r--r--   0        0        0     5135 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py
--rw-r--r--   0        0        0    14499 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py
--rw-r--r--   0        0        0        0 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/__init__.py
--rw-r--r--   0        0        0      694 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py
--rw-r--r--   0        0        0     2762 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_loader.py
--rw-r--r--   0        0        0     6630 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_monitor.py
--rw-r--r--   0        0        0     1843 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_plotter.py
--rw-r--r--   0        0        0     6954 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_runner.py
--rw-r--r--   0        0        0     3150 2023-05-24 04:33:23.041390 sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_validator.py
--rw-r--r--   0        0        0    11900 1970-01-01 00:00:00.000000 sdc_scissor-2.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-05-24 05:05:14.501191 sdc_scissor-2.2.0rc0/LICENSE.md
+-rw-r--r--   0        0        0    10829 2023-05-24 05:05:14.501191 sdc_scissor-2.2.0rc0/README.md
+-rw-r--r--   0        0        0     1461 2023-05-24 05:05:14.609191 sdc_scissor-2.2.0rc0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/can_api/__init__.py
+-rw-r--r--   0        0        0     4668 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/can_api/can_bus_handler.py
+-rw-r--r--   0        0        0     1730 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/can_api/can_msg_generator.py
+-rw-r--r--   0        0        0     3907 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/can_api/can_output.py
+-rw-r--r--   0        0        0    18875 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/cli.py
+-rw-r--r--   0        0        0     1448 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/config.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/__init__.py
+-rw-r--r--   0        0        0     4763 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/angle_based_strategy.py
+-rw-r--r--   0        0        0     3980 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/equi_distance_strategy.py
+-rw-r--r--   0        0        0    10519 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/feature_extraction.py
+-rw-r--r--   0        0        0     2587 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py
+-rw-r--r--   0        0        0     3203 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/road_geometry_calculator.py
+-rw-r--r--   0        0        0      401 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/segmentation_strategy.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/machine_learning_api/__init__.py
+-rw-r--r--   0        0        0     9597 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py
+-rw-r--r--   0        0        0      255 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/machine_learning_api/csv_loader.py
+-rw-r--r--   0        0        0     7726 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/machine_learning_api/model_evaluator.py
+-rw-r--r--   0        0        0     2382 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/machine_learning_api/predictor.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/__init__.py
+-rw-r--r--   0        0        0      643 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/beamng_bump.py
+-rw-r--r--   0        0        0      569 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/beamng_delineator.py
+-rw-r--r--   0        0        0      764 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/beamng_obstacle_factory.py
+-rw-r--r--   0        0        0      675 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/beamng_tree.py
+-rw-r--r--   0        0        0      828 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/bump.py
+-rw-r--r--   0        0        0      160 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/carla_bump.py
+-rw-r--r--   0        0        0      190 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/carla_delineator.py
+-rw-r--r--   0        0        0      753 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/carla_obstacle_factory.py
+-rw-r--r--   0        0        0      160 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/carla_tree.py
+-rw-r--r--   0        0        0      664 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/delineator.py
+-rw-r--r--   0        0        0      522 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/obstacle_factory.py
+-rw-r--r--   0        0        0      709 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/tree.py
+-rw-r--r--   0        0        0      966 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization
+-rw-r--r--   0        0        0       95 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/__init__.py
+-rw-r--r--   0        0        0      510 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/faultDetection.m
+-rw-r--r--   0        0        0     6298 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m
+-rw-r--r--   0        0        0      463 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/featureSelection.m
+-rw-r--r--   0        0        0      391 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/fitness.m
+-rw-r--r--   0        0        0     1075 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/initialPopulation.m
+-rw-r--r--   0        0        0      574 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/main.m
+-rw-r--r--   0        0        0      609 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/mainGreedy.m
+-rw-r--r--   0        0        0      220 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/objectives.m
+-rw-r--r--   0        0        0      750 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m
+-rw-r--r--   0        0        0     1501 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/permutationMutation.m
+-rw-r--r--   0        0        0      302 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/plotResults.m
+-rw-r--r--   0        0        0     1367 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py
+-rw-r--r--   0        0        0    10251 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R
+-rw-r--r--   0        0        0     5034 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf
+-rw-r--r--   0        0        0     2128 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv
+-rw-r--r--   0        0        0      125 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/medians_APFDc.csv
+-rw-r--r--   0        0        0     1869 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/plot.R
+-rw-r--r--   0        0        0     1694 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/table.R
+-rw-r--r--   0        0        0      395 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/utils.R
+-rw-r--r--   0        0        0      584 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv
+-rw-r--r--   0        0        0      958 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv
+-rw-r--r--   0        0        0     1051 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/runGreedy.m
+-rw-r--r--   0        0        0     4258 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/runMOSearch.m
+-rw-r--r--   0        0        0     3480 2023-05-24 05:05:14.657191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/runSearch.m
+-rw-r--r--   0        0        0   239182 2023-05-24 05:05:14.661191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv
+-rw-r--r--   0        0        0  1146691 2023-05-24 05:05:14.669191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv
+-rw-r--r--   0        0        0   440097 2023-05-24 05:05:14.673191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv
+-rw-r--r--   0        0        0     1070 2023-05-24 05:05:14.673191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py
+-rw-r--r--   0        0        0   353423 2023-05-24 05:05:14.673191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv
+-rw-r--r--   0        0        0      660 2023-05-24 05:05:14.673191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md
+-rw-r--r--   0        0        0  1142098 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv
+-rw-r--r--   0        0        0     4431 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md
+-rw-r--r--   0        0        0      650 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh
+-rw-r--r--   0        0        0      725 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh
+-rw-r--r--   0        0        0       65 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/requirements.txt
+-rw-r--r--   0        0        0      324 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/setup.cfg
+-rw-r--r--   0        0        0       38 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/setup.py
+-rw-r--r--   0        0        0     2413 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/__init__.py
+-rw-r--r--   0        0        0      780 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py
+-rw-r--r--   0        0        0     1306 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py
+-rw-r--r--   0        0        0      843 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py
+-rw-r--r--   0        0        0     7798 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/run.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/simulator_api/__init__.py
+-rw-r--r--   0        0        0     1661 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/simulator_api/abstract_simulator.py
+-rw-r--r--   0        0        0     6672 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/simulator_api/beamng_simulator.py
+-rw-r--r--   0        0        0      807 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/simulator_api/simulator_factory.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/__init__.py
+-rw-r--r--   0        0        0      424 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/road_model.py
+-rw-r--r--   0        0        0     2323 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test.py
+-rw-r--r--   0        0        0     5482 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generator.py
+-rw-r--r--   0        0        0    13513 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py
+-rw-r--r--   0        0        0      304 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/duplicate_elimination.py
+-rw-r--r--   0        0        0      862 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py
+-rw-r--r--   0        0        0    13276 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py
+-rw-r--r--   0        0        0     2443 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py
+-rw-r--r--   0        0        0     2580 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py
+-rw-r--r--   0        0        0     3786 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py
+-rw-r--r--   0        0        0      587 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py
+-rw-r--r--   0        0        0     8854 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/__init__.py
+-rw-r--r--   0        0        0     2829 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py
+-rw-r--r--   0        0        0      575 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/config.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/__init__.py
+-rw-r--r--   0        0        0     1067 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.677191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/__init__.py
+-rw-r--r--   0        0        0   372723 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/__init__.py
+-rw-r--r--   0        0        0     2658 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py
+-rw-r--r--   0        0        0     4908 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py
+-rw-r--r--   0        0        0    14117 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/utils/__init__.py
+-rw-r--r--   0        0        0      731 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/__init__.py
+-rw-r--r--   0        0        0     1067 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/__init__.py
+-rw-r--r--   0        0        0   372723 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/__init__.py
+-rw-r--r--   0        0        0     5693 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py
+-rw-r--r--   0        0        0     5135 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py
+-rw-r--r--   0        0        0    14499 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/__init__.py
+-rw-r--r--   0        0        0      694 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py
+-rw-r--r--   0        0        0     2762 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_loader.py
+-rw-r--r--   0        0        0     6630 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_monitor.py
+-rw-r--r--   0        0        0     1843 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_plotter.py
+-rw-r--r--   0        0        0     6954 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_runner.py
+-rw-r--r--   0        0        0     3150 2023-05-24 05:05:14.681191 sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_validator.py
+-rw-r--r--   0        0        0    11963 1970-01-01 00:00:00.000000 sdc_scissor-2.2.0rc0/PKG-INFO
```

### Comparing `sdc_scissor-2.2.0a0/LICENSE.md` & `sdc_scissor-2.2.0rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/README.md` & `sdc_scissor-2.2.0rc0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -96,25 +96,27 @@
   author={Birchler, Christian and Ganz, Nicolas and Khatiri, Sajad and Gambi, Alessio, and Panichella, Sebastiano},
   booktitle={2022 IEEE 29th International Conference on Software Analysis, Evolution and Reengineering (SANER)},
   title={Cost-effective Simulationbased Test Selection in Self-driving Cars Software with SDC-Scissor},
   year={2022},
   doi={10.1109/SANER53432.2022.00030}
 }
 ````
-- **Christian Birchler**, Nicolas Ganz, Sajad Khatiri, Alessio Gambi, and Sebastiano Panichella, "Cost-effective Simulation-based Test Selection in Self-driving Cars Software," *Science of Computer Programming (SCP)*, doi: to appear, 2022.
-  - [Accepted manuscript version](https://doi.org/10.48550/arXiv.2211.11409)
+- **Christian Birchler**, Nicolas Ganz, Sajad Khatiri, Alessio Gambi, and Sebastiano Panichella, "Cost-effective Simulation-based Test Selection in Self-driving Cars Software," *Science of Computer Programming (SCP)*, doi: 10.1016/j.scico.2023.102926, 2023.
+  - [Elsevier](https://doi.org/10.1016/j.scico.2023.102926)
 ````{code-block} bibtex
 @article{Birchler2022Cost2,
   author    = {Christian Birchler and Nicolas Ganz and Sajad Khatiri and Alessio Gambi and Sebastiano Panichella},
   title     = {Cost-effective Simulation-based Test Selection in Self-driving Cars Software},
   journal   = {Science of Computer Programming (SCP)},
-  year      = {2022},
-  doi       = {to appear},
-  eprinttype = {arXiv},
-  eprint    = {2211.11409}
+  volume    = {226},
+  year      = {2023},
+  doi       = {10.1016/j.scico.2023.102926},
+  pages     = {102926},
+  year      = {2023},
+  issn      = {0167-6423},
 }
 ````
 - **Christian Birchler**, Sajad Khatiri, Bill Bosshard, Alessio Gambi, and Sebastiano Panichella, "Machine Learning-based Test Selection for Simulation-based Testing of Self-driving Cars Software," *Empirical Software Engineering (EMSE)*, doi: to appear, 2022.
   - [Preprint](https://doi.org/10.48550/arXiv.2212.04769)
 ````{code-block} bibtex
 @article{Birchler2022Machine,
   author    = {Christian Birchler and Sajad Khatiri and Bill Bosshard and Alessio Gambi and Sebastiano Panichella},
```

#### html2text {}

```diff
@@ -102,42 +102,43 @@
 Nicolas and Khatiri, Sajad and Gambi, Alessio, and Panichella, Sebastiano},
 booktitle={2022 IEEE 29th International Conference on Software Analysis,
 Evolution and Reengineering (SANER)}, title={Cost-effective Simulationbased
 Test Selection in Self-driving Cars Software with SDC-Scissor}, year={2022},
 doi={10.1109/SANER53432.2022.00030} } ```` - **Christian Birchler**, Nicolas
 Ganz, Sajad Khatiri, Alessio Gambi, and Sebastiano Panichella, "Cost-effective
 Simulation-based Test Selection in Self-driving Cars Software," *Science of
-Computer Programming (SCP)*, doi: to appear, 2022. - [Accepted manuscript
-version](https://doi.org/10.48550/arXiv.2211.11409) ````{code-block} bibtex
+Computer Programming (SCP)*, doi: 10.1016/j.scico.2023.102926, 2023. -
+[Elsevier](https://doi.org/10.1016/j.scico.2023.102926) ````{code-block} bibtex
 @article{Birchler2022Cost2, author = {Christian Birchler and Nicolas Ganz and
 Sajad Khatiri and Alessio Gambi and Sebastiano Panichella}, title = {Cost-
 effective Simulation-based Test Selection in Self-driving Cars Software},
-journal = {Science of Computer Programming (SCP)}, year = {2022}, doi = {to
-appear}, eprinttype = {arXiv}, eprint = {2211.11409} } ```` - **Christian
-Birchler**, Sajad Khatiri, Bill Bosshard, Alessio Gambi, and Sebastiano
-Panichella, "Machine Learning-based Test Selection for Simulation-based Testing
-of Self-driving Cars Software," *Empirical Software Engineering (EMSE)*, doi:
-to appear, 2022. - [Preprint](https://doi.org/10.48550/arXiv.2212.04769) ````
-{code-block} bibtex @article{Birchler2022Machine, author = {Christian Birchler
-and Sajad Khatiri and Bill Bosshard and Alessio Gambi and Sebastiano
-Panichella}, title = {Machine Learning-based Test Selection for Simulation-
-based Testing of Self-driving Cars Software}, journal = {Empirical Software
-Engineering (EMSE)}, year = {2022}, doi = {to appear}, eprinttype = {arXiv},
-eprint = {2212.04769} } ```` - **Christian Birchler**, Sajad Khatiri, Pouria
-Derakhshanfar, Sebastiano Panichella, and Annibale Panichella, "Single and
-Multi-objective Test Cases Prioritization for Self-driving Cars in Virtual
-Environments," *ACM Transactions on Software Engineering and Methodology
-(TOSEM)*, doi: 10.1145/3533818, 2022. - [ACM Digital Library](https://doi.org/
-10.1145/3533818) - [Preprint](https://doi.org/10.48550/arXiv.2107.09614) ```
-{code-block} bibtex @article{Birchler2022Single, author={Birchler, Christian
-and Khatiri, Sajad and Derakhshanfar, Pouria and Panichella, Sebastiano and
-Panichella, Annibale}, title={Single and Multi-objective Test Cases
-Prioritization for Self-driving Cars in Virtual Environments}, year={2022},
-publisher={Association for Computing Machinery}, journal={ACM Transactions on
-Software Engineering and Methodology (TOSEM)}, doi={10.1145/3533818} } ``` ##
-Contacts * Christian Birchler * Zurich University of Applied Sciences (ZHAW),
-Switzerland - birc@zhaw.ch * Nicolas Ganz * Zurich University of Applied
-Sciences (ZHAW), Switzerland - gann@zhaw.ch * Sajad Khatiri * Zurich University
-of Applied Sciences (ZHAW), Switzerland - mazr@zhaw.ch * Dr. Alessio Gambi *
-IMC University Of Applied Sciences Krems, Austria - alessio.gambi@fh-
-krems.ac.at * Dr. Sebastiano Panichella * Zurich University of Applied Sciences
-(ZHAW), Switzerland - panc@zhaw.ch
+journal = {Science of Computer Programming (SCP)}, volume = {226}, year =
+{2023}, doi = {10.1016/j.scico.2023.102926}, pages = {102926}, year = {2023},
+issn = {0167-6423}, } ```` - **Christian Birchler**, Sajad Khatiri, Bill
+Bosshard, Alessio Gambi, and Sebastiano Panichella, "Machine Learning-based
+Test Selection for Simulation-based Testing of Self-driving Cars Software,"
+*Empirical Software Engineering (EMSE)*, doi: to appear, 2022. - [Preprint]
+(https://doi.org/10.48550/arXiv.2212.04769) ````{code-block} bibtex @article
+{Birchler2022Machine, author = {Christian Birchler and Sajad Khatiri and Bill
+Bosshard and Alessio Gambi and Sebastiano Panichella}, title = {Machine
+Learning-based Test Selection for Simulation-based Testing of Self-driving Cars
+Software}, journal = {Empirical Software Engineering (EMSE)}, year = {2022},
+doi = {to appear}, eprinttype = {arXiv}, eprint = {2212.04769} } ```` -
+**Christian Birchler**, Sajad Khatiri, Pouria Derakhshanfar, Sebastiano
+Panichella, and Annibale Panichella, "Single and Multi-objective Test Cases
+Prioritization for Self-driving Cars in Virtual Environments," *ACM
+Transactions on Software Engineering and Methodology (TOSEM)*, doi: 10.1145/
+3533818, 2022. - [ACM Digital Library](https://doi.org/10.1145/3533818) -
+[Preprint](https://doi.org/10.48550/arXiv.2107.09614) ```{code-block} bibtex
+@article{Birchler2022Single, author={Birchler, Christian and Khatiri, Sajad and
+Derakhshanfar, Pouria and Panichella, Sebastiano and Panichella, Annibale},
+title={Single and Multi-objective Test Cases Prioritization for Self-driving
+Cars in Virtual Environments}, year={2022}, publisher={Association for
+Computing Machinery}, journal={ACM Transactions on Software Engineering and
+Methodology (TOSEM)}, doi={10.1145/3533818} } ``` ## Contacts * Christian
+Birchler * Zurich University of Applied Sciences (ZHAW), Switzerland -
+birc@zhaw.ch * Nicolas Ganz * Zurich University of Applied Sciences (ZHAW),
+Switzerland - gann@zhaw.ch * Sajad Khatiri * Zurich University of Applied
+Sciences (ZHAW), Switzerland - mazr@zhaw.ch * Dr. Alessio Gambi * IMC
+University Of Applied Sciences Krems, Austria - alessio.gambi@fh-krems.ac.at *
+Dr. Sebastiano Panichella * Zurich University of Applied Sciences (ZHAW),
+Switzerland - panc@zhaw.ch
```

### Comparing `sdc_scissor-2.2.0a0/pyproject.toml` & `sdc_scissor-2.2.0rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SDC-Scissor"
-version = "2.2.0-a.0"
+version = "2.2.0-rc.0"
 description = "A cost-effective test selection for self-driving cars in virtual environments"
 authors = ["Christian Birchler <birchler.chr@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/ChristianBirchler/sdc-scissor"
 documentation = "https://sdc-scissor.readthedocs.io/"
 packages = [
```

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/can_api/can_bus_handler.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/can_api/can_bus_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 import can
 import cantools
 
 from sdc_scissor.can_api.can_output import ICANBusOutput
 from sdc_scissor.config import CONFIG
 
+_logger = logging.getLogger(__file__)
+
 
 def get_can_frame_list(can_db):
     """
     Returns a list of all sample frames in the given can database
 
     :param can_db: The CAN database
     :return: A list of all sample frames in the given can database
@@ -72,17 +74,19 @@
 
             example_msg = frame["example_message"]
             frame_id = frame["frame_id"]
             frame_sig_list = frame["signal_list"]
 
             # Transform the simulation values to assure they are within the dbc range and named correctly
             frame_values = self.get_frame_values(frame_sig_list, data)
+            _logger.info("can frame data values: {}".format(frame_values))
 
             # Generate the CAN message
             frame_data = example_msg.encode(frame_values)
+            _logger.info("can frame data encoded: {}".format(frame_data))
             msg = can.Message(arbitration_id=frame_id, data=frame_data)
             msg.timestamp = time.time()
 
             self.send_can_msg(msg)
 
     def send_can_msg(self, msg):
         self.output_handler.output_can_msg(msg)
```

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/can_api/can_msg_generator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/can_api/can_msg_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/can_api/can_output.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/can_api/can_output.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import logging
 from pathlib import Path
 
 import can
 import cantools
 import click
 from influxdb_client import InfluxDBClient, Point
-from influxdb_client.client.write_api import SYNCHRONOUS
+from influxdb_client.client.write_api import ASYNCHRONOUS
 
 from sdc_scissor.config import CONFIG
 
+_logger = logging.getLogger(__file__)
+
 
 class ICANBusOutput(abc.ABC):
     @abc.abstractmethod
     def output_can_msg(self, msg: can.Message):
         pass
 
 
@@ -64,45 +66,48 @@
         :return:
         """
         click.echo(click.style(msg, fg="green"))
         self.wrappee.output_can_msg(msg)
 
 
 def _write_influxdb_data_record(api, bucket: str, org: str, record: Point):
+    _logger.info("write to influxdb")
     try:
         api.write(bucket=bucket, org=org, record=record)
     except Exception as ex:
-        logging.error(ex)
+        logging.error("cannot write record: {}\texception: {}".format(record, ex))
 
 
 def _influxdb_bucket_setup(write_client: InfluxDBClient, bucket, org):
     bucket_api = write_client.buckets_api()
     if bucket_api.find_bucket_by_name(bucket_name=bucket) is None:
         bucket_api.create_bucket(bucket_name=bucket, org=org)
 
 
 class InfluxDBDecorator(AbstractOutputDecorator):
     def __init__(self, wrappee: ICANBusOutput, write_client: InfluxDBClient, bucket: str, org: str):
         super().__init__(wrappee)
         _influxdb_bucket_setup(write_client, bucket, org)
         self.write_client = write_client
-        self.write_api = write_client.write_api(write_options=SYNCHRONOUS)
+        self.write_api = write_client.write_api(write_options=ASYNCHRONOUS, batch_size=500)
         self.bucket = bucket
         self.org = org
         self.can_db = cantools.db.load_file(Path(CONFIG.CAN_DBC_PATH))
+        self.cache = []
 
     def output_can_msg(self, msg: can.Message):
         for msg_specs in self.can_db.messages:
+            decoded_msg = None
             try:
                 decoded_msg = self.can_db.decode_message(msg_specs.frame_id, msg.data)
             except Exception as ex:
-                logging.warning(ex)
+                _logger.info("can msg: {}\tdecoded msg: {}\texception: {}".format(msg, decoded_msg, ex))
                 continue
 
             point = Point(CONFIG.EXECUTION_START_TIME).tag("test_id", CONFIG.CURRENT_TEST_ID)
             for signal_name, signal_value in decoded_msg.items():
                 msg_sample_time = datetime.datetime.utcfromtimestamp(msg.timestamp)
+                print("utc: {}\traw: {}".format(msg_sample_time, msg.timestamp))
                 point = point.field(field=signal_name, value=signal_value).time(str(msg_sample_time))
-
-            _write_influxdb_data_record(self.write_api, CONFIG.INFLUXDB_BUCKET, CONFIG.INFLUXDB_ORG, point)
+                _write_influxdb_data_record(self.write_api, CONFIG.INFLUXDB_BUCKET, CONFIG.INFLUXDB_ORG, point)
 
         self.wrappee.output_can_msg(msg)
```

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/cli.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/cli.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/config.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/config.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/angle_based_strategy.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/angle_based_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/equi_distance_strategy.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/equi_distance_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/feature_extraction.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/feature_extraction_api/road_geometry_calculator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/feature_extraction_api/road_geometry_calculator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/machine_learning_api/model_evaluator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/machine_learning_api/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/machine_learning_api/predictor.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/machine_learning_api/predictor.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/beamng_bump.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/beamng_bump.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/beamng_delineator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/beamng_delineator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/beamng_obstacle_factory.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/beamng_obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/beamng_tree.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/beamng_tree.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/bump.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/bump.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/carla_obstacle_factory.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/carla_obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/delineator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/delineator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/obstacle_factory.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/obstacle_api/tree.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/obstacle_api/tree.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/initialPopulation.m` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/initialPopulation.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/main.m` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/main.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/mainGreedy.m` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/mainGreedy.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/permutationMutation.m` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/permutationMutation.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/plot.R` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/plot.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/table.R` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/table.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/runGreedy.m` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/runGreedy.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/runMOSearch.m` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/runMOSearch.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/code/runSearch.m` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/code/runSearch.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/README.md` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/sdc_prioritizer/testPrioritization/run.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/sdc_prioritizer/testPrioritization/run.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/simulator_api/abstract_simulator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/simulator_api/abstract_simulator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/simulator_api/beamng_simulator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/simulator_api/beamng_simulator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/simulator_api/simulator_factory.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/simulator_api/simulator_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/ambiegen/config.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/ambiegen/config.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_loader.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_loader.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_monitor.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_plotter.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_plotter.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_runner.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_runner.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/sdc_scissor/testing_api/test_validator.py` & `sdc_scissor-2.2.0rc0/sdc_scissor/testing_api/test_validator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0a0/PKG-INFO` & `sdc_scissor-2.2.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdc-scissor
-Version: 2.2.0a0
+Version: 2.2.0rc0
 Summary: A cost-effective test selection for self-driving cars in virtual environments
 Home-page: https://github.com/ChristianBirchler/sdc-scissor
 License: GPL-3.0-or-later
 Author: Christian Birchler
 Author-email: birchler.chr@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -123,25 +123,27 @@
   author={Birchler, Christian and Ganz, Nicolas and Khatiri, Sajad and Gambi, Alessio, and Panichella, Sebastiano},
   booktitle={2022 IEEE 29th International Conference on Software Analysis, Evolution and Reengineering (SANER)},
   title={Cost-effective Simulationbased Test Selection in Self-driving Cars Software with SDC-Scissor},
   year={2022},
   doi={10.1109/SANER53432.2022.00030}
 }
 ````
-- **Christian Birchler**, Nicolas Ganz, Sajad Khatiri, Alessio Gambi, and Sebastiano Panichella, "Cost-effective Simulation-based Test Selection in Self-driving Cars Software," *Science of Computer Programming (SCP)*, doi: to appear, 2022.
-  - [Accepted manuscript version](https://doi.org/10.48550/arXiv.2211.11409)
+- **Christian Birchler**, Nicolas Ganz, Sajad Khatiri, Alessio Gambi, and Sebastiano Panichella, "Cost-effective Simulation-based Test Selection in Self-driving Cars Software," *Science of Computer Programming (SCP)*, doi: 10.1016/j.scico.2023.102926, 2023.
+  - [Elsevier](https://doi.org/10.1016/j.scico.2023.102926)
 ````{code-block} bibtex
 @article{Birchler2022Cost2,
   author    = {Christian Birchler and Nicolas Ganz and Sajad Khatiri and Alessio Gambi and Sebastiano Panichella},
   title     = {Cost-effective Simulation-based Test Selection in Self-driving Cars Software},
   journal   = {Science of Computer Programming (SCP)},
-  year      = {2022},
-  doi       = {to appear},
-  eprinttype = {arXiv},
-  eprint    = {2211.11409}
+  volume    = {226},
+  year      = {2023},
+  doi       = {10.1016/j.scico.2023.102926},
+  pages     = {102926},
+  year      = {2023},
+  issn      = {0167-6423},
 }
 ````
 - **Christian Birchler**, Sajad Khatiri, Bill Bosshard, Alessio Gambi, and Sebastiano Panichella, "Machine Learning-based Test Selection for Simulation-based Testing of Self-driving Cars Software," *Empirical Software Engineering (EMSE)*, doi: to appear, 2022.
   - [Preprint](https://doi.org/10.48550/arXiv.2212.04769)
 ````{code-block} bibtex
 @article{Birchler2022Machine,
   author    = {Christian Birchler and Sajad Khatiri and Bill Bosshard and Alessio Gambi and Sebastiano Panichella},
```

