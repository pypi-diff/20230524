# Comparing `tmp/stlock-0.0.7.1.tar.gz` & `tmp/stlock-0.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlock-0.0.7.1.tar", last modified: Tue May 23 16:23:39 2023, max compression
+gzip compressed data, was "stlock-0.0.7.2.tar", last modified: Wed May 24 10:28:15 2023, max compression
```

## Comparing `stlock-0.0.7.1.tar` & `stlock-0.0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-23 16:23:39.451447 stlock-0.0.7.1/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5180 2023-05-23 16:23:39.451447 stlock-0.0.7.1/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5033 2023-05-23 16:21:22.000000 stlock-0.0.7.1/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-23 16:23:39.451447 stlock-0.0.7.1/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      404 2023-05-23 16:23:36.000000 stlock-0.0.7.1/setup.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-23 16:23:39.451447 stlock-0.0.7.1/stlock/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.7.1/stlock/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2138 2023-05-23 15:50:14.000000 stlock-0.0.7.1/stlock/stlock.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-23 16:23:39.451447 stlock-0.0.7.1/stlock.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5180 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.7.1/stlock.egg-info/not-zip-safe
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-23 16:23:39.000000 stlock-0.0.7.1/stlock.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-24 10:28:15.576876 stlock-0.0.7.2/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5558 2023-05-24 10:28:15.576876 stlock-0.0.7.2/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5033 2023-05-24 09:48:58.000000 stlock-0.0.7.2/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-24 10:28:15.576876 stlock-0.0.7.2/setup.cfg
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      886 2023-05-24 10:28:13.000000 stlock-0.0.7.2/setup.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-24 10:28:15.576876 stlock-0.0.7.2/stlock/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       31 2023-05-22 16:05:24.000000 stlock-0.0.7.2/stlock/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2138 2023-05-23 15:50:14.000000 stlock-0.0.7.2/stlock/stlock.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-24 10:28:15.576876 stlock-0.0.7.2/stlock.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5558 2023-05-24 10:28:15.000000 stlock-0.0.7.2/stlock.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      242 2023-05-24 10:28:15.000000 stlock-0.0.7.2/stlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-24 10:28:15.000000 stlock-0.0.7.2/stlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-22 16:50:38.000000 stlock-0.0.7.2/stlock.egg-info/not-zip-safe
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       15 2023-05-24 10:28:15.000000 stlock-0.0.7.2/stlock.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-24 10:28:15.000000 stlock-0.0.7.2/stlock.egg-info/top_level.txt
```

### Comparing `stlock-0.0.7.1/PKG-INFO` & `stlock-0.0.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: stlock
-Version: 0.0.7.1
-Summary: oauth2.0 stlock
-Author-email: office@stl.im
-Description-Content-Type: text/markdown
-
 # Библиотека Python stlock
 
 
 # Быстрый старт
 Пример с библиотекой FastAPI
 
 
@@ -24,15 +17,15 @@
 from stlock import AuthClient
 
 # создание экземпляра класса
 AC = AuthClient(
     client_id="client",  # id клиента
     client_secret="secret",  # secret клиента
     code_redirect_uri="http://localhost:8000/code",  # ссылка перенаправления запроса с кодом
-    service_endpoint="https://bba6q6chdp0eatf6n0ms.containers.yandexcloud.net",  # ссылка на сервис авторизации
+    service_endpoint="https://bbac70hrtmfdqn5drnga.containers.yandexcloud.net",  # ссылка на сервис авторизации
 )
 
 # service_endpoint="https://bba6q6chdp0eatf6n0ms.containers.yandexcloud.net"
 # dev версия проекта, очищается каждые 24 часа
 
 app = FastAPI()
 
@@ -176,8 +169,8 @@
 ```
 {
     "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ4NTg0MzgsInN1YiI6ImQ5YjBmYjE1LWJjYmQtNDNkNy1hMDdlLTAxNTIwMjBlZWI2ZiIsInJvbGUiOiJUZXN0In0.5hFJg-U6i9E9GFp0Gxsn9ME3Dy-JtqKEyZotHT7WmnAsdZeLrDBjDU20ttb5f5HMLep8SWruTOoWjlfiZuGBKg",
     "expires_in": 60,
     "refresh_token": "NTC1ZDY5YJYTZTC0MC01ZJRMLTHJZTUTY2E1MMFJMTAZNZI0",
     "token_type": "Bearer"
 }
-```
+```
```

### Comparing `stlock-0.0.7.1/README.md` & `stlock-0.0.7.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: stlock
+Version: 0.0.7.2
+Summary: oauth2.0 stlock
+Author: Smart Techno Lab
+Author-email: office@stl.im
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+
 # Библиотека Python stlock
 
 
 # Быстрый старт
 Пример с библиотекой FastAPI
 
 
@@ -17,15 +32,15 @@
 from stlock import AuthClient
 
 # создание экземпляра класса
 AC = AuthClient(
     client_id="client",  # id клиента
     client_secret="secret",  # secret клиента
     code_redirect_uri="http://localhost:8000/code",  # ссылка перенаправления запроса с кодом
-    service_endpoint="https://bba6q6chdp0eatf6n0ms.containers.yandexcloud.net",  # ссылка на сервис авторизации
+    service_endpoint="https://bbac70hrtmfdqn5drnga.containers.yandexcloud.net",  # ссылка на сервис авторизации
 )
 
 # service_endpoint="https://bba6q6chdp0eatf6n0ms.containers.yandexcloud.net"
 # dev версия проекта, очищается каждые 24 часа
 
 app = FastAPI()
 
@@ -169,8 +184,8 @@
 ```
 {
     "access_token": "eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJjbGllbnQiLCJleHAiOjE2ODQ4NTg0MzgsInN1YiI6ImQ5YjBmYjE1LWJjYmQtNDNkNy1hMDdlLTAxNTIwMjBlZWI2ZiIsInJvbGUiOiJUZXN0In0.5hFJg-U6i9E9GFp0Gxsn9ME3Dy-JtqKEyZotHT7WmnAsdZeLrDBjDU20ttb5f5HMLep8SWruTOoWjlfiZuGBKg",
     "expires_in": 60,
     "refresh_token": "NTC1ZDY5YJYTZTC0MC01ZJRMLTHJZTUTY2E1MMFJMTAZNZI0",
     "token_type": "Bearer"
 }
-```
+```
```

### Comparing `stlock-0.0.7.1/stlock/stlock.py` & `stlock-0.0.7.2/stlock/stlock.py`

 * *Files identical despite different names*

### Comparing `stlock-0.0.7.1/stlock.egg-info/PKG-INFO` & `stlock-0.0.7.2/stlock.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 Metadata-Version: 2.1
 Name: stlock
-Version: 0.0.7.1
+Version: 0.0.7.2
 Summary: oauth2.0 stlock
+Author: Smart Techno Lab
 Author-email: office@stl.im
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # Библиотека Python stlock
 
 
 # Быстрый старт
 Пример с библиотекой FastAPI
@@ -24,15 +32,15 @@
 from stlock import AuthClient
 
 # создание экземпляра класса
 AC = AuthClient(
     client_id="client",  # id клиента
     client_secret="secret",  # secret клиента
     code_redirect_uri="http://localhost:8000/code",  # ссылка перенаправления запроса с кодом
-    service_endpoint="https://bba6q6chdp0eatf6n0ms.containers.yandexcloud.net",  # ссылка на сервис авторизации
+    service_endpoint="https://bbac70hrtmfdqn5drnga.containers.yandexcloud.net",  # ссылка на сервис авторизации
 )
 
 # service_endpoint="https://bba6q6chdp0eatf6n0ms.containers.yandexcloud.net"
 # dev версия проекта, очищается каждые 24 часа
 
 app = FastAPI()
```

