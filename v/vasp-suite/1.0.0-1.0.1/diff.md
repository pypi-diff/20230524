# Comparing `tmp/vasp_suite-1.0.0.tar.gz` & `tmp/vasp_suite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.0.0.tar", last modified: Tue May 23 15:01:05 2023, max compression
+gzip compressed data, was "vasp_suite-1.0.1.tar", last modified: Wed May 24 09:19:06 2023, max compression
```

## Comparing `vasp_suite-1.0.0.tar` & `vasp_suite-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:01:05.949262 vasp_suite-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-23 15:01:05.949262 vasp_suite-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 15:01:05.949262 vasp_suite-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-23 15:01:02.000000 vasp_suite-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:01:05.947262 vasp_suite-1.0.0/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-23 15:01:02.000000 vasp_suite-1.0.0/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    10476 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3362 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/core.py
--rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)    16803 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-05-23 15:00:48.000000 vasp_suite-1.0.0/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:01:05.949262 vasp_suite-1.0.0/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-23 15:01:05.000000 vasp_suite-1.0.0/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:19:06.188717 vasp_suite-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 09:19:06.188717 vasp_suite-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 09:19:06.189717 vasp_suite-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-24 09:19:03.000000 vasp_suite-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:19:06.187717 vasp_suite-1.0.1/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-24 09:19:03.000000 vasp_suite-1.0.1/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10765 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3461 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/vasp_suite/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)    16913 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-05-24 09:18:52.000000 vasp_suite-1.0.1/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:19:06.188717 vasp_suite-1.0.1/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 09:19:06.000000 vasp_suite-1.0.1/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-24 09:19:06.000000 vasp_suite-1.0.1/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:19:06.000000 vasp_suite-1.0.1/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-24 09:19:06.000000 vasp_suite-1.0.1/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 09:19:06.000000 vasp_suite-1.0.1/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-24 09:19:06.000000 vasp_suite-1.0.1/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.0.0/LICENSE` & `vasp_suite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.0/PKG-INFO` & `vasp_suite-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.0.0/README.md` & `vasp_suite-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.0/setup.py` & `vasp_suite-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.0.0/vasp_suite/cli.py` & `vasp_suite-1.0.1/vasp_suite/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,27 +91,27 @@
     '''
     core.generate_job(
             title=args.title,
             cores=args.cores,
             vasp_type=args.vasp_type,
             )
 
-def start_up_func():
+def start_up_func(args):
     '''
     Wrapper function for the start_up function
 
     parameters
     ----------
     None
 
     Returns
     -------
     configuration files : file
     '''
-    core.start_up()
+    core.create_input_configurations()
 
 def dope_structure_func(args):
     '''
     Wrapper function for the dope_structure function
 
     parameters
     ----------
@@ -233,15 +233,15 @@
 
                 vasp_suite generate_input relaxation
                 '''
                 )
             )
 
     gen_inp.add_argument(
-            '--filename, -f',
+            '--filename', '-f',
             help=dedent(
                 '''
                 The name of the structure file, default is POSCAR
                 '''
                 ),
             default='POSCAR'
             )
@@ -281,14 +281,24 @@
         'calculate_kpoints',
         help='Calculate the possible kpoint meshes for a given structure',
         formatter_class=argparse.RawDescriptionHelpFormatter
         )
 
     calc_kpoints.set_defaults(func=calculate_kpoints_func)
 
+    calc_kpoints.add_argument(
+            '--filename', '-f',
+            help=dedent(
+                '''
+                The name of the structure file, default is POSCAR
+                '''
+                ),
+            default='POSCAR'
+            )
+
     gen_kpoints = subparsers.add_parser(
         'generate_kpoints',
         help='Generate the kpoints file for a given structure',
         formatter_class=argparse.RawDescriptionHelpFormatter
         )
 
     gen_kpoints.set_defaults(func=generate_kpoints_func)
@@ -310,19 +320,19 @@
         help='Generate a supercell from a given structure',
         formatter_class=argparse.RawDescriptionHelpFormatter
         )
 
     gen_supercell.set_defaults(func=generate_supercell_func)
 
     gen_supercell.add_argument(
-        'Expansion',
+        'expansion',
         nargs=3,
         help=dedent(
             '''
-            The expansion factor for the a lattice vector.
+            The expansion vector for the supercell, a b c
             '''
             ),
         )
 
     start_up = subparsers.add_parser(
         'start_up',
         help='Generate the configuration files for the suite',
@@ -336,15 +346,15 @@
         help='Dope a structure with a given element',
         formatter_class=argparse.RawDescriptionHelpFormatter
         )
 
     dope_struct.set_defaults(func=dope_structure_func)
 
     dope_struct.add_argument(
-        '--filename, -f',
+        '--filename', '-f',
         help='The name of the structure file',
         default='POSCAR',
         )
 
     dope_struct.add_argument(
             'dopant',
             help='The element to dope the structure with',
@@ -367,15 +377,15 @@
         help='Generate a defect structure',
         formatter_class=argparse.RawDescriptionHelpFormatter
         )
 
     gen_defect.set_defaults(func=generate_defect_func)
 
     gen_defect.add_argument(
-            '--filename, -f',
+            '--filename', '-f',
             help='The name of the structure file',
             default='POSCAR',
             )
 
     gen_defect.add_argument(
             'site',
             help='The name of the atom to remove',
@@ -393,26 +403,26 @@
         help='Generate the asymmetric unit of a structure',
         formatter_class=argparse.RawDescriptionHelpFormatter
         )
 
     asym.set_defaults(func=asymmetric_unit_func)
 
     asym.add_argument(
-            '--filename, -f',
+            '--filename', '-f',
             help='The name of the structure file',
             default='POSCAR',
             )
 
     asym.add_argument(
             'atom',
             help='The name of the spin centre in the molecular crystal',
             )
 
     asym.add_argument(
-            '--bond_max, -b',
+            '--bond_max', '-b',
             help='The maximum bond length/ Å',
             type=float,
             default=2.6,
             )
 
 
     # Parse the ArgumentParser
```

### Comparing `vasp_suite-1.0.0/vasp_suite/core.py` & `vasp_suite-1.0.1/vasp_suite/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 def generate_supercell(expansion: np.ndarray) -> None: 
     '''
     Generates a supercell from a given expansion matrix.
     '''
     _s = structure.Structure('POSCAR')
     _s.Vasp_reader()
-    _s.supercell(expansion)
+    _s.Supercell(expansion)
     _s.write_poscar()
     return None
 
 def dope_structure(filename: str, dopant: str, replace: str, instances: int) -> None:
     '''
     Dopes a structure with a given dopant and generates all possible structures.
     '''
@@ -54,15 +54,15 @@
 def generate_defect(filename: str, site: str, instances: int) -> None:
     '''
     Generates a defect structure from a given structure.
     '''
     _d = structure.DOPE(filename, 'D', site, instances)
     _d.Generate_structure()
     _d.Create_defect()
-    _d.write_poscar()
+    _d.write_poscars()
     return None
 
 def asymmetric_unit(filename: str, atom: str, bond_max: float) -> None:
     '''
     Generates the asymmetric unit of a structure.
     '''
     _a = structure.Asymmetric_unit(filename, atom, bond_max)
@@ -87,17 +87,19 @@
         f.write('mesh{0} mesh{1} mesh{2}\n')
         f.write('0 0 0')
 
 def create_input_configurations() -> None:
     '''
     Creates input configurations for VASP calculations.
     '''
-    if not os.path.exits(os.path.expanduser('~/.vasp_suite_configs')):
+    if not os.path.exists(os.path.expanduser('~/.vasp_suite_configs')):
         os.mkdir(os.path.expanduser('~/.vasp_suite_configs'))
 
+    cwd = os.getcwd()
+    os.chdir(os.path.expanduser('~/.vasp_suite_configs'))
     with open('relaxation.ini', 'w') as f:
         f.write('''[Relaxation]
 prec = ACCURATE
 lreal = .FALSE.
 lasph = .TRUE.
 ismear = 0
 sigma = 0.1
@@ -133,8 +135,8 @@
 potim = 0.5
 lwave = .FALSE.
 lcharg = .FALSE.
 lorbit = 11
 gga = PE
 ivdw = 11
 ''')
-
+    os.chdir(cwd)
```

### Comparing `vasp_suite-1.0.0/vasp_suite/ewald.py` & `vasp_suite-1.0.1/vasp_suite/ewald.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.0/vasp_suite/input.py` & `vasp_suite-1.0.1/vasp_suite/input.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.0/vasp_suite/structure.py` & `vasp_suite-1.0.1/vasp_suite/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         '''
         coords = self.coords
         n1, n2, n3 = n 
         supercell = np.array([[x[0]+a, x[1]+b, x[2]+c] for x in coords for a in range(n1) for b in range(n2) for c in range(n3)]) 
         supercell /= n
         self.av = self.av * n
         self.coords = supercell 
-        atom_list = self._s._atom_list
+        atom_list = self._atom_list
         atom_list = np.array([(f'{x} ' * 8).split() for x in atom_list])
         atom_list = atom_list.flatten().reshape(-1,1)
         self._atom_list = atom_list
         self.natoms = [x*n1*n2*n3 for x in self.natoms]
 
     def Const_shift(self, vector: np.ndarray) -> np.ndarray:
         '''
@@ -281,20 +281,22 @@
         self._structures = structures
         print(f'Number of structures found = {len(structures)}')
 
     def Create_defect(self):
         '''
         Creates defects in the stucture
         '''
+        structures = []
         for structure in self._structures:
-            for i in range(len(structure)):
+            for i in range(len(structure)-1):
                 if structure[i][0] == self.dopant:
-                    del structure[i]
-                else:
-                    continue
+                    structure = np.delete(structure, i, axis=0)
+                    structures.append(structure)
+                    
+        self._structures = np.array(structures)
 
     def write_poscars(self) -> None:
         '''
         Writes the doped structures to POSCAR files.
         '''
         name: str = self._s.name 
         scale: int  = self._s.scale 
@@ -421,14 +423,18 @@
 
     def _locate_atom(self) -> None: 
         '''
         Locates the atom in the structure
         '''
         atom = re.split(r'(\d+)', self.atom)
         symbol, index = atom[0], int(atom[1])
+
+        if symbol not in self._s.atoms:
+            raise ValueError(f'Atom {symbol} not found in the structure.') 
+
         coords = self._s.coords 
         atoms = self._s.atoms 
         natoms = self._s.natoms 
 
         # find the atom in the structure 
         for ind, sym in enumerate(atoms):
             if sym == symbol:
@@ -477,15 +483,15 @@
     def find_unit(self) -> None:
         '''
         Finds the asymmetric unit.
         '''
         self._locate_atom()
         self._translate()
         origin = self._origin_index()
-        coords = np.hstack((self._atom_list, np.array(self._s.cart_coords, dtype=float)))
+        coords = np.hstack((self._s._atom_list, np.array(self._s.cart_coords, dtype=float)))
 
         asymm_unit = np.array([coords[origin]])
         searching = True 
         while searching:
             total_coords = []
             for i in asymm_unit:
                 if not i[0] == 'H':
@@ -497,14 +503,7 @@
             if len(total_coords) == len(asymm_unit):
                 searching = False
             else: 
                 asymm_unit = total_coords
         self.asymm_unit = asymm_unit
         self._write_xyz()
 
-
-if __name__ == '__main__': 
-    dope = DOPE('POSCAR', 'Gd', 'Ca', 2) 
-    dope.Generate_structure()
-    dope.write_poscars()
-
-
```

### Comparing `vasp_suite-1.0.0/vasp_suite/submission.py` & `vasp_suite-1.0.1/vasp_suite/submission.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.0.0/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.0.1/vasp_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

