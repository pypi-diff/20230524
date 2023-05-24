# Comparing `tmp/deklinacija-0.0.3.tar.gz` & `tmp/deklinacija-1.0.0.tar.gz`

## Comparing `deklinacija-0.0.3.tar` & `deklinacija-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-0.0.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 deklinacija-0.0.3/deklinacija/__init__.py
--rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 deklinacija-0.0.3/deklinacija/module.py
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 deklinacija-0.0.3/deklinacija/utils.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-0.0.3/LICENSE
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 deklinacija-0.0.3/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 deklinacija-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.0.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.0.0/deklinacija/__init__.py
+-rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 deklinacija-1.0.0/deklinacija/module.py
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 deklinacija-1.0.0/deklinacija/utils.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 deklinacija-1.0.0/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 deklinacija-1.0.0/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 deklinacija-1.0.0/PKG-INFO
```

### Comparing `deklinacija-0.0.3/.github/workflows/python-package.yml` & `deklinacija-1.0.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-0.0.3/deklinacija/module.py` & `deklinacija-1.0.0/deklinacija/module.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import deklinacija.utils as utils
 
 VOWELS = ["a", "а", "e", "е", "i", "и", "o", "о",
           "u", "у"]  # used for identifying consonants
 
-NEP_A = ["ар","ај","ађ"] # words ending with these letters aren't prone to the nepostojano a sound change, the majority of names end like this
+NEP_A = ["ар","ац","ај","ађ"] # words ending with these letters aren't prone to the nepostojano a sound change, the majority of names end like this
 
 INSTRUMENTAL_LETTERS = ["ј", "љ", "њ", "ђ", "ћ", "ч", "џ", "ш", "ж"]
-SOUND_CHANGE = {"k": "č", "g": "ž", "h": "š", }
+PALATALIZACIJA = {"k": "č", "g": "ž", "h": "š", }
 
 
 def genitiv(name, gender, latin=True):
     utils.check(name, gender, latin)
 
     name = list(name.strip())
 
@@ -138,14 +138,90 @@
         if lastChar == "e":
             name[-1] = "u"
         elif lastChar == "E":
             name[-1] = "U"
 
     return "".join(name)
 
+def vokativ(name, gender, latin=True):
+    utils.check(name, gender, latin)
+    name = name.strip()
+    nameGenitiv = list(genitiv(name,gender,latin))
+    name = list(name)
+    nameSep = utils.separateLetters(name)
+
+    if gender.lower() == "female" and name[-1].lower() != "a":
+        return "".join(name)
+    if name[-1].lower() in ["k","g","h"]:
+        if nameGenitiv[-1].islower():
+            nameGenitiv[-1] = "e"
+            if nameGenitiv[-2].lower() in PALATALIZACIJA:
+                if nameGenitiv[-2].islower():
+                    nameGenitiv[-2] = PALATALIZACIJA[nameGenitiv[-2].lower()]
+                else:
+                    nameGenitiv[-2] = PALATALIZACIJA[nameGenitiv[-2].lower()].upper()
+            return "".join(nameGenitiv)
+        else:
+            nameGenitiv[-1] = "E"
+            if nameGenitiv[-2].lower() in PALATALIZACIJA:
+                if nameGenitiv[-2].islower():
+                    nameGenitiv[-2] = PALATALIZACIJA[nameGenitiv[-2].lower()]
+                else:
+                    nameGenitiv[-2] = PALATALIZACIJA[nameGenitiv[-2].lower()].upper()
+            return "".join(nameGenitiv)
+    
+    if name[-1].lower() == "e":
+        return "".join(name)
+    
+    if name[-1].lower() == "j":
+        if nameGenitiv[-1].islower():
+            nameGenitiv[-1] = "u"
+        else:
+            nameGenitiv[-1] = "U"
+        return "".join(nameGenitiv)
+    
+    if name[-3].lower()+name[-2].lower()+name[-1].lower() == "ica":
+        if name[-1].islower():
+            name[-1] = "e"
+        else:
+            name[-1] = "E"
+        return "".join(name)
+    
+    if name[-1].lower() == "o":
+        return "".join(name)
+    
+    if name[-1].lower() == "i":
+        return "".join(name)
+    
+    if name[-1].lower() == "u":
+        return "".join(name)
+    
+    if name[-1].lower() in ["a","а"]:
+        if len(nameSep) <= 4:
+            try:
+                if utils.isLatin(name[-1]):
+                    return utils.toLatin(utils.vokativ_db[utils.toCyrillic(name)])
+                else:
+                    return utils.vokativ_db[utils.toCyrillic(name)]
+            except KeyError:
+                if name[-1].islower():
+                    name[-1] = "o"
+                else:
+                    name[-1] = "O"
+                return "".join(name)
+
+    else:
+        if name[-1].islower():
+            nameGenitiv[-1] = "e"
+        else:
+            nameGenitiv[-1] = "E"
+        return "".join(nameGenitiv)
+
+    
+    return "".join(name)
 
 def instrumental(name, gender, latin=True):
     utils.check(name, gender, latin)
     name = name.strip()
     
     lastChar = name[-1]
     secToLastChar = name[-2]
@@ -156,15 +232,15 @@
         if gender.lower() == "female":
             if lastChar not in VOWELS:
                 return "".join(name)
 
         nameGenitiv.pop(-1)
 
         if gender.lower() == "male" and utils.toCyrillic(nameGenitiv)[-1] in INSTRUMENTAL_LETTERS:
-            if nameGenitiv[-2].lower() == "e":
+            if nameGenitiv[-2].lower() in ["i","e"]:
                 if lastChar.isupper():
                     nameGenitiv.append("OM")
                     return "".join(nameGenitiv)
                 else:
                     nameGenitiv.append("om")
                     return "".join(nameGenitiv)
 
@@ -189,10 +265,11 @@
 
 
 def declineAll(name, gender, latin=True):
     utils.check(name, gender, latin)
     name = name.strip()
 
     allDek = {"nominativ": name, "genitiv": genitiv(name, gender, latin), "dativ": dativ(name, gender, latin), "akuzativ": akuzativ(
-        name, gender, latin), "instrumental": instrumental(name, gender, latin), "lokativ": lokativ(name, gender, latin)}
+        name, gender, latin), "vokativ": vokativ(name, gender, latin), "instrumental": instrumental(name, gender, latin), "lokativ": lokativ(name, gender, latin)}
 
     return allDek
+
```

### Comparing `deklinacija-0.0.3/LICENSE` & `deklinacija-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-0.0.3/README.md` & `deklinacija-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # deklinacija
 A Python library for declension of personal names in Serbian. The  grammatical rules utlized in this library also apply to Croatian and Bosnian.
 
 ## Installation
 The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
 
-The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/).
+The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/)
 ```properties
 pip install deklinacija
 ```
 ## Usage
 Simply `import` the package. It is recommended to set the alias to `dek`.
 
 ```python
@@ -16,34 +16,40 @@
 ```
 **As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. There is also the third `latin` parameter, which indicates whether the provided `name` parameter is written in the Cyrillic or Latin script. **Currently, only the Latin script is supported.**
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
 
-changedName1 = dek.genitiv("Velja","male") #Velje
-changedName2 = dek.dativ("Petar","male") #Petru
-changedName3 = dek.akuzativ("Jana","female") #Janu
-changedName4 = dek.instrumental("Uroš","male") #Urošem
-changedName5 = dek.instrumental("Vuk","male") #Vukom
-changedName6 = dek.lokativ("Lana","female") #Lani
-
-print("Dobili ste zahtev za prijateljstvo od",changedName1) #Dobili ste zahtev za prijateljstvo od Velje - Translation: You have received a friend request from Velja
+genitiv = dek.genitiv("Velja","male") #Velje
+dativ = dek.dativ("Petar","male") #Petru
+akuzativ = dek.akuzativ("Jana","female") #Janu
+vokativ = dek.vokativ("Predrag","male") #Predraže
+instrumental = dek.instrumental("Uroš","male") #Urošem
+instrumental2 = dek.instrumental("Vuk","male") #Vukom
+lokativ = dek.lokativ("Lana","female") #Lani
+
+print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv}.") 
+#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje.
+#Translation: Hello Predrag! You have received a friend request from Velja.
 ```
 
 You can also immediatelly decline a name through all grammatical cases by calling the `declineAll()` function.
 
 The `declineAll()` function returns a `dictionary`.
 
 ```python
 import deklinacija as dek
 
-Nikola = dek.declineAll("Nikola","male") #{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
-
-print("Dali ste poklon",Nikola['dativ']) #Dali ste poklon Nikoli - Translation: You have given a gift to Nikola
+Nikola = dek.declineAll("Nikola","male") 
+#{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 
+#'vokativ':'Nikola', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
+
+print("Dali ste poklon",Nikola['dativ']) 
+#Dali ste poklon Nikoli
+#Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
-- The vocative case
 - Support for both Latin and Cyrillic scripts
 - Declension of last names
```

### Comparing `deklinacija-0.0.3/pyproject.toml` & `deklinacija-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "0.0.3"
+version = "1.0.0"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-0.0.3/PKG-INFO` & `deklinacija-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 0.0.3
+Version: 1.0.0
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 
 # deklinacija
 A Python library for declension of personal names in Serbian. The  grammatical rules utlized in this library also apply to Croatian and Bosnian.
 
 ## Installation
 The source code is currently hosted on GitHub: [https://github.com/urelja/deklinacija](https://github.com/urelja/deklinacija)
 
-The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/).
+The latest binary versions are hosted on the Python Package Index (PyPI): [https://pypi.org/project/deklinacija/](https://pypi.org/project/deklinacija/)
 ```properties
 pip install deklinacija
 ```
 ## Usage
 Simply `import` the package. It is recommended to set the alias to `dek`.
 
 ```python
@@ -30,34 +30,40 @@
 ```
 **As of right now, only first names are supported.** To decline names, all you have to do is to call the appropriate function for the grammatical case you want to use, and specify the `name` and the `gender` parameter. There is also the third `latin` parameter, which indicates whether the provided `name` parameter is written in the Cyrillic or Latin script. **Currently, only the Latin script is supported.**
 
 The functions in this example return a `string`.
 ```python
 import deklinacija as dek
 
-changedName1 = dek.genitiv("Velja","male") #Velje
-changedName2 = dek.dativ("Petar","male") #Petru
-changedName3 = dek.akuzativ("Jana","female") #Janu
-changedName4 = dek.instrumental("Uroš","male") #Urošem
-changedName5 = dek.instrumental("Vuk","male") #Vukom
-changedName6 = dek.lokativ("Lana","female") #Lani
-
-print("Dobili ste zahtev za prijateljstvo od",changedName1) #Dobili ste zahtev za prijateljstvo od Velje - Translation: You have received a friend request from Velja
+genitiv = dek.genitiv("Velja","male") #Velje
+dativ = dek.dativ("Petar","male") #Petru
+akuzativ = dek.akuzativ("Jana","female") #Janu
+vokativ = dek.vokativ("Predrag","male") #Predraže
+instrumental = dek.instrumental("Uroš","male") #Urošem
+instrumental2 = dek.instrumental("Vuk","male") #Vukom
+lokativ = dek.lokativ("Lana","female") #Lani
+
+print(f"Zdravo, {vokativ}! Dobio si zahtev za prijateljstvo od {genitiv}.") 
+#Zdravo Predraže! Dobio si zahtev za prijateljstvo od Velje.
+#Translation: Hello Predrag! You have received a friend request from Velja.
 ```
 
 You can also immediatelly decline a name through all grammatical cases by calling the `declineAll()` function.
 
 The `declineAll()` function returns a `dictionary`.
 
 ```python
 import deklinacija as dek
 
-Nikola = dek.declineAll("Nikola","male") #{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
-
-print("Dali ste poklon",Nikola['dativ']) #Dali ste poklon Nikoli - Translation: You have given a gift to Nikola
+Nikola = dek.declineAll("Nikola","male") 
+#{'nominativ': 'Nikola', 'genitiv': 'Nikole', 'dativ': 'Nikoli', 'akuzativ': 'Nikolu', 
+#'vokativ':'Nikola', 'instrumental': 'Nikolom', 'lokativ': 'Nikoli'}
+
+print("Dali ste poklon",Nikola['dativ']) 
+#Dali ste poklon Nikoli
+#Translation: You have given a gift to Nikola
 ```
 
 ## Todo
 The following features are on the roadmap:
-- The vocative case
 - Support for both Latin and Cyrillic scripts
 - Declension of last names
```

