# Comparing `tmp/vasp_suite-1.1.1.tar.gz` & `tmp/vasp_suite-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.1.1.tar", last modified: Wed May 24 09:58:58 2023, max compression
+gzip compressed data, was "vasp_suite-1.1.2.tar", last modified: Wed May 24 10:18:38 2023, max compression
```

## Comparing `vasp_suite-1.1.1.tar` & `vasp_suite-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:58:58.775412 vasp_suite-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 09:58:58.775412 vasp_suite-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 09:58:58.775412 vasp_suite-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-24 09:58:56.000000 vasp_suite-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:58:58.773412 vasp_suite-1.1.1/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-24 09:58:56.000000 vasp_suite-1.1.1/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    10765 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3461 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/vasp_suite/core.py
--rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)    16913 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-05-24 09:58:45.000000 vasp_suite-1.1.1/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:58:58.775412 vasp_suite-1.1.1/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 09:58:58.000000 vasp_suite-1.1.1/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-24 09:58:58.000000 vasp_suite-1.1.1/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:58:58.000000 vasp_suite-1.1.1/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-24 09:58:58.000000 vasp_suite-1.1.1/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 09:58:58.000000 vasp_suite-1.1.1/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-24 09:58:58.000000 vasp_suite-1.1.1/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:18:38.450837 vasp_suite-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 10:18:38.449838 vasp_suite-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 10:18:38.450837 vasp_suite-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-24 10:18:36.000000 vasp_suite-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:18:38.448837 vasp_suite-1.1.2/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-24 10:18:36.000000 vasp_suite-1.1.2/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10765 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3461 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/vasp_suite/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)    16913 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-05-24 10:18:25.000000 vasp_suite-1.1.2/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:18:38.449838 vasp_suite-1.1.2/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 10:18:38.000000 vasp_suite-1.1.2/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-24 10:18:38.000000 vasp_suite-1.1.2/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 10:18:38.000000 vasp_suite-1.1.2/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-24 10:18:38.000000 vasp_suite-1.1.2/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 10:18:38.000000 vasp_suite-1.1.2/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-24 10:18:38.000000 vasp_suite-1.1.2/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.1.1/LICENSE` & `vasp_suite-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.1/PKG-INFO` & `vasp_suite-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.1.1/README.md` & `vasp_suite-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.1/setup.py` & `vasp_suite-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.1.1/vasp_suite/cli.py` & `vasp_suite-1.1.2/vasp_suite/cli.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.1/vasp_suite/core.py` & `vasp_suite-1.1.2/vasp_suite/core.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.1/vasp_suite/ewald.py` & `vasp_suite-1.1.2/vasp_suite/ewald.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.1/vasp_suite/input.py` & `vasp_suite-1.1.2/vasp_suite/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,39 +22,43 @@
         hostname = socket.gethostname()
         if 'csf3' in hostname: 
             self.pseudopotentials = '/opt/apps/apps/intel-19.1/vasp/5.4.4/pseudopotentials/potpaw_PBE.54'
             self.module = 'apps/intel-19.1/vasp/5.4.4'
         elif 'csf4' in hostname: 
             self.pseudopotentials = '/opt/software/RI/apps/VASP/5.4.4-iomkl-2020.02/pseudopotentials/potpaw_PBE.54'
             self.module = 'VASP/5.4.4-iomkl-2020.02'
-        else:
-            raise Warning('Unknown hostname. Generation of POTCAR file not possible.')
+        #else:
+        #    raise Warning('Unknown hostname. Generation of POTCAR file not possible.')
 
 
     def _INCAR(self):
         config = cp.ConfigParser()
         input_file = os.path.join(os.path.expanduser('~'), '.vasp_suite_configs', f'''{self.configuration}.ini''')
+        print(os.path.join(os.path.expanduser('~'), '.vasp_suite_configs', f'''{self.configuration}.ini'''))
         config.read(input_file)
+        print(config.sections())
         with open('INCAR', 'w') as f:
             for section in config.sections():
                 for key in config[section]:
                     key = key.upper()
                     f.write(f'''{key} = {config[section][key]}\n''')
 
     def _POTCAR(self):
         pseudo = self.pseudopotentials 
-        module = self.module 
         potpaw = ['H', 'He', 'Li_sv', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na_pv', 'Mg', 'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K_sv', 'Ca_sv', 'Sc_sv', 'Ti_sv', 'V_sv', 'Cr_pv', 'Mn_pv', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga_d', 'Ge_d', 'As', 'Se', 'Br', 'Kr', 'Rb_sv', 'Sr_sv', 'Y_sv', 'Zr_sv', 'Nb_sv', 'Mo_sv', 'Tc_pv', 'Ru_pv', 'Rh_pv', 'Pd', 'Ag', 'Cd', 'In_d', 'Sn_d', 'Sb', 'Te', 'I', 'Xe', 'Cs_sv', 'Ba_sv', 'La', 'Ce_3', 'Nd_3', 'Pm_3', 'Sm_3', 'Eu_2', 'Gd_3', 'Tb_3', 'Dy_3', 'Ho_3', 'Er_3', 'Tm_3', 'Yb_2', 'Lu_3', 'Hf_pv', 'Ta_pv', 'W_sv', 'Re', 'Os', 'Ir', 'Pt', 'Au', 'Hg', 'Tl_d', 'Pb_d', 'Bi_d', 'Po_d', 'At', 'Rn', 'Fr_sv', 'Ra_sv', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm']
         atoms = self._s.atoms 
 
         files = [x for x in potpaw if x.split('_')[0] in atoms]
         cwd = os.getcwd() 
 
         with open('POTCAR', 'w') as f:
-            os.system(f'''module load {module}''')
+            os.system(f'''module load vasp''')
             os.chdir(pseudo)
             for file in files:
-                os.system(f'''cat {file} >> {cwd}/POTCAR''')
+                os.chdir(str(file))
+                with open('POTCAR', 'r') as g:
+                    f.write(g.read()) 
+                os.chdir(pseudo)
             os.chdir(cwd)
```

### Comparing `vasp_suite-1.1.1/vasp_suite/structure.py` & `vasp_suite-1.1.2/vasp_suite/structure.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.1/vasp_suite/submission.py` & `vasp_suite-1.1.2/vasp_suite/submission.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.1/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.1.2/vasp_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

