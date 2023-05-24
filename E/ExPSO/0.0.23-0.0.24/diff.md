# Comparing `tmp/ExPSO-0.0.23.tar.gz` & `tmp/ExPSO-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExPSO-0.0.23.tar", last modified: Wed May 24 09:58:46 2023, max compression
+gzip compressed data, was "ExPSO-0.0.24.tar", last modified: Wed May 24 10:16:36 2023, max compression
```

## Comparing `ExPSO-0.0.23.tar` & `ExPSO-0.0.24.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:58:46.080567 ExPSO-0.0.23/
--rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.0.23/LICENSE
--rw-rw-rw-   0        0        0    20483 2023-05-24 09:58:46.079567 ExPSO-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0    19619 2023-05-24 09:55:26.000000 ExPSO-0.0.23/README.md
--rw-rw-rw-   0        0        0     1042 2023-05-24 09:55:44.000000 ExPSO-0.0.23/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 09:58:46.081547 ExPSO-0.0.23/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 09:58:45.995464 ExPSO-0.0.23/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 09:58:46.063536 ExPSO-0.0.23/src/ExPSO/
--rw-rw-rw-   0        0        0    10375 2023-05-22 10:42:29.000000 ExPSO-0.0.23/src/ExPSO/ExPSOClass.py
--rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.0.23/src/ExPSO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:58:46.075545 ExPSO-0.0.23/src/ExPSO.egg-info/
--rw-rw-rw-   0        0        0    20483 2023-05-24 09:58:45.000000 ExPSO-0.0.23/src/ExPSO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-24 09:58:45.000000 ExPSO-0.0.23/src/ExPSO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:58:45.000000 ExPSO-0.0.23/src/ExPSO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-24 09:58:45.000000 ExPSO-0.0.23/src/ExPSO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 10:16:36.210047 ExPSO-0.0.24/
+-rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.0.24/LICENSE
+-rw-rw-rw-   0        0        0    20528 2023-05-24 10:16:36.208048 ExPSO-0.0.24/PKG-INFO
+-rw-rw-rw-   0        0        0    19664 2023-05-24 10:13:04.000000 ExPSO-0.0.24/README.md
+-rw-rw-rw-   0        0        0     1042 2023-05-24 10:13:42.000000 ExPSO-0.0.24/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 10:16:36.210047 ExPSO-0.0.24/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 10:16:36.157010 ExPSO-0.0.24/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 10:16:36.170019 ExPSO-0.0.24/src/ExPSO/
+-rw-rw-rw-   0        0        0    10375 2023-05-22 10:42:29.000000 ExPSO-0.0.24/src/ExPSO/ExPSOClass.py
+-rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.0.24/src/ExPSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:16:36.183028 ExPSO-0.0.24/src/ExPSO.egg-info/
+-rw-rw-rw-   0        0        0    20528 2023-05-24 10:16:36.000000 ExPSO-0.0.24/src/ExPSO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-24 10:16:36.000000 ExPSO-0.0.24/src/ExPSO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:16:36.000000 ExPSO-0.0.24/src/ExPSO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-24 10:16:36.000000 ExPSO-0.0.24/src/ExPSO.egg-info/top_level.txt
```

### Comparing `ExPSO-0.0.23/LICENSE` & `ExPSO-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `ExPSO-0.0.23/PKG-INFO` & `ExPSO-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExPSO
-Version: 0.0.23
+Version: 0.0.24
 Summary: The Exponential Particle Swarm Optimization (ExPSO) is a Python library that implements an extended variant of the Particle Swarm Optimization (PSO) algorithm. 
 Author-email: Insaf Kraidia <insaf.kraidia@univ-constantine2.dz>, Khelil Kassoul <khelil.kassoul@etu.unige.ch>, Samir Brahim Belhaouari <sbelhaouari@hbku.edu.qa>, Naoufel Cheikhrouhou <naoufel.cheikhrouhou@hesge.ch>, Nicolas Zufferey <nicolas.zufferey.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/insafkraidia/ExPSO.git
 Project-URL: Bug Tracker, https://github.com/insafkraidia/ExPSO.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to pspso's documentation!
 
 # Exponential Particle Swarm Optimization for Global Optimization (ExPSO)
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/05.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/05.png?raw=true"> </p>
 
 The ExPSO package is a Python library that includes an algorithm designed to optimize machine and deep learning parameters/hyperparameters. The algorithm divides the swarm population into three subpopulations and utilizes a search strategy based on an exponential function, allowing particles to make large leaps in the search space. It also adapts the control of the velocity range of each particle to balance the exploration and exploitation search phases. The leaping strategy is integrated into the velocity equation, and a new linearly decreasing cognitive parameter is included in the proposed method, along with a dynamic inertia weight strategy. The algorithm is designed to make large jumps at the beginning of the search and then small jumps for further improvements in specific regions of the solution search space. To obtain further information, we recommend referring to the journal paper available at [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/).
 
 ## Table of content
 
 | Section                                | Description                                                            |
 | -------------------------------------- | ---------------------------------------------------------------------- |
@@ -31,15 +31,15 @@
 | [Examples with public data](#examples) | Different examples for API                                             |
 | [Results](#results)                    | Comparative study between ExPSO and PSO for CNN,LSTM, XLNET,MLP models |
 | [References](#reference)               | References to cite                                                     |
 | [License](#license)                    | Package license                                                        |
 
 ## Flowchart of the proposed ExPSO
 
-<p align="center" style="max-width: 100%;height: 900px;width: 600px;"> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/01.png"> </p>
+<p align="center" style="max-width: 100%;height: 900px;width: 600px;"> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/01.png?raw=true"> </p>
 
 ## Installation
 
 ExPSO can be installed using [pip](https://pip.pypa.io/en/stable/), a tool
 for installing Python packages. To do it, run the following command:
 
 ```
@@ -110,15 +110,15 @@
 
 <a name="item1"></a>
 
 ## Examples
 
 ### Experiment 1. ExPSO with rosenbrock function
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/10.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/10.png?raw=true"> </p>
 
 The following example demonstrates the optimization process of ExPSO using the rosenbrock function:
 
 ```
 def ObjFunction(x):
     # rosenbrock function
     n = len(x)
@@ -154,15 +154,15 @@
 - WorstSol: It refers to the highest value of the best cost found during the optimization process. It helps evaluate the quality of the obtained solutions and identify the worst-performing solution.
 - BestSol: It refers to the lowest value of the best cost found during the optimization process.
 - STD (Standard Deviation): It refers to the standard deviation, which is often used to assess the diversity or convergence of the obtained solutions.
 - Avg_FES (Average Function Evaluations): It represents the average number of function evaluations performed during the optimization process.
 
 ### Experiment 2. ExPSO with ackley function
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/08.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/08.png?raw=true"> </p>
 
 The following example demonstrates the optimization process of ExPSO using the ackley function:
 
 ```
 def ObjFunction(x):
     # ackley function version 2.22
     z = -20*np.exp(-0.2*np.sqrt(np.sum(x**2, axis=1)/x.shape[1])) \
@@ -317,15 +317,15 @@
 - Fuzzy Self-Tuning PSO (FST-PSO) https://pypi.org/project/fst-pso/.
 - Pyswarms: a reference librarythat used pure PSO (Particle Swarm Optimization). https://github.com/ljvmiranda921/pyswarms .
 - Quantum particle swarm optimization (QPSO) https://pypi.org/project/qpso/.
 - FastPSO :Fast parallel Particle Swarm Optimization package (FastPSO) https://pypi.org/project/fastPSO/.
 
 The findings demonstrate notable advancements and efficient optimization achieved through ExPSO for various models such as CNN, LSTM, XLNET, and MLP.
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/88.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/88.png?raw=true"> </p>
 
 ## Reference
 
 If you use `ExPSO` in your research papers, please refer to it using following reference:
 
 ```
 [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/)
```

### Comparing `ExPSO-0.0.23/README.md` & `ExPSO-0.0.24/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Welcome to pspso's documentation!
 
 # Exponential Particle Swarm Optimization for Global Optimization (ExPSO)
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/05.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/05.png?raw=true"> </p>
 
 The ExPSO package is a Python library that includes an algorithm designed to optimize machine and deep learning parameters/hyperparameters. The algorithm divides the swarm population into three subpopulations and utilizes a search strategy based on an exponential function, allowing particles to make large leaps in the search space. It also adapts the control of the velocity range of each particle to balance the exploration and exploitation search phases. The leaping strategy is integrated into the velocity equation, and a new linearly decreasing cognitive parameter is included in the proposed method, along with a dynamic inertia weight strategy. The algorithm is designed to make large jumps at the beginning of the search and then small jumps for further improvements in specific regions of the solution search space. To obtain further information, we recommend referring to the journal paper available at [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/).
 
 ## Table of content
 
 | Section                                | Description                                                            |
 | -------------------------------------- | ---------------------------------------------------------------------- |
@@ -17,15 +17,15 @@
 | [Examples with public data](#examples) | Different examples for API                                             |
 | [Results](#results)                    | Comparative study between ExPSO and PSO for CNN,LSTM, XLNET,MLP models |
 | [References](#reference)               | References to cite                                                     |
 | [License](#license)                    | Package license                                                        |
 
 ## Flowchart of the proposed ExPSO
 
-<p align="center" style="max-width: 100%;height: 900px;width: 600px;"> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/01.png"> </p>
+<p align="center" style="max-width: 100%;height: 900px;width: 600px;"> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/01.png?raw=true"> </p>
 
 ## Installation
 
 ExPSO can be installed using [pip](https://pip.pypa.io/en/stable/), a tool
 for installing Python packages. To do it, run the following command:
 
 ```
@@ -96,15 +96,15 @@
 
 <a name="item1"></a>
 
 ## Examples
 
 ### Experiment 1. ExPSO with rosenbrock function
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/10.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/10.png?raw=true"> </p>
 
 The following example demonstrates the optimization process of ExPSO using the rosenbrock function:
 
 ```
 def ObjFunction(x):
     # rosenbrock function
     n = len(x)
@@ -140,15 +140,15 @@
 - WorstSol: It refers to the highest value of the best cost found during the optimization process. It helps evaluate the quality of the obtained solutions and identify the worst-performing solution.
 - BestSol: It refers to the lowest value of the best cost found during the optimization process.
 - STD (Standard Deviation): It refers to the standard deviation, which is often used to assess the diversity or convergence of the obtained solutions.
 - Avg_FES (Average Function Evaluations): It represents the average number of function evaluations performed during the optimization process.
 
 ### Experiment 2. ExPSO with ackley function
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/08.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/08.png?raw=true"> </p>
 
 The following example demonstrates the optimization process of ExPSO using the ackley function:
 
 ```
 def ObjFunction(x):
     # ackley function version 2.22
     z = -20*np.exp(-0.2*np.sqrt(np.sum(x**2, axis=1)/x.shape[1])) \
@@ -303,15 +303,15 @@
 - Fuzzy Self-Tuning PSO (FST-PSO) https://pypi.org/project/fst-pso/.
 - Pyswarms: a reference librarythat used pure PSO (Particle Swarm Optimization). https://github.com/ljvmiranda921/pyswarms .
 - Quantum particle swarm optimization (QPSO) https://pypi.org/project/qpso/.
 - FastPSO :Fast parallel Particle Swarm Optimization package (FastPSO) https://pypi.org/project/fastPSO/.
 
 The findings demonstrate notable advancements and efficient optimization achieved through ExPSO for various models such as CNN, LSTM, XLNET, and MLP.
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/88.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/88.png?raw=true"> </p>
 
 ## Reference
 
 If you use `ExPSO` in your research papers, please refer to it using following reference:
 
 ```
 [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/)
```

### Comparing `ExPSO-0.0.23/pyproject.toml` & `ExPSO-0.0.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "scikit-learn"
 ]
 
 
 
 [project]
 name = "ExPSO"
-version = "0.0.23"
+version = "0.0.24"
 authors = [
   { name="Insaf Kraidia", email="insaf.kraidia@univ-constantine2.dz" },
   { name="Khelil Kassoul", email="khelil.kassoul@etu.unige.ch" },
   { name="Samir Brahim Belhaouari", email="sbelhaouari@hbku.edu.qa" },
   { name="Naoufel Cheikhrouhou",email="naoufel.cheikhrouhou@hesge.ch"},
   { name="Nicolas Zufferey",email="nicolas.zufferey.1@ulaval.ca"}
```

### Comparing `ExPSO-0.0.23/src/ExPSO/ExPSOClass.py` & `ExPSO-0.0.24/src/ExPSO/ExPSOClass.py`

 * *Files identical despite different names*

### Comparing `ExPSO-0.0.23/src/ExPSO.egg-info/PKG-INFO` & `ExPSO-0.0.24/src/ExPSO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExPSO
-Version: 0.0.23
+Version: 0.0.24
 Summary: The Exponential Particle Swarm Optimization (ExPSO) is a Python library that implements an extended variant of the Particle Swarm Optimization (PSO) algorithm. 
 Author-email: Insaf Kraidia <insaf.kraidia@univ-constantine2.dz>, Khelil Kassoul <khelil.kassoul@etu.unige.ch>, Samir Brahim Belhaouari <sbelhaouari@hbku.edu.qa>, Naoufel Cheikhrouhou <naoufel.cheikhrouhou@hesge.ch>, Nicolas Zufferey <nicolas.zufferey.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/insafkraidia/ExPSO.git
 Project-URL: Bug Tracker, https://github.com/insafkraidia/ExPSO.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to pspso's documentation!
 
 # Exponential Particle Swarm Optimization for Global Optimization (ExPSO)
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/05.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/05.png?raw=true"> </p>
 
 The ExPSO package is a Python library that includes an algorithm designed to optimize machine and deep learning parameters/hyperparameters. The algorithm divides the swarm population into three subpopulations and utilizes a search strategy based on an exponential function, allowing particles to make large leaps in the search space. It also adapts the control of the velocity range of each particle to balance the exploration and exploitation search phases. The leaping strategy is integrated into the velocity equation, and a new linearly decreasing cognitive parameter is included in the proposed method, along with a dynamic inertia weight strategy. The algorithm is designed to make large jumps at the beginning of the search and then small jumps for further improvements in specific regions of the solution search space. To obtain further information, we recommend referring to the journal paper available at [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/).
 
 ## Table of content
 
 | Section                                | Description                                                            |
 | -------------------------------------- | ---------------------------------------------------------------------- |
@@ -31,15 +31,15 @@
 | [Examples with public data](#examples) | Different examples for API                                             |
 | [Results](#results)                    | Comparative study between ExPSO and PSO for CNN,LSTM, XLNET,MLP models |
 | [References](#reference)               | References to cite                                                     |
 | [License](#license)                    | Package license                                                        |
 
 ## Flowchart of the proposed ExPSO
 
-<p align="center" style="max-width: 100%;height: 900px;width: 600px;"> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/01.png"> </p>
+<p align="center" style="max-width: 100%;height: 900px;width: 600px;"> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/01.png?raw=true"> </p>
 
 ## Installation
 
 ExPSO can be installed using [pip](https://pip.pypa.io/en/stable/), a tool
 for installing Python packages. To do it, run the following command:
 
 ```
@@ -110,15 +110,15 @@
 
 <a name="item1"></a>
 
 ## Examples
 
 ### Experiment 1. ExPSO with rosenbrock function
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/10.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/10.png?raw=true"> </p>
 
 The following example demonstrates the optimization process of ExPSO using the rosenbrock function:
 
 ```
 def ObjFunction(x):
     # rosenbrock function
     n = len(x)
@@ -154,15 +154,15 @@
 - WorstSol: It refers to the highest value of the best cost found during the optimization process. It helps evaluate the quality of the obtained solutions and identify the worst-performing solution.
 - BestSol: It refers to the lowest value of the best cost found during the optimization process.
 - STD (Standard Deviation): It refers to the standard deviation, which is often used to assess the diversity or convergence of the obtained solutions.
 - Avg_FES (Average Function Evaluations): It represents the average number of function evaluations performed during the optimization process.
 
 ### Experiment 2. ExPSO with ackley function
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/08.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/08.png?raw=true"> </p>
 
 The following example demonstrates the optimization process of ExPSO using the ackley function:
 
 ```
 def ObjFunction(x):
     # ackley function version 2.22
     z = -20*np.exp(-0.2*np.sqrt(np.sum(x**2, axis=1)/x.shape[1])) \
@@ -317,15 +317,15 @@
 - Fuzzy Self-Tuning PSO (FST-PSO) https://pypi.org/project/fst-pso/.
 - Pyswarms: a reference librarythat used pure PSO (Particle Swarm Optimization). https://github.com/ljvmiranda921/pyswarms .
 - Quantum particle swarm optimization (QPSO) https://pypi.org/project/qpso/.
 - FastPSO :Fast parallel Particle Swarm Optimization package (FastPSO) https://pypi.org/project/fastPSO/.
 
 The findings demonstrate notable advancements and efficient optimization achieved through ExPSO for various models such as CNN, LSTM, XLNET, and MLP.
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/88.png"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/88.png?raw=true"> </p>
 
 ## Reference
 
 If you use `ExPSO` in your research papers, please refer to it using following reference:
 
 ```
 [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/)
```

