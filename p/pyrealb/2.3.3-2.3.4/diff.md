# Comparing `tmp/pyrealb-2.3.3.tar.gz` & `tmp/pyrealb-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrealb-2.3.3.tar", last modified: Wed Mar 29 13:20:34 2023, max compression
+gzip compressed data, was "pyrealb-2.3.4.tar", last modified: Wed May 24 15:28:17 2023, max compression
```

## Comparing `pyrealb-2.3.3.tar` & `pyrealb-2.3.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-03-29 13:20:34.624501 pyrealb-2.3.3/
--rw-r--r--   0 lapalme    (503) staff       (20)    35129 2021-12-01 22:24:50.000000 pyrealb-2.3.3/LICENSE
--rw-r--r--   0 lapalme    (503) staff       (20)       23 2022-01-27 01:45:34.000000 pyrealb-2.3.3/MANIFEST.in
--rw-r--r--   0 lapalme    (503) staff       (20)     7541 2023-03-29 13:20:34.624651 pyrealb-2.3.3/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)     7044 2023-03-29 02:30:13.000000 pyrealb-2.3.3/README.md
--rw-r--r--   0 lapalme    (503) staff       (20)      104 2021-12-13 01:31:17.000000 pyrealb-2.3.3/pyproject.toml
--rw-r--r--   0 lapalme    (503) staff       (20)      649 2023-03-29 13:20:34.625301 pyrealb-2.3.3/setup.cfg
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-03-29 13:20:34.578612 pyrealb-2.3.3/src/
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-03-29 13:20:34.593468 pyrealb-2.3.3/src/pyrealb/
--rw-r--r--   0 lapalme    (503) staff       (20)    44041 2023-03-27 02:43:34.000000 pyrealb-2.3.3/src/pyrealb/Constituent.py
--rw-r--r--   0 lapalme    (503) staff       (20)    39667 2023-03-27 02:39:55.000000 pyrealb-2.3.3/src/pyrealb/Dependent.py
--rw-r--r--   0 lapalme    (503) staff       (20)     2873 2022-09-05 21:16:34.000000 pyrealb-2.3.3/src/pyrealb/Lexicon.py
--rw-r--r--   0 lapalme    (503) staff       (20)     7663 2023-03-22 14:56:11.000000 pyrealb-2.3.3/src/pyrealb/Number.py
--rw-r--r--   0 lapalme    (503) staff       (20)    57516 2023-03-27 02:29:23.000000 pyrealb-2.3.3/src/pyrealb/Phrase.py
--rw-r--r--   0 lapalme    (503) staff       (20)    37178 2023-03-27 01:48:34.000000 pyrealb-2.3.3/src/pyrealb/Terminal.py
--rw-r--r--   0 lapalme    (503) staff       (20)    14266 2023-03-27 13:03:50.000000 pyrealb-2.3.3/src/pyrealb/Warning.py
--rw-r--r--   0 lapalme    (503) staff       (20)      856 2023-02-03 22:50:26.000000 pyrealb-2.3.3/src/pyrealb/__init__.py
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-03-29 13:20:34.616720 pyrealb-2.3.3/src/pyrealb/data/
--rw-r--r--   0 lapalme    (503) staff       (20)  1321684 2023-02-14 02:05:27.000000 pyrealb-2.3.3/src/pyrealb/data/lexicon-en.json
--rw-r--r--   0 lapalme    (503) staff       (20)  2476720 2023-02-20 01:55:39.000000 pyrealb-2.3.3/src/pyrealb/data/lexicon-fr.json
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-03-29 13:20:34.622369 pyrealb-2.3.3/src/pyrealb/data/pyrealb.egg-info/
--rw-r--r--   0 lapalme    (503) staff       (20)     4155 2022-01-26 22:41:53.000000 pyrealb-2.3.3/src/pyrealb/data/pyrealb.egg-info/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)        0 2022-01-26 22:41:53.000000 pyrealb-2.3.3/src/pyrealb/data/pyrealb.egg-info/SOURCES.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        1 2022-01-26 22:41:53.000000 pyrealb-2.3.3/src/pyrealb/data/pyrealb.egg-info/dependency_links.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        8 2022-01-26 22:41:53.000000 pyrealb-2.3.3/src/pyrealb/data/pyrealb.egg-info/top_level.txt
--rw-r--r--   0 lapalme    (503) staff       (20)    85976 2022-06-14 19:32:16.000000 pyrealb-2.3.3/src/pyrealb/data/rules-en.json
--rw-r--r--   0 lapalme    (503) staff       (20)   173554 2022-06-14 19:51:41.000000 pyrealb-2.3.3/src/pyrealb/data/rules-fr.json
--rw-r--r--   0 lapalme    (503) staff       (20)     2953 2023-03-29 02:30:13.000000 pyrealb-2.3.3/src/pyrealb/utils.py
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-03-29 13:20:34.596267 pyrealb-2.3.3/src/pyrealb.egg-info/
--rw-r--r--   0 lapalme    (503) staff       (20)     7541 2023-03-29 13:20:34.000000 pyrealb-2.3.3/src/pyrealb.egg-info/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)      756 2023-03-29 13:20:34.000000 pyrealb-2.3.3/src/pyrealb.egg-info/SOURCES.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        1 2023-03-29 13:20:34.000000 pyrealb-2.3.3/src/pyrealb.egg-info/dependency_links.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        8 2023-03-29 13:20:34.000000 pyrealb-2.3.3/src/pyrealb.egg-info/top_level.txt
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-03-29 13:20:34.623764 pyrealb-2.3.3/tests/
--rw-r--r--   0 lapalme    (503) staff       (20)     1879 2023-03-04 13:28:19.000000 pyrealb-2.3.3/tests/test.py
--rw-r--r--   0 lapalme    (503) staff       (20)     2870 2023-02-24 19:49:08.000000 pyrealb-2.3.3/tests/testAll.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.997204 pyrealb-2.3.4/
+-rw-r--r--   0 lapalme    (503) staff       (20)    35129 2021-12-01 22:24:50.000000 pyrealb-2.3.4/LICENSE
+-rw-r--r--   0 lapalme    (503) staff       (20)       23 2022-01-27 01:45:34.000000 pyrealb-2.3.4/MANIFEST.in
+-rw-r--r--   0 lapalme    (503) staff       (20)     7577 2023-05-24 15:28:17.997257 pyrealb-2.3.4/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)     7080 2023-05-24 15:15:37.000000 pyrealb-2.3.4/README.md
+-rw-r--r--   0 lapalme    (503) staff       (20)      104 2021-12-13 01:31:17.000000 pyrealb-2.3.4/pyproject.toml
+-rw-r--r--   0 lapalme    (503) staff       (20)      649 2023-05-24 15:28:17.997477 pyrealb-2.3.4/setup.cfg
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.982825 pyrealb-2.3.4/src/
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.986068 pyrealb-2.3.4/src/pyrealb/
+-rw-r--r--   0 lapalme    (503) staff       (20)    44540 2023-05-24 14:55:41.000000 pyrealb-2.3.4/src/pyrealb/Constituent.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    40808 2023-05-24 14:36:19.000000 pyrealb-2.3.4/src/pyrealb/Dependent.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     3050 2023-05-24 14:52:06.000000 pyrealb-2.3.4/src/pyrealb/Lexicon.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     7663 2023-03-22 14:56:11.000000 pyrealb-2.3.4/src/pyrealb/Number.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    57924 2023-05-24 14:43:55.000000 pyrealb-2.3.4/src/pyrealb/Phrase.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    37505 2023-05-23 20:26:22.000000 pyrealb-2.3.4/src/pyrealb/Terminal.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    14266 2023-03-27 13:03:50.000000 pyrealb-2.3.4/src/pyrealb/Warning.py
+-rw-r--r--   0 lapalme    (503) staff       (20)      857 2023-05-24 14:58:21.000000 pyrealb-2.3.4/src/pyrealb/__init__.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.991475 pyrealb-2.3.4/src/pyrealb/data/
+-rw-r--r--   0 lapalme    (503) staff       (20)  1321684 2023-02-14 02:05:27.000000 pyrealb-2.3.4/src/pyrealb/data/lexicon-en.json
+-rw-r--r--   0 lapalme    (503) staff       (20)  2476751 2023-05-23 21:08:01.000000 pyrealb-2.3.4/src/pyrealb/data/lexicon-fr.json
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.996651 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/
+-rw-r--r--   0 lapalme    (503) staff       (20)     4155 2022-01-26 22:41:53.000000 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)        0 2022-01-26 22:41:53.000000 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/SOURCES.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        1 2022-01-26 22:41:53.000000 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/dependency_links.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        8 2022-01-26 22:41:53.000000 pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/top_level.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)    85976 2023-05-24 15:04:29.000000 pyrealb-2.3.4/src/pyrealb/data/rules-en.json
+-rw-r--r--   0 lapalme    (503) staff       (20)   173554 2022-06-14 19:51:41.000000 pyrealb-2.3.4/src/pyrealb/data/rules-fr.json
+-rw-r--r--   0 lapalme    (503) staff       (20)     2953 2023-05-24 15:15:37.000000 pyrealb-2.3.4/src/pyrealb/utils.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.986591 pyrealb-2.3.4/src/pyrealb.egg-info/
+-rw-r--r--   0 lapalme    (503) staff       (20)     7577 2023-05-24 15:28:17.000000 pyrealb-2.3.4/src/pyrealb.egg-info/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)      756 2023-05-24 15:28:17.000000 pyrealb-2.3.4/src/pyrealb.egg-info/SOURCES.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        1 2023-05-24 15:28:17.000000 pyrealb-2.3.4/src/pyrealb.egg-info/dependency_links.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        8 2023-05-24 15:28:17.000000 pyrealb-2.3.4/src/pyrealb.egg-info/top_level.txt
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-24 15:28:17.997062 pyrealb-2.3.4/tests/
+-rw-r--r--   0 lapalme    (503) staff       (20)     1879 2023-03-04 13:28:19.000000 pyrealb-2.3.4/tests/test.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     2870 2023-02-24 19:49:08.000000 pyrealb-2.3.4/tests/testAll.py
```

### Comparing `pyrealb-2.3.3/LICENSE` & `pyrealb-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.3/PKG-INFO` & `pyrealb-2.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrealb
-Version: 2.3.3
+Version: 2.3.4
 Summary: A French-English text realizer
 Home-page: https://github.com/lapalme/pyrealb
 Author: Guy Lapalme
 Author-email: lapalme@iro.umontreal.ca
 Project-URL: Bug Tracker, https://github.com/lapalme/pyrealb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.3 - March 2023*
+*Version 2.3.4 - May 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
 
@@ -119,15 +119,15 @@
 ## For the maintainer mainly
 ### Updating package version on PyPI 
 
 see [this tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 
 These steps take for granted that the password for PyPI has already been given...
 
-1. update version number in `setup.cfg` (it should be the same as `python_version` in `src/pyrealb/utils.py`)
+1. update version number in `setup.cfg` (it should be the same as `python_version` in `src/pyrealb/utils.py` and at the beginning of this document)
 2. `cd` into the directory with the `pyproject.toml` file (the same as this `README.md`)
 3. Build the distribution package  
        `python3 -m build`
 4. Upload to PyPi the last version I.J.K
       `twine upload dist/*-I.J.K.*`
 5. Install new version from PyPI  
     `python3 -m pip install pyrealb --upgrade`
```

### Comparing `pyrealb-2.3.3/README.md` & `pyrealb-2.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.3 - March 2023*
+*Version 2.3.4 - May 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
 
@@ -104,15 +104,15 @@
 ## For the maintainer mainly
 ### Updating package version on PyPI 
 
 see [this tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 
 These steps take for granted that the password for PyPI has already been given...
 
-1. update version number in `setup.cfg` (it should be the same as `python_version` in `src/pyrealb/utils.py`)
+1. update version number in `setup.cfg` (it should be the same as `python_version` in `src/pyrealb/utils.py` and at the beginning of this document)
 2. `cd` into the directory with the `pyproject.toml` file (the same as this `README.md`)
 3. Build the distribution package  
        `python3 -m build`
 4. Upload to PyPi the last version I.J.K
       `twine upload dist/*-I.J.K.*`
 5. Install new version from PyPI  
     `python3 -m pip install pyrealb --upgrade`
```

### Comparing `pyrealb-2.3.3/setup.cfg` & `pyrealb-2.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrealb
-version = 2.3.3
+version = 2.3.4
 author = Guy Lapalme
 author_email = lapalme@iro.umontreal.ca
 description = A French-English text realizer
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lapalme/pyrealb
 project_urls =
```

### Comparing `pyrealb-2.3.3/src/pyrealb/Constituent.py` & `pyrealb-2.3.4/src/pyrealb/Constituent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import re,datetime,sys
 
-from .Lexicon import getLexicon, getLemma, getRules, currentLanguage
+from .Lexicon import getLexicon, getLemma, getRules, currentLanguage, load
 
 defaultProps = {"en":{"g":"n","n":"s","pe":3,"t":"p"},             # language dependent default properties
                 "fr":{"g":"m","n":"s","pe":3,"t":"p","aux":"av"}}
 
 quoteOOV=False # TODO: make this settable globally
 
 optionListMethods = ('a', 'b', 'ba', 'en')
@@ -441,32 +441,37 @@
         if last==0:return # do not try to elide a single word
         i=0
         while i < last:
             if i>0 and cList[i-1].getProp("lier") is not None: # ignore if the preceding word is "lié" to this one
                 i+=1
                 continue
             m1=sepWordREfr.match(cList[i].realization) if cList[i].realization is not None else None
-            if m1  is None or m1.group(2) is None: continue
+            if m1  is None or m1.group(2) is None:
+                i+=1
+                continue
             m2=sepWordREfr.match(cList[i+1].realization) if cList[i].realization is not None else None
-            if m2  is None or m2.group(2) is None: continue
+            if m2  is None or m2.group(2) is None:
+                i+=1
+                continue
             # HACK: m1 and m2 save the parts before and after the first word (w1 and w2) which is in m_i[2]
             # for a single word
             w1=m1.group(2)
             w2=m2.group(2)
             w3NoWords = not re.match(r"^\s*\w",m1.group(3)) # check that the rest of the first word does not start with a word
             elisionFound = False
             if isElidableFr(w2,cList[i+1].lemma,cList[i+1].constType):
                 if elidableWordFrRE.match(w1) and w3NoWords:
                     cList[i].realization=m1[1]+w1[:-1]+"'"+m1[3]
                     elisionFound = True
                 elif euphonieFrRE.match(w1) and  w3NoWords and cList[i].getProp("n")=="s": # euphonie
                     if re.match(r"ce",w1,re.I) and re.match(r"(^est$)|(^étai)|(^a$)",w2,re.I):
                         # very special case but very frequent
                         cList[i].realization=m1[1]+w1[:-1]+"'"+m1[3]
-                    else:
+                    elif w2 not in ["et","ou","où","aujourd'hui"]:
+                        # avoid euphonie before "et", "or" ....: e.g. "beau et fort" and not "bel et fort"
                         cList[i].realization=m1[1]+euphonieFrTable[w1]+m1[3]
                     elisionFound = True
             if elisionFound:
                 i += 1
             elif (w1+"+"+w2) in contractionFrTable and w3NoWords:
                 # try contraction
                 contr=contractionFrTable[w1+"+"+w2]
@@ -486,19 +491,23 @@
         from .Terminal import Adv,Pro,Q
         iDeb = 0
         i = iDeb
         while i < len(cList):
             c = cList[i]
             if c.isA("V") and hasattr(c, "neg2"):
                 if hasattr(c, "isMod") or hasattr(c, "isProg"):
-                    c.insertReal(cList, Q(c.neg2, "fr"), i + 1)
+                    if (c.getProp("lier")==None):
+                        c.insertReal(cList, Q(c.neg2, "fr"), i + 2)
+                    else:
+                        c.insertReal(cList, Q(c.neg2, "fr"), i + 1)
                     c.insertReal(cList, Adv("ne", "fr"), i)
                     del c.neg2  # remove negation from the original verb
                     iDeb = i + 3  # skip these in the following loop
                     if hasattr(c, "isProg"): iDeb += 2  # skip "en train","de"
+                    break
             i += 1
         # gather verb position and pronouns coming after the verb possibly adding a reflexive pronoun
         verbPos = None
         prog = None
         neg2 = None
         pros = []
         i = iDeb
@@ -523,14 +532,15 @@
                     # check for negation
                     if hasattr(c, "neg2") and c.neg2 is not None:
                         c.insertReal(pros, Adv("ne", "fr"))
                         if t == "b":
                             c.insertReal(pros, Q(c.neg2, "fr"))
                         else:
                             neg2 = c.neg2
+                            del c.neg2
                     if c.isReflexive() and c.getProp("t") != "pp":
                         if prog is not None: c = prog
                         c.insertReal(pros,
                                      Pro("moi", "fr").c("refl").pe(c.getProp("pe")).n(c.getProp("n")).g(c.getProp("g")))
                 i += 1
             elif c.isA("Pro") and verbPos is not None:
                 if c.getProp("pos") is None or (c.parentConst is not None and c.parentConst.getProp("pos") is None):
@@ -765,15 +775,16 @@
                         # taking into account any trailing HTML tag
                         m=re.search(r"(.)( |(<[^>]+>))*$",s)
                         if m is not None and m.group(1) not in "?!.:;/)]}":
                             s+=". "   # add a space after "." , like for rule "pc4"
         return s
     
     ## this looks very simple, but it is the start of the realization process
-    def realize(self) -> str:
+    def realize(self,lang=None) -> str:
+        if lang is not None:load(lang)
         terminals=self.real()
         return self.detokenize(terminals)
     
     def __str__(self):
         ## in Javascript, the realization is implicit with .toString(),
         ## so in Python, it should be also implicit with str(), but
         ## the Python debugger in PyCharm also uses str() to display information
@@ -854,15 +865,15 @@
 # shared properties 
 #   pe,n and g : can be applied to components of NP and Sentences
 setattr(Constituent,"pe",makeOptionMethod("pe",[1,2,3,'1','2','3'],["D","Pro","N","NP","A","AP","V","VP","S","SP","CP"]))
 setattr(Constituent,"n",makeOptionMethod("n",["s","p","x"],["D","Pro","N","NP","A","AP","V","VP","S","SP","CP"]))
 setattr(Constituent,"g",makeOptionMethod("g",["m","f","n","x"],["D","Pro","N","NP","A","AP","V","VP","S","SP","CP"]))
 #  t, aux : can be applied to VP and sentence
 setattr(Constituent,"t",makeOptionMethod("t",["p", "i", "f", "ps", "c", "s", "si", "ip", "pr", "pp", "b","b-to", # simple tenses
-                   "pc", "pq", "cp", "pa", "fa", "spa", "spq","bp"],["V","VP","S","SP","CP"]))  # compound tenses
+                   "pc", "pq", "cp", "pa", "fa", "spa", "spq","bp","bp-to"],["V","VP","S","SP","CP"]))  # compound tenses
 setattr(Constituent,"aux",makeOptionMethod("aux",["av","êt","aê"],["V","VP","S","SP","CP"]))
 # ordinary properties
 setattr(Constituent,"f",makeOptionMethod("f",["co","su"],["A","Adv"]))
 setattr(Constituent,"tn",makeOptionMethod("tn",["","refl"],["Pro"]))
 setattr(Constituent,"c",makeOptionMethod("c",["nom","acc","dat","refl","gen"],["Pro"]))
 
 setattr(Constituent,"pos",makeOptionMethod("pos",["post","pre"],["A","Adv",*deprels]))
```

### Comparing `pyrealb-2.3.3/src/pyrealb/Dependent.py` & `pyrealb-2.3.4/src/pyrealb/Dependent.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,20 +128,21 @@
             deprel=dep.constType
             if deprel=="subj":
                 if headTerm.isA("V"):
                     headTerm.peng=dep.peng
             elif deprel=="det":
                 if depTerm.isA("D"):
                     if hasattr(self,"peng"):
-                        if hasattr(depTerm,"peng") and "pe" in depTerm.peng: # save person (for possessives)
-                            pe=depTerm.peng["pe"]
-                            depTerm.peng=self.peng
-                            depTerm.peng["pe"]=pe
-                        else: #some strange determiner construct do not have peng
-                            depTerm.peng=self.peng
+                    #     if hasattr(depTerm,"peng") and "pe" in depTerm.peng: # save person (for possessives)
+                    #         pe=depTerm.peng["pe"]
+                    #         depTerm.peng=self.peng
+                    #         depTerm.peng["pe"]=pe
+                    #     else: #some strange determiner construct do not have peng
+                    #         depTerm.peng=self.peng
+                        depTerm.peng=self.peng
                 elif depTerm.isA("NO"):
                     depTerm.peng=headTerm.peng
                 elif depTerm.isA("P") and depTerm.lemma == "de":  # HACK: deal with specific case : det(P("de"),mod(D(...)))
                     if len(dep.dependents)==1 and dep.dependents[0].isA("mod") and dep.dependents[0].isA("D"):
                         dep.dependents[0].terminal.peng = self.peng
             elif deprel=="mod" or deprel=="comp":
                 if depTerm.isA("A") or (depTerm.isA("V") and depTerm.getProp("t")=="pp"):
@@ -172,15 +173,16 @@
                     if self.isFr() and depTerm.getProp("t")=="pp":
                         depTerm.peng=self.peng
                 elif depTerm.isA("Pro") and depTerm.lemma in ["qui","que","who","that"]:
                     # a relative linked to depTerm in which the new peng should be propagated
                     if hasattr(self,"peng"):
                         depTerm.peng=self.peng
                     for depI in dep.dependents:
-                        self.setPengRecursive(depI,depI.peng["pengNO"],self.peng)
+                        if hasattr(depI,"peng"):
+                            self.setPengRecursive(depI,depI.peng["pengNO"],self.peng)
             elif deprel=="root":
                 # self.error("An internal root was found")
                 pass
             elif deprel=="coord":
                 if len(dep.dependents)>0:
                     firstDep=dep.dependents[0]
                     if firstDep.isA("subj"):
@@ -290,16 +292,26 @@
         subj=None # original subject and object, they are swapped below...
         obj=None
         # find the subject
         if self.terminal.isA("V"):
             subjIdx=self.findIndex(lambda d:d.isA("subj"))
             if subjIdx>=0:
                 subj=self.dependents[subjIdx]
-                if subj.terminal.isA("Pro"):
-                    subj.terminal = subj.terminal.getTonicPro()
+                # if subj.terminal.isA("Pro"):
+                #     subj.terminal = subj.terminal.getTonicPro()
+                subject = subj.terminal
+                if subject.isA("Pro"):
+                    if self.isEn() and subject.lemma=="I":
+                        subj.terminal = Pro("me").tn("").g(subject.getProp("g"))\
+                                         .n(subject.getProp("n")).pe(subject.getProp("pe"))
+                    elif self.isFr() and subject.lemma=="je":
+                        subj.terminal = Pro("moi").tn("").g(subject.getProp("g"))\
+                                         .n(subject.getProp("n")).pe(subject.getProp("pe"))
+                    else:
+                        subj.terminal=subject.getTonicPro()
             else:
                 subj=None
             # find direct object (first N or Pro of a comp) from dependents
             objIdx=self.findIndex(lambda d: d.isA("comp") and d.terminal.isOneOf(["N","Pro"]))
             if objIdx>=0:
                 obj=self.dependents[objIdx]
                 if obj.terminal.isA("Pro"):
@@ -336,15 +348,14 @@
                 self.addDependent(comp(P(prep,self.lang),subj))
             if self.isFr():
                 # do self only for French because in English self is done by processTyp_en
                 # change verbe into an "être" auxiliary and make it agree with the newSubj
                 # force person to be 3rd (number and tense will come from the new subject)
                 verbe=self.terminal.lemma
                 self.terminal.setLemma("avoir" if verbe == "être" else "être")
-                self.terminal.pe(3)
                 if self.getProp("t")=="ip":
                     self.t("s") # set subjonctive present tense for an imperative
                 pp = V(verbe,"fr").t("pp")
                 if obj is not None: # self can be undefined when a subject is Q or missing
                     self.terminal.peng=obj.peng
                     pp.peng=obj.peng
                 # insert the pp before the comp, so that it appears immediately after the verb
@@ -439,25 +450,29 @@
             if subjIdx>=0:
                 self.dependents[subjIdx].pos("post")
 
     def invertSubject(self):
         # in French : use inversion rule which is quite "delicate"
         # rules from https:#francais.lingolia.com/fr/grammaire/la-phrase/la-phrase-interrogative
         # if subject is a pronoun, invert and add "-t-" or "-"
+        # except for first person singular ("je") which is most often non colloquial (e.g. aime-je or prends-je)
         # if subject is a noun, the subject stays but add a new pronoun
         subjIdx = self.findIndex(lambda d: d.isA("subj"))
         if subjIdx >= 0:
-            subj = self.dependents[subjIdx].terminal
-            if subj.isA("Pro"):
+            subject = self.dependents[subjIdx].terminal
+            if subject.isA("Pro"):
+                if subject.getProp("pe")==1 and subject.getProp("n")=="s": # add est-ce que at the start
+                    self.add(det(Q("est-ce que")),0)
+                    return
                 pro = self.removeDependent(subjIdx).terminal  # remove subject
-            elif subj.isA("C"):
+            elif subject.isA("C"):
                 pro = Pro("moi", "fr").c("nom").g("m").n("p").pe(3)  # create a "standard" pronoun, to be patched by cpReal
-                subj.pronoun = pro  # add a flag to be processed by cpReal
+                subject.pronoun = pro  # add a flag to be processed by cpReal
             else:
-                pro = Pro("moi", "fr").g(subj.getProp("g")).n(subj.getProp("n")).pe(3).c("nom")  # create a pronoun
+                pro = Pro("moi", "fr").g(subject.getProp("g")).n(subject.getProp("n")).pe(3).c("nom")  # create a pronoun
             if self.terminal.isA("V"):
                 self.addPost(pro)
                 self.terminal.lier()
 
     def processTypInt(self,types):
         int_=types["int"]
         sentenceTypeInt = getRules()["sentence_type"]["int"]
@@ -566,14 +581,15 @@
                             pro=Pro("I").n("p") # they
                             if subject.lemma=="nobody":neg=True
                         else:
                             pro=subject.clone()
                         pro=subj(pro).pos("post")
                     elif subject.isA("N"):
                         pro = self.dependents[subjIdx].clone().pro().pos("post")
+                        pro.g(subject.getProp("g")).n(subject.getProp("n")) # ensure proper number and gender
                     else:
                         # must wrap into comp("",...) to force pronominalization of children
                         pro=subj(Pro("it").c("nom")).pos("post")
                 else:  #  no subject, but check if the verb is imperative
                     if t == "ip":
                         if aux == "do": aux = "will" # change aux when the aux is default
                         pro = Pro("I").pe(2).n(n).g(g)
```

### Comparing `pyrealb-2.3.3/src/pyrealb/Lexicon.py` & `pyrealb-2.3.4/src/pyrealb/Lexicon.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,21 @@
     __lexicon.lang="en"
     if trace: print("English lexicon and rules loaded",file=sys.stderr)
 
 def loadFr(trace=False):
     __lexicon.lang="fr"
     if trace: print("Règles et lexique français chargés",file=sys.stderr)
 
+def load(lang,trace=False):
+    from .Terminal import Q
+    if lang=="en": loadEn(trace)
+    elif lang=="fr": loadFr(trace)
+    else:
+        Q(lang).warn("bad language",lang)
+
 # add to lexicon and return the updated object
 #     to remove from lexicon (give None as newInfos)
 def addToLexicon(lemma,newInfos=None,lang=None):
     lexicon=getLexicon(lang)
     if isinstance(lemma,dict): # convenient when called with a single JSON object as shown in the IDE
         item=list(lemma.items())[0]
         newInfos=item[1]
```

### Comparing `pyrealb-2.3.3/src/pyrealb/Number.py` & `pyrealb-2.3.4/src/pyrealb/Number.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.3/src/pyrealb/Phrase.py` & `pyrealb-2.3.4/src/pyrealb/Phrase.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,15 +453,22 @@
             vp = self
         else:
             vp = self.getConst("VP")
             if vp is not None:
                 if len(self.elements) > 0 and self.elements[0].isOneOf(["N", "NP", "Pro","S"]):
                     subject = self.removeElement(0)
                     if subject.isA("Pro"):
-                         subject = subject.getTonicPro()
+                        if self.isEn() and subject.lemma == "I":
+                            subject = Pro("me").tn("").g(subject.getProp("g")) \
+                                .n(subject.getProp("n")).pe(subject.getProp("pe"))
+                        elif self.isFr() and subject.lemma == "je":
+                            subject = Pro("moi").tn("").g(subject.getProp("g")) \
+                                .n(subject.getProp("n")).pe(subject.getProp("pe"))
+                        else:
+                            subject = subject.getTonicPro()
                 else:
                     subject = None
             else:
                 return self.warn("not found", "VP", "contexte passif" if self.isFr() else "passive context")
         # remove object (first NP or Pro within VP) from elements
         newSubject = None
         if vp is not None:
@@ -510,15 +517,14 @@
                 verbe = vp.removeElement(verbeIdx)
                 aux = V("avoir" if verbe.lemma == "être" else "être", "fr")
                 aux.parentConst = vp
                 aux.taux = verbe.taux
                 if newSubject is not None:  # this can happen when a subject is Q
                     aux.peng = newSubject.peng
                 aux.props = verbe.props
-                aux.pe(3)  # force person to be 3rd (number and tense will come from the pyrealb subject)
                 if vp.getProp("t") == "ip":
                     aux.t("s")  # set subjonctive present tense for an imperative
                 pp = V(verbe.lemma, "fr").t("pp")
                 if newSubject is not None:  # self can happen when a subject is Q
                     # make the past participle agree with the new subject
                     pp.setProp("g",newSubject.getProp("g"))
                     pp.setProp("n",newSubject.getProp("n"))
@@ -652,17 +658,17 @@
         auxils.append(v.lemma)
         # realise the first verb, modal or auxiliary
         # but make the difference between "have" as an auxiliary and "have" as a verb
         vAux = auxils.pop(0)
         words = []
         # conjugate the first verb
         if neg:  # negate the first verb
-            if t in ["pp","pr","b-to","b"]:  # special case for these tenses
+            if t in ["pp","pr","b-to","b","bp","bp-to"]:  # special case for these tenses
                 words.append(Adv("not", "en"))
-                if t == "b" : words.append(P("to","en"))
+                if t == "b" or t=="bp" : words.append(P("to","en"))
                 words.append(V(vAux, "en").t(t))
             elif t == "ip" and v_peng["pe"] == 1 and v_peng["n"]=="p":
                 # very special case: insert "not" between "let's" and verb
                 words.append(Q("let's"))
                 words.append(Adv("not","en"))
                 words.append(V(vAux,"en").t("b"))
             elif vAux in negMod:
@@ -733,31 +739,31 @@
         # in English move the auxiliary to the front 
         if self.isEn():
             if self.isOneOf(["S", "SP"]):
                 (idx, vpElems) = self.getIdxCtx("VP", "V")
                 if idx is not None and self.getProp("t") not in ["pp","pr","b-to"]:
                     # do not move when tense is participle or infinitive
                     v = vpElems.pop(0)  # remove first V
-                    # check if V is followed by a negation, if so move it also
-                    if len(vpElems) > 0 and vpElems[0].isA("Adv") and vpElems[0].lemma == "not":
-                        not_ = vpElems[0].parentConst.removeElement(0)
-                        self.addElement(v, 0).addElement(not_, 1)
-                    else:
-                        self.addElement(v, 0)
+                    self.addElement(v, 0)
 
     def invertSubject(self):
         # in French : use inversion rule which is quite "delicate"
         # rules from https:#francais.lingolia.com/fr/grammaire/la-phrase/la-phrase-interrogative
         # if subject is a pronoun, invert and add "-t-" or "-"
+        # except for first person singular ("je") which is most often non colloquial (e.g. aime-je or prends-je)
         # if subject is a noun, the subject stays but add a pyrealb pronoun
         subjIdx = self.getIndex(["NP", "N", "Pro", "SP", "CP"])
         if subjIdx >= 0:
             subj = self.elements[subjIdx]
             if subj.isA("Pro"):
-                pro = self.removeElement(subjIdx)  # remove subject pronoun
+                if subj.getProp("pe")==1 and subj.getProp("n")=="s": # add "est-ce que" at the start
+                    self.add(Q("est-ce que"),subjIdx)
+                    return
+                else:
+                    pro = self.removeElement(subjIdx)  # remove subject pronoun
             elif subj.isA("CP"):
                 pro = Pro("moi", "fr").c("nom").g("m").n("p").pe(
                     3)  # create a "standard" pronoun, to be patched by cpReal
                 subj.pronoun = pro  # add a flag to be processed by cpReal
             else:
                 pro = Pro("moi", "fr").g(subj.getProp("g")).n(subj.getProp("n")).pe(3).c("nom")  # create a pronoun
             (idx, vpElems) = self.getIdxCtx("VP", "V")
@@ -987,15 +993,15 @@
                     r = e.cpReal()
                 # TODO: is it worth the trouble ?
                 # elif e.isA("VP") and reorderVPcomplements:
                 #     r=e.vpReal()
                 else:
                     r = e.real()
                 res.extend(r)
-            if self.isA("VP"):
+            if self.isA("VP") and len(res) > 1:
                 self.checkAdverbPos(res)
         return self.doFormat(res)
 
     # recreate a jsRealB expression
     # if indent is >=0 create an indented pretty-print (call it with 0 at the root)
     def toSource(self, indent=-1):
         if indent >= 0:
```

### Comparing `pyrealb-2.3.3/src/pyrealb/Terminal.py` & `pyrealb-2.3.4/src/pyrealb/Terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
                 if isinstance(lemma,str):
                     self.date=self.parseDateString(lemma)
                 elif isinstance(lemma,datetime.datetime):
                     self.date=lemma
                 else:
                     self.warn("bad parameter","str,datetime.datetime",type(lemma).__name__)
                     self.date=datetime.datetime.today()                   
-            self.lemma=str(self.date)
             ## set defaults
             self.props["dOpt"]={"year":True,"month":True,"date":True,"day":True,
                         "hour":True,"minute":True,"second":True,
                         "nat":True,"det":True,"rtime":False}
         elif terminalType=="NO":
             if not isinstance(lemma,(str,int,float)):
                 self.warn("bad parameter",["str","int","float"],type(lemma).__name__)
@@ -523,14 +522,22 @@
                 return [self]
         elif t == "f":
             self.realization=self.lemma
             self.insertReal(res,V("will"),0)
         elif t == "c":
             self.realization=self.lemma
             self.insertReal(res,V("will").t("ps"),0)
+        elif t=="bp" or t=="bp-to":
+            if t in conjugationTable and "pp" in conjugationTable.t:
+                self.realization = self.stem+conjugationTable.t["pp"]
+            else:
+                self.realization = self.lemma
+            self.insertReal(res,V("have").t("b"),0)
+            if t=="bp-to":
+                self.insertReal(res,P("to"),0)
         elif t == "b-to":
             self.realization = self.lemma
             self.insertReal(res,P("to"),0)
         elif t == "ip":
             self.realization=self.lemma
             if pe == 1 and n == "p":
                 self.insertReal(res,Q("let's"),0)
```

### Comparing `pyrealb-2.3.3/src/pyrealb/Warning.py` & `pyrealb-2.3.4/src/pyrealb/Warning.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.3/src/pyrealb/__init__.py` & `pyrealb-2.3.4/src/pyrealb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 from pyrealb.utils import *
 from pyrealb.Warning import *
 
 __all__ = ['Constituent',
      'A', 'Adv', 'C', 'D', 'DT', 'N', 'NO', 'P', 'Pro', 'Q', 'V', 'Terminal',           # from Terminal
      'AP',  'AdvP',  'CP', 'NP', 'PP',  'VP', 'S', 'SP', 'Phrase',                      # from Phrase
      'root', 'subj', 'det', 'mod', 'comp', 'compObj', 'compObl', 'coord', 'Dependent',  # from Dependent
-     'currentLanguage', 'addToLexicon', 'getLemma', 'loadEn', 'loadFr',                 # from Lexicon
+     'currentLanguage', 'addToLexicon', 'getLemma', 'loadEn', 'loadFr', 'load',          # from Lexicon
      'fromJSON', 'oneOf', 'false', 'true', 'null', 'pyrealb_version',                   # from utils
      'pyrealb_datecreated',
      'test_warnings'                                                                    # from Warning
  ]
```

### Comparing `pyrealb-2.3.3/src/pyrealb/data/lexicon-en.json` & `pyrealb-2.3.4/src/pyrealb/data/lexicon-en.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.3/src/pyrealb/data/lexicon-fr.json` & `pyrealb-2.3.4/src/pyrealb/data/lexicon-fr.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999976215845955%*

 * *Differences: {"'certain'": "{'D': OrderedDict([('tab', 'n28')])}"}*

```diff
@@ -54361,14 +54361,17 @@
     "certain": {
         "A": {
             "tab": "n28"
         },
         "Adv": {
             "tab": "av"
         },
+        "D": {
+            "tab": "n28"
+        },
         "basic": true
     },
     "certainement": {
         "Adv": {
             "tab": "av"
         },
         "basic": true
```

### Comparing `pyrealb-2.3.3/src/pyrealb/data/pyrealb.egg-info/PKG-INFO` & `pyrealb-2.3.4/src/pyrealb/data/pyrealb.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.3/src/pyrealb/data/rules-en.json` & `pyrealb-2.3.4/src/pyrealb/data/rules-en.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999919871794872%*

 * *Differences: {"'conjugation'": "{'v57': {'t': {'pp': 'n'}}, 'v90': {'t': {'ps': 'owed', 'pp': 'own'}}}"}*

```diff
@@ -2218,15 +2218,15 @@
                     "",
                     "",
                     "s",
                     "",
                     "",
                     ""
                 ],
-                "pp": "ed",
+                "pp": "n",
                 "pr": "ing",
                 "ps": "ed"
             }
         },
         "v58": {
             "ending": "",
             "t": {
@@ -2816,17 +2816,17 @@
                     "ow",
                     "ow",
                     "ows",
                     "ow",
                     "ow",
                     "ow"
                 ],
-                "pp": "owed",
+                "pp": "own",
                 "pr": "owing",
-                "ps": "ew"
+                "ps": "owed"
             }
         },
         "v91": {
             "ending": "ow",
             "t": {
                 "b": "ow",
                 "p": [
```

### Comparing `pyrealb-2.3.3/src/pyrealb/data/rules-fr.json` & `pyrealb-2.3.4/src/pyrealb/data/rules-fr.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.3/src/pyrealb/utils.py` & `pyrealb-2.3.4/src/pyrealb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,9 +71,9 @@
 
 # useful variables for using expressions written originally for the javascript version
 false = False
 true = True
 null = None
 
 # version and date informations
-pyrealb_version = "2.3.3"
+pyrealb_version = "2.3.4"
 pyrealb_datecreated = datetime.datetime.today()
```

### Comparing `pyrealb-2.3.3/src/pyrealb.egg-info/PKG-INFO` & `pyrealb-2.3.4/src/pyrealb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrealb
-Version: 2.3.3
+Version: 2.3.4
 Summary: A French-English text realizer
 Home-page: https://github.com/lapalme/pyrealb
 Author: Guy Lapalme
 Author-email: lapalme@iro.umontreal.ca
 Project-URL: Bug Tracker, https://github.com/lapalme/pyrealb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.3 - March 2023*
+*Version 2.3.4 - May 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
 
@@ -119,15 +119,15 @@
 ## For the maintainer mainly
 ### Updating package version on PyPI 
 
 see [this tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
 
 These steps take for granted that the password for PyPI has already been given...
 
-1. update version number in `setup.cfg` (it should be the same as `python_version` in `src/pyrealb/utils.py`)
+1. update version number in `setup.cfg` (it should be the same as `python_version` in `src/pyrealb/utils.py` and at the beginning of this document)
 2. `cd` into the directory with the `pyproject.toml` file (the same as this `README.md`)
 3. Build the distribution package  
        `python3 -m build`
 4. Upload to PyPi the last version I.J.K
       `twine upload dist/*-I.J.K.*`
 5. Install new version from PyPI  
     `python3 -m pip install pyrealb --upgrade`
```

### Comparing `pyrealb-2.3.3/src/pyrealb.egg-info/SOURCES.txt` & `pyrealb-2.3.4/src/pyrealb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.3/tests/test.py` & `pyrealb-2.3.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.3/tests/testAll.py` & `pyrealb-2.3.4/tests/testAll.py`

 * *Files identical despite different names*

