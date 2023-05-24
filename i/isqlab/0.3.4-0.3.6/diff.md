# Comparing `tmp/isqlab-0.3.4.tar.gz` & `tmp/isqlab-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isqlab-0.3.4.tar", last modified: Mon May 15 07:44:54 2023, max compression
+gzip compressed data, was "isqlab-0.3.6.tar", last modified: Wed May 24 04:14:31 2023, max compression
```

## Comparing `isqlab-0.3.4.tar` & `isqlab-0.3.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-15 07:44:54.818248 isqlab-0.3.4/
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1073 2023-05-15 07:44:28.000000 isqlab-0.3.4/LICENSE
--rw-r--r--   0 yangys    (1000) yangys    (1000)      850 2023-05-15 07:44:54.818248 isqlab-0.3.4/PKG-INFO
--rw-r--r--   0 yangys    (1000) yangys    (1000)      616 2023-05-15 07:44:28.000000 isqlab-0.3.4/README.md
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-15 07:44:54.808248 isqlab-0.3.4/isqlab/
--rw-r--r--   0 yangys    (1000) yangys    (1000)      592 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/__init__.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-15 07:44:54.808248 isqlab-0.3.4/isqlab/circuits/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       65 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/circuits/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)    23483 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/circuits/quantum_circuit.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-15 07:44:54.808248 isqlab-0.3.4/isqlab/linkers/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       74 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/linkers/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1350 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/linkers/torch_layer.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)    10449 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/linkers/torch_linker.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-15 07:44:54.818248 isqlab-0.3.4/isqlab/neural_networks/
--rw-r--r--   0 yangys    (1000) yangys    (1000)      148 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/neural_networks/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     8563 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/neural_networks/neural_network.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1573 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/neural_networks/qnn_autograd.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1519 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/neural_networks/qnn_jax.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     4223 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/neural_networks/qnn_simulator.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-15 07:44:54.818248 isqlab-0.3.4/isqlab/vqe/
--rw-r--r--   0 yangys    (1000) yangys    (1000)      130 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/vqe/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     7048 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/vqe/chem.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     4251 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/vqe/hamiltonian_measure.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     3564 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/vqe/kupccgsd.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     2534 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/vqe/symmetry_preserving.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)    10853 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/vqe/ucc.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     3477 2023-05-15 07:44:28.000000 isqlab-0.3.4/isqlab/vqe/uccsd.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-15 07:44:54.808248 isqlab-0.3.4/isqlab.egg-info/
--rw-r--r--   0 yangys    (1000) yangys    (1000)      850 2023-05-15 07:44:54.000000 isqlab-0.3.4/isqlab.egg-info/PKG-INFO
--rw-r--r--   0 yangys    (1000) yangys    (1000)      686 2023-05-15 07:44:54.000000 isqlab-0.3.4/isqlab.egg-info/SOURCES.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)        1 2023-05-15 07:44:54.000000 isqlab-0.3.4/isqlab.egg-info/dependency_links.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)        7 2023-05-15 07:44:54.000000 isqlab-0.3.4/isqlab.egg-info/top_level.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)      107 2023-05-15 07:44:54.818248 isqlab-0.3.4/setup.cfg
--rw-r--r--   0 yangys    (1000) yangys    (1000)      752 2023-05-15 07:44:28.000000 isqlab-0.3.4/setup.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-24 04:14:30.991932 isqlab-0.3.6/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1073 2023-05-24 04:14:10.000000 isqlab-0.3.6/LICENSE
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      886 2023-05-24 04:14:30.991932 isqlab-0.3.6/PKG-INFO
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      616 2023-05-24 04:14:10.000000 isqlab-0.3.6/README.md
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-24 04:14:30.981932 isqlab-0.3.6/isqlab/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      592 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/__init__.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-24 04:14:30.981932 isqlab-0.3.6/isqlab/circuits/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)       65 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/circuits/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)    23106 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/circuits/quantum_circuit.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-24 04:14:30.981932 isqlab-0.3.6/isqlab/linkers/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)       74 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/linkers/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1350 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/linkers/torch_layer.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)    10449 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/linkers/torch_linker.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-24 04:14:30.981932 isqlab-0.3.6/isqlab/neural_networks/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      148 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/neural_networks/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     8563 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/neural_networks/neural_network.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1573 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/neural_networks/qnn_autograd.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1519 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/neural_networks/qnn_jax.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     4223 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/neural_networks/qnn_simulator.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-24 04:14:30.991932 isqlab-0.3.6/isqlab/vqe/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      130 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/vqe/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     7048 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/vqe/chem.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     4227 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/vqe/hamiltonian_measure.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     3564 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/vqe/kupccgsd.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     2534 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/vqe/symmetry_preserving.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)    10853 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/vqe/ucc.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     3477 2023-05-24 04:14:10.000000 isqlab-0.3.6/isqlab/vqe/uccsd.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-05-24 04:14:30.981932 isqlab-0.3.6/isqlab.egg-info/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      886 2023-05-24 04:14:30.000000 isqlab-0.3.6/isqlab.egg-info/PKG-INFO
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      686 2023-05-24 04:14:30.000000 isqlab-0.3.6/isqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 yangys    (1000) yangys    (1000)        1 2023-05-24 04:14:30.000000 isqlab-0.3.6/isqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 yangys    (1000) yangys    (1000)        7 2023-05-24 04:14:30.000000 isqlab-0.3.6/isqlab.egg-info/top_level.txt
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      107 2023-05-24 04:14:30.991932 isqlab-0.3.6/setup.cfg
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      800 2023-05-24 04:14:10.000000 isqlab-0.3.6/setup.py
```

### Comparing `isqlab-0.3.4/LICENSE` & `isqlab-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/PKG-INFO` & `isqlab-0.3.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: isqlab
-Version: 0.3.4
+Version: 0.3.6
 Summary: application modules for isq
 Author: Yusheng Yang
 Author-email: yangys@arclightquantum.com
+License: MIT
 Platform: python 3.8+
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Isqlab is a Python library for isQ.
 
 ## Key Features
 
@@ -25,15 +27,15 @@
 Isqlab requires Python version 3.8 and above. Installation of isqlab can be done using:
 
 ```console
 git clone http://www.arclighttest.cn:8090/yangys/isqlab.git
 cd isqlab
 python setup.py bdist_wheel sdist
 cd dist
-pip install isqlab-0.3.4-py3-none-any.whl
+pip install isqlab-0.3.6-py3-none-any.whl
 ```
 
 ## Getting started
 
 See examples.
 
 ## Authors
```

### Comparing `isqlab-0.3.4/README.md` & `isqlab-0.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Isqlab requires Python version 3.8 and above. Installation of isqlab can be done using:
 
 ```console
 git clone http://www.arclighttest.cn:8090/yangys/isqlab.git
 cd isqlab
 python setup.py bdist_wheel sdist
 cd dist
-pip install isqlab-0.3.4-py3-none-any.whl
+pip install isqlab-0.3.6-py3-none-any.whl
 ```
 
 ## Getting started
 
 See examples.
 
 ## Authors
```

### Comparing `isqlab-0.3.4/isqlab/__init__.py` & `isqlab-0.3.6/isqlab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from isqlab.linkers import TorchLayer
 from isqlab.circuits import QuantumCircuit
 import os
 import logging
-__version__ = "0.3.4"
+__version__ = "0.3.6"
 __author__ = "Arclight Quantum"
 __creator__ = "Yusheng Yang"
 
 # 0 = all messages are logged (default behavior)
 # 1 = INFO messages are not printed
 # 2 = INFO and WARNING messages are not printed
 # 3 = INFO, WARNING, and ERROR messages are not printed
```

### Comparing `isqlab-0.3.4/isqlab/circuits/quantum_circuit.py` & `isqlab-0.3.6/isqlab/circuits/quantum_circuit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # This code is part of isQ.
 # (C) Copyright ArcLight Quantum 2023.
 # This code is licensed under the MIT License.
 
 """Quantum circuit object."""
 
 from isq import LocalDevice, quantumCor
-from isq.device.device import Device, AwsDevice
+from isq.device.device import Device, AwsDevice, QcisDevice
 from isq import Drawer
 from typing import Callable, Union, Sequence, Literal, Optional
 from functools import partial
 import numpy as np
 import itertools
 import time
+import re
 
 
 try:
     import jax.numpy as jnp
     HAS_JAX = True
 except Exception:
     HAS_JAX = False
@@ -60,15 +61,15 @@
 
         if backend is None:
             backend = LocalDevice()
 
         self.use_hardware = False
         self.run_time = None
         self.sleep_time = None
-        if isinstance(backend, AwsDevice):
+        if isinstance(backend, (AwsDevice, QcisDevice)):
             self.use_hardware = True
             self.run_time = run_time
             self.sleep_time = sleep_time
         # When using hardware, `method` is invalid
 
         if method == "jax":
             if not HAS_JAX:
@@ -80,14 +81,15 @@
 
         if method in ["torch", "pytorch"]:
             if not HAS_TORCH:
                 raise QuantumCircuitError("Pytorch is not installed.")
 
         self._circuit_recording = []  # to record isqfile
         self._measure_recording = []  # to recoed measurement
+        self.is_pauli_measure = False
 
         self.backend = backend
         self.method = method
         self.dict_format = dict_format
 
         self.num_qubits = num_qubits
         self._qbit_init(num_qubits)
@@ -536,14 +538,15 @@
         self,
         *qubit_idx: Union[Sequence[int], int],
     ) -> None:
         """
         Specifies the object to be measured.
         """
 
+        self.is_pauli_measure = False
         self._len_qubit_measure = len(qubit_idx)
         # reset measurement
         self._measure_recording = []
 
         for idx in qubit_idx:
             self._measure_recording.append(f"M(q[{idx}]);")
 
@@ -556,14 +559,17 @@
         self,
         **params,
     ):
         """
         Forward calculation.
         """
 
+        if self.is_pauli_measure:
+            print("Warning: don't use pauli measurement after giving pauli operators.")
+
         if len(self._measure_recording) == 0:
             raise ValueError("Please set measurement.")
 
         if self.use_hardware:
             task = self._measure_hardware(**params)
             if self.dict_format:
                 return task.result()
@@ -616,80 +622,69 @@
 
         for bin_idx, freq in result_dicts.items():
             results_arrays[int(bin_idx, 2)] = float(freq/shots)
         return results_arrays
 
     def pauli(
         self,
-        gate_name: Union[str, tuple],
+        gates: Union[str, tuple],
         format: str = "str",
     ) -> None:
         """
         Pauli measurement.
         """
-        self._measure_recording = []
+
+        self._measure_recording = []  # reset measurement
+        self.is_pauli_measure = True
 
         if format == "str":
-            gates = gate_name[0::2]
-            locations = [int(location) for location in gate_name[1::2]]
+            if not isinstance(gates, str):
+                raise TypeError(f"Strings are needs but get f{type(gates)}")
+            gate_op = re.findall("[a-zA-Z]+", gates)
+            gate_idx = [int(idx) for idx in re.findall("[0-9]+", gates)]
+            if len(gate_op) != len(gate_idx):
+                raise ValueError("Illegal pauli measurement.")
+            gates = zip(gate_idx, gate_op)
 
-            if not len(locations) == len(set(locations)):
-                raise ValueError("Error pauli measurement.")
+        elif format == "openfermion":
+            pass
 
-            for i in range(len(gates)):
-                if gates[i] in ["x", "X"]:
-                    self._measure_recording.append(
-                        f"H(q[{locations[i]}]);",
-                    )
-                    self._measure_recording.append(
-                        f"M(q[{locations[i]}]);",
-                    )
-                elif gates[i] in ["y", "Y"]:
-                    self._measure_recording.append(
-                        f"X2P(q[{locations[i]}]);",
-                    )
-                    self._measure_recording.append(
-                        f"M(q[{locations[i]}]);",
-                    )
-                elif gates[i] in ["z", "Z"]:
-                    self._measure_recording.append(
-                        f"M(q[{locations[i]}]);",
-                    )
-                else:
-                    raise ValueError(
-                        f"Please input correct Pauli gates instead of {gates[i]}.")
+        else:
+            raise QuantumCircuitError(f"Unsupported format {format!s}")
 
-        elif format == "openfermion":
-            for single_gate in gate_name:
-                if single_gate[1] == "X":
-                    self._measure_recording.append(
-                        f"H(q[{single_gate[0]}]);",
-                    )
-                    self._measure_recording.append(
-                        f"M(q[{single_gate[0]}]);",
-                    )
-                elif single_gate[1] == "Y":
-                    self._measure_recording.append(
-                        f"X2P(q[{single_gate[0]}]);",
-                    )
-                    self._measure_recording.append(
-                        f"M(q[{single_gate[0]}]);",
-                    )
-                elif single_gate[1] == "Z":
-                    self._measure_recording.append(
-                        f"M(q[{single_gate[0]}]);",
-                    )
-                else:
-                    raise ValueError("Please input correct Pauli gates.")
+        for gate in gates:
+            if gate[1].upper() == "X":
+                self._measure_recording.append(
+                    f"H(q[{gate[0]}]);",
+                )
+                self._measure_recording.append(
+                    f"M(q[{gate[0]}]);",
+                )
+            elif gate[1].upper() == "Y":
+                self._measure_recording.append(
+                    f"X2P(q[{gate[0]}]);",
+                )
+                self._measure_recording.append(
+                    f"M(q[{gate[0]}]);",
+                )
+            elif gate[1].upper() == "Z":
+                self._measure_recording.append(
+                    f"M(q[{gate[0]}]);",
+                )
+            else:
+                raise ValueError("Please input correct Pauli gates.")
 
     def pauli_measure(self, **params):
         """
         Pauli measurement.
         """
 
+        if not self.is_pauli_measure:
+            print("Warning: using pauli measurement without giving pauli operators.")
+
         if len(self._measure_recording) == 0:
             raise ValueError("Please set measurement.")
 
         if self.use_hardware:
             task = self._measure_hardware(**params)
             measure_result_dict = task.result()
             result = 0
```

### Comparing `isqlab-0.3.4/isqlab/linkers/torch_layer.py` & `isqlab-0.3.6/isqlab/linkers/torch_layer.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/linkers/torch_linker.py` & `isqlab-0.3.6/isqlab/linkers/torch_linker.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/neural_networks/neural_network.py` & `isqlab-0.3.6/isqlab/neural_networks/neural_network.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/neural_networks/qnn_autograd.py` & `isqlab-0.3.6/isqlab/neural_networks/qnn_autograd.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/neural_networks/qnn_jax.py` & `isqlab-0.3.6/isqlab/neural_networks/qnn_jax.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/neural_networks/qnn_simulator.py` & `isqlab-0.3.6/isqlab/neural_networks/qnn_simulator.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/vqe/chem.py` & `isqlab-0.3.6/isqlab/vqe/chem.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/vqe/hamiltonian_measure.py` & `isqlab-0.3.6/isqlab/vqe/hamiltonian_measure.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,21 +35,20 @@
 def hamiltonian_measure(
     circuit: QuantumCircuit,
     qubit_hamiltonian: QubitOperator,
     **params,
 ) -> np.float64:
     """transform qubit hamiltonian to pauli measurements."""
 
-    coeffs, gates = _openfermion_to_pauligates(qubit_hamiltonian)
+    coeffs, gates_group = _openfermion_to_pauligates(qubit_hamiltonian)
 
     if circuit.use_hardware or circuit.method in ["simulator"]:
         measure_results = [1.0, ]
-        for gate in gates:
-            circuit.pauli(gate, format="openfermion")
-            # circuit.pauli(gate, format="str")
+        for gates in gates_group:
+            circuit.pauli(gates, format="openfermion")
             measure_results.append(circuit.pauli_measure(**params))
         return np.dot(measure_results, coeffs)
 
     # TODO: anp.array type??? support
     # elif circuit.method == "autograd":
     #     measure_results = anp.zeros(len(gates) + 1)
     #     measure_results[0] = 1.0
@@ -57,17 +56,16 @@
     #         circuit.pauli(gate, format="openfermion")
     #         # circuit.pauli(gate, format="str")
     #         measure_results[idx+1] = circuit.pauli_measure(**params)
     #     return anp.dot(measure_results, anp.array(coeffs))
 
     elif circuit.method == "autograd":
         measure_results = [1.0, ]
-        for gate in gates:
-            circuit.pauli(gate, format="openfermion")
-            # circuit.pauli(gate, format="str")
+        for gates in gates_group:
+            circuit.pauli(gates, format="openfermion")
             measure_results.append(circuit.pauli_measure(**params))
         return anp.dot(anp.array(measure_results), anp.array(coeffs))
 
     # TODO: jnp.array type??? support
     # elif circuit.method == "jax":
     #     measure_results = jnp.zeros(len(gates) + 1)
     #     measure_results = measure_results.at[0].set(1.0)
@@ -77,48 +75,49 @@
     #         measure_results = measure_results.at[idx + 1].set(
     #             circuit.pauli_measure(**params),
     #         )
     #     return jnp.vdot(measure_results, jnp.array(coeffs))
 
     elif circuit.method == "jax":
         measure_results = [1.0, ]
-        for gate in gates:
-            circuit.pauli(gate, format="openfermion")
-            # circuit.pauli(gate, format="str")
+        for gates in gates_group:
+            circuit.pauli(gates, format="openfermion")
             measure_results.append(circuit.pauli_measure(**params))
         return jnp.vdot(jnp.array(measure_results), jnp.array(coeffs))
 
     elif circuit.method in ["torch", "pytorch"]:
-        measure_results = torch.zeros(len(gates) + 1, dtype=torch.float)
+        measure_results = torch.zeros(len(gates_group) + 1, dtype=torch.float)
         # dtype
         measure_results[0] = 1.0
-        for idx, gate in enumerate(gates):
-            circuit.pauli(gate, format="openfermion")
+        for idx, gates in enumerate(gates_group):
+            circuit.pauli(gates, format="openfermion")
             measure_results[idx+1] = circuit.pauli_measure(**params)
         return torch.dot(
             measure_results,
             torch.tensor(coeffs).type_as(measure_results)
         )
 
     else:
         raise QuantumCircuitError("Method is not implemented yet.")
 
 
 def _openfermion_to_pauligates(
     qubit_hamiltonian: QubitOperator,
-) -> Tuple[List[float], List[str]]:
+) -> Tuple[List[float], List[tuple]]:
     """
     extract coefficients and gates of qubit hamiltonian.
     """
     coeffs = []
-    gates = []
-    for gate, coeff in qubit_hamiltonian.terms.items():
+    gates_group = []
+    for idx, (gate, coeff) in enumerate(qubit_hamiltonian.terms.items()):
         coeffs.append(coeff)
-        gates.append(gate)
-    return coeffs, gates[1:]
+        if idx == 0:
+            continue
+        gates_group.append(gate)
+    return coeffs, gates_group
 
     # hamiltonian_strs = str(qubit_hamiltonian).split("\n")
     # hamiltonian_strs[-1] += " +"
     #
     # coeffs = []
     # gates = []
     #
```

### Comparing `isqlab-0.3.4/isqlab/vqe/kupccgsd.py` & `isqlab-0.3.6/isqlab/vqe/kupccgsd.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/vqe/symmetry_preserving.py` & `isqlab-0.3.6/isqlab/vqe/symmetry_preserving.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/vqe/ucc.py` & `isqlab-0.3.6/isqlab/vqe/ucc.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab/vqe/uccsd.py` & `isqlab-0.3.6/isqlab/vqe/uccsd.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/isqlab.egg-info/PKG-INFO` & `isqlab-0.3.6/isqlab.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: isqlab
-Version: 0.3.4
+Version: 0.3.6
 Summary: application modules for isq
 Author: Yusheng Yang
 Author-email: yangys@arclightquantum.com
+License: MIT
 Platform: python 3.8+
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Isqlab is a Python library for isQ.
 
 ## Key Features
 
@@ -25,15 +27,15 @@
 Isqlab requires Python version 3.8 and above. Installation of isqlab can be done using:
 
 ```console
 git clone http://www.arclighttest.cn:8090/yangys/isqlab.git
 cd isqlab
 python setup.py bdist_wheel sdist
 cd dist
-pip install isqlab-0.3.4-py3-none-any.whl
+pip install isqlab-0.3.6-py3-none-any.whl
 ```
 
 ## Getting started
 
 See examples.
 
 ## Authors
```

### Comparing `isqlab-0.3.4/isqlab.egg-info/SOURCES.txt` & `isqlab-0.3.6/isqlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.4/setup.py` & `isqlab-0.3.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,20 @@
     # "pyscf",
     # "openfermion",
     # "openfermionpyscf",
 ]
 
 setup(
     name="isqlab",
-    version="0.3.4",
+    version="0.3.6",
     description="application modules for isq",
     platforms="python 3.8+",
+    python_requires=">=3.8",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yusheng Yang",
     author_email="yangys@arclightquantum.com",
+    license="MIT",
     packages=find_packages(where="."),
     package_data={"": ["*.txt"]},
     install_requires=requirements,
 )
```

