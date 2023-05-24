# Comparing `tmp/isqopen-1.0.1.tar.gz` & `tmp/isqopen-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isqopen-1.0.1.tar", last modified: Thu Apr 20 09:17:47 2023, max compression
+gzip compressed data, was "dist/isqopen-1.0.2.tar", last modified: Wed May 24 10:19:57 2023, max compression
```

## Comparing `isqopen-1.0.1.tar` & `isqopen-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.595718 isqopen-1.0.1/
--rw-r--r--   0 huazhelou   (501) staff       (20)     1093 2022-09-07 10:16:53.000000 isqopen-1.0.1/LICENSE
--rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-04-20 09:17:47.595852 isqopen-1.0.1/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)      734 2022-09-24 07:03:24.000000 isqopen-1.0.1/README.md
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.587623 isqopen-1.0.1/isq/
--rw-r--r--   0 huazhelou   (501) staff       (20)      247 2023-04-17 07:47:49.000000 isqopen-1.0.1/isq/__init__.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.590577 isqopen-1.0.1/isq/compile/
--rw-r--r--   0 huazhelou   (501) staff       (20)     5836 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/compile/QSyn.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    11380 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/compile/Simplify.py
--rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-04-17 07:26:56.000000 isqopen-1.0.1/isq/compile/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5152 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/compile/matlab_gsvd.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    14686 2023-04-17 07:39:03.000000 isqopen-1.0.1/isq/compile/parser.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    22701 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/compile/parsetab.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    27549 2023-04-17 07:28:07.000000 isqopen-1.0.1/isq/compile/passes.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5050 2023-04-17 07:27:41.000000 isqopen-1.0.1/isq/compile/qtypes.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2183 2023-04-17 07:28:19.000000 isqopen-1.0.1/isq/compile/tokrules.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2539 2023-04-17 07:38:44.000000 isqopen-1.0.1/isq/compile/tools.py
--rw-r--r--   0 huazhelou   (501) staff       (20)       18 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/config.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.592009 isqopen-1.0.1/isq/device/
--rw-r--r--   0 huazhelou   (501) staff       (20)      142 2023-04-17 07:47:47.000000 isqopen-1.0.1/isq/device/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     6293 2023-04-20 08:59:29.000000 isqopen-1.0.1/isq/device/device.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     1882 2023-04-17 07:43:57.000000 isqopen-1.0.1/isq/device/grad.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2907 2023-04-17 07:45:20.000000 isqopen-1.0.1/isq/device/task.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     3578 2023-04-17 07:45:26.000000 isqopen-1.0.1/isq/device/translate.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.592799 isqopen-1.0.1/isq/draw/
--rw-r--r--   0 huazhelou   (501) staff       (20)       26 2023-04-17 07:47:34.000000 isqopen-1.0.1/isq/draw/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     7986 2023-04-17 07:42:07.000000 isqopen-1.0.1/isq/draw/drawer.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2652 2023-04-17 06:46:09.000000 isqopen-1.0.1/isq/errors.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     1221 2023-04-17 07:31:53.000000 isqopen-1.0.1/isq/globalVar.py
--rw-r--r--   0 huazhelou   (501) staff       (20)      250 2023-04-17 07:48:53.000000 isqopen-1.0.1/isq/qpu.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     6707 2023-04-20 08:59:15.000000 isqopen-1.0.1/isq/quantum.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.593737 isqopen-1.0.1/isq/simulate/
--rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-04-17 07:29:05.000000 isqopen-1.0.1/isq/simulate/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    12918 2023-04-17 07:29:15.000000 isqopen-1.0.1/isq/simulate/operation.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5256 2023-04-17 07:28:56.000000 isqopen-1.0.1/isq/simulate/simulator.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-20 09:17:47.595488 isqopen-1.0.1/isqopen.egg-info/
--rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)      760 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/SOURCES.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/dependency_links.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/not-zip-safe
--rw-r--r--   0 huazhelou   (501) staff       (20)       46 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/requires.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        4 2023-04-20 09:17:47.000000 isqopen-1.0.1/isqopen.egg-info/top_level.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-04-20 09:17:47.596386 isqopen-1.0.1/setup.cfg
--rw-r--r--   0 huazhelou   (501) staff       (20)      700 2023-04-20 09:10:33.000000 isqopen-1.0.1/setup.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.737680 isqopen-1.0.2/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1093 2022-09-07 10:16:53.000000 isqopen-1.0.2/LICENSE
+-rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-05-24 10:19:57.737844 isqopen-1.0.2/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)      734 2022-09-24 07:03:24.000000 isqopen-1.0.2/README.md
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.728250 isqopen-1.0.2/isq/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      247 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/__init__.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.731938 isqopen-1.0.2/isq/compile/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5836 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/QSyn.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    11380 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/Simplify.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5152 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/matlab_gsvd.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    14686 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/parser.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    22701 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/parsetab.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    27584 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/passes.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5050 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/qtypes.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2183 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/tokrules.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2539 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/compile/tools.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)       18 2023-05-24 10:17:35.000000 isqopen-1.0.2/isq/config.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.733715 isqopen-1.0.2/isq/device/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      142 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     6547 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/device.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1882 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/grad.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     3166 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/task.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     4293 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/device/translate.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.734467 isqopen-1.0.2/isq/draw/
+-rw-r--r--   0 huazhelou   (501) staff       (20)       26 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/draw/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     7986 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/draw/drawer.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2652 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/errors.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1221 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/globalVar.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    10006 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/mapping.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)      250 2023-05-24 10:17:35.000000 isqopen-1.0.2/isq/qpu.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     6707 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/quantum.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.735461 isqopen-1.0.2/isq/simulate/
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:17:35.000000 isqopen-1.0.2/isq/simulate/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    12918 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/simulate/operation.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5256 2023-05-24 10:17:36.000000 isqopen-1.0.2/isq/simulate/simulator.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-05-24 10:19:57.737412 isqopen-1.0.2/isqopen.egg-info/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      957 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)      775 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/SOURCES.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/dependency_links.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/not-zip-safe
+-rw-r--r--   0 huazhelou   (501) staff       (20)       57 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/requires.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        4 2023-05-24 10:19:57.000000 isqopen-1.0.2/isqopen.egg-info/top_level.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-05-24 10:19:57.738368 isqopen-1.0.2/setup.cfg
+-rw-r--r--   0 huazhelou   (501) staff       (20)      738 2023-05-24 10:19:36.000000 isqopen-1.0.2/setup.py
```

### Comparing `isqopen-1.0.1/LICENSE` & `isqopen-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/PKG-INFO` & `isqopen-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isqopen
-Version: 1.0.1
+Version: 1.0.2
 Summary: isq quantum kernel
 Author: Lou Huazhe
 Author-email: louhz@arclightquantum.com
 Platform: python 3.8+
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `isqopen-1.0.1/README.md` & `isqopen-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/compile/QSyn.py` & `isqopen-1.0.2/isq/compile/QSyn.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/compile/Simplify.py` & `isqopen-1.0.2/isq/compile/Simplify.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/compile/matlab_gsvd.py` & `isqopen-1.0.2/isq/compile/matlab_gsvd.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/compile/parser.py` & `isqopen-1.0.2/isq/compile/parser.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/compile/parsetab.py` & `isqopen-1.0.2/isq/compile/parsetab.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/compile/passes.py` & `isqopen-1.0.2/isq/compile/passes.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,15 +695,16 @@
                     if t not in self.lamb:
                         self.lamb[t] = eval("lambda {}:{}".format("args", t), self.param)
                         #self.lamb[val[0][1]] = eval("f'"+val[0][1]+"'", {'args': self.for_val})
                     theta = self.lamb[t](self.for_val)
                     #theta = eval(self.lamb[val[0][1]], self.param)
                     theta %= 4*np.pi
                     if theta > 2*np.pi: theta -= 4*np.pi
-                    theta= round(theta,4)
+                    # theta /= 2
+                    # theta= round(theta,4)
             except Exception as e:
                 ErrorThrow('in line {}, expression calc error: {}'.format(pos, str(e)))
 
         qlist = []
         try:
             for q in val[1]:
                 if q[1] == 0:
```

### Comparing `isqopen-1.0.1/isq/compile/qtypes.py` & `isqopen-1.0.2/isq/compile/qtypes.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/compile/tokrules.py` & `isqopen-1.0.2/isq/compile/tokrules.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/compile/tools.py` & `isqopen-1.0.2/isq/compile/tools.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/device/device.py` & `isqopen-1.0.2/isq/device/device.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from isq.errors import *
 from isq.compile.parser import IR, compile
 from isq.config import debug_mode
 from isq.simulate.simulator import simulate, getprobs
 import random
 from isq.quantum import quantumCor
-from .translate import translate_to_aws, translate_to_qcis
+from .translate import translate_to_aws, translate_to_qcis, split_rotation_gates
 from .task import *
 from .grad import optv
 from isq.draw.drawer import Drawer
 import logging
 from isq.globalVar import isq_env
 
 try:
@@ -71,14 +71,17 @@
                 isq_str = f.read()
         
         ir = IR()
         res = compile(ir, isq_str, target, quantumCor.getGate(), kw, args)
         if res == -1: raise CoreError(ir.error)
         self._ir = ir.out
         return args
+
+    def simulate(self, ir):
+        return dict(simulate(ir, self._shots))
     
     def getargs(self, kwargs):
         args = {}
         kw = {}
         for k,v in kwargs.items():
             if isinstance(v, optv):
                 args[k] = v._value
@@ -127,36 +130,49 @@
         return getprobs(self._ir, mod, **args)
 
         
 
 
 class QcisDevice(Device):
 
-    def __init__(self, user, passwd, shots = 1000, max_wait_time = 60, name = None, logger=logging.getLogger(__name__)):
+    def __init__(
+        self,
+        login_key = None,
+        machine_name = None,
+        shots = 1000,
+        max_wait_time = 60,
+        name = None,
+        logger=logging.getLogger(__name__),
+    ):
         if name == None: name = "qcis_device"
         
         if not isq_env.get_env('qcis'):
             raise Exception("ezQpy is not supported in this env, please install ezQpy first")
 
         super().__init__(name, shots, max_wait_time, logger)
 
-        username = user
-        password = passwd
-        
-        self._account = Account(username=username, password=password, full_expr_record=True)
+        self._account = Account(login_key=login_key, machine_name=machine_name)
         self._qid = 0
     
-    def run(self, isq_str = '', file = None, automap = False, init_map = None, **kwargs):
+    def run(
+        self,
+        isq_str = '',
+        file = None,
+        automap = False,
+        init_map = None,
+        **kwargs,
+    ):
 
         qcis = self.compile_to_ir(isq_str, file, "qcis", **kwargs)
         #circuit = quantumCor.getMapping(12, [[1, 2], [2, 3], [3, 4], [4, 5], [5, 6], [6, 7], [7, 8], [8, 9], [9, 10], [10, 11], [11, 12]], qcis)
         self._ir = qcis
 
+        qcis_split_rotation_gates = split_rotation_gates(qcis)
         exp_name = "{}_{}".format(self._name, getRandom())
-        query_id = self._account.submit_job(circuit=qcis, exp_name=exp_name, version="1.0", num_shots=self._shots)
+        query_id = self._account.submit_job(circuit=qcis_split_rotation_gates, exp_name=exp_name, version="1.0", num_shots=self._shots)
         if query_id:
             self.logger.info('qcis提交任务成功')
             return ISQTask(query_id, TaskType.QCSI, TaskState.WAIT, self)
         else:
             self.logger.error('qcis提交失败, 请确认硬件是否正常，或稍后再试')
             return ISQTask(0, TaskType.QCSI, TaskState.FAIL, self)
 
@@ -186,8 +202,8 @@
             #task = self._device.run(circuit, shots=self._shots)
             self.logger.info('aws提交任务成功')
             return ISQTask(task.id, TaskType.AWS, TaskState.WAIT, self, measure = q_measure, logger =self.logger)
             
         except Exception as e:
             self.logger.error(str(e))
             self.logger.error('aws提交失败, 请确认硬件是否正常，或稍后再试')
-            return ISQTask(0, TaskType.AWS, TaskState.FAIL, self)
+            return ISQTask(0, TaskType.AWS, TaskState.FAIL, self)
```

### Comparing `isqopen-1.0.1/isq/device/grad.py` & `isqopen-1.0.2/isq/device/grad.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/device/task.py` & `isqopen-1.0.2/isq/device/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,61 +2,73 @@
     from isq.globalVar import isq_env
     from braket.aws.aws_quantum_task import AwsQuantumTask
     isq_env.set_env('aws', True)
 except:
     pass
 from typing import Union
 from logging import getLogger
+from collections import defaultdict
 class TaskType:
     QCSI = "QCIS"
     AWS = "AWS"
 
 class TaskState:
     WAIT = "WAITING"
     COMPLETE = "COMPLETED"
     FAIL = "FAILED"
     CANCEL = "CANCELLED"
 
 class ISQTask:
 
     NO_RESULT_TERMINAL_STATES = {TaskState.FAIL, TaskState.CANCEL}
 
-    def __init__(self, task_id: Union[int, str], task_type, state, device, **kwargs) -> None:
+    def __init__(
+        self,
+        task_id: Union[int, str],
+        task_type,
+        state,
+        device,
+        **kwargs,
+    ) -> None:
         
         self._id = task_id
         self._type = task_type
         self._state = state
         self._res = {}
         self._device = device
         self.logger = getLogger(__name__)
         if 'logger' in kwargs:
             self.logger = kwargs['logger']
         if self._type == TaskType.AWS and self._state not in self.NO_RESULT_TERMINAL_STATES:
             if not isq_env.get_env('aws'):
                 raise "aws is not support in this env, please `pip install amazon-braket-sdk`"
-    
+
             self._task = AwsQuantumTask(self._id, poll_timeout_seconds = self._device._max_wait_time, logger=self.logger)
             self._measure = kwargs['measure']
 
     @property
     def state(self):
         return self._state
-    
+
     def result(self):
         if self._state in self.NO_RESULT_TERMINAL_STATES:
             return {}
 
         if self._state == TaskState.COMPLETE: return self._res
         
         if self._type == TaskType.QCSI:
             m_res = self._device._account.query_experiment(self._id, max_wait_time = self._device._max_wait_time)
             if m_res:
                 self.logger.info("任务执行成功")
                 self._state = TaskState.COMPLETE
-                self._res = m_res
+                ans = defaultdict(int)
+                for t in m_res['results'][1:]:
+                    x = ''.join([str(v) for v in t])
+                    ans[x] += 1
+                self._res = dict(ans)
             else:
                 self.logger.info("任务执行中，请等待")
         
         if self._type == TaskType.AWS:
             state = self._task.state()
             if state in self.NO_RESULT_TERMINAL_STATES:
                 self.logger.info("任务已失败或已取消")
@@ -81,8 +93,8 @@
         return self._res
 
     def cancel(self):
 
         if self._state == TaskState.WAIT:
             if self._type == TaskType.AWS:
                 self._task.cancel()
-                self._state = TaskState.CANCEL
+                self._state = TaskState.CANCEL
```

### Comparing `isqopen-1.0.1/isq/draw/drawer.py` & `isqopen-1.0.2/isq/draw/drawer.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/errors.py` & `isqopen-1.0.2/isq/errors.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/globalVar.py` & `isqopen-1.0.2/isq/globalVar.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/quantum.py` & `isqopen-1.0.2/isq/quantum.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/simulate/operation.py` & `isqopen-1.0.2/isq/simulate/operation.py`

 * *Files identical despite different names*

### Comparing `isqopen-1.0.1/isq/simulate/simulator.py` & `isqopen-1.0.2/isq/simulate/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
             if strArr[2] not in qdic:
                 qdic[strArr[2]] = qnum
                 qnum += 1
         if strArr[0] in ['RX', 'RY', 'RZ']:
             if len(strArr) != 3:
                 raise CoreError('simulate error: in line {}, qbit number error'.format(idx))
     
-    if qnum > 16:
-        raise CoreError('simulate error: qbit number out of 16, can not simulate')
+    if qnum > 22:
+        raise CoreError('simulate error: qbit number out of 22, can not simulate')
 
     return qnum, qdic
 
 def getstate(line_data, qnum, qdic, mod, **kwargs):
 
     state = anp.zeros(pow(2, qnum), dtype = complex)
     state[0] = 1
```

### Comparing `isqopen-1.0.1/isqopen.egg-info/PKG-INFO` & `isqopen-1.0.2/isqopen.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isqopen
-Version: 1.0.1
+Version: 1.0.2
 Summary: isq quantum kernel
 Author: Lou Huazhe
 Author-email: louhz@arclightquantum.com
 Platform: python 3.8+
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `isqopen-1.0.1/isqopen.egg-info/SOURCES.txt` & `isqopen-1.0.2/isqopen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 isq/__init__.py
 isq/config.py
 isq/errors.py
 isq/globalVar.py
+isq/mapping.py
 isq/qpu.py
 isq/quantum.py
 isq/compile/QSyn.py
 isq/compile/Simplify.py
 isq/compile/__init__.py
 isq/compile/matlab_gsvd.py
 isq/compile/parser.py
```

### Comparing `isqopen-1.0.1/setup.py` & `isqopen-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "isqopen",
-    version = "1.0.1",
+    version = "1.0.2",
     keyword = {"isq", "quantum", "cor"},
     description = "isq quantum kernel",
     platforms='python 3.8+',
     long_description=long_description,
 	long_description_content_type="text/markdown",
     author = "Lou Huazhe",
     author_email = "louhz@arclightquantum.com",
 
     package_data = {'':['*.txt']},
     install_requires = ['numpy>=1.21.3',
                         'ply>=3.11',
                         'scipy>=1.7.1',
-                        'autograd'],
+                        'autograd',
+                        'matplotlib'],
     packages = find_packages(),
     zip_safe=False
 )
```

