# Comparing `tmp/simplefourierfilter-0.1.tar.gz` & `tmp/simplefourierfilter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplefourierfilter-0.1.tar", last modified: Wed May 24 11:51:30 2023, max compression
+gzip compressed data, was "simplefourierfilter-0.2.tar", last modified: Wed May 24 14:23:58 2023, max compression
```

## Comparing `simplefourierfilter-0.1.tar` & `simplefourierfilter-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 11:51:30.483137 simplefourierfilter-0.1/
--rw-rw-rw-   0        0        0     1039 2023-05-24 11:43:05.000000 simplefourierfilter-0.1/LICENCE.txt
--rw-rw-rw-   0        0        0      146 2023-05-24 11:51:30.482139 simplefourierfilter-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-05-24 11:43:41.000000 simplefourierfilter-0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 11:51:30.483137 simplefourierfilter-0.1/setup.cfg
--rw-rw-rw-   0        0        0      274 2023-05-24 11:51:05.000000 simplefourierfilter-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 11:51:30.480137 simplefourierfilter-0.1/simplefourierfilter.egg-info/
--rw-rw-rw-   0        0        0      146 2023-05-24 11:51:30.000000 simplefourierfilter-0.1/simplefourierfilter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-24 11:51:30.000000 simplefourierfilter-0.1/simplefourierfilter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 11:51:30.000000 simplefourierfilter-0.1/simplefourierfilter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-24 11:51:30.000000 simplefourierfilter-0.1/simplefourierfilter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-24 11:51:30.000000 simplefourierfilter-0.1/simplefourierfilter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4913 2023-05-24 11:38:51.000000 simplefourierfilter-0.1/simplefourierfilter.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:23:58.568966 simplefourierfilter-0.2/
+-rw-rw-rw-   0        0        0     1039 2023-05-24 11:43:05.000000 simplefourierfilter-0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0      146 2023-05-24 14:23:58.567961 simplefourierfilter-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-05-24 11:43:41.000000 simplefourierfilter-0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 14:23:58.568966 simplefourierfilter-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      274 2023-05-24 14:23:51.000000 simplefourierfilter-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:23:58.566960 simplefourierfilter-0.2/simplefourierfilter.egg-info/
+-rw-rw-rw-   0        0        0      146 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-24 14:23:58.000000 simplefourierfilter-0.2/simplefourierfilter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4933 2023-05-24 14:21:20.000000 simplefourierfilter-0.2/simplefourierfilter.py
```

### Comparing `simplefourierfilter-0.1/LICENCE.txt` & `simplefourierfilter-0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `simplefourierfilter-0.1/simplefourierfilter.py` & `simplefourierfilter-0.2/simplefourierfilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
             plt.axvline(x = ratio,color = 'r')
             plt.legend(("Frequency spectrum","Cut-off frequency"))
             
         elif method == "dist":
             n = len(cauchy)
             plt.plot(omega_plot,cauchy[int(n/2):-1])
             plt.legend(("Frequency spectrum","Scaling distribution"))
+        plt.show()
         return X_f
 
 
 def spectralDensity(X,Fs=1):
     """
     Function used to plot normalised spectral density distribution from time seriers
     :param X: numpy array
```

