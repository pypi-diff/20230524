# Comparing `tmp/mielib-0.1.8.tar.gz` & `tmp/mielib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mielib-0.1.8.tar", max compression
+gzip compressed data, was "mielib-0.1.9.tar", max compression
```

## Comparing `mielib-0.1.8.tar` & `mielib-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      686 2023-01-16 23:28:04.867660 mielib-0.1.8/README.md
--rw-r--r--   0        0        0      130 2022-11-21 00:00:43.979943 mielib-0.1.8/mielib/__init__.py
--rw-r--r--   0        0        0      709 2022-11-21 01:02:48.058607 mielib-0.1.8/mielib/extraspecial.py
--rw-r--r--   0        0        0    14835 2022-11-21 22:22:13.300431 mielib-0.1.8/mielib/harmonics.py
--rw-r--r--   0        0        0     2472 2022-11-21 04:04:09.683768 mielib-0.1.8/mielib/mieacoustics.py
--rw-r--r--   0        0        0     5165 2022-11-21 23:32:23.127643 mielib-0.1.8/mielib/mieoptics.py
--rw-r--r--   0        0        0     1788 2023-01-16 23:29:03.024034 mielib-0.1.8/mielib/rotations.py
--rw-r--r--   0        0        0      284 2023-01-16 23:52:35.284906 mielib-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1296 2023-01-16 23:57:11.158285 mielib-0.1.8/setup.py
--rw-r--r--   0        0        0     1010 2023-01-16 23:57:11.158441 mielib-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      686 2023-03-01 03:20:48.118558 mielib-0.1.9/README.md
+-rw-r--r--   0        0        0      130 2023-03-01 03:20:48.120558 mielib-0.1.9/mielib/__init__.py
+-rw-r--r--   0        0        0      709 2023-03-01 03:20:48.120558 mielib-0.1.9/mielib/extraspecial.py
+-rw-r--r--   0        0        0    14835 2023-03-01 03:20:48.120558 mielib-0.1.9/mielib/harmonics.py
+-rw-r--r--   0        0        0     3127 2023-03-01 03:25:31.332046 mielib-0.1.9/mielib/mieacoustics.py
+-rw-r--r--   0        0        0     5165 2023-03-01 03:20:48.120558 mielib-0.1.9/mielib/mieoptics.py
+-rw-r--r--   0        0        0     1788 2023-03-01 03:20:48.120558 mielib-0.1.9/mielib/rotations.py
+-rw-r--r--   0        0        0      284 2023-03-01 03:26:05.563105 mielib-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1296 2023-03-01 03:30:33.832523 mielib-0.1.9/setup.py
+-rw-r--r--   0        0        0     1010 2023-03-01 03:30:33.832748 mielib-0.1.9/PKG-INFO
```

### Comparing `mielib-0.1.8/README.md` & `mielib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mielib-0.1.8/mielib/extraspecial.py` & `mielib-0.1.9/mielib/extraspecial.py`

 * *Files identical despite different names*

### Comparing `mielib-0.1.8/mielib/harmonics.py` & `mielib-0.1.9/mielib/harmonics.py`

 * *Files identical despite different names*

### Comparing `mielib-0.1.8/mielib/mieacoustics.py` & `mielib-0.1.9/mielib/mieacoustics.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,39 @@
     
     ans = np.where(
         down == 0,
         0,
         up/down
     )
     return ans
+
+def acoustics_mie_c(n, ka, rho1, beta1):
+    """
+        n - multipole order
+        ka - size parameter in host media
+        rho1 - relative density
+        beta1 - relative compressibility
+    """
+    gamma = np.sqrt(beta1/rho1)
+    k1a = ka * np.sqrt(beta1*rho1)
+    jn1 = sp.spherical_jn(n, k1a)
+    jn = sp.spherical_jn(n, ka)
+    jn1p = sp.spherical_jn(n, k1a, 1)
+    jnp = sp.spherical_jn(n, ka, 1)
+    hn = extraspecial.spherical_h1(n, ka)
+    hnp = extraspecial.spherical_h1(n, ka, p=1)
+    up = 1j / (ka**2)
+    down = (jn1 * hnp - gamma * jn1p * hn)
+    
+    ans = np.where(
+        down == 0,
+        0,
+        up/down
+    )
+    return ans
     
     
 def acoustics_scattering_cross_section(k, a, rho_rel, beta_rel, nmin=0, nmax=50, norm='none'):
     ka = a * k
     
     sigma_norm = 1.0
     if norm == 'geom':
```

### Comparing `mielib-0.1.8/mielib/mieoptics.py` & `mielib-0.1.9/mielib/mieoptics.py`

 * *Files identical despite different names*

### Comparing `mielib-0.1.8/mielib/rotations.py` & `mielib-0.1.9/mielib/rotations.py`

 * *Files identical despite different names*

### Comparing `mielib-0.1.8/setup.py` & `mielib-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['scipy>=1.9.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'mielib',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '# MieLib\n\nPython library with many Mie-related functions for optics and acoustics. In particular:\n- Scattering Mie coefficients for isotropic spheres:\n    -  Acoustic Mie coefficients based on Phys. Rev. Lett. 123, 183901 (2019) (see SM)\n    - Optics Mie coefficients based on Bohren Huffmann book.\n- Scalar spherical harmonics\n- Vector spherical harmonics (complex and real)\n\n## Instalation\n\nFrom [PYPI/mielib](https://pypi.org/project/mielib/):\n```\npip install mielib\n```\n\n## Examples\n\nSee examples folder with Jupyter Notebooks.\n\n## ToDo\n\n* Make tests\n* Setup github actions\n* Search for complex poles of Mie scattering coefficients\n\n## Credits\nIvan Toftul \n\n`toftul.ivan@gmail.com`\n',
     'author': 'Ivan Toftul',
     'author_email': 'toftul.ivan@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `mielib-0.1.8/PKG-INFO` & `mielib-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mielib
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Ivan Toftul
 Author-email: toftul.ivan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
```

