# Comparing `tmp/PrimeBotFramework-1.0.12.tar.gz` & `tmp/PrimeBotFramework-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-ceqp5mot/PrimeBotFramework-1.0.12.tar", last modified: Tue May 23 18:21:57 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-o214huiw/PrimeBotFramework-1.0.14.tar", last modified: Wed May 24 13:25:17 2023, max compression
```

## Comparing `PrimeBotFramework-1.0.12.tar` & `PrimeBotFramework-1.0.14.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/.pypirc
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/CHANGELOG.txt
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6609 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    26928 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/Pipfile.lock
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/B2E/
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/B2E/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/D4Sign/
--rw-rw-rw-   0 root         (0) root         (0)     2600 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/D4Sign/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0 root         (0) root         (0)     2822 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/Documents/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/Elastic/
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0 root         (0) root         (0)     8987 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/IntegracaoSendGrid/
--rw-rw-rw-   0 root         (0) root         (0)     4251 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/IntegracaoSendGrid/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.671050 PrimeBotFramework-1.0.12/PrimeBot/ListenerECS/
--rw-rw-rw-   0 root         (0) root         (0)     4096 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/ListenerECS/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PrimeBot/Mongo/
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PrimeBot/OracleDB/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/OracleDB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PrimeBot/Vault/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/PrimeBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6609 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      817 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-23 18:21:57.000000 PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     4332 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/README.md
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-23 18:21:57.675051 PrimeBotFramework-1.0.12/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-05-23 18:21:47.000000 PrimeBotFramework-1.0.12/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.949772 PrimeBotFramework-1.0.14/
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/.pypirc
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.949772 PrimeBotFramework-1.0.14/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/CHANGELOG.txt
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6609 2023-05-24 13:25:17.957772 PrimeBotFramework-1.0.14/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    26928 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/Pipfile.lock
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/CNAB/
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/CNAB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-24 13:25:17.953771 PrimeBotFramework-1.0.14/PrimeBotFramework.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6609 2023-05-24 13:25:17.000000 PrimeBotFramework-1.0.14/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-05-24 13:25:17.000000 PrimeBotFramework-1.0.14/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-24 13:25:17.000000 PrimeBotFramework-1.0.14/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-24 13:25:17.000000 PrimeBotFramework-1.0.14/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-24 13:25:17.000000 PrimeBotFramework-1.0.14/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4332 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-24 13:25:17.957772 PrimeBotFramework-1.0.14/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-05-24 13:25:08.000000 PrimeBotFramework-1.0.14/setup.py
```

### Comparing `PrimeBotFramework-1.0.12/.gitignore` & `PrimeBotFramework-1.0.14/.gitignore`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/CHANGELOG.txt` & `PrimeBotFramework-1.0.14/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PKG-INFO` & `PrimeBotFramework-1.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.12
+Version: 1.0.14
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.12/Pipfile.lock` & `PrimeBotFramework-1.0.14/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/B2E/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/B2E/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/CpfCnpj/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/CpfCnpj/api_codes.py` & `PrimeBotFramework-1.0.14/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/D4Sign/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/D4Sign/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/DeathByCaptcha/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/DeathByCaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/Documents/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/Elastic/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/ExchangeGraph/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/IntegracaoSendGrid/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/IntegracaoSendGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/ListenerECS/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/ListenerECS/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/OracleDB/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/OracleDB/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBot/Vault/__init__.py` & `PrimeBotFramework-1.0.14/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/PKG-INFO` & `PrimeBotFramework-1.0.14/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.12
+Version: 1.0.14
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.12/PrimeBotFramework.egg-info/SOURCES.txt` & `PrimeBotFramework-1.0.14/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 bitbucket-pipelines.yml
 requirements.txt
 setup.cfg
 setup.py
 .vscode/settings.json
 PrimeBot/__init__.py
 PrimeBot/B2E/__init__.py
+PrimeBot/CNAB/__init__.py
 PrimeBot/CpfCnpj/__init__.py
 PrimeBot/CpfCnpj/api_codes.py
 PrimeBot/CpfCnpj/model.py
 PrimeBot/D4Sign/__init__.py
 PrimeBot/DeathByCaptcha/__init__.py
 PrimeBot/Documents/__init__.py
 PrimeBot/Elastic/__init__.py
```

### Comparing `PrimeBotFramework-1.0.12/README.md` & `PrimeBotFramework-1.0.14/README.md`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/bitbucket-pipelines.yml` & `PrimeBotFramework-1.0.14/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.12/setup.py` & `PrimeBotFramework-1.0.14/setup.py`

 * *Files identical despite different names*

