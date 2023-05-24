# Comparing `tmp/simplefourierfilter-0.2.tar.gz` & `tmp/simplefourierfilter-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplefourierfilter-0.2.tar", last modified: Wed May 24 14:23:58 2023, max compression
+gzip compressed data, was "simplefourierfilter-0.21.tar", last modified: Wed May 24 15:03:52 2023, max compression
```

## Comparing `simplefourierfilter-0.2.tar` & `simplefourierfilter-0.21.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:23:58.568966 simplefourierfilter-0.2/
--rw-rw-rw-   0        0        0     1039 2023-05-24 11:43:05.000000 simplefourierfilter-0.2/LICENCE.txt
--rw-rw-rw-   0        0        0      146 2023-05-24 14:23:58.567961 simplefourierfilter-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-05-24 11:43:41.000000 simplefourierfilter-0.2/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 14:23:58.568966 simplefourierfilter-0.2/setup.cfg
--rw-rw-rw-   0        0        0      274 2023-05-24 14:23:51.000000 simplefourierfilter-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:23:58.566960 simplefourierfilter-0.2/simplefourierfilter.egg-info/
--rw-rw-rw-   0        0        0      146 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4933 2023-05-24 14:21:20.000000 simplefourierfilter-0.2/simplefourierfilter.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:03:52.695164 simplefourierfilter-0.21/
+-rw-rw-rw-   0        0        0     1085 2023-05-24 14:26:57.000000 simplefourierfilter-0.21/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-05-24 15:03:52.695164 simplefourierfilter-0.21/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-05-24 11:43:41.000000 simplefourierfilter-0.21/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:03:52.695164 simplefourierfilter-0.21/setup.cfg
+-rw-rw-rw-   0        0        0      275 2023-05-24 15:03:49.000000 simplefourierfilter-0.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:03:52.687150 simplefourierfilter-0.21/simplefourierfilter.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-23 10:47:59.000000 simplefourierfilter-0.21/simplefourierfilter.egg-info/.gitignore
+-rw-rw-rw-   0        0        0      143 2023-05-24 15:03:52.000000 simplefourierfilter-0.21/simplefourierfilter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-05-24 15:03:52.000000 simplefourierfilter-0.21/simplefourierfilter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:03:52.000000 simplefourierfilter-0.21/simplefourierfilter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-24 15:03:52.000000 simplefourierfilter-0.21/simplefourierfilter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-24 15:03:52.000000 simplefourierfilter-0.21/simplefourierfilter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4925 2023-05-24 15:03:26.000000 simplefourierfilter-0.21/simplefourierfilter.py
```

### Comparing `simplefourierfilter-0.2/LICENCE.txt` & `simplefourierfilter-0.21/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-License
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2023 PauliAnt
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `simplefourierfilter-0.2/simplefourierfilter.py` & `simplefourierfilter-0.21/simplefourierfilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,16 +115,16 @@
             plt.axvline(x = ratio,color = 'r')
             plt.legend(("Frequency spectrum","Cut-off frequency"))
             
         elif method == "dist":
             n = len(cauchy)
             plt.plot(omega_plot,cauchy[int(n/2):-1])
             plt.legend(("Frequency spectrum","Scaling distribution"))
-        plt.show()
-        return X_f
+    plt.show()
+    return X_f
 
 
 def spectralDensity(X,Fs=1):
     """
     Function used to plot normalised spectral density distribution from time seriers
     :param X: numpy array
         Time sequence with equal spacing.
```

