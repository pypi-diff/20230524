# Comparing `tmp/mecapacktools-1.0.1.tar.gz` & `tmp/mecapacktools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecapacktools-1.0.1.tar", max compression
+gzip compressed data, was "mecapacktools-1.0.2.tar", max compression
```

## Comparing `mecapacktools-1.0.1.tar` & `mecapacktools-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.0.1/mecapacktools/__init__.py
--rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.0.1/mecapacktools/libCfg.py
--rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.0.1/mecapacktools/libLog.py
--rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.0.1/mecapacktools/libMail.py
--rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.0.1/mecapacktools/libSql.py
--rw-r--r--   0        0        0    14859 2023-05-03 07:59:47.610440 mecapacktools-1.0.1/mecapacktools/libTool.py
--rw-r--r--   0        0        0    20041 2023-05-22 08:10:44.484275 mecapacktools-1.0.1/mecapacktools/libWebServices.py
--rw-r--r--   0        0        0     1090 2023-05-22 08:46:34.874177 mecapacktools-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      668 2023-04-27 13:23:11.491614 mecapacktools-1.0.1/README.md
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 mecapacktools-1.0.1/setup.py
--rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 mecapacktools-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 mecapacktools-1.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-13 14:01:51.082497 mecapacktools-1.0.2/mecapacktools/__init__.py
+-rw-r--r--   0        0        0     6529 2023-05-03 07:55:13.913793 mecapacktools-1.0.2/mecapacktools/libCfg.py
+-rw-r--r--   0        0        0    13097 2023-05-03 08:05:32.051592 mecapacktools-1.0.2/mecapacktools/libLog.py
+-rw-r--r--   0        0        0    19660 2023-05-03 07:56:55.469052 mecapacktools-1.0.2/mecapacktools/libMail.py
+-rw-r--r--   0        0        0     8738 2023-05-11 06:01:29.168121 mecapacktools-1.0.2/mecapacktools/libSql.py
+-rw-r--r--   0        0        0    14859 2023-05-03 07:59:47.610440 mecapacktools-1.0.2/mecapacktools/libTool.py
+-rw-r--r--   0        0        0    20330 2023-05-24 07:28:15.036814 mecapacktools-1.0.2/mecapacktools/libWebServices.py
+-rw-r--r--   0        0        0     1090 2023-05-24 10:18:52.423811 mecapacktools-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      668 2023-04-27 13:23:11.491614 mecapacktools-1.0.2/README.md
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 mecapacktools-1.0.2/setup.py
+-rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 mecapacktools-1.0.2/PKG-INFO
```

### Comparing `mecapacktools-1.0.1/LICENSE` & `mecapacktools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.1/mecapacktools/libCfg.py` & `mecapacktools-1.0.2/mecapacktools/libCfg.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.1/mecapacktools/libLog.py` & `mecapacktools-1.0.2/mecapacktools/libLog.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.1/mecapacktools/libMail.py` & `mecapacktools-1.0.2/mecapacktools/libMail.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.1/mecapacktools/libSql.py` & `mecapacktools-1.0.2/mecapacktools/libSql.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.1/mecapacktools/libTool.py` & `mecapacktools-1.0.2/mecapacktools/libTool.py`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.1/mecapacktools/libWebServices.py` & `mecapacktools-1.0.2/mecapacktools/libWebServices.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,27 +269,28 @@
                 f"Response {pcode} : {resp.json()}",
             )
         self.log.setStep = ""
 
     # //////////////////////////////////////////////////
     #     Get_pj
     # //////////////////////////////////////////////////
-    def Get_pj(self, pcode, **kw):
+    def Get_pj(self, pcode, pfilename=None, **kw):
         """
         Récupère le document selon l'id
 
         Args:
             pcode (str): Sylob9 ID du document
+            pfilename (str, optional): filename to save document. "None" returns fileObject. Defaults to None.
             **piteration (int): First launch function for authentication problems(not to be changed)
             **plogrequest (LOG_LEVEL): Log level display for request. "None" for no display (default=DEBUG)
 
-        Raises:
-            Exception: No connection
-            Exception: Returned Error
+        Returns:
+            str: File Object or filename if not None
         """
+
         hshOption = {"piteration": 0, "plogrequest": "DEBUG"}
         if isinstance(kw, dict):
             hshOption.update(kw)
 
         self.log.setStep = f"R[{pcode}]"
         site = (
             self.hshParam["auth"]["address"].replace("/rest", "")
@@ -313,14 +314,20 @@
             return None
         if hshOption["plogrequest"]:
             self.log.Write(
                 self.log.LEVEL[hshOption["plogrequest"]],
                 f"Response {pcode} : {resp.content}",
             )
         self.log.setStep = ""
+        if pfilename:
+            # write to file
+            with open(pfilename, "wb") as newFile:
+                newFile.write(resp.content)
+            return pfilename
+
         return resp.content
 
     def _analyse_reponse_s9(self, reponse, CR):
         retour = {}
         if not isinstance(reponse["status"], dict):
             # Erreur
             self.log.Error(f"Erreur {reponse['status']} : {reponse['errors']}")
```

### Comparing `mecapacktools-1.0.1/pyproject.toml` & `mecapacktools-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mecapacktools"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 authors = ["Informatique Mecapack <informatique@mecapack.com>"]
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 exclude = ["mecapacktools/libExcel.py"]
```

### Comparing `mecapacktools-1.0.1/README.md` & `mecapacktools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mecapacktools-1.0.1/setup.py` & `mecapacktools-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'sql': ['pypyodbc>=1.3.6,<2.0.0'],
  'webservices': ['requests>=2.28.2,<3.0.0',
                  'suds>=1.1.2,<2.0.0',
                  'xmltodict>=0.13.0,<0.14.0']}
 
 setup_kwargs = {
     'name': 'mecapacktools',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': '',
     'long_description': '# Tools for Mecapack\n\nLa doc est disponible en Html ou en MD\n\n## installation par pip\n\n`pip install mecapacktools`\n\nInstaller les extensions :\n\n`pip install mecapacktools[excel,sql,webservices]`\n\n### Extensions diponibles :\n\n- excel \n- Sql \n- WebServices \n\n## Notes pour le développement:\n\n### Installation\n\n`poetry install --with dev --all-extras`\n\n### Génération de la doc\n\n`poetry run .\\make.bat html`\n`poetry run .\\make.bat markdown`\n\n### Publier une nouvelle version\n\nChanger la version :\nDans le fichier pyproject.toml modifier :\n```\n[tool.poetry]\nversion = "1.0.0"\n ```\n\nPublier sur pypi `poetry publish --build`\n\n\n\n',
     'author': 'Informatique Mecapack',
     'author_email': 'informatique@mecapack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mecapacktools-1.0.1/PKG-INFO` & `mecapacktools-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecapacktools
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: Informatique Mecapack
 Author-email: informatique@mecapack.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

