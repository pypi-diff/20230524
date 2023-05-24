# Comparing `tmp/ezQgd-0.0.0.3-py3-none-any.whl.zip` & `tmp/ezQgd-1.0.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 16842 bytes, number of entries: 13
--rw-r--r--  2.0 unx    27958 b- defN 23-Apr-13 13:36 ezQgd.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 11:54 qasmtoqcis/__init__.py
--rw-r--r--  2.0 unx     3973 b- defN 23-Apr-13 11:54 qasmtoqcis/const.py
--rw-r--r--  2.0 unx     7400 b- defN 23-Apr-13 11:54 qasmtoqcis/qasm.py
--rw-r--r--  2.0 unx    11185 b- defN 23-Apr-13 11:54 qasmtoqcis/qasm_to_qcis.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 11:54 qcistoqasm/__init__.py
--rw-r--r--  2.0 unx      409 b- defN 23-Apr-13 11:54 qcistoqasm/const.py
--rw-r--r--  2.0 unx     2612 b- defN 23-Apr-13 11:54 qcistoqasm/qcis.py
--rw-r--r--  2.0 unx     2216 b- defN 23-Apr-13 11:54 qcistoqasm/qcis_to_qasm.py
--rw-r--r--  2.0 unx      825 b- defN 23-Apr-13 13:40 ezQgd-0.0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 13:40 ezQgd-0.0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-13 13:40 ezQgd-0.0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      983 b- defN 23-Apr-13 13:40 ezQgd-0.0.0.3.dist-info/RECORD
-13 files, 57681 bytes uncompressed, 15220 bytes compressed:  73.6%
+Zip file size: 17199 bytes, number of entries: 13
+-rw-r--r--  2.0 unx    33043 b- defN 23-May-24 15:55 ezQgd.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 15:55 qasmtoqcis/__init__.py
+-rw-r--r--  2.0 unx     3973 b- defN 23-May-24 15:55 qasmtoqcis/const.py
+-rw-r--r--  2.0 unx     7400 b- defN 23-May-24 15:55 qasmtoqcis/qasm.py
+-rw-r--r--  2.0 unx    11185 b- defN 23-May-24 15:55 qasmtoqcis/qasm_to_qcis.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 15:55 qcistoqasm/__init__.py
+-rw-r--r--  2.0 unx      409 b- defN 23-May-24 15:55 qcistoqasm/const.py
+-rw-r--r--  2.0 unx     2612 b- defN 23-May-24 15:55 qcistoqasm/qcis.py
+-rw-r--r--  2.0 unx     2216 b- defN 23-May-24 15:55 qcistoqasm/qcis_to_qasm.py
+-rw-r--r--  2.0 unx      872 b- defN 23-May-24 16:02 ezQgd-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-24 16:02 ezQgd-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 23-May-24 16:02 ezQgd-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      976 b- defN 23-May-24 16:02 ezQgd-1.0.0.dist-info/RECORD
+13 files, 62824 bytes uncompressed, 15593 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: qcistoqasm/qcis.py
 Comment: 
 
 Filename: qcistoqasm/qcis_to_qasm.py
 Comment: 
 
-Filename: ezQgd-0.0.0.3.dist-info/METADATA
+Filename: ezQgd-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: ezQgd-0.0.0.3.dist-info/WHEEL
+Filename: ezQgd-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: ezQgd-0.0.0.3.dist-info/top_level.txt
+Filename: ezQgd-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ezQgd-0.0.0.3.dist-info/RECORD
+Filename: ezQgd-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ezQgd.py

```diff
@@ -1,117 +1,42 @@
 # -*- coding: utf-8 -*-
 import json
 import requests
 import re
+import os
 import traceback
 from time import time, sleep
 import random
 import datetime
 import numpy as np
 from qasmtoqcis.qasm_to_qcis import QasmToQcis
 from qcistoqasm.qcis_to_qasm import QcisToQasm
 from isqmap import transpile
+from sabreMapper.sabre_mapper import SabreMapper
+from typing import List, Optional, Dict
 
 
-class QcisCheck():
-
-    def __init__(self, circuit=None):
-        self.circuit = circuit
-
-    def circuit_regular(self):
-        regular_exp_map = {
-            'X': r'^X(?:\s(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'Y': r'^Y(?:\s(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'Z': r'^Z(?:\s(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'X2P': r'^X2P(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'X2M': r'^X2M(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'Y2P': r'^Y2P(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'Y2M': r'^Y2M(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'H': r'^H(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'S': r'^S(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'SD': r'^SD(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'T': r'^T(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'TD': r'^TD(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){1}$',
-            'CZ': r'^CZ(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9]))){2}$',
-            'RX': r'^RX\s(?:Q(?:[1-5][0-9]|60|[1-9]))\s([+-]?([0-9]*[.])?([0-9]+|[0-9]+[E][+-]?[0-9]+))$',
-            'RY': r'^RY\s(?:Q(?:[1-5][0-9]|60|[1-9]))\s([+-]?([0-9]*[.])?([0-9]+|[0-9]+[E][+-]?[0-9]+))$',
-            'RZ': r'^RZ\s(?:Q(?:[1-5][0-9]|60|[1-9]))\s([+-]?([0-9]*[.])?([0-9]+|[0-9]+[E][+-]?[0-9]+))$',
-            'RXY': r'^RXY\s(?:Q(?:[1-5][0-9]|60|[1-9]))\s([+-]?([0-9]*[.])?([0-9]+|[0-9]+[E][+-]?[0-9]+))\s([+-]?([0-9]*[.])?([0-9]+|[0-9]+[E][+-]?[0-9]+))$',
-            'M': r'^M(?:\s+(?:Q(?:[1-5][0-9]|60|[1-9])))+$'
-        }
-        self.circuit = self.circuit.upper()
-        circuit_list = self.circuit.strip().split('\n')
-        measure_list = []  # 所有的M门，M门不能为空，并且所有的qubit不能重复
-        new_circuit_list = circuit_list.copy()
-        for index, circuit in enumerate(circuit_list):
-            circuit = circuit.strip()
-            cir = re.sub(' + ', ' ', circuit)  # 去掉中间多余的空格
-            gate = cir.split(' ')[0]
-            if gate in regular_exp_map.keys():
-                # 判断是否符合基本的正则
-                pattern = re.compile(regular_exp_map[gate], re.I)
-                result = pattern.match(cir)
-                if result is None:
-                    return False
-            else:
-                return False
-            if gate == 'M':
-                # M后面不能存在相同的qubit
-                qubit_list = cir.split(' ')[1:]
-                measure_list.extend(qubit_list)
-                after_measure_list = circuit_list[index:]
-                for after_cir in after_measure_list:
-                    after_cir = after_cir.strip()
-                    if after_cir.startswith('M'):
-                        continue
-                    # 判断M之后的指令是否有M中的qubit
-                    is_correct = [False if qubit in after_cir else True
-                                  for qubit in qubit_list]
-                    if not all(is_correct):
-                        return False
-            # if gate == 'CZ':
-            #     # CZ指令需要两个qubit相减必须等于1，必须相邻qubit
-            #     qubit_list = cir.split(' ')[1:]
-            #     qubit0 = int(re.findall(r'\d+', qubit_list[0])[0])
-            #     qubit1 = int(re.findall(r'\d+', qubit_list[1])[0])
-            #     if abs(qubit1 - qubit0) != 1:
-            #         return False
-            if gate.startswith('R'):  # RX RY RZ RXY
-                gate_qubit = cir.split(' ')[:2]
-                gate_params = cir.split(' ')[2]
-                if abs(float(gate_params)) > np.pi:
-                    return False
-                # 匹配出指令中的小数，不包含科学计数法
-                r_result = re.findall(r'([+-]*?[0-9]\.\d*(?!E|e)[0-9])', cir)
-                n_result = []
-                for r in r_result:
-                    num_list = r.split('.')
-                    before = ''.join(num_list[0])
-                    after = num_list[1]
-                    if float(r) > 0 and len(after) > 2:
-                        n_r = before + '.' + ''.join(after[:2])
-                        n_result.append(n_r)
-                    elif float(r) < 0 and len(after) > 20:
-                        n_r = before + '.' + ''.join(after[:20])
-                        n_result.append(n_r)
-                if n_result:
-                    new_cir = [*gate_qubit, *n_result]
-                    new_circuit_list[index] = ' '.join(new_cir)
-        if len(measure_list) == 0 or \
-           len(measure_list) != len(set(measure_list)):
-            return False
-        new_circuit = '\n'.join(
-            [circuit.strip() for circuit in new_circuit_list])
-        return new_circuit
+class Account():
 
+    def __init__(
+            self, 
+            login_key: Optional[str]=None, 
+            machine_name: Optional[str]=None
+        ):
+        """accout initialization
 
-class Account():
+        Args:
+            login_key: 
+                API Token under personal center on the web. Defaults to None.. Defaults to None.
+            machine_name: 
+                name of quantum computer. Defaults to None.
 
-    def __init__(self, login_key=None, machine_name=None):
-        self.qcis_check = QcisCheck()
+        Raises:
+            Exception: throw an exception when login fails
+        """
         self.qasmtoqcis = QasmToQcis()
         self.qcistoqasm = QcisToQasm()
         self.login_key = login_key
         self.token = None
         self.machine_name = machine_name
         self.base_url = 'https://quantumctek-cloud.com/agency/'  # 生产环境url
         self.base_login_url = 'https://quantumctek-cloud.com/api-uaa/oauth/token' # 生产环境登录url
@@ -122,16 +47,15 @@
             print('登录成功')
 
     def log_in(self):
         """
         Authenticate username and password and return user credit
 
         Returns
-        -------
-        log in state, 0 means pass authentication, 1 means failed
+            int: log in state, 1 means pass authentication, 0 means failed
 
         """
         data = {
             'grant_type': 'openId',
             'openId': self.login_key,
             'account_type': 'member'
         }
@@ -147,22 +71,27 @@
         if code != 0:
             print(f'登录失败：{msg}')
             return 0
         token = result.get('data').get('access_token')
         self.token = token
         return 1
 
-    def create_experiment(self, exp_name, remark='测试'):
-        """create experiment
+    def create_experiment(
+            self, 
+            exp_name: str, 
+            remark: Optional[str]="测试"
+        ):
+        """create a new experiment, the new one is the experiment set ID.
 
         Args:
-            url (string): request the address
+            exp_name: new experiment collection Name.
+            remark: experimental remarks. Defaults to 测试.
 
         Returns:
-            0--失败, 非0成功
+            Union[int, str]: 0 failed, not 0 successful, success returns the experimental set id
         """
         url = f'{self.base_url}/service/sdk/api/experiment/save'
         data = {"name": exp_name,
                 "remark": remark}
         headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
         res = requests.post(url, json=data, headers=headers)
         status_code = res.status_code
@@ -174,30 +103,33 @@
         msg = result.get('message', '创建实验失败')
         if code != 0:
             print(f'创建实验失败：{msg}')
             return 0
         lab_id = result.get('data').get('lab_id')
         return lab_id
 
-    def save_experiment(self, lab_id, exp_data, name='detailtest', language='qcis'):
-        """save experiment
+    def save_experiment(
+            self, 
+            lab_id: str, 
+            exp_data: str, 
+            name: Optional[str]="detailtest", 
+            language: Optional[str]="qcis"
+        ):
+        """save the experiment and return the experiment ID.
 
         Args:
-            url (string): request the addresslab_id
+            lab_id: 
+                the result returned by the create_experiment interface, experimental set id
+            exp_data: 
+                experimental content, qics
+            name: experimental Details Name. Defaults to "detailtest".
+            language: Quantum computer language, including ['isq', 'quingo', 'qcis']. Defaults to "qcis".
 
         Returns:
-            0--失败, 非0成功
-
-        12比特异常情况：
-            1.保存实验返回的结果-->{'code':500, 'msg': XXX}
-            2.保存实验返回的结果-->  (多进程同时请求可能出现的情况)
-            3.保存实验返回的结果-->exp_id,当前实验已保存
-            4.保存实验返回的结果-->量子线路指令输入错误，请检查你的输入
-        正常情况：
-            1.保存实验返回的结果-->exp_id
+            Union[int, str]: 0 failed, not 0 successful, success returns the experiment id.
         """
         language_list = ['isq', 'quingo', 'qcis']
         if language not in language_list:
             print(f'保存实验失败, 量子语言只能在{language_list}中选择')
         exp_data = self.get_experiment_data(exp_data.upper())
         url = self.base_url + '/service/sdk/api/experiment/detail/save'
         data = {
@@ -216,27 +148,37 @@
         msg = result.get('message', '保存实验失败')
         if code != 0:
             print(f'保存实验失败：{msg}')
             return 0
         save_result = result.get('data').get('exp_id')
         return save_result
 
-    def run_experiment(self, exp_id, num_shots=12000):
-        """run experiment
+    def run_experiment(
+            self,
+            exp_id: str, 
+            num_shots: Optional[int]=12000
+        ):
+        """running the experiment returns the query result id.
 
         Args:
-            url (string): request the address
+            exp_id: 
+                the result returned by the save_experiment interface, experimental id
+            num_shots: 
+                number of repetitions per experiment. Defaults to 12000.
 
         Returns:
-            0--失败, 非0成功
+            Union[int, str]: 0 failed, not 0 successful, success returns the query id
         """
         data = {"exp_id": exp_id, "shots": num_shots}
         return self.handler_run_experiment_result(data)
 
-    def handler_run_experiment_result(self, data):
+    def handler_run_experiment_result(
+            self, 
+            data
+        ):
         url = self.base_url + '/service/sdk/api/experiment/temporary/save'
         headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
         res = requests.post(url, json=data, headers=headers)
         status_code = res.status_code
         if status_code != 200:
             print('运行实验接口请求失败')
             return 0
@@ -246,17 +188,47 @@
         if code != 0:
             print(f'运行实验失败：{msg}')
             return 0
         run_result = result.get('data').get('query_id')
         return run_result
 
     def submit_job(
-            self, circuit=None, exp_name="exp0",
-            parameters=None, values=None, num_shots=12000,
-            lab_id=None, exp_id=None, version="version01"):
+            self,
+            circuit: Optional[str]=None, 
+            exp_name: Optional[str]="exp0",
+            parameters: Optional[List]=None, 
+            values: Optional[List]=None,
+            num_shots: Optional[int]=12000,
+            lab_id: Optional[str]=None, 
+            exp_id: Optional[str]=None, 
+            version: Optional[str]="version01"
+        ):
+        """submit experimental tasks
+
+        Args:
+            circuit: 
+                experimental content, qics. Defaults to None.
+            exp_name:
+                new experiment collection Name. Defaults to 'exp0'.
+            parameters: 
+                parameters that need to be assigned in the experimental content. Defaults to None.
+            values: 
+                The values corresponding to the parameters that need to be assigned in the experimental content. Defaults to None.
+            num_shots:
+                number of repetitions per experiment. Defaults to 12000.
+            lab_id: 
+                the result returned by the create_experiment interface, experimental set id. Defaults to None.
+            exp_id: 
+                the result returned by the save_experiment interface, experimental id. Defaults to None.
+            version: 
+                version description. Defaults to 'version01'.
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, success returns the query id.
+        """
         if circuit:
             circuit = self.assign_parameters(
                 circuit.upper(), parameters, values)
             if not circuit:
                 print('无法为线路赋值，请检查线路，参数和参数值之后重试')
                 return 0
         data = {
@@ -266,26 +238,31 @@
             "languageCode": "qcis",
             "name": exp_name,
             "shots": num_shots,
             "source": "SDK",
             "computerCode": self.machine_name,
             "experimentDetailName": version
         }
-        print(data)
         return self.handler_run_experiment_result(data)
 
-    def query_experiment(self, query_id, max_wait_time=60):
-        """query experiment
+    def query_experiment(
+            self,
+            query_id: str,
+            max_wait_time: Optional[int]=60
+        ):
+        """query experimental results
 
         Args:
-            query_id (int): 查询id
-            max_wait_time(int): 最大等待时间
+            query_id: 
+                the result returned by the run_experiment interface, experimental set id
+            max_wait_time: 
+                maximum waiting time for querying experiments. Defaults to 60.
 
         Returns:
-            0--失败, 非0成功
+            Union[int, str]: 0 failed, not 0 successful, success returns the experimental result
         """
         t0 = time()
         while time()-t0 < max_wait_time:
             try:
                 url = f'{self.base_url}/service/sdk/api/experiment/result/find/{query_id}'
                 headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
                 res = requests.get(url, headers=headers)
@@ -306,27 +283,32 @@
             sleep_time = random.randint(
                 0, 15)*0.3+round(random.uniform(0, 1.5), 2)
             print(f'查询实验结果请等待: {{:.2f}}秒'.format(sleep_time))
             sleep(sleep_time)
         print(f'查询实验结果失败')
         return 0
 
-    def assign_parameters(self, circuit, parameters, values):
-        """
-        Check if the number of parameters, values match the circuit definition
+    def assign_parameters(
+            self,
+            circuit: str, 
+            parameters: List, 
+            values: List
+        ):
+        """Check if the number of parameters, values match the circuit definition
 
-        Parameters
-        ----------
-        circuit : string, QCIS circuit definition with or without parameter place holder
-        parameters : list or ndarray of strings, parameters to be filled
-        values : list or ndarray of floats, values to be assigned
+        Args:
+            circuit: 
+                string, QCIS circuit definition with or without parameter place holder
+            parameters: 
+                list or ndarray of strings, parameters to be filled
+            values: 
+                list or ndarray of floats, values to be assigned
 
-        Returns
-        -------
-        circuit : circuit with parameters replaced by values or empty string
+        Returns:
+            circuit: circuit with parameters replaced by values or empty string
             empty string occurs when errors prevents parameters to be assigned
         """
         circuit = circuit.upper()
         p = re.compile(r'\{(\w+)\}')
         circuit_parameters = p.findall(circuit)
         if circuit_parameters:
 
@@ -371,42 +353,62 @@
             error_message = '线路定义中不含有参数，无法接受您输入的参数或参数值'
             print(error_message)
             return ''
         else:
             expData = circuit
             return expData
 
-    def get_experiment_data(self, circuit):
-        """
-        Parse circuit description and generate 
-        experiment script and extract number
-        of measured qubits
-
-        Parameters
-        ----------
-        circuit : string, QCIS circuit
+    def get_experiment_data(
+            self, 
+            circuit: str
+        ):
+        """Parse circuit description and generate 
+           experiment script and extract number of measured qubits.
 
-        Returns
-        -------
-        expData : string, transformed circuit
+        Args:
+            circuit: 
+                string, QCIS circuit
 
+        Returns:
+            expData: 
+                string, transformed circuit
         """
         # get gates from circuit
         gates_list = circuit.split('\n')
         gates_list_strip = [g.strip() for g in gates_list if g]
         gates_list_strip = [g for g in gates_list_strip if g]
 
         # transform circuit from QCIS to expData
         expData = '\n'.join(gates_list_strip)
         return expData
 
-    def set_machine(self, machine_name):
+    def set_machine(
+            self, 
+            machine_name: str
+        ):
+        """set the machine name.
+
+        Args:
+            machine_name: name of quantum computer.
+        """
         self.machine_name = machine_name
 
-    def download_config(self, down_file=True):
+    def download_config(
+            self, 
+            down_file: Optional[bool]=True
+        ):
+        """download experimental parameters.
+
+        Args:
+            down_file: 
+                the parameter is True to write to the file, and False to directly return the experimental parameters. Defaults to True.
+
+        Returns:
+           Union[int, str]: 0 failed, not 0 successful, success returns the experimental parameters.
+        """
         url = f'{self.base_url}/service/sdk/api/experiment/download/config/{self.machine_name}'
         headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
         res = requests.get(url, headers=headers)
         status_code = res.status_code
         if status_code != 200:
             return 0
         result = json.loads(res.text)
@@ -418,76 +420,182 @@
         data = result.get('data')
         cur_time = self.current_time()
         if down_file:
             with open(f'./{self.machine_name}_config_param_{cur_time}.json', 'w') as f:
                 f.write(json.dumps(data))
         return data
 
-    def convert_qasm_to_qcis(self, qasm):
-        qcis_raw = self.qasmtoqcis.convert_qasm_to_qcis(qasm)
+    def convert_qasm_to_qcis(
+            self, 
+            qasm: str, 
+            qubit_map: Optional[Dict]=None
+        ):
+        """convert qasm to qcis.
+
+        Args:
+            qasm: 
+                qasm.
+            qubit_map: 
+                Number mapping in qasm, where the value is None, 
+                directly maps bits based on the format of number plus 1. Defaults to None.
+        Raises:
+            Exception: language conversion failed.
+
+        Returns:
+            str: simplified qcis.
+        """
+        qcis_raw = self.qasmtoqcis.convert_qasm_to_qcis(qasm, qubit_map=qubit_map)
         simplity_qcis = self.qasmtoqcis.simplify(qcis_raw)
         return simplity_qcis
 
-    def convert_qasm_to_qcis_from_file(self, qasm_file):
-        qcis_raw = self.qasmtoqcis.convert_qasm_to_qcis_from_file(qasm_file)
+    def convert_qasm_to_qcis_from_file(
+            self, 
+            qasm_file: str, 
+            qubit_map: Optional[Dict]=None
+        ):
+        """Read qasm from file and convert it to qcis
+
+        Args:
+            qasm_file: 
+                qasm file.
+            qubit_map: 
+                Number mapping in qasm, where the value is None, 
+                directly maps bits based on the format of number plus 1. Defaults to None.
+
+        Raises:
+            Exception: language conversion failed.
+
+        Returns:
+            str: simplified qcis.
+        """
+        qcis_raw = self.qasmtoqcis.convert_qasm_to_qcis_from_file(qasm_file, qubit_map=qubit_map)
         simplity_qcis = self.qasmtoqcis.simplify(qcis_raw)
         return simplity_qcis
     
-    def convert_qcis_to_qasm(self, qcis):
+    def convert_qcis_to_qasm(
+            self, 
+            qcis: str
+        ):
+        """convert qcis to qasm.
+
+        Args:
+            qcis: qcis
+
+        Returns:
+            str: converted qasm.
+        """
         qasm_circuit = self.qcistoqasm.convert_qcis_to_qasm(qcis)
         return qasm_circuit
 
-    def qcis_check_regular(self, qcis_raw):
-        self.qcis_check.circuit = qcis_raw
-        res = self.qcis_check.circuit_regular()
-        if isinstance(res, bool):
-            print('量子线路指令输入错误，请检查你的输入')
+    def qcis_check_regular(
+            self, 
+            qcis_raw: str
+        ):
+        """qcis regular check,normal returns 1, abnormal returns 0
+
+        Args:
+            qcis_raw: qcis
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, successfully returned the input qics.
+        """
+        url = f'{self.base_url}service/sdk/api/experiment/qcis/rule/verify'
+        data = {
+            "computerCode": self.machine_name,
+            "qcis": qcis_raw
+        }
+        res = requests.post(url, json=data)
+        status_code = res.status_code
+        if status_code != 200:
+            print(f'qcis检验失败, code:{status_code}')
             return 0
-        return res
+        result = json.loads(res.text)
+        code = result.get('code', -1)
+        msg = result.get('message', 'qcis检验失败')
+        if code != 0:
+            print(f'qcis检验失败: {msg}')
+            return 0
+        return qcis_raw
+
+    def simplify(
+            self, 
+            qcis_raw: str
+        ):
+        """simplification of qcis lines.
+
+        Args:
+            qcis_raw: qcis
 
-    def simplify(self, qcis_raw):
+        Returns:
+            str: simplified qcis.
+        """
         new_qcis_raw = self.qcis_check_regular(qcis_raw)
         simplity_qcis = self.qasmtoqcis.simplify(new_qcis_raw)
         return simplity_qcis
     
     def current_time(self):
+        """get the current time
+
+        Returns:
+            str: time string
+        """
         timestamp = datetime.datetime.fromtimestamp(time())
         str_time = timestamp.strftime('%Y%m%d%H%M%S')
         return str_time
 
-    def readout_data_to_state_probabilities(self, result):
-        '''
-            circuit: 线路
-            result: 原始数据
-        '''
+    def readout_data_to_state_probabilities(
+            self, 
+            result
+        ):
         state01 = result.get('resultStatus')
         basis_list = []
         basis_content = ''.join([''.join([str(s) for s in state]) for state in state01[1:]])
         qubits_num = len(state01[0])  # 测量比特个数
         for idx in range(qubits_num):
             basis_result = basis_content[idx: len(basis_content): qubits_num]
             basis_list.append([True if res == "1" else False for res in basis_result])
         return basis_list
 
     # 读取数据转换成量子态概率
-    def readout_data_to_state_probabilities_whole(self, result):
-        '''
-            circuit: 线路
-            result: 原始数据
-        '''
+    def readout_data_to_state_probabilities_whole(
+            self, 
+            result: Dict
+        ):
+        """read data and convert it into a quantum state probability, all returns.
+
+        Args:
+            result: the results returned after query_experiment.
+
+        Returns:
+            Dict: probability
+        """
         basis_list = self.readout_data_to_state_probabilities(result)
         probabilities = self.original_onversion_whole(basis_list)
         return probabilities
     
-    def readout_data_to_state_probabilities_part(self, result):
+    def readout_data_to_state_probabilities_part(
+            self, 
+            result: Dict
+        ):
+        """read data and convert it into a quantum state probability, do not return with a probability of 0.
+
+        Args:
+            result: the results returned after query_experiment.
+
+        Returns:
+            Dict: probability
+        """
         basis_list = self.readout_data_to_state_probabilities(result)
         probabilities = self.original_onversion_part(basis_list)
         return probabilities
     
-    def original_onversion_whole(self, state01):
+    def original_onversion_whole(
+            self, 
+            state01
+        ):
         #当state01为一维时转换成二维数据
         if isinstance(state01[0], bool):
             state01=[state01]
         n = len(state01)  # 读取比特数
         # 测量比特概率限制
         # if n > MAX_QUBIT_NUM:
         #     print(f'Number of qubits > {MAX_QUBIT_NUM}, cannot calculate probabilities.')
@@ -501,15 +609,18 @@
                 k += state01_T[num][i] * (2 ** i)
             counts[k] += 1
         # 计算概率
         # P=[counts[k]/numShots for k in range(2**n)]
         P = {bin(k)[2:].zfill(n): counts[k]/numShots for k in range(2**n)}
         return P
     
-    def original_onversion_part(self, state01):
+    def original_onversion_part(
+            self, 
+            state01
+        ):
         #当state01为一维时转换成二维数据
         if isinstance(state01[0], bool):
             state01=[state01]
         n = len(state01)  # 读取比特数
         # 测量比特概率限制
         # if n > MAX_QUBIT_NUM:
         #     raise Exception(f'Number of qubits > {MAX_QUBIT_NUM}, cannot calculate probabilities.')
@@ -528,35 +639,40 @@
                 counts[prob_state] += 1
         # 计算概率
         # P=[counts[k]/numShots for k in range(2**n)]
         P = {k: v/numShots for k, v in counts.items()}
         return P
     
     # 量子态概率矫正
-    def probability_calibration(self, result):
-        '''
-            对测量得到的 01 量子态概率进行校正
-            参数
-            • iq2probFidelity (list[list]) -- 校正系数矩阵，列表每个元素是一个 list, 存
-            储一个比特的概率校正系数，每个比特有两个校正系数，例如
-                [
-                [0.5, 0.5], # 比 特0
-                [0.1, 0.9], # 比 特1
-                [0.8, 0.2], # 比 特2
-                ]
-            • pm (list[float]) -- 待矫正的 01 量子态概率，长度为 2*k, 其中 k 是 iq2probFidelity
-            的行数 (即比特个数)
-            返回类型 list[float]
+    def probability_calibration(
+            self, 
+            result: Dict, 
+            config_json: Optional[Dict]=None):
+        """correction of the measured probability of 01 quantum state.
+
+        Args:
+            result:
+                the results returned after query_experiment.
+            config_json: 
+                experimental parameters of quantum computer. 
+                config_json value is None, read the latest experimental parameters for calculation.
+                Defaults to None.
+
+        Raises:
+            Exception: cannot calibrate probability with fidelity.
 
-        '''
+        Returns:
+            Dict: corrected probability.
+        """
         CM_CACHE = {}
-        config_json = self.download_config(down_file=False)
+        if config_json is None:
+            config_json = self.download_config(down_file=False)
         qubit_num = [f'Q{i}' for i in result.get('resultStatus')[0]]
         n = len(qubit_num)  # 测量比特个数
-        qubits = config_json['overview']['qubits']
+        qubits = config_json['readout']['readoutArray']['|0> readout fidelity']['qubit_used']
         readout_fidelity0 = config_json['readout']['readoutArray']['|0> readout fidelity']['param_list']
         readout_fidelity1 = config_json['readout']['readoutArray']['|1> readout fidelity']['param_list']
         iq2probFidelity = [[readout_fidelity0[qubits.index(q)], readout_fidelity1[qubits.index(q)]] for q in qubit_num]
         P = self.readout_data_to_state_probabilities_whole(result)
         Pm = list(P.values())
         if not isinstance(iq2probFidelity[0], list):
             iq2probFidelity=[iq2probFidelity]
@@ -573,17 +689,77 @@
             CM_CACHE[f] = inv_CM
         else:
             inv_CM = CM_CACHE[f]
         Pi = np.dot(inv_CM, (np.array(Pm, ndmin=2).T))
         Pi = {bin(idx)[2:].zfill(n): k[0] for idx, k in enumerate(Pi)}
         return Pi
     
+    # 对矫正后的概率进行修正
+    def probability_correction(self, probabilities):
+        """correction of the measured probability of 01 quantum state.
+           If there is a probability greater than 1, change this item to 1; 
+           If there is anything less than 0, change the item to 0.
+
+        Args:
+            probabilities:
+               corrected probability.
+            
+        Returns:
+            Dict: corrected probability.
+        """
+        abnormal_fidelity_list = list(filter(lambda x: x < 0 or x > 1, probabilities.values()))
+        if not abnormal_fidelity_list:
+            return probabilities
+        for k, v in probabilities.items():
+            if v > 1:
+                probabilities[k] = 1
+            elif v < 0:
+                probabilities[k] = 0
+        fidelity_sum = sum(probabilities.values())
+        for k, v in probabilities.items():
+            probabilities[k] = v / fidelity_sum
+        return probabilities
+    
     def qcis_mapping_isq(
-            self, qcis_circuit, initial_layout=None,
-            objective='size', seed=None, use_post_opt=False):
+            self, 
+            qcis_circuit: str, 
+            initial_layout: Optional[Dict]=None,
+            objective: Optional[str]='size', 
+            seed: Optional[int]=None, 
+            use_post_opt: Optional[bool]=False
+        ):
+        """The script transpiles qcis string by searching for a mapping from virtual to physical qubit 
+           and a swap strategy such that the circuit described by qcis can be fitted into a hardware 
+           described by the coupling_map, in the meanwhile reduces circuit depth.
+
+        Args:
+            qcis_circuit: qcis circuit
+            initial_layout: 
+                Initial position of virtual qubits on physical qubits.
+                If given, this is the initial state in search of virtual to physical qubit mapping
+                e.g.:
+                    {0:4, 1:1, 2:5, 3:2, 4:0, 5:3}. Defaults to None.
+            objective: 
+                size: min. # of added swaps
+                depth: min. depth
+                no_swap: try best to find an initial mapping requiring no swaps; raise 
+                an error if fail. Defaults to 'size'.
+            seed: 
+                Set random seed for the stochastic part of the tranpiler. Defaults to None.
+            use_post_opt: 
+                we provide a genetic alg. which utilizes exchange rules for
+                swaps to futher min. depth. Defaults to False.
+
+        raised:
+            TranspileError:
+                if graph specified by coupling map is disconnected.
+
+        Returns:
+            str: qcis string after transpilation
+        """
         config_json = self.download_config(down_file=False)
         try:
             qasm_circuit = self.convert_qcis_to_qasm(qcis_circuit)
             cur_time = self.current_time()
             qpu_file = f'./{self.machine_name}_config_param_{cur_time}.json'
             with open(qpu_file, 'w') as f:
                 f.write(json.dumps(config_json))
@@ -597,41 +773,43 @@
             return simplity_qcis
         except Exception as e:
             print(e)
             print(traceback.format_exc())
             print('circuit mapping error, will submit using the original route')
             return qcis_circuit
     
-    """
-        qcis mapping quingo temporary comment blocking
-    """
-    """
-    def qcis_mapping_quingo(self, qcis_circuit):
-        '''qcis mapping
+    def qcis_mapping_sabre(
+            self, 
+            qcis_circuit: str):
+        """The script transpiles qcis string by searching for a mapping from virtual to physical qubit 
+           and a swap strategy such that the circuit described by qcis can be fitted into a hardware 
+           described by the coupling_map, in the meanwhile reduces circuit depth.
 
         Args:
-            qcis_circuit (str): qcis circuit
+            qcis_circuit: qcis circuit
 
         Returns:
             str : qcis after mapping
-        '''        
+        """       
         config_json = self.download_config(down_file=False)
         try:
             # qcis转换成qasm并写入qasm_file中
             qasm_circuit = self.qcistoqasm.convert_qcis_to_qasm(qcis_circuit)
+            if not os.path.exists('temp'):
+                os.makedirs('temp')
             qasm_file = 'temp/qasm.qasm'
             with open(qasm_file, 'w') as f:
                 f.write(qasm_circuit)
             sabre = SabreMapper()
             # 组装chip_info_fn映射信息
             chip_info_fn = {}
             couplings = []
             coupler_maps = config_json.get('overview').get('coupler_map')
-            coupler_used = config_json.get('two qubit gate').get('czGate').get('gate error').get('qubit_used')
-            cz_gate_error = config_json.get('two qubit gate').get('czGate').get('gate error').get('param_list')
+            coupler_used = config_json.get('twoQubitGate').get('czGate').get('gate error').get('qubit_used')
+            cz_gate_error = config_json.get('twoQubitGate').get('czGate').get('gate error').get('param_list')
             for coupler, error in zip(coupler_used, cz_gate_error):
                 fidelity = 1- error
                 coupler_qubit_map = coupler_maps.get(coupler)
                 couplings.append({"fidelity": fidelity, "qubit pair": coupler_qubit_map})
             chip_info_fn['couplings'] = couplings
             qubit_used = config_json.get('qubit').get('singleQubit').get('gate error').get('qubit_used')
             qubit_gate_error = config_json.get('qubit').get('singleQubit').get('gate error').get('param_list')
@@ -654,10 +832,37 @@
                     qubit_mapping_fn = json.load(f)
                 qubit_map = qubit_mapping_fn.get('physical qubits idx')
                 # mapping成功，将转换后的qasm转为qcis，其中编号根据physical qubits idx做映射
                 simplity_qcis = self.convert_qasm_to_qcis_from_file(mapped_qasm_fn_file, qubit_map)
                 return simplity_qcis
         except Exception as e:
             print(e)
+            import traceback
+            print(traceback.format_exc())
             print('circuit mapping error, will submit using the original route')
             return qcis_circuit
-    """
+
+    def get_experiment_circuit(
+            self,
+            exp_id: str):
+        """according to the exp_id obtained experimental circuit
+
+        Args:
+            exp_id: the result returned by the save_experiment interface, experimental id.
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, success returns the experimental circuit
+        """
+        url = f'{self.base_url}service/sdk/api/experiment/getQcis/by/{exp_id}'
+        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
+        res = requests.get(url, headers=headers)
+        status_code = res.status_code
+        if status_code != 200:
+            return 0
+        result = json.loads(res.text)
+        code = result.get('code', -1)
+        msg = result.get('msg', '查询实验线路失败')
+        if code != 0:
+            print(f'查询实验线路: {msg}')
+            return 0
+        circuit = result.get('data').get('qcis')
+        return circuit
```

## Comparing `ezQgd-0.0.0.3.dist-info/METADATA` & `ezQgd-1.0.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezQgd
-Version: 0.0.0.3
+Version: 1.0.0
 Summary: A SDK to use Quantum Computer @ quantumctek-cloud.com with QCIS.
 Home-page: https://quantumctek-cloud.com
 Author: Code42
 Author-email: support@quantumctek-cloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4
 Requires-Dist: numpy
 Requires-Dist: requests
+Requires-Dist: isqmap
+Requires-Dist: sabreMapper
 
 
 # 国盾量子计算云平台量子编程教学(Readme版)
 # https://quantumctek-cloud.com
```

## Comparing `ezQgd-0.0.0.3.dist-info/RECORD` & `ezQgd-1.0.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-ezQgd.py,sha256=GM4359c87JMFvKcLg31-0n9PfK8hLNccsUdQ9jI6FE8,27958
+ezQgd.py,sha256=5yqx39Gd64sNI4eA2cA88W79BaCca7VnKVC0TlfJiIU,33043
 qasmtoqcis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qasmtoqcis/const.py,sha256=AZTrt8AjrREnIHsK_VQrd_fEcB3TNBJqR1TiatsIurY,3973
 qasmtoqcis/qasm.py,sha256=Uu8zrTXpDCQok2lAeMCSChzjY6oE1xoV8LulgpAJSYc,7400
 qasmtoqcis/qasm_to_qcis.py,sha256=MSCwpWKtqcc5kY9tUgqg_0x30yi7J9v98_p89ikcKgI,11185
 qcistoqasm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qcistoqasm/const.py,sha256=jeuG0MbtqK3MxFlCC_eGwlsUO1nYp6B20KGztuJgmoc,409
 qcistoqasm/qcis.py,sha256=r5ae12O9ZFkCl3Bgw3ldyt2l451rESfZUC7P-qEaTL8,2612
 qcistoqasm/qcis_to_qasm.py,sha256=458xj6Z6rYhCD8918bc7TZZXLKcHhdJgPwQYCqOKIfM,2216
-ezQgd-0.0.0.3.dist-info/METADATA,sha256=2mcxRS0zCbIEsKat84bwUiTzUgrhmXxa09AqlE2UUt8,825
-ezQgd-0.0.0.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-ezQgd-0.0.0.3.dist-info/top_level.txt,sha256=5SxS9D4ntYSuP5DotvN8wGdQVSZzRN2_NfaD7QO5U8o,28
-ezQgd-0.0.0.3.dist-info/RECORD,,
+ezQgd-1.0.0.dist-info/METADATA,sha256=WK3IaUl31d_zCL1M4Xp2fIkBJ2UJjg10STRcdJz_OxM,872
+ezQgd-1.0.0.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+ezQgd-1.0.0.dist-info/top_level.txt,sha256=5SxS9D4ntYSuP5DotvN8wGdQVSZzRN2_NfaD7QO5U8o,28
+ezQgd-1.0.0.dist-info/RECORD,,
```

