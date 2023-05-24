# Comparing `tmp/calfpy-1.17.0.tar.gz` & `tmp/calfpy-1.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfpy-1.17.0.tar", last modified: Mon Mar  7 18:04:24 2022, max compression
+gzip compressed data, was "calfpy-1.20.1.tar", last modified: Wed May 24 19:56:19 2023, max compression
```

## Comparing `calfpy-1.17.0.tar` & `calfpy-1.20.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-03-07 18:04:24.289144 calfpy-1.17.0/
--rw-rw-rw-   0        0        0    18429 2021-08-04 01:22:06.000000 calfpy-1.17.0/LICENSE.txt
--rw-rw-rw-   0        0        0    17096 2022-03-07 18:04:24.289144 calfpy-1.17.0/PKG-INFO
--rw-rw-rw-   0        0        0    16474 2022-03-07 17:21:34.000000 calfpy-1.17.0/README.md
--rw-rw-rw-   0        0        0      108 2021-08-04 01:22:06.000000 calfpy-1.17.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-03-07 18:04:24.289144 calfpy-1.17.0/setup.cfg
--rw-rw-rw-   0        0        0     1009 2022-03-07 18:02:38.000000 calfpy-1.17.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-07 18:04:24.201474 calfpy-1.17.0/src/
-drwxrwxrwx   0        0        0        0 2022-03-07 18:04:24.253607 calfpy-1.17.0/src/calfpy/
--rw-rw-rw-   0        0        0        0 2021-08-04 01:22:06.000000 calfpy-1.17.0/src/calfpy/__init__.py
--rw-rw-rw-   0        0        0    58148 2021-11-08 17:26:19.000000 calfpy-1.17.0/src/calfpy/methods.py
-drwxrwxrwx   0        0        0        0 2022-03-07 18:04:24.287176 calfpy-1.17.0/src/calfpy.egg-info/
--rw-rw-rw-   0        0        0    17096 2022-03-07 18:04:23.000000 calfpy-1.17.0/src/calfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2022-03-07 18:04:24.000000 calfpy-1.17.0/src/calfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-07 18:04:24.000000 calfpy-1.17.0/src/calfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2022-03-07 18:04:24.000000 calfpy-1.17.0/src/calfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-03-07 18:04:24.000000 calfpy-1.17.0/src/calfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 19:56:19.528799 calfpy-1.20.1/
+-rw-rw-rw-   0        0        0    18429 2021-08-04 01:22:06.000000 calfpy-1.20.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    17047 2023-05-24 19:56:19.527795 calfpy-1.20.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16464 2023-05-24 19:55:13.000000 calfpy-1.20.1/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-04 01:22:06.000000 calfpy-1.20.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 19:56:19.528799 calfpy-1.20.1/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2023-05-24 19:55:25.000000 calfpy-1.20.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:56:19.491342 calfpy-1.20.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 19:56:19.506802 calfpy-1.20.1/src/calfpy/
+-rw-rw-rw-   0        0        0        0 2021-08-04 01:22:06.000000 calfpy-1.20.1/src/calfpy/__init__.py
+-rw-rw-rw-   0        0        0    58279 2023-05-24 19:54:42.000000 calfpy-1.20.1/src/calfpy/methods.py
+drwxrwxrwx   0        0        0        0 2023-05-24 19:56:19.526827 calfpy-1.20.1/src/calfpy.egg-info/
+-rw-rw-rw-   0        0        0    17047 2023-05-24 19:56:19.000000 calfpy-1.20.1/src/calfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-24 19:56:19.000000 calfpy-1.20.1/src/calfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 19:56:19.000000 calfpy-1.20.1/src/calfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-24 19:56:19.000000 calfpy-1.20.1/src/calfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-24 19:56:19.000000 calfpy-1.20.1/src/calfpy.egg-info/top_level.txt
```

### Comparing `calfpy-1.17.0/LICENSE.txt` & `calfpy-1.20.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `calfpy-1.17.0/PKG-INFO` & `calfpy-1.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: calfpy
-Version: 1.17.0
+Version: 1.20.1
 Summary: Contains greedy algorithms for coarse approximation linear functions.
 Home-page: https://github.com/jorufo/CALF_Python
 Author: John Ford, Clark Jeffries, Diana Perkins
 Author-email: JoRuFo@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jorufo/CALF_Python/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# CALF v1.17.0 README
+# CALF v1.20.1 README
 
 
 # Setup and Usage
 You can install CALF by running `pip install calfpy`
 
-You can import all CALF functions by using the folliwng import statement  
-`import caflpy.methods`
+You can import all CALF methods by using the folliwng import statement  
+`from calfpy.methods import *`
 
 Calling a function (example)
-`calfpy.methods.calf(data, 3, "binary", optimize = 'pval', verbose = False)`  
+`calf(data, 3, "binary", optimize = 'pval', verbose = False)`  
 
 # Library Documentation
 
 ## *calf(data, nMarkers, targetVector, optimize = 'pval', verbose = False)*  
 
 Coarse Approximation Linear function.  The main function used to invoke the CALF algorithm on a dataset.  
 
@@ -262,8 +260,7 @@
 auc | The AUC determined during running CALF.  AUC can be provided for given markers AUC represented for selected markers will only be optimal if set to optimzie for AUC.
 randomize | False
 proportion | Undefined
 targetVec | Target vector argument given in the function call.
 rocPlot | Receiver operating curve plot, if applicable for dataset type and optimizer supplied.
 finalBest | The optimal value for the provided optimization type, e.g. if optimize='pval" this will have the calculated p-value for the run.
 optimize | The optimizer argument given in the function call.
-
```

### Comparing `calfpy-1.17.0/README.md` & `calfpy-1.20.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# CALF v1.17.0 README
+# CALF v1.20.1 README
 
 
 # Setup and Usage
 You can install CALF by running `pip install calfpy`
 
-You can import all CALF functions by using the folliwng import statement  
-`import caflpy.methods`
+You can import all CALF methods by using the folliwng import statement  
+`from calfpy.methods import *`
 
 Calling a function (example)
-`calfpy.methods.calf(data, 3, "binary", optimize = 'pval', verbose = False)`  
+`calf(data, 3, "binary", optimize = 'pval', verbose = False)`  
 
 # Library Documentation
 
 ## *calf(data, nMarkers, targetVector, optimize = 'pval', verbose = False)*  
 
 Coarse Approximation Linear function.  The main function used to invoke the CALF algorithm on a dataset.
```

### Comparing `calfpy-1.17.0/setup.py` & `calfpy-1.20.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="calfpy",
-    version="1.17.0",
+    version="1.20.1",
     author="John Ford, Clark Jeffries, Diana Perkins",
     author_email="JoRuFo@gmail.com",
     description="Contains greedy algorithms for coarse approximation linear functions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jorufo/CALF_Python",
     project_urls={
         "Bug Tracker": "https://github.com/jorufo/CALF_Python/issues",
     },
-    install_requires = ['numpy==1.20.2', 'pandas==1.2.4', 'plotnine==0.8.0', 'scipy==1.6.3'],
+    install_requires = ['numpy>=1.20.2,<=1.23.0', 'pandas>=1.2.4,<=1.5.2', 'plotnine==0.10.0', 'scipy>=1.6.3,<=1.9.3'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `calfpy-1.17.0/src/calfpy/methods.py` & `calfpy-1.20.1/src/calfpy/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -768,15 +768,15 @@
 					resultsDropped = results.drop(results.columns[0:3], axis=1)
 
 					weightsTimesUnkept = unkeptDropped.dot(resultsDropped.iloc[rowCount,:])
 					
 					resultCtrlData = weightsTimesUnkept[unkeptCtrlRows.index]
 					resultCaseData = weightsTimesUnkept[unkeptCaseRows.index]
 					
-					optimizedUnkeptList.append(ttest_ind(resultCaseData, resultCtrlData, equal_var=False).pvalue)
+					optimizedUnkeptList.append(ttest_ind(resultCaseData.astype(float), resultCtrlData.astype(float), equal_var=False).pvalue)
 
 				elif optimize == 'auc':
 					unkeptDropped = unkeptData.drop(unkeptData.columns[0], axis=1)
 					resultsDropped = results.drop(results.columns[0:2], axis=1)
 
 					weightsTimesUnkept = unkeptDropped.dot(resultsDropped.iloc[rowCount,:])
 					
@@ -975,15 +975,15 @@
 					resultsDropped = results.drop(results.columns[0:3], axis=1)
 
 					weightsTimesUnkept = unkeptDropped.dot(resultsDropped.iloc[rowCount,:])
 					
 					resultCtrlData = weightsTimesUnkept[unkeptCtrlRows.index]
 					resultCaseData = weightsTimesUnkept[unkeptCaseRows.index]
 					
-					optimizedUnkeptList.append(ttest_ind(resultCaseData, resultCtrlData, equal_var=False).pvalue)
+					optimizedUnkeptList.append(ttest_ind(resultCaseData.astype(float), resultCtrlData.astype(float), equal_var=False).pvalue)
 
 				elif optimize == 'auc':
 					unkeptDropped = unkeptData.drop(unkeptData.columns[0], axis=1)
 					resultsDropped = results.drop(results.columns[0:2], axis=1)
 
 					weightsTimesUnkept = unkeptDropped.dot(resultsDropped.iloc[rowCount,:])
 					
@@ -1085,25 +1085,28 @@
 			file.write(str(x['finalBest']))
 			file.close()
 	else:
 		file = open(filename,'a')
 		file.write('\n')
 		file.close()
 		if x['targetVec'] == 'binary' and x['optimize'] == 'auc':
-			auc = pandas.DataFrame(x['auc'])
-			auc.columns = ['AUC']
-			auc.to_csv(filename, index = False, mode='a')
+			if x['auc'] is not None:
+				auc = pandas.DataFrame(x['auc'])
+				auc.columns = ['AUC']
+				auc.to_csv(filename, index = False, mode='a')
 		elif x['targetVec'] == 'binary' and x['optimize'] == 'pval':
-			finalBest = pandas.DataFrame(x['finalBest'])
-			finalBest.columns = ['pval']
-			finalBest.to_csv(filename, index = False, mode='a')
+			if x['finalBest'] is not None:
+				finalBest = pandas.DataFrame(x['finalBest'])
+				finalBest.columns = ['pval']
+				finalBest.to_csv(filename, index = False, mode='a')
 		elif x['targetVec'] == 'nonbinary':
-			finalBest = pandas.DataFrame(x['finalBest'])
-			finalBest.columns = ['corr']
-			finalBest.to_csv(filename, index = False, mode='a')
+			if x['finalBest'] is not None:
+				finalBest = pandas.DataFrame(x['finalBest'])
+				finalBest.columns = ['corr']
+				finalBest.to_csv(filename, index = False, mode='a')
 
 
 
 
 def write_calf_subset(x, filename):
 	'''Writes the results from a call to calf_subset() to a file
 
@@ -1117,16 +1120,17 @@
 		mode='w')
 
 	file = open(filename,'a')
 	file.write('\n')
 	file.close()
 	
  
-	finalBest = pandas.DataFrame(x['finalBest'])
-	if finalBest is not None:
+	
+	if x['finalBest'] is not None:
+		finalBest = pandas.DataFrame(x['finalBest'])
 		if x['targetVec'] == 'binary' and x['optimize'] == 'auc':
 			finalBest.columns = ['AUC']
 		elif x['targetVec'] == 'binary' and x['optimize'] == 'pval':
 			finalBest.columns = ['pval']
 		elif x['targetVec'] == 'nonbinary':
 			finalBest.columns = ['corr']
 		
@@ -1189,15 +1193,15 @@
 	refy = None
 
 	if targetVector == 'nonbinary':
 		optimize = None
 
 	nVars = data.shape[1] - 1
 	dNeg  = -data.iloc[:,1:data.shape[1]]
-	dNeg.columns = list(map(lambda i: i+'.1',dNeg.columns))
+	dNeg.columns = list(map(lambda i: str(i)+'.1',dNeg.columns))
 	data = pandas.concat([data,dNeg], axis=1)
 
 	if nMarkers > nVars:
 		raise Exception('CALF ERROR: Requested number of markers is larger than the number of markers in data set.  Please revise this value or make sure your data were read in properly.')
 
 	if randomize == True:
 		data.iloc[:,0] = data.iloc[:,0].sample(frac=1).values
@@ -1431,15 +1435,15 @@
 		print("\n")
 
 	indexNegPos = numpy.array([0] * 2 * nVars)
 	indexNegPos[[i for i in keepIndices if i > nVars]] = -1
 	indexNegPos[[i for i in keepIndices if i <= nVars]] = 1
 
 	# Produce the table of results
-	output = pandas.DataFrame({'Marker': [i.replace('.1','') for i in keepMarkers], 'Weight': indexNegPos[keepIndices]})
+	output = pandas.DataFrame({'Marker': [str(i).replace('.1','') for i in keepMarkers], 'Weight': indexNegPos[keepIndices]})
 
 	if targetVector == "nonbinary" or optimize == "auc":
 		finalBestCrit = 1 / bestCrits[-1]
 	else:
 		finalBestCrit = bestCrits[-1]
 
 	if targetVector == "binary":
@@ -1455,21 +1459,20 @@
 
 
 		# set up plot -----------------------------------------------------#
 
 		all_result = pandas.concat([funcValue, pandas.DataFrame(seqCaseCtrl).set_index(funcValue.index), ranks], axis= 1)
 		all_result.columns = ['funcValue', 'seqCaseCtrl', 'ranks']
 		all_result = all_result.sort_values(by='ranks')
+		print(len(all_result))
 
-		x_list = numpy.arange(0,1,1/(len(all_result)-1))
-		x_list = numpy.append(x_list, 1)
+		x_list = numpy.arange(0,1,1/(len(all_result)))
 		refx = pandas.DataFrame(x_list).set_index(all_result.index)
 
-		y_list = numpy.arange(0,1,1/(len(all_result)-1))
-		y_list = numpy.append(y_list, 1)
+		y_list = numpy.arange(0,1,1/(len(all_result)))
 		refy = pandas.DataFrame(y_list).set_index(all_result.index)
 
 		all_result = pandas.concat([all_result, refx, refy], axis = 1)
 
 		initVal = all_result['seqCaseCtrl'].iloc[0]
 		moveRight = len(case) if initVal == 0 else len(ctrl)
 		moveUp = len(ctrl) if initVal == 0 else len(case)
@@ -1516,8 +1519,8 @@
 	return {'selection': output,
 			'auc': auc,
 			'randomize': randomize,
 			'proportion': proportion,
 			'targetVec': targetVector,
 			'rocPlot': rocPlot,
 			'finalBest': finalBestCrit,
-			'optimize': optimize}
+			'optimize': optimize}
```

### Comparing `calfpy-1.17.0/src/calfpy.egg-info/PKG-INFO` & `calfpy-1.20.1/src/calfpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: calfpy
-Version: 1.17.0
+Version: 1.20.1
 Summary: Contains greedy algorithms for coarse approximation linear functions.
 Home-page: https://github.com/jorufo/CALF_Python
 Author: John Ford, Clark Jeffries, Diana Perkins
 Author-email: JoRuFo@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jorufo/CALF_Python/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# CALF v1.17.0 README
+# CALF v1.20.1 README
 
 
 # Setup and Usage
 You can install CALF by running `pip install calfpy`
 
-You can import all CALF functions by using the folliwng import statement  
-`import caflpy.methods`
+You can import all CALF methods by using the folliwng import statement  
+`from calfpy.methods import *`
 
 Calling a function (example)
-`calfpy.methods.calf(data, 3, "binary", optimize = 'pval', verbose = False)`  
+`calf(data, 3, "binary", optimize = 'pval', verbose = False)`  
 
 # Library Documentation
 
 ## *calf(data, nMarkers, targetVector, optimize = 'pval', verbose = False)*  
 
 Coarse Approximation Linear function.  The main function used to invoke the CALF algorithm on a dataset.  
 
@@ -262,8 +260,7 @@
 auc | The AUC determined during running CALF.  AUC can be provided for given markers AUC represented for selected markers will only be optimal if set to optimzie for AUC.
 randomize | False
 proportion | Undefined
 targetVec | Target vector argument given in the function call.
 rocPlot | Receiver operating curve plot, if applicable for dataset type and optimizer supplied.
 finalBest | The optimal value for the provided optimization type, e.g. if optimize='pval" this will have the calculated p-value for the run.
 optimize | The optimizer argument given in the function call.
-
```

