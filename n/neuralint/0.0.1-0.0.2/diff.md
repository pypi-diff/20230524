# Comparing `tmp/neuralint-0.0.1.tar.gz` & `tmp/neuralint-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\neuralint-0.0.1.tar", last modified: Tue May 23 20:25:03 2023, max compression
+gzip compressed data, was "dist\neuralint-0.0.2.tar", last modified: Wed May 24 20:45:10 2023, max compression
```

## Comparing `neuralint-0.0.1.tar` & `neuralint-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 20:25:03.533703 neuralint-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-23 20:25:03.493662 neuralint-0.0.1/Neuralint/
--rw-rw-rw-   0        0        0        0 2023-04-04 14:08:16.000000 neuralint-0.0.1/Neuralint/__init__.py
--rw-rw-rw-   0        0        0     4155 2023-05-19 18:51:52.000000 neuralint-0.0.1/Neuralint/endToEnd.py
--rw-rw-rw-   0        0        0     9648 2023-05-19 18:51:52.000000 neuralint-0.0.1/Neuralint/grooveParser.py
--rw-rw-rw-   0        0        0     4840 2023-05-19 18:51:52.000000 neuralint-0.0.1/Neuralint/mix_bugs_1.py
--rw-rw-rw-   0        0        0    63375 2023-05-19 18:51:52.000000 neuralint-0.0.1/Neuralint/nodes_Keras.py
--rw-rw-rw-   0        0        0    60891 2023-05-19 18:51:52.000000 neuralint-0.0.1/Neuralint/nodes_TF.py
--rw-rw-rw-   0        0        0    11164 2023-05-19 18:51:52.000000 neuralint-0.0.1/Neuralint/parser_Keras.py
--rw-rw-rw-   0        0        0     9675 2023-05-19 18:51:52.000000 neuralint-0.0.1/Neuralint/parser_TF.py
--rw-rw-rw-   0        0        0      582 2023-05-23 20:25:03.533703 neuralint-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 20:25:03.525699 neuralint-0.0.1/neuralint.egg-info/
--rw-rw-rw-   0        0        0      582 2023-05-23 20:25:03.000000 neuralint-0.0.1/neuralint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-05-23 20:25:03.000000 neuralint-0.0.1/neuralint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 20:25:03.000000 neuralint-0.0.1/neuralint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-23 20:25:03.000000 neuralint-0.0.1/neuralint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-23 20:25:03.000000 neuralint-0.0.1/neuralint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 20:25:03.533703 neuralint-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-05-23 20:21:58.000000 neuralint-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 20:45:10.602153 neuralint-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-24 20:45:10.586135 neuralint-0.0.2/Neuralint/
+-rw-rw-rw-   0        0        0        0 2023-04-04 14:08:16.000000 neuralint-0.0.2/Neuralint/__init__.py
+-rw-rw-rw-   0        0        0     3934 2023-05-24 16:22:31.000000 neuralint-0.0.2/Neuralint/endToEnd.py
+-rw-rw-rw-   0        0        0     9648 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/grooveParser.py
+-rw-rw-rw-   0        0        0     4840 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/mix_bugs_1.py
+-rw-rw-rw-   0        0        0    63375 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/nodes_Keras.py
+-rw-rw-rw-   0        0        0    60891 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/nodes_TF.py
+-rw-rw-rw-   0        0        0    11164 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/parser_Keras.py
+-rw-rw-rw-   0        0        0     9675 2023-05-19 18:51:52.000000 neuralint-0.0.2/Neuralint/parser_TF.py
+-rw-rw-rw-   0        0        0      582 2023-05-24 20:45:10.602153 neuralint-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 20:45:10.602153 neuralint-0.0.2/neuralint.egg-info/
+-rw-rw-rw-   0        0        0      582 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 20:45:10.000000 neuralint-0.0.2/neuralint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 20:45:10.602153 neuralint-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      844 2023-05-24 20:43:30.000000 neuralint-0.0.2/setup.py
```

### Comparing `neuralint-0.0.1/Neuralint/endToEnd.py` & `neuralint-0.0.2/Neuralint/endToEnd.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,38 +68,27 @@
         return False
     inOut = inOut[1:len(inOut)-1]
     inOutList = inOut.split(",")
     inOutList = list(map(int, inOutList))
 
     return inOutList
 
-def main():
-    arguments = sys.argv
-    if len(arguments) != 6:
-        raise SystemExit('usage: endToEnd.py [input filename] [input size] [output size] [parser type] [output filename]')
-    else:
-        file_folderName = arguments[1]
-        inputSize = checkInOutSize(arguments[2])
-        outputSize = checkInOutSize(arguments[3])
-
-        if inputSize == False or outputSize==False:
-            raise SystemExit("Error : Input and output size should be entered as array([x1, x2, x3, ...]).")
-
-        parserName = arguments[4].lower()
-        resultFileName = arguments[5]
-        if parserName != "tf" and parserName != "keras":
-            raise SystemExit("Error : Parser type should be 'tf' or 'keras'")
+def main(file_folderName,inputSize,outputSize,parserName,resultFileName):
+    if inputSize == False or outputSize==False:
+        raise SystemExit("Error : Input and output size should be entered as array([x1, x2, x3, ...]).")
+    parserName=parserName.lower()
+    if parserName != "tf" and parserName != "keras":
+        raise SystemExit("Error : Parser type should be 'tf' or 'keras'")
     try:
         outputFile = open(f"{resultFileName}.txt" ,"w", encoding="ISO-8859-1")
     except IOError:
         raise SystemExit("Error : output filename should meet host operating system filename rules")
-
     extention = os.path.splitext(file_folderName)[1]
-
     if extention == ".py":
         output = parsDnnScript(fileName = os.path.splitext(file_folderName)[0], inputSize = inputSize ,outputSize = outputSize , parser=parserName)
         outputFile.write(output)
     else:
         raise SystemExit("Error : input should be a python script file")
+    
 if __name__ == '__main__':
-    main()
+    main(file_folderName="mix_bugs_1.py",inputSize=[32,28,28,1],outputSize=[32,10],parserName="tf",resultFileName="result")
```

### Comparing `neuralint-0.0.1/Neuralint/grooveParser.py` & `neuralint-0.0.2/Neuralint/grooveParser.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.1/Neuralint/mix_bugs_1.py` & `neuralint-0.0.2/Neuralint/mix_bugs_1.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.1/Neuralint/nodes_Keras.py` & `neuralint-0.0.2/Neuralint/nodes_Keras.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.1/Neuralint/nodes_TF.py` & `neuralint-0.0.2/Neuralint/nodes_TF.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.1/Neuralint/parser_Keras.py` & `neuralint-0.0.2/Neuralint/parser_Keras.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.1/Neuralint/parser_TF.py` & `neuralint-0.0.2/Neuralint/parser_TF.py`

 * *Files identical despite different names*

### Comparing `neuralint-0.0.1/PKG-INFO` & `neuralint-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralint
-Version: 0.0.1
+Version: 0.0.2
 Summary: Neuralint package
 Home-page: UNKNOWN
 Author: Poly
 Author-email: <ghassendaoud99@gmail.com>
 License: UNKNOWN
 Description: Neuralint package.
 Keywords: python,cnn,test
```

### Comparing `neuralint-0.0.1/neuralint.egg-info/PKG-INFO` & `neuralint-0.0.2/neuralint.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralint
-Version: 0.0.1
+Version: 0.0.2
 Summary: Neuralint package
 Home-page: UNKNOWN
 Author: Poly
 Author-email: <ghassendaoud99@gmail.com>
 License: UNKNOWN
 Description: Neuralint package.
 Keywords: python,cnn,test
```

### Comparing `neuralint-0.0.1/setup.py` & `neuralint-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Neuralint package'
 LONG_DESCRIPTION = 'Neuralint package.'
 
 # Setting up
 setup(
     name="neuralint",
     version=VERSION,
```

