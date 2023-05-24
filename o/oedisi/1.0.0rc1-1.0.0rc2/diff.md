# Comparing `tmp/oedisi-1.0.0rc1.tar.gz` & `tmp/oedisi-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oedisi-1.0.0rc1.tar", last modified: Wed May 24 17:32:49 2023, max compression
+gzip compressed data, was "oedisi-1.0.0rc2.tar", last modified: Wed May 24 17:36:11 2023, max compression
```

## Comparing `oedisi-1.0.0rc1.tar` & `oedisi-1.0.0rc2.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.593586 oedisi-1.0.0rc1/
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.510407 oedisi-1.0.0rc1/.github/
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.518932 oedisi-1.0.0rc1/.github/workflows/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      849 2023-05-23 21:34:08.000000 oedisi-1.0.0rc1/.github/workflows/build-docs.yml
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1164 2022-09-13 19:49:51.000000 oedisi-1.0.0rc1/.github/workflows/test-api.yml
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      799 2023-05-23 21:34:08.000000 oedisi-1.0.0rc1/.github/workflows/unit-tests.yml
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2770 2022-04-15 20:05:01.000000 oedisi-1.0.0rc1/.gitignore
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1238 2022-04-15 20:05:01.000000 oedisi-1.0.0rc1/ALGORITHM_DEVELOPERS.md
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1523 2023-03-15 22:40:58.000000 oedisi-1.0.0rc1/LICENSE.md
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2080 2023-05-24 17:32:49.593304 oedisi-1.0.0rc1/PKG-INFO
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1355 2023-05-24 16:29:22.000000 oedisi-1.0.0rc1/README.md
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.524997 oedisi-1.0.0rc1/docs/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        8 2023-03-15 22:40:58.000000 oedisi-1.0.0rc1/docs/.gitignore
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      634 2022-04-15 20:05:01.000000 oedisi-1.0.0rc1/docs/Makefile
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1945 2023-05-23 21:47:03.000000 oedisi-1.0.0rc1/docs/conf.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1306 2022-05-20 18:27:04.000000 oedisi-1.0.0rc1/docs/design.rst
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      226 2022-04-15 20:05:01.000000 oedisi-1.0.0rc1/docs/examples.rst
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4842 2023-05-23 21:47:27.000000 oedisi-1.0.0rc1/docs/getting_started.rst
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      307 2023-05-23 22:01:17.000000 oedisi-1.0.0rc1/docs/index.rst
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      795 2022-04-15 20:05:01.000000 oedisi-1.0.0rc1/docs/make.bat
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1922 2023-05-23 21:59:36.000000 oedisi-1.0.0rc1/docs/oedisi_cli.rst
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       88 2023-05-23 21:34:08.000000 oedisi-1.0.0rc1/docs/requirements.txt
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.528027 oedisi-1.0.0rc1/docs/source/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       55 2023-05-23 21:58:53.000000 oedisi-1.0.0rc1/docs/source/modules.rst
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1106 2023-05-23 21:58:53.000000 oedisi-1.0.0rc1/docs/source/oedisi.componentframework.rst
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      258 2023-05-23 21:58:53.000000 oedisi-1.0.0rc1/docs/source/oedisi.rst
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      849 2023-05-23 21:58:53.000000 oedisi-1.0.0rc1/docs/source/oedisi.tools.rst
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      517 2023-05-23 21:58:53.000000 oedisi-1.0.0rc1/docs/source/oedisi.types.rst
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.528458 oedisi-1.0.0rc1/oedisi/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2023-05-24 15:15:07.000000 oedisi-1.0.0rc1/oedisi/__init__.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.535227 oedisi-1.0.0rc1/oedisi/componentframework/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2023-05-24 15:15:14.000000 oedisi-1.0.0rc1/oedisi/componentframework/__init__.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3588 2023-05-04 15:42:34.000000 oedisi-1.0.0rc1/oedisi/componentframework/basic_component.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4291 2022-12-23 05:00:13.000000 oedisi-1.0.0rc1/oedisi/componentframework/mock_component.py
--rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       63 2023-05-23 21:41:49.000000 oedisi-1.0.0rc1/oedisi/componentframework/mock_component.sh
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     8955 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/componentframework/system_configuration.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3891 2023-05-04 15:42:34.000000 oedisi-1.0.0rc1/oedisi/componentframework/wiring_diagram_utils.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.538504 oedisi-1.0.0rc1/oedisi/tools/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       47 2023-05-24 15:15:22.000000 oedisi-1.0.0rc1/oedisi/tools/__init__.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      908 2023-05-04 15:42:34.000000 oedisi-1.0.0rc1/oedisi/tools/broker_utils.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     9698 2023-05-23 21:42:03.000000 oedisi-1.0.0rc1/oedisi/tools/cli_tools.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1074 2023-05-04 15:42:34.000000 oedisi-1.0.0rc1/oedisi/tools/pausing_broker.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2074 2023-05-04 15:42:34.000000 oedisi-1.0.0rc1/oedisi/tools/testing_broker.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.540521 oedisi-1.0.0rc1/oedisi/types/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2023-05-24 15:15:33.000000 oedisi-1.0.0rc1/oedisi/types/__init__.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     7490 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/data_types.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1088 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/generate_schema.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.560842 oedisi-1.0.0rc1/oedisi/types/schemas/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1006 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/AdmittanceMatrix.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1285 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/AdmittanceSparse.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/CapacitorStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1349 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/Command.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1973 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/CommandList.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      963 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/CostArray.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1397 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/CurrentsAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/CurrentsImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/CurrentsMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/CurrentsReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    13378 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/Injection.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3831 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/InverterControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4268 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/InverterControlList.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1149 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/MeasurementArray.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      970 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/OperationalCosts.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/PowersAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1535 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/PowersImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/PowersMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1528 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/PowersReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      975 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/ReactiveCostFunctions.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      977 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/ReactiveWholesalePrices.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      971 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/RealCostFunctions.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      973 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/RealWholesalePrices.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/RegulatorStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1399 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/SolarIrradiances.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      690 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/StateArray.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1398 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/StatesOfCharge.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      692 2023-05-04 16:54:04.000000 oedisi-1.0.0rc1/oedisi/types/schemas/SwitchStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/Temperatures.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    22316 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/Topology.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1539 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/VVControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      679 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/VWControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1193 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/VoltagesAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/VoltagesImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/VoltagesMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1187 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/VoltagesReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/oedisi/types/schemas/WindSpeeds.json
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.531139 oedisi-1.0.0rc1/oedisi.egg-info/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2080 2023-05-24 17:32:49.000000 oedisi-1.0.0rc1/oedisi.egg-info/PKG-INFO
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     5397 2023-05-24 17:32:49.000000 oedisi-1.0.0rc1/oedisi.egg-info/SOURCES.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        1 2023-05-24 17:32:49.000000 oedisi-1.0.0rc1/oedisi.egg-info/dependency_links.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       44 2023-05-24 17:32:49.000000 oedisi-1.0.0rc1/oedisi.egg-info/entry_points.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       78 2023-05-24 17:32:49.000000 oedisi-1.0.0rc1/oedisi.egg-info/requires.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        7 2023-05-24 17:32:49.000000 oedisi-1.0.0rc1/oedisi.egg-info/top_level.txt
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        1 2023-05-23 21:58:13.000000 oedisi-1.0.0rc1/oedisi.egg-info/zip-safe
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       38 2023-05-24 17:32:49.593668 oedisi-1.0.0rc1/setup.cfg
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1591 2023-05-24 17:32:17.000000 oedisi-1.0.0rc1/setup.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.562052 oedisi-1.0.0rc1/tests/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       15 2022-08-19 19:46:38.000000 oedisi-1.0.0rc1/tests/.gitignore
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      632 2022-09-13 19:49:51.000000 oedisi-1.0.0rc1/tests/runtests.sh
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.566712 oedisi-1.0.0rc1/tests/test_basic_system/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       52 2022-08-19 19:46:38.000000 oedisi-1.0.0rc1/tests/test_basic_system/.gitignore
--rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       55 2022-09-13 19:49:51.000000 oedisi-1.0.0rc1/tests/test_basic_system/helics-run.sh
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    21680 2022-08-19 19:46:38.000000 oedisi-1.0.0rc1/tests/test_basic_system/sgidal-super-basic-example.png
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      749 2023-05-23 21:44:47.000000 oedisi-1.0.0rc1/tests/test_basic_system/test_basic_component.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      611 2023-05-24 15:16:21.000000 oedisi-1.0.0rc1/tests/test_basic_system/test_basic_system.json
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.568649 oedisi-1.0.0rc1/tests/test_basic_system/test_component_type/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      297 2023-05-24 15:16:09.000000 oedisi-1.0.0rc1/tests/test_basic_system/test_component_type/component_definition.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2470 2022-08-19 19:46:38.000000 oedisi-1.0.0rc1/tests/test_basic_system/test_component_type/test_component_type.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.573907 oedisi-1.0.0rc1/tests/test_mock_system/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       43 2022-09-13 19:49:51.000000 oedisi-1.0.0rc1/tests/test_mock_system/.gitignore
--rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       61 2022-09-13 19:49:51.000000 oedisi-1.0.0rc1/tests/test_mock_system/helics-run.sh
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      368 2023-05-23 21:45:08.000000 oedisi-1.0.0rc1/tests/test_mock_system/test_mock_component.py
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       63 2022-08-19 19:46:38.000000 oedisi-1.0.0rc1/tests/test_mock_system/test_mock_federate.sh
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      835 2023-05-24 15:16:17.000000 oedisi-1.0.0rc1/tests/test_mock_system/test_system.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      498 2023-05-23 21:44:27.000000 oedisi-1.0.0rc1/tests/test_mock_system/test_system_configuration.py
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.513759 oedisi-1.0.0rc1/tests/unit_tests/
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.574653 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/
-drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:32:49.592759 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      183 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/AdmittanceMatrix.1.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      210 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/AdmittanceSparse.1.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      103 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/CapacitorStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       79 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/Command.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      103 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/CommandList.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      210 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/CurrentsAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      199 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/CurrentsImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      203 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/CurrentsMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      203 2023-05-04 16:45:53.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/CurrentsReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      722 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/Injection.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      295 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/InverterControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      343 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/InverterControlList.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/OperationalCosts.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      308 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/PowersAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      302 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/PowersImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      303 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/PowersMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      302 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/PowersReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/ReactiveCostFunctions.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/ReactiveWholesalePrices.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/RealCostFunctions.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/RealWholesalePrices.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      103 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/RegulatorStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      202 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/SolarIrradiances.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      215 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/StatesOfCharge.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      103 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/SwitchStates.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      200 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/Temperatures.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      886 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/Topology.1.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1271 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/Topology.2.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      188 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/VVControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      106 2023-05-23 17:15:20.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/VWControl.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      204 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/VoltagesAngle.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      203 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/VoltagesImaginary.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      210 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/VoltagesMagnitude.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      210 2022-08-26 18:02:21.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/VoltagesReal.json
--rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      488 2023-05-23 21:44:57.000000 oedisi-1.0.0rc1/tests/unit_tests/test_data_types/test_data_types.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.972547 oedisi-1.0.0rc2/
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.892674 oedisi-1.0.0rc2/.github/
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.899361 oedisi-1.0.0rc2/.github/workflows/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      849 2023-05-23 21:34:08.000000 oedisi-1.0.0rc2/.github/workflows/build-docs.yml
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1164 2022-09-13 19:49:51.000000 oedisi-1.0.0rc2/.github/workflows/test-api.yml
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      799 2023-05-23 21:34:08.000000 oedisi-1.0.0rc2/.github/workflows/unit-tests.yml
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2770 2022-04-15 20:05:01.000000 oedisi-1.0.0rc2/.gitignore
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1238 2022-04-15 20:05:01.000000 oedisi-1.0.0rc2/ALGORITHM_DEVELOPERS.md
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1523 2023-03-15 22:40:58.000000 oedisi-1.0.0rc2/LICENSE.md
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2073 2023-05-24 17:36:11.972048 oedisi-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1348 2023-05-24 17:34:51.000000 oedisi-1.0.0rc2/README.md
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.903792 oedisi-1.0.0rc2/docs/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        8 2023-03-15 22:40:58.000000 oedisi-1.0.0rc2/docs/.gitignore
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      634 2022-04-15 20:05:01.000000 oedisi-1.0.0rc2/docs/Makefile
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1945 2023-05-23 21:47:03.000000 oedisi-1.0.0rc2/docs/conf.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1306 2022-05-20 18:27:04.000000 oedisi-1.0.0rc2/docs/design.rst
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      226 2022-04-15 20:05:01.000000 oedisi-1.0.0rc2/docs/examples.rst
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4842 2023-05-23 21:47:27.000000 oedisi-1.0.0rc2/docs/getting_started.rst
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      307 2023-05-23 22:01:17.000000 oedisi-1.0.0rc2/docs/index.rst
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      795 2022-04-15 20:05:01.000000 oedisi-1.0.0rc2/docs/make.bat
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1922 2023-05-23 21:59:36.000000 oedisi-1.0.0rc2/docs/oedisi_cli.rst
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       88 2023-05-23 21:34:08.000000 oedisi-1.0.0rc2/docs/requirements.txt
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.906165 oedisi-1.0.0rc2/docs/source/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       55 2023-05-23 21:58:53.000000 oedisi-1.0.0rc2/docs/source/modules.rst
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1106 2023-05-23 21:58:53.000000 oedisi-1.0.0rc2/docs/source/oedisi.componentframework.rst
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      258 2023-05-23 21:58:53.000000 oedisi-1.0.0rc2/docs/source/oedisi.rst
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      849 2023-05-23 21:58:53.000000 oedisi-1.0.0rc2/docs/source/oedisi.tools.rst
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      517 2023-05-23 21:58:53.000000 oedisi-1.0.0rc2/docs/source/oedisi.types.rst
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.906503 oedisi-1.0.0rc2/oedisi/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2023-05-24 15:15:07.000000 oedisi-1.0.0rc2/oedisi/__init__.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.912591 oedisi-1.0.0rc2/oedisi/componentframework/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2023-05-24 15:15:14.000000 oedisi-1.0.0rc2/oedisi/componentframework/__init__.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3588 2023-05-04 15:42:34.000000 oedisi-1.0.0rc2/oedisi/componentframework/basic_component.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4291 2022-12-23 05:00:13.000000 oedisi-1.0.0rc2/oedisi/componentframework/mock_component.py
+-rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       63 2023-05-23 21:41:49.000000 oedisi-1.0.0rc2/oedisi/componentframework/mock_component.sh
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     8955 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/componentframework/system_configuration.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3891 2023-05-04 15:42:34.000000 oedisi-1.0.0rc2/oedisi/componentframework/wiring_diagram_utils.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.915363 oedisi-1.0.0rc2/oedisi/tools/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       47 2023-05-24 15:15:22.000000 oedisi-1.0.0rc2/oedisi/tools/__init__.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      908 2023-05-04 15:42:34.000000 oedisi-1.0.0rc2/oedisi/tools/broker_utils.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     9698 2023-05-23 21:42:03.000000 oedisi-1.0.0rc2/oedisi/tools/cli_tools.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1074 2023-05-04 15:42:34.000000 oedisi-1.0.0rc2/oedisi/tools/pausing_broker.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2074 2023-05-04 15:42:34.000000 oedisi-1.0.0rc2/oedisi/tools/testing_broker.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.917114 oedisi-1.0.0rc2/oedisi/types/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       22 2023-05-24 15:15:33.000000 oedisi-1.0.0rc2/oedisi/types/__init__.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     7490 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/data_types.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1088 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/generate_schema.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.941018 oedisi-1.0.0rc2/oedisi/types/schemas/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1006 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/AdmittanceMatrix.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1285 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/AdmittanceSparse.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/CapacitorStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1349 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/Command.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1973 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/CommandList.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      963 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/CostArray.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1397 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/CurrentsAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/CurrentsImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1395 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/CurrentsMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/CurrentsReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    13378 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/Injection.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     3831 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/InverterControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     4268 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/InverterControlList.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1149 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/MeasurementArray.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      970 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/OperationalCosts.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/PowersAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1535 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/PowersImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1534 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/PowersMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1528 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/PowersReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      975 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/ReactiveCostFunctions.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      977 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/ReactiveWholesalePrices.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      971 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/RealCostFunctions.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      973 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/RealWholesalePrices.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      695 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/RegulatorStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1399 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/SolarIrradiances.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      690 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/StateArray.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1398 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/StatesOfCharge.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      692 2023-05-04 16:54:04.000000 oedisi-1.0.0rc2/oedisi/types/schemas/SwitchStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/Temperatures.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    22316 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/Topology.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1539 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/VVControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      679 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/VWControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1193 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/VoltagesAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/VoltagesImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1192 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/VoltagesMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1187 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/VoltagesReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1390 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/oedisi/types/schemas/WindSpeeds.json
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.908996 oedisi-1.0.0rc2/oedisi.egg-info/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2073 2023-05-24 17:36:11.000000 oedisi-1.0.0rc2/oedisi.egg-info/PKG-INFO
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     5397 2023-05-24 17:36:11.000000 oedisi-1.0.0rc2/oedisi.egg-info/SOURCES.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        1 2023-05-24 17:36:11.000000 oedisi-1.0.0rc2/oedisi.egg-info/dependency_links.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       44 2023-05-24 17:36:11.000000 oedisi-1.0.0rc2/oedisi.egg-info/entry_points.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       78 2023-05-24 17:36:11.000000 oedisi-1.0.0rc2/oedisi.egg-info/requires.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        7 2023-05-24 17:36:11.000000 oedisi-1.0.0rc2/oedisi.egg-info/top_level.txt
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        1 2023-05-23 21:58:13.000000 oedisi-1.0.0rc2/oedisi.egg-info/zip-safe
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       38 2023-05-24 17:36:11.972696 oedisi-1.0.0rc2/setup.cfg
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1591 2023-05-24 17:35:42.000000 oedisi-1.0.0rc2/setup.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.942381 oedisi-1.0.0rc2/tests/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       15 2022-08-19 19:46:38.000000 oedisi-1.0.0rc2/tests/.gitignore
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      632 2022-09-13 19:49:51.000000 oedisi-1.0.0rc2/tests/runtests.sh
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.945796 oedisi-1.0.0rc2/tests/test_basic_system/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       52 2022-08-19 19:46:38.000000 oedisi-1.0.0rc2/tests/test_basic_system/.gitignore
+-rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       55 2022-09-13 19:49:51.000000 oedisi-1.0.0rc2/tests/test_basic_system/helics-run.sh
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)    21680 2022-08-19 19:46:38.000000 oedisi-1.0.0rc2/tests/test_basic_system/sgidal-super-basic-example.png
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      749 2023-05-23 21:44:47.000000 oedisi-1.0.0rc2/tests/test_basic_system/test_basic_component.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      611 2023-05-24 15:16:21.000000 oedisi-1.0.0rc2/tests/test_basic_system/test_basic_system.json
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.947230 oedisi-1.0.0rc2/tests/test_basic_system/test_component_type/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      297 2023-05-24 15:16:09.000000 oedisi-1.0.0rc2/tests/test_basic_system/test_component_type/component_definition.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     2470 2022-08-19 19:46:38.000000 oedisi-1.0.0rc2/tests/test_basic_system/test_component_type/test_component_type.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.950840 oedisi-1.0.0rc2/tests/test_mock_system/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       43 2022-09-13 19:49:51.000000 oedisi-1.0.0rc2/tests/test_mock_system/.gitignore
+-rwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       61 2022-09-13 19:49:51.000000 oedisi-1.0.0rc2/tests/test_mock_system/helics-run.sh
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      368 2023-05-23 21:45:08.000000 oedisi-1.0.0rc2/tests/test_mock_system/test_mock_component.py
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       63 2022-08-19 19:46:38.000000 oedisi-1.0.0rc2/tests/test_mock_system/test_mock_federate.sh
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      835 2023-05-24 15:16:17.000000 oedisi-1.0.0rc2/tests/test_mock_system/test_system.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      498 2023-05-23 21:44:27.000000 oedisi-1.0.0rc2/tests/test_mock_system/test_system_configuration.py
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.895557 oedisi-1.0.0rc2/tests/unit_tests/
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.951432 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/
+drwxr-xr-x   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)        0 2023-05-24 17:36:11.971348 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      183 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/AdmittanceMatrix.1.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      210 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/AdmittanceSparse.1.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      103 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/CapacitorStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)       79 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/Command.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      103 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/CommandList.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      210 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/CurrentsAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      199 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/CurrentsImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      203 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/CurrentsMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      203 2023-05-04 16:45:53.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/CurrentsReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      722 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/Injection.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      295 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/InverterControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      343 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/InverterControlList.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/OperationalCosts.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      308 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/PowersAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      302 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/PowersImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      303 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/PowersMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      302 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/PowersReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/ReactiveCostFunctions.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/ReactiveWholesalePrices.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/RealCostFunctions.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      167 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/RealWholesalePrices.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      103 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/RegulatorStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      202 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/SolarIrradiances.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      215 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/StatesOfCharge.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      103 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/SwitchStates.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      200 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/Temperatures.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      886 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/Topology.1.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)     1271 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/Topology.2.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      188 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/VVControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      106 2023-05-23 17:15:20.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/VWControl.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      204 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/VoltagesAngle.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      203 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/VoltagesImaginary.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      210 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/VoltagesMagnitude.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      210 2022-08-26 18:02:21.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/VoltagesReal.json
+-rw-r--r--   0 jmckinse (1978262345) NREL_NT\Domain Users (18434217)      488 2023-05-23 21:44:57.000000 oedisi-1.0.0rc2/tests/unit_tests/test_data_types/test_data_types.py
```

### Comparing `oedisi-1.0.0rc1/.github/workflows/build-docs.yml` & `oedisi-1.0.0rc2/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/.github/workflows/test-api.yml` & `oedisi-1.0.0rc2/.github/workflows/test-api.yml`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/.github/workflows/unit-tests.yml` & `oedisi-1.0.0rc2/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/.gitignore` & `oedisi-1.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/ALGORITHM_DEVELOPERS.md` & `oedisi-1.0.0rc2/ALGORITHM_DEVELOPERS.md`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/LICENSE.md` & `oedisi-1.0.0rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/PKG-INFO` & `oedisi-1.0.0rc2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oedisi
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Orchestration interface for HELICS power simulations
 Author: Joseph McKinsey
 Author-email: joseph.mckinsey@nrel.gov
 License: BSD 3-Clause
 Keywords: oedisi gadal helics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -15,20 +15,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
-# `oeidisi`
+# `oedisi`
 
 
-[![Main - Integration Tests](https://github.com/openEDI/oeidisi/actions/workflows/test-api.yml/badge.svg)](https://github.com/openEDI/oeidisi/actions/workflows/test-api.yml)
-[![Main - Unit Tests](https://github.com/openEDI/oeidisi/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/openEDI/oeidisi/actions/workflows/unit-tests.yml)
-[![Documentation](https://github.com/openEDI/oeidisi/actions/workflows/build-docs.yml/badge.svg)](https://openedi.github.io/oeidisi/)
+[![Main - Integration Tests](https://github.com/openEDI/oedisi/actions/workflows/test-api.yml/badge.svg)](https://github.com/openEDI/oedisi/actions/workflows/test-api.yml)
+[![Main - Unit Tests](https://github.com/openEDI/oedisi/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/openEDI/oedisi/actions/workflows/unit-tests.yml)
+[![Documentation](https://github.com/openEDI/oedisi/actions/workflows/build-docs.yml/badge.svg)](https://openedi.github.io/oedisi/)
 
 `oedisi` (OpenEDI - System Integration) is an orchestration interface for HELICS power simulations.
 
 - connects algorithms and data in a co-simulation framework HELICS by instantiating new components with the right HELICS configuration
 - runs simulations (including with debug features) using the `oedisi` CLI tool.
 - provides common [Pydantic](https://github.com/pydantic/pydantic) models for communications between power system algorithms and data in `oedisi.types`
```

### Comparing `oedisi-1.0.0rc1/README.md` & `oedisi-1.0.0rc2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# `oeidisi`
+# `oedisi`
 
 
-[![Main - Integration Tests](https://github.com/openEDI/oeidisi/actions/workflows/test-api.yml/badge.svg)](https://github.com/openEDI/oeidisi/actions/workflows/test-api.yml)
-[![Main - Unit Tests](https://github.com/openEDI/oeidisi/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/openEDI/oeidisi/actions/workflows/unit-tests.yml)
-[![Documentation](https://github.com/openEDI/oeidisi/actions/workflows/build-docs.yml/badge.svg)](https://openedi.github.io/oeidisi/)
+[![Main - Integration Tests](https://github.com/openEDI/oedisi/actions/workflows/test-api.yml/badge.svg)](https://github.com/openEDI/oedisi/actions/workflows/test-api.yml)
+[![Main - Unit Tests](https://github.com/openEDI/oedisi/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/openEDI/oedisi/actions/workflows/unit-tests.yml)
+[![Documentation](https://github.com/openEDI/oedisi/actions/workflows/build-docs.yml/badge.svg)](https://openedi.github.io/oedisi/)
 
 `oedisi` (OpenEDI - System Integration) is an orchestration interface for HELICS power simulations.
 
 - connects algorithms and data in a co-simulation framework HELICS by instantiating new components with the right HELICS configuration
 - runs simulations (including with debug features) using the `oedisi` CLI tool.
 - provides common [Pydantic](https://github.com/pydantic/pydantic) models for communications between power system algorithms and data in `oedisi.types`
```

### Comparing `oedisi-1.0.0rc1/docs/Makefile` & `oedisi-1.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/docs/conf.py` & `oedisi-1.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/docs/design.rst` & `oedisi-1.0.0rc2/docs/design.rst`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/docs/getting_started.rst` & `oedisi-1.0.0rc2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/docs/make.bat` & `oedisi-1.0.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/docs/oedisi_cli.rst` & `oedisi-1.0.0rc2/docs/oedisi_cli.rst`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/docs/source/oedisi.componentframework.rst` & `oedisi-1.0.0rc2/docs/source/oedisi.componentframework.rst`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/docs/source/oedisi.tools.rst` & `oedisi-1.0.0rc2/docs/source/oedisi.tools.rst`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/docs/source/oedisi.types.rst` & `oedisi-1.0.0rc2/docs/source/oedisi.types.rst`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/componentframework/basic_component.py` & `oedisi-1.0.0rc2/oedisi/componentframework/basic_component.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/componentframework/mock_component.py` & `oedisi-1.0.0rc2/oedisi/componentframework/mock_component.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/componentframework/system_configuration.py` & `oedisi-1.0.0rc2/oedisi/componentframework/system_configuration.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/componentframework/wiring_diagram_utils.py` & `oedisi-1.0.0rc2/oedisi/componentframework/wiring_diagram_utils.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/tools/broker_utils.py` & `oedisi-1.0.0rc2/oedisi/tools/broker_utils.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/tools/cli_tools.py` & `oedisi-1.0.0rc2/oedisi/tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/tools/pausing_broker.py` & `oedisi-1.0.0rc2/oedisi/tools/pausing_broker.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/tools/testing_broker.py` & `oedisi-1.0.0rc2/oedisi/tools/testing_broker.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/data_types.py` & `oedisi-1.0.0rc2/oedisi/types/data_types.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/generate_schema.py` & `oedisi-1.0.0rc2/oedisi/types/generate_schema.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/AdmittanceMatrix.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/AdmittanceMatrix.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/AdmittanceSparse.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/AdmittanceSparse.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/CapacitorStates.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/CapacitorStates.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/Command.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/Command.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/CommandList.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/CommandList.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/CostArray.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/CostArray.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/CurrentsAngle.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/CurrentsAngle.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/CurrentsImaginary.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/CurrentsImaginary.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/CurrentsMagnitude.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/CurrentsMagnitude.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/CurrentsReal.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/CurrentsReal.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/Injection.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/Injection.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/InverterControl.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/InverterControl.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/InverterControlList.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/InverterControlList.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/MeasurementArray.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/MeasurementArray.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/OperationalCosts.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/OperationalCosts.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/PowersAngle.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/PowersAngle.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/PowersImaginary.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/PowersImaginary.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/PowersMagnitude.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/PowersMagnitude.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/PowersReal.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/PowersReal.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/ReactiveCostFunctions.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/ReactiveCostFunctions.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/ReactiveWholesalePrices.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/ReactiveWholesalePrices.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/RealCostFunctions.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/RealCostFunctions.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/RealWholesalePrices.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/RealWholesalePrices.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/RegulatorStates.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/RegulatorStates.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/SolarIrradiances.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/SolarIrradiances.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/StateArray.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/StateArray.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/StatesOfCharge.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/StatesOfCharge.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/SwitchStates.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/SwitchStates.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/Temperatures.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/Temperatures.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/Topology.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/Topology.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/VVControl.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/VVControl.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/VWControl.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/VWControl.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/VoltagesAngle.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/VoltagesAngle.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/VoltagesImaginary.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/VoltagesImaginary.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/VoltagesMagnitude.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/VoltagesMagnitude.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/VoltagesReal.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/VoltagesReal.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi/types/schemas/WindSpeeds.json` & `oedisi-1.0.0rc2/oedisi/types/schemas/WindSpeeds.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/oedisi.egg-info/PKG-INFO` & `oedisi-1.0.0rc2/oedisi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oedisi
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Orchestration interface for HELICS power simulations
 Author: Joseph McKinsey
 Author-email: joseph.mckinsey@nrel.gov
 License: BSD 3-Clause
 Keywords: oedisi gadal helics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -15,20 +15,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
-# `oeidisi`
+# `oedisi`
 
 
-[![Main - Integration Tests](https://github.com/openEDI/oeidisi/actions/workflows/test-api.yml/badge.svg)](https://github.com/openEDI/oeidisi/actions/workflows/test-api.yml)
-[![Main - Unit Tests](https://github.com/openEDI/oeidisi/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/openEDI/oeidisi/actions/workflows/unit-tests.yml)
-[![Documentation](https://github.com/openEDI/oeidisi/actions/workflows/build-docs.yml/badge.svg)](https://openedi.github.io/oeidisi/)
+[![Main - Integration Tests](https://github.com/openEDI/oedisi/actions/workflows/test-api.yml/badge.svg)](https://github.com/openEDI/oedisi/actions/workflows/test-api.yml)
+[![Main - Unit Tests](https://github.com/openEDI/oedisi/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/openEDI/oedisi/actions/workflows/unit-tests.yml)
+[![Documentation](https://github.com/openEDI/oedisi/actions/workflows/build-docs.yml/badge.svg)](https://openedi.github.io/oedisi/)
 
 `oedisi` (OpenEDI - System Integration) is an orchestration interface for HELICS power simulations.
 
 - connects algorithms and data in a co-simulation framework HELICS by instantiating new components with the right HELICS configuration
 - runs simulations (including with debug features) using the `oedisi` CLI tool.
 - provides common [Pydantic](https://github.com/pydantic/pydantic) models for communications between power system algorithms and data in `oedisi.types`
```

### Comparing `oedisi-1.0.0rc1/oedisi.egg-info/SOURCES.txt` & `oedisi-1.0.0rc2/oedisi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/setup.py` & `oedisi-1.0.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 
 with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="oedisi",
-    version="1.0.0rc1",
+    version="1.0.0rc2",
     description=description,
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Joseph McKinsey",
     author_email="joseph.mckinsey@nrel.gov",
     packages=find_packages(),
     package_dir={"oedisi": "oedisi"},
```

### Comparing `oedisi-1.0.0rc1/tests/runtests.sh` & `oedisi-1.0.0rc2/tests/runtests.sh`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/tests/test_basic_system/sgidal-super-basic-example.png` & `oedisi-1.0.0rc2/tests/test_basic_system/sgidal-super-basic-example.png`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/tests/test_basic_system/test_basic_component.py` & `oedisi-1.0.0rc2/tests/test_basic_system/test_basic_component.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/tests/test_basic_system/test_basic_system.json` & `oedisi-1.0.0rc2/tests/test_basic_system/test_basic_system.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/tests/test_basic_system/test_component_type/test_component_type.py` & `oedisi-1.0.0rc2/tests/test_basic_system/test_component_type/test_component_type.py`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/tests/test_mock_system/test_system.json` & `oedisi-1.0.0rc2/tests/test_mock_system/test_system.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/Injection.json` & `oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/Injection.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/Topology.1.json` & `oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/Topology.1.json`

 * *Files identical despite different names*

### Comparing `oedisi-1.0.0rc1/tests/unit_tests/test_data_types/data/Topology.2.json` & `oedisi-1.0.0rc2/tests/unit_tests/test_data_types/data/Topology.2.json`

 * *Files identical despite different names*

