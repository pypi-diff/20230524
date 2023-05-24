# Comparing `tmp/isotopylog-0.0.6.tar.gz` & `tmp/isotopylog-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isotopylog-0.0.6.tar", last modified: Fri Jul 16 14:11:04 2021, max compression
+gzip compressed data, was "isotopylog-0.0.7.tar", last modified: Wed Aug 25 09:46:22 2021, max compression
```

## Comparing `isotopylog-0.0.6.tar` & `isotopylog-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-07-16 14:11:04.044409 isotopylog-0.0.6/
--rw-r--r--   0 jhemingway (2020370277) 1294540650       82 2021-07-14 14:46:09.000000 isotopylog-0.0.6/MANIFEST.in
--rw-r--r--   0 jhemingway (2020370277) 1294540650     8205 2021-07-16 14:11:04.044263 isotopylog-0.0.6/PKG-INFO
--rw-r--r--   0 jhemingway (2020370277) 1294540650     6257 2021-07-14 15:39:36.000000 isotopylog-0.0.6/README.rst
-drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-07-16 14:11:04.040660 isotopylog-0.0.6/docs/
--rw-r--r--   0 jhemingway (2020370277) 1294540650     1690 2021-07-14 14:46:09.000000 isotopylog-0.0.6/docs/examples.rst
--rw-r--r--   0 jhemingway (2020370277) 1294540650     6077 2021-07-16 13:36:28.000000 isotopylog-0.0.6/docs/index.rst
--rw-r--r--   0 jhemingway (2020370277) 1294540650     2286 2021-07-16 13:35:56.000000 isotopylog-0.0.6/docs/package_reference.rst
--rw-r--r--   0 jhemingway (2020370277) 1294540650    12812 2021-07-16 13:45:58.000000 isotopylog-0.0.6/docs/quick_guide.rst
-drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-07-16 14:11:04.043223 isotopylog-0.0.6/isotopylog/
--rw-r--r--   0 jhemingway (2020370277) 1294540650     1189 2021-07-15 13:16:36.000000 isotopylog-0.0.6/isotopylog/__init__.py
--rw-r--r--   0 jhemingway (2020370277) 1294540650    38168 2021-07-16 13:42:41.000000 isotopylog-0.0.6/isotopylog/calc_funcs.py
--rw-r--r--   0 jhemingway (2020370277) 1294540650    14029 2021-07-16 13:02:26.000000 isotopylog-0.0.6/isotopylog/core_functions.py
--rw-r--r--   0 jhemingway (2020370277) 1294540650     6063 2021-07-16 12:32:51.000000 isotopylog-0.0.6/isotopylog/dictionaries.py
-drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-07-16 14:11:04.043960 isotopylog-0.0.6/isotopylog/lit_values/
--rw-r--r--   0 jhemingway (2020370277) 1294540650     4004 2021-07-16 12:10:46.000000 isotopylog-0.0.6/isotopylog/lit_values/lit_values.csv
--rw-r--r--   0 jhemingway (2020370277) 1294540650    45211 2021-07-16 13:43:10.000000 isotopylog-0.0.6/isotopylog/ratedata.py
--rw-r--r--   0 jhemingway (2020370277) 1294540650    32862 2021-07-16 13:51:28.000000 isotopylog-0.0.6/isotopylog/ratedata_helper.py
--rw-r--r--   0 jhemingway (2020370277) 1294540650    37232 2021-07-16 12:53:57.000000 isotopylog-0.0.6/isotopylog/timedata.py
--rw-r--r--   0 jhemingway (2020370277) 1294540650    13402 2021-07-16 13:44:39.000000 isotopylog-0.0.6/isotopylog/timedata_helper.py
-drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-07-16 14:11:04.043858 isotopylog-0.0.6/isotopylog.egg-info/
--rw-r--r--   0 jhemingway (2020370277) 1294540650     8205 2021-07-16 14:11:03.000000 isotopylog-0.0.6/isotopylog.egg-info/PKG-INFO
--rw-r--r--   0 jhemingway (2020370277) 1294540650      528 2021-07-16 14:11:03.000000 isotopylog-0.0.6/isotopylog.egg-info/SOURCES.txt
--rw-r--r--   0 jhemingway (2020370277) 1294540650        1 2021-07-16 14:11:03.000000 isotopylog-0.0.6/isotopylog.egg-info/dependency_links.txt
--rw-r--r--   0 jhemingway (2020370277) 1294540650       30 2021-07-16 14:11:03.000000 isotopylog-0.0.6/isotopylog.egg-info/requires.txt
--rw-r--r--   0 jhemingway (2020370277) 1294540650       11 2021-07-16 14:11:03.000000 isotopylog-0.0.6/isotopylog.egg-info/top_level.txt
--rw-r--r--   0 jhemingway (2020370277) 1294540650       38 2021-07-16 14:11:04.044448 isotopylog-0.0.6/setup.cfg
--rw-r--r--   0 jhemingway (2020370277) 1294540650     1146 2021-07-14 15:32:40.000000 isotopylog-0.0.6/setup.py
+drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-08-25 09:46:22.663670 isotopylog-0.0.7/
+-rw-r--r--   0 jhemingway (2020370277) 1294540650       82 2021-07-14 14:46:09.000000 isotopylog-0.0.7/MANIFEST.in
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     8204 2021-08-25 09:46:22.663481 isotopylog-0.0.7/PKG-INFO
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     6259 2021-08-25 09:27:32.000000 isotopylog-0.0.7/README.rst
+drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-08-25 09:46:22.659657 isotopylog-0.0.7/docs/
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     1690 2021-07-14 14:46:09.000000 isotopylog-0.0.7/docs/examples.rst
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     6073 2021-08-25 09:30:05.000000 isotopylog-0.0.7/docs/index.rst
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     2286 2021-07-16 13:35:56.000000 isotopylog-0.0.7/docs/package_reference.rst
+-rw-r--r--   0 jhemingway (2020370277) 1294540650    12812 2021-07-16 13:45:58.000000 isotopylog-0.0.7/docs/quick_guide.rst
+drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-08-25 09:46:22.662434 isotopylog-0.0.7/isotopylog/
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     1191 2021-08-25 09:31:13.000000 isotopylog-0.0.7/isotopylog/__init__.py
+-rw-r--r--   0 jhemingway (2020370277) 1294540650    39430 2021-08-25 09:32:36.000000 isotopylog-0.0.7/isotopylog/calc_funcs.py
+-rw-r--r--   0 jhemingway (2020370277) 1294540650    14029 2021-08-09 13:13:54.000000 isotopylog-0.0.7/isotopylog/core_functions.py
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     6063 2021-08-10 10:29:22.000000 isotopylog-0.0.7/isotopylog/dictionaries.py
+drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-08-25 09:46:22.663189 isotopylog-0.0.7/isotopylog/lit_values/
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     4004 2021-07-16 12:10:46.000000 isotopylog-0.0.7/isotopylog/lit_values/lit_values.csv
+-rw-r--r--   0 jhemingway (2020370277) 1294540650    45211 2021-07-16 13:43:10.000000 isotopylog-0.0.7/isotopylog/ratedata.py
+-rw-r--r--   0 jhemingway (2020370277) 1294540650    32862 2021-07-16 13:51:28.000000 isotopylog-0.0.7/isotopylog/ratedata_helper.py
+-rw-r--r--   0 jhemingway (2020370277) 1294540650    37232 2021-07-16 12:53:57.000000 isotopylog-0.0.7/isotopylog/timedata.py
+-rw-r--r--   0 jhemingway (2020370277) 1294540650    13402 2021-07-16 13:44:39.000000 isotopylog-0.0.7/isotopylog/timedata_helper.py
+drwxr-xr-x   0 jhemingway (2020370277) 1294540650        0 2021-08-25 09:46:22.663096 isotopylog-0.0.7/isotopylog.egg-info/
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     8204 2021-08-25 09:46:22.000000 isotopylog-0.0.7/isotopylog.egg-info/PKG-INFO
+-rw-r--r--   0 jhemingway (2020370277) 1294540650      528 2021-08-25 09:46:22.000000 isotopylog-0.0.7/isotopylog.egg-info/SOURCES.txt
+-rw-r--r--   0 jhemingway (2020370277) 1294540650        1 2021-08-25 09:46:22.000000 isotopylog-0.0.7/isotopylog.egg-info/dependency_links.txt
+-rw-r--r--   0 jhemingway (2020370277) 1294540650       30 2021-08-25 09:46:22.000000 isotopylog-0.0.7/isotopylog.egg-info/requires.txt
+-rw-r--r--   0 jhemingway (2020370277) 1294540650       11 2021-08-25 09:46:22.000000 isotopylog-0.0.7/isotopylog.egg-info/top_level.txt
+-rw-r--r--   0 jhemingway (2020370277) 1294540650       38 2021-08-25 09:46:22.663703 isotopylog-0.0.7/setup.cfg
+-rw-r--r--   0 jhemingway (2020370277) 1294540650     1143 2021-08-25 09:26:42.000000 isotopylog-0.0.7/setup.py
```

### Comparing `isotopylog-0.0.6/PKG-INFO` & `isotopylog-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: isotopylog
-Version: 0.0.6
+Version: 0.0.7
 Summary: Clumped isotope kinetic analysis
 Home-page: https://github.com/FluvialSeds/isotopylog
 Author: Jordon D. Hemingway
-Author-email: jordon_hemingway@fas.harvard.edu
+Author-email: jordon.hemingway@erdw.ethz.ch
 License: GNU GPL Version 3
-Download-URL: https://github.com/FluvialSeds/isotopylog/tarball/0.0.6
+Download-URL: https://github.com/FluvialSeds/isotopylog/tarball/0.0.7
 Description: About isotopylog
         ================
         ``isotopylog`` is a Python package for analyzing "clumped" isotope kinetic data; it is particularly suited for assessing carbonate clumped isotope (i.e., ∆\ :sub:`47`\) bond reordering and closure temperatures, but will be expanded in the future to include clumped isotopes of other isotopologues (e.g., ∆\ :sub:`48`\) molecular species (e.g., sulfate). This package currently performs two basic functions: 
         
         (1) it fits ∆\ :sub:`47`\ reordering data from carbonate heating experiments (inverse model) and 
         (2) it predicts geologic ∆\ :sub:`47`\ evolution given any time/temperature sample history (forward model). 
         
@@ -20,18 +20,18 @@
         
         Package Information
         -------------------
         :Authors:
           Jordon D. Hemingway (jordon.hemingway@erdw.ethz.ch)
         
         :Version:
-          0.0.6
+          0.0.7
         
         :Release:
-          15 July 2021
+          25 August 2021
         
         :License:
           GNU GPL v3 (or greater)
         
         :url:
           http://github.com/FluvialSeds/isotopylog
           http://pypi.python.org/pypi/isotopylog
```

### Comparing `isotopylog-0.0.6/README.rst` & `isotopylog-0.0.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 Package Information
 -------------------
 :Authors:
   Jordon D. Hemingway (jordon.hemingway@erdw.ethz.ch)
 
 :Version:
-  0.0.6
+  0.0.7
 
 :Release:
-  15 July 2021
+  25 August 2021
 
 :License:
   GNU GPL v3 (or greater)
 
 :url:
   http://github.com/FluvialSeds/isotopylog
   http://pypi.python.org/pypi/isotopylog
```

### Comparing `isotopylog-0.0.6/docs/examples.rst` & `isotopylog-0.0.7/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/docs/index.rst` & `isotopylog-0.0.7/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
 This package allows users to quickly and easily assess whether their clumped isotope measurements reflect primary signatures, or if these values have been reset during diagenetic heating. Similarly, it also allows users to easily assess geologic cooling rates using the apparent "closure" or "blocking" temperatures recorded in carbonates that have been diagenetically heated.
 
 
 Package Information
 -------------------
 :Authors:
-  Jordon D. Hemingway (jordon_hemingway@fas.harvard.edu)
+  Jordon D. Hemingway (jordon.hemingway@erdw.ethz.ch)
 
 :Version:
-  0.0.6
+  0.0.7
 
 :Release:
-  15 July 2021
+  25 August 2021
 
 :License:
   GNU GPL v3 (or greater)
 
 :url:
   http://github.com/FluvialSeds/isotopylog
   http://pypi.python.org/pypi/isotopylog
@@ -37,15 +37,15 @@
 :doi:
   |doi|
 
 Bug Reports
 -----------
 This software is still in active deveopment. Please report any bugs directly to me at:
 
-	jordon_hemingway@fas.harvard.edu
+	jordon.hemingway@erdw.ethz.ch
 
 How to Cite
 -----------
 When analyzing data with ``isotopylog`` to be used in a peer-reviewed journal, please cite this package as:
 
 * J.D. Hemingway. *isotopylog*: open-source tools for clumped isotope kinetic data analysis, 2020-, http://pypi.python.org/pypi/isotopylog [online; accessed |date|]
```

### Comparing `isotopylog-0.0.6/docs/package_reference.rst` & `isotopylog-0.0.7/docs/package_reference.rst`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/docs/quick_guide.rst` & `isotopylog-0.0.7/docs/quick_guide.rst`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/isotopylog/__init__.py` & `isotopylog-0.0.7/isotopylog/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 	
 	https://github.com/FluvialSeds/isotopylog
 
 documentation can be found at:
 
 	http://isotopylog.readthedocs.io
 
-Version 0.0.6 is current as of 15 July 2021 and reflects the notation used
+Version 0.0.7 is current as of 25 August 2021 and reflects the notation used
 in Hemingway and Henkes (2021).
 '''
 
 from __future__ import(
 	division,
 	print_function,
 	)
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 __docformat__ = 'restructuredtext en'
 
 
 #import timedata classes
 from .timedata import(
 	HeatingExperiment,
```

### Comparing `isotopylog-0.0.6/isotopylog/calc_funcs.py` & `isotopylog-0.0.7/isotopylog/calc_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -840,50 +840,94 @@
 
 	References
 	----------
 
 	[1] Hemingway and Henkes (2021) *Earth Planet. Sci. Lett.*, **566**, 116962.
 	'''
 
+	#----------------------------------#
+	# NEW CODE USING UPDATED EQUATION! #
+	# JDH 25 August 2021               #
+	#----------------------------------#
+
 	#get constants
 	nt = len(t)
 	dt = np.gradient(t)
 	R = 8.314/1000 #in kJ/mol/K
 
-	#calculate overall k at each temperature point, termed kappa
-	#calculate nu_mu and nu_sig from Emu and Esig
-	nu_mu = lnkmuref + (Emu/R)*(1/Tref - 1/T)
-	nu_sig = lnksigref - (Esig/R)*(1/T)
-
-	#calculate pnu from nu_mu and nu_sig
-	# pnu is an [nt x nnu] matrix
-
-	#first, make nu array that spans from 5*sigma above max(nu_mu) to 5*sigma
-	# below min(nu_mu)
-	nu_min = np.floor(nu_mu.min() - 5*nu_sig.max())
-	nu_max = np.ceil(nu_mu.max() + 5*nu_sig.max())
-
-	nu = np.linspace(nu_min, nu_max, nnu)
-	dnu = nu[1] - nu[0]
-
-	#then, make into matrix
-	rhonu = _Gaussian(nu, nu_mu, nu_sig)
-
-	#make array of kappa = integral(rho_nu * e^(-k*dt))
-	b = np.exp(-np.outer(np.exp(nu), dt))
-	kappa = np.sum(rhonu * b * dnu, axis = 0)
-
-	#pre-allocate D array
-	D = np.zeros(nt)
-	D[0] = D0
+	#pre-allocate D matrix
+	Dmat = np.zeros([nnu,nt])
+	Dmat[:,0] = D0
+
+	#calculate E and p(E) arrays
+	#go from 5*Esig above Emu to 5*Esig below Emu
+	E_min = np.floor(Emu + 5*Esig)
+	E_max = np.ceil(Emu - 5*Esig)
+
+	#get E array
+	E = np.linspace(E_min, E_max, nnu)
+	dE = E[1] - E[0]
+
+	#get p(E) array
+	pE = _Gaussian(E, Emu, Esig)
+
+	#get nu matrix from T and E arrays
+	numat = lnkmuref + np.outer((E/R),(1/Tref - 1/T))
 
-	#loop through and solve for D at each time point
+	#calculate b, the exponential decay for each E value at each time step
+	b = np.exp(-np.exp(numat)*np.outer(np.ones(nnu),dt))
+
+	#loop through and solve for D(E,t)
 	for i in range(1,nt):
 
-		D[i] = (D[i-1] - Deq[i])*kappa[i] + Deq[i]
+	    Dmat[:,i] = (Dmat[:,i-1] - Deq[i])*b[:,i] + Deq[i]
+
+	#calcualte overall D value
+	D = np.sum(np.outer(pE,np.ones(nt))*Dmat*dE, axis = 0)
+
+	#-------------------------------------------------------------------------#
+	#OLD CODE: USED THE WRONG EQUATION FOR GEOLOGIC HISTORY RECONSTRUCTIONS!! #
+	#-------------------------------------------------------------------------#
+
+	# #get constants
+	# nt = len(t)
+	# dt = np.gradient(t)
+	# R = 8.314/1000 #in kJ/mol/K
+
+	# #calculate overall k at each temperature point, termed kappa
+	# #calculate nu_mu and nu_sig from Emu and Esig
+	# nu_mu = lnkmuref + (Emu/R)*(1/Tref - 1/T)
+	# nu_sig = lnksigref - (Esig/R)*(1/T)
+
+	# #calculate pnu from nu_mu and nu_sig
+	# # pnu is an [nt x nnu] matrix
+
+	# #first, make nu array that spans from 5*sigma above max(nu_mu) to 5*sigma
+	# # below min(nu_mu)
+	# nu_min = np.floor(nu_mu.min() - 5*nu_sig.max())
+	# nu_max = np.ceil(nu_mu.max() + 5*nu_sig.max())
+
+	# nu = np.linspace(nu_min, nu_max, nnu)
+	# dnu = nu[1] - nu[0]
+
+	# #then, make into matrix
+	# rhonu = _Gaussian(nu, nu_mu, nu_sig)
+
+	# #make array of kappa = integral(rho_nu * e^(-k*dt))
+	# b = np.exp(-np.outer(np.exp(nu), dt))
+	# kappa = np.sum(rhonu * b * dnu, axis = 0)
+
+	# #pre-allocate D array
+	# D = np.zeros(nt)
+	# D[0] = D0
+
+	# #loop through and solve for D at each time point
+	# for i in range(1,nt):
+
+	# 	D[i] = (D[i-1] - Deq[i])*kappa[i] + Deq[i]
 
 	return D
 
 #function for calcualting geologic history with PH12 model
 def _ghPH12(t, E, lnkref, D0, Deq, T, Tref):
 	'''
 	Calculates the D47 value for a given geologic t-T history using the PH12
```

### Comparing `isotopylog-0.0.6/isotopylog/core_functions.py` & `isotopylog-0.0.7/isotopylog/core_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
 			E2,
 			lnk2ref,
 			D0,
 			Deq,
 			T,
 			Tref)
 
-	#Hemingway and Henkes 2020 model
+	#Hemingway and Henkes 2021 model
 	elif ed.model == 'HH21':
 
 		#extract relevant parameters and uncertainty in the order:
 		# Emu, lnkmuref, Esig, lnksigref
 		p = ed.Eparams.T.flatten()
 		pcov = ed.Eparams_cov
```

### Comparing `isotopylog-0.0.6/isotopylog/dictionaries.py` & `isotopylog-0.0.7/isotopylog/dictionaries.py`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/isotopylog/lit_values/lit_values.csv` & `isotopylog-0.0.7/isotopylog/lit_values/lit_values.csv`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/isotopylog/ratedata.py` & `isotopylog-0.0.7/isotopylog/ratedata.py`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/isotopylog/ratedata_helper.py` & `isotopylog-0.0.7/isotopylog/ratedata_helper.py`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/isotopylog/timedata.py` & `isotopylog-0.0.7/isotopylog/timedata.py`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/isotopylog/timedata_helper.py` & `isotopylog-0.0.7/isotopylog/timedata_helper.py`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/isotopylog.egg-info/PKG-INFO` & `isotopylog-0.0.7/isotopylog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: isotopylog
-Version: 0.0.6
+Version: 0.0.7
 Summary: Clumped isotope kinetic analysis
 Home-page: https://github.com/FluvialSeds/isotopylog
 Author: Jordon D. Hemingway
-Author-email: jordon_hemingway@fas.harvard.edu
+Author-email: jordon.hemingway@erdw.ethz.ch
 License: GNU GPL Version 3
-Download-URL: https://github.com/FluvialSeds/isotopylog/tarball/0.0.6
+Download-URL: https://github.com/FluvialSeds/isotopylog/tarball/0.0.7
 Description: About isotopylog
         ================
         ``isotopylog`` is a Python package for analyzing "clumped" isotope kinetic data; it is particularly suited for assessing carbonate clumped isotope (i.e., ∆\ :sub:`47`\) bond reordering and closure temperatures, but will be expanded in the future to include clumped isotopes of other isotopologues (e.g., ∆\ :sub:`48`\) molecular species (e.g., sulfate). This package currently performs two basic functions: 
         
         (1) it fits ∆\ :sub:`47`\ reordering data from carbonate heating experiments (inverse model) and 
         (2) it predicts geologic ∆\ :sub:`47`\ evolution given any time/temperature sample history (forward model). 
         
@@ -20,18 +20,18 @@
         
         Package Information
         -------------------
         :Authors:
           Jordon D. Hemingway (jordon.hemingway@erdw.ethz.ch)
         
         :Version:
-          0.0.6
+          0.0.7
         
         :Release:
-          15 July 2021
+          25 August 2021
         
         :License:
           GNU GPL v3 (or greater)
         
         :url:
           http://github.com/FluvialSeds/isotopylog
           http://pypi.python.org/pypi/isotopylog
```

### Comparing `isotopylog-0.0.6/isotopylog.egg-info/SOURCES.txt` & `isotopylog-0.0.7/isotopylog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isotopylog-0.0.6/setup.py` & `isotopylog-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from setuptools import setup
 
 def readme():
 	with open('README.rst') as f:
 		return f.read()
 
 setup(name='isotopylog',
-	version='0.0.6',
+	version='0.0.7',
 	description='Clumped isotope kinetic analysis',
 	long_description=readme(),
 	classifiers=[
 		'Development Status :: 3 - Alpha',
 		'Intended Audience :: Science/Research',
 		'License :: Free for non-commercial use',
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 2',
 		'Programming Language :: Python :: 3.5',
 		'Programming Language :: Python :: 2.7',
 		'Topic :: Scientific/Engineering'
 	],
 	url='https://github.com/FluvialSeds/isotopylog',
-	download_url='https://github.com/FluvialSeds/isotopylog/tarball/0.0.6',
+	download_url='https://github.com/FluvialSeds/isotopylog/tarball/0.0.7',
 	keywords=[
 		'geochemistry',
 		'clumped isotopes',
 		'kinetics',
 		'inverse modeling',
 		'carbon cycle'
 	],
 	author='Jordon D. Hemingway',
-	author_email='jordon_hemingway@fas.harvard.edu',
+	author_email='jordon.hemingway@erdw.ethz.ch',
 	license='GNU GPL Version 3',
 	packages=['isotopylog'],
 	install_requires=[
 		'matplotlib',
 		'numpy',
 		'pandas',
 		'scipy'
```

