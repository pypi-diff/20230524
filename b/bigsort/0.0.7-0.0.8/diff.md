# Comparing `tmp/bigsort-0.0.7.tar.gz` & `tmp/bigsort-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigsort-0.0.7.tar", last modified: Wed Apr 12 14:41:38 2023, max compression
+gzip compressed data, was "bigsort-0.0.8.tar", last modified: Wed May 24 14:00:55 2023, max compression
```

## Comparing `bigsort-0.0.7.tar` & `bigsort-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:41:38.007960 bigsort-0.0.7/
--rw-rw-rw-   0        0        0     1310 2023-04-12 14:41:38.007010 bigsort-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 14:41:38.005012 bigsort-0.0.7/bigsort.egg-info/
--rw-rw-rw-   0        0        0     1310 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 14:41:37.000000 bigsort-0.0.7/bigsort.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10564 2023-04-12 14:41:27.000000 bigsort-0.0.7/bigsort.py
--rw-rw-rw-   0        0        0       42 2023-04-12 14:41:38.008215 bigsort-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-04-12 14:39:29.000000 bigsort-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 14:00:55.095916 bigsort-0.0.8/
+-rw-rw-rw-   0        0        0     1359 2023-05-24 14:00:55.094916 bigsort-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 14:00:55.093917 bigsort-0.0.8/bigsort.egg-info/
+-rw-rw-rw-   0        0        0     1359 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-24 14:00:54.000000 bigsort-0.0.8/bigsort.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10658 2023-05-24 13:37:18.000000 bigsort-0.0.8/bigsort.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 14:00:55.095916 bigsort-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-05-24 13:46:49.000000 bigsort-0.0.8/setup.py
```

### Comparing `bigsort-0.0.7/PKG-INFO` & `bigsort-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigsort
-Version: 0.0.7
+Version: 0.0.8
 Summary: sort big file or streams
 Home-page: https://github.com/laohur/bigsort
 Author: laohur
 Author-email: laohur@gmail.com
 License: [Anti-996 License](https: // github.com/996icu/996.ICU/blob/master/LICENSE)
 Keywords: bigsort,sort,external sort,big file sort
 Requires-Python: >=3.0
@@ -21,21 +21,22 @@
 ```shell
 bigsort -i  readme.md -o sorted.txt  # default sort in increase 
 cat readme.md |  bigsort --sortType=d --unique=1 > sorted.txt  # sort pipe, order in descend, unique
 bigsort -i sorted.txt -c ">"  # check order
 bigsort -i  readme.md --unique=1   | bigsort --sortType=R > sorted.txt   # unique and shufle 
 seq 0  1123456789  | bigsort --sortType=d -T "./"  > sorted.txt  # just try sort 10^10 numbers
 wc -l *.py | bigsort   -k 1n,2  -b 1 -t " "   # sort by key
+bigsort -i  readme.md -s R -g 10   # get first 10 lines
 ```
 
 ### python
 
 ```python
 import os
-from bigsort import  bigsort, sortFile, check, bisect
+from bigsort import  bigsort, sortFile, check
 
 # sort in file
 sortFile("cat readme.md","sorted.txt")
 check(open("sorted.txt"),"<=")
 
 # sort in pipe
 bigsort(os.popen("cat readme.md"),open("sorted.txt",'w'),unique=1,sortType="d")
```

### Comparing `bigsort-0.0.7/bigsort.egg-info/PKG-INFO` & `bigsort-0.0.8/bigsort.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigsort
-Version: 0.0.7
+Version: 0.0.8
 Summary: sort big file or streams
 Home-page: https://github.com/laohur/bigsort
 Author: laohur
 Author-email: laohur@gmail.com
 License: [Anti-996 License](https: // github.com/996icu/996.ICU/blob/master/LICENSE)
 Keywords: bigsort,sort,external sort,big file sort
 Requires-Python: >=3.0
@@ -21,21 +21,22 @@
 ```shell
 bigsort -i  readme.md -o sorted.txt  # default sort in increase 
 cat readme.md |  bigsort --sortType=d --unique=1 > sorted.txt  # sort pipe, order in descend, unique
 bigsort -i sorted.txt -c ">"  # check order
 bigsort -i  readme.md --unique=1   | bigsort --sortType=R > sorted.txt   # unique and shufle 
 seq 0  1123456789  | bigsort --sortType=d -T "./"  > sorted.txt  # just try sort 10^10 numbers
 wc -l *.py | bigsort   -k 1n,2  -b 1 -t " "   # sort by key
+bigsort -i  readme.md -s R -g 10   # get first 10 lines
 ```
 
 ### python
 
 ```python
 import os
-from bigsort import  bigsort, sortFile, check, bisect
+from bigsort import  bigsort, sortFile, check
 
 # sort in file
 sortFile("cat readme.md","sorted.txt")
 check(open("sorted.txt"),"<=")
 
 # sort in pipe
 bigsort(os.popen("cat readme.md"),open("sorted.txt",'w'),unique=1,sortType="d")
```

### Comparing `bigsort-0.0.7/bigsort.py` & `bigsort-0.0.8/bigsort.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,16 +199,18 @@
         if ' ' not in src:
             src = "cat " + src
         reader = os.popen(src)
     if not tgt:
         writer = sys.stdout
     else:
         writer = open(tgt, 'w', buffering=buffering)
+
     bigsort(reader, writer, sortType=sortType, unique=unique, keyFn=keyFn, nHead=nHead, budget=budget, tmpDir=tmpDir, nSplit=nSplit, nLine=nLine)
-    writer.close()
+    if tgt:
+        writer.close()
 
 
 # https://docs.python.org/3/library/operator.html
 OrderingFn = {
     '<': operator.le,
     '<=': operator.lt,
     '==': operator.eq,
@@ -233,27 +235,28 @@
     return True
 
 
 def main():
     parser = argparse.ArgumentParser()
     # parser.add_argument("src") # sys.stdin
     # parser.add_argument("tgt") # sys.stdout
-    parser.add_argument("-i", "--input", default=None)
+    parser.add_argument("-i", "--input", default="readme.md")
+    # parser.add_argument("-i", "--input", default=None)
     parser.add_argument("-o", "--output", default=None)
     parser.add_argument("--buffering", type=int, default=1024*1024)
     parser.add_argument("--nSplit", type=int, default=10)  # bigger if skew or shuffle
     parser.add_argument("--nLine", type=int, default=100000)
     parser.add_argument("-M", "--budget", type=float, default=0.4)  # 0.8 memary budget in ratio if single pipe
     parser.add_argument("-u", "--unique", default=False)  # remove repeat neighbor; only when sort
     parser.add_argument("-s", "--sortType", default="i")  # one of  'i/d/R': increase descend random
     parser.add_argument("-b", "--blanks", default=None)  # ignore-leading-blanks
     parser.add_argument("-t", "--sep", default=None)  # seperator of line
     parser.add_argument("-k", "--key", default=None)  # sort by key; '3n,5'
     parser.add_argument("-n", "--number", type=int, default=0)  # key as number instead of string
-    parser.add_argument("--head", type=int, default=-1)  # number from head, like head -n
+    parser.add_argument("-g","--get", type=int, default=-1)  # get first number lines , like head -n
     parser.add_argument("-T", "--tmpDir", default=None)  # None "_tmp_"
     parser.add_argument("-c", "--checkOrdering")  # check file order; < > <= !=...
     args = parser.parse_args()
     logger.info(args)
 
     def keyFn(l):
         if args.blanks:
@@ -288,14 +291,14 @@
             reader = sys.stdin
         else:
             if ' ' not in src:
                 src = "cat " + src
             reader = os.popen(src)
         check(reader, args.checkOrdering, keyFn=keyFn)
     else:
-        sortFile(args.input, args.output, sortType=args.sortType, unique=args.unique, keyFn=keyFn, nHead=args.head, budget=args.budget, tmpDir=args.tmpDir, nSplit=args.nSplit, nLine=args.nLine, buffering=args.buffering)
+        sortFile(args.input, args.output, sortType=args.sortType, unique=args.unique, keyFn=keyFn, nHead=args.get, budget=args.budget, tmpDir=args.tmpDir, nSplit=args.nSplit, nLine=args.nLine, buffering=args.buffering)
     # sortFile("cat bookcorpus.txt","sorted.txt")
     # check(open("sorted.txt"),"<=")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bigsort-0.0.7/setup.py` & `bigsort-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     long_description = f.read()
 
 
 setup(
     name="bigsort",
     # packages=find_packages(),
     py_modules=['bigsort'],
-    version='0.0.7',
+    version='0.0.8',
     description='sort big file or streams',
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.0',
     install_requires=[
         "psutil",
         "logzero"
```

