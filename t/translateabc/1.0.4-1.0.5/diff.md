# Comparing `tmp/translateabc-1.0.4.tar.gz` & `tmp/translateabc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translateabc-1.0.4.tar", last modified: Tue May 23 12:49:35 2023, max compression
+gzip compressed data, was "translateabc-1.0.5.tar", last modified: Tue May 23 15:37:00 2023, max compression
```

## Comparing `translateabc-1.0.4.tar` & `translateabc-1.0.5.tar`

### file list

```diff
@@ -1,89 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.253058 translateabc-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.207870 translateabc-1.0.4/.idea/
--rw-rw-rw-   0        0        0      184 2023-05-23 11:40:39.000000 translateabc-1.0.4/.idea/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.209371 translateabc-1.0.4/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      174 2023-05-23 11:40:38.000000 translateabc-1.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      182 2023-05-23 11:48:08.000000 translateabc-1.0.4/.idea/misc.xml
--rw-rw-rw-   0        0        0      283 2023-05-23 11:40:38.000000 translateabc-1.0.4/.idea/modules.xml
--rw-rw-rw-   0        0        0      318 2023-05-23 11:48:08.000000 translateabc-1.0.4/.idea/translateabc.iml
--rw-rw-rw-   0        0        0     4010 2023-05-23 12:49:33.000000 translateabc-1.0.4/.idea/workspace.xml
--rw-rw-rw-   0        0        0        0 2023-05-23 11:45:45.000000 translateabc-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-23 12:30:23.000000 translateabc-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      491 2023-05-23 12:49:35.252557 translateabc-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-23 11:45:51.000000 translateabc-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.212406 translateabc-1.0.4/dist/
--rw-rw-rw-   0        0        0   934425 2023-05-23 12:49:25.000000 translateabc-1.0.4/dist/translateabc-1.0.3.tar.gz
--rw-rw-rw-   0        0        0   532260 2023-05-23 12:49:26.000000 translateabc-1.0.4/dist/translateabc-1.0.3.win-amd64.zip
--rw-rw-rw-   0        0        0       88 2023-05-23 11:45:30.000000 translateabc-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 12:49:35.253058 translateabc-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-23 12:49:33.000000 translateabc-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.183767 translateabc-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.215908 translateabc-1.0.4/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.186301 translateabc-1.0.4/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.185300 translateabc-1.0.4/src/translateabc/READMEhh/ai35/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.227948 translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/
--rw-rw-rw-   0        0        0     2469 2023-05-22 14:26:06.000000 translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/1.ipynb
--rw-rw-rw-   0        0        0     5078 2023-05-22 14:26:04.000000 translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/2.ipynb
--rw-rw-rw-   0        0        0     2661 2023-05-22 14:30:18.000000 translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/3.ipynb
--rw-rw-rw-   0        0        0    12943 2023-05-22 14:36:23.000000 translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/4.ipynb
--rw-rw-rw-   0        0        0     4965 2023-05-22 14:48:13.000000 translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/5.ipynb
--rw-rw-rw-   0        0        0     3570 2023-05-22 15:10:05.000000 translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/6.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.228948 translateabc-1.0.4/src/translateabc/READMEhh/ai35/02/
--rw-rw-rw-   0        0        0        0 2023-05-22 14:53:43.000000 translateabc-1.0.4/src/translateabc/READMEhh/ai35/02/01.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.235491 translateabc-1.0.4/src/translateabc/READMEhh/moni/
--rw-rw-rw-   0        0        0  4928289 2022-08-06 03:19:14.000000 translateabc-1.0.4/src/translateabc/READMEhh/moni/bankmarketing.csv
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.4/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.241014 translateabc-1.0.4/src/translateabc/READMEhh/pandas-exercise/
--rw-rw-rw-   0        0        0      124 2023-05-22 15:56:25.000000 translateabc-1.0.4/src/translateabc/READMEhh/pandas-exercise/1.csv
--rw-rw-rw-   0        0        0     5625 2023-05-22 16:09:33.000000 translateabc-1.0.4/src/translateabc/READMEhh/pandas-exercise/1.ipynb
--rw-rw-rw-   0        0        0       53 2023-05-22 15:56:19.000000 translateabc-1.0.4/src/translateabc/READMEhh/pandas-exercise/2.csv
--rw-rw-rw-   0        0        0      167 2023-05-22 15:59:00.000000 translateabc-1.0.4/src/translateabc/READMEhh/pandas-exercise/output.csv
--rw-rw-rw-   0        0        0       74 2023-05-23 12:49:18.000000 translateabc-1.0.4/src/translateabc/__init__.py
--rw-rw-rw-   0        0        0      386 2023-05-23 11:44:03.000000 translateabc-1.0.4/src/translateabc/g.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.220416 translateabc-1.0.4/src/translateabc.egg-info/
--rw-rw-rw-   0        0        0      491 2023-05-23 12:49:35.000000 translateabc-1.0.4/src/translateabc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2023-05-23 12:49:35.000000 translateabc-1.0.4/src/translateabc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 12:49:35.000000 translateabc-1.0.4/src/translateabc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-23 12:49:35.000000 translateabc-1.0.4/src/translateabc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.187301 translateabc-1.0.4/translateabc-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.187301 translateabc-1.0.4/translateabc-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.187301 translateabc-1.0.4/translateabc-1.0.1/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.187802 translateabc-1.0.4/translateabc-1.0.1/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.242014 translateabc-1.0.4/translateabc-1.0.1/src/translateabc/READMEhh/moni/
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.4/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.189303 translateabc-1.0.4/translateabc-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.188803 translateabc-1.0.4/translateabc-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.188803 translateabc-1.0.4/translateabc-1.0.2/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.189303 translateabc-1.0.4/translateabc-1.0.2/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.243524 translateabc-1.0.4/translateabc-1.0.2/src/translateabc/READMEhh/moni/
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.4/translateabc-1.0.2/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.189303 translateabc-1.0.4/translateabc-1.0.2/translateabc-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.190307 translateabc-1.0.4/translateabc-1.0.2/translateabc-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.190307 translateabc-1.0.4/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.190827 translateabc-1.0.4/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.245025 translateabc-1.0.4/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.4/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.194331 translateabc-1.0.4/translateabc-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.191828 translateabc-1.0.4/translateabc-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.191828 translateabc-1.0.4/translateabc-1.0.3/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.192329 translateabc-1.0.4/translateabc-1.0.3/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.246527 translateabc-1.0.4/translateabc-1.0.3/src/translateabc/READMEhh/moni/
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.4/translateabc-1.0.3/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.192829 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.193330 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.193330 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.1/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.193830 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.1/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.248028 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.1/src/translateabc/READMEhh/moni/
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.195832 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.194831 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.194831 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.195331 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.249529 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/src/translateabc/READMEhh/moni/
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.195832 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.196332 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.196332 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.196833 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:49:35.251056 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.4/translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.896851 translateabc-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.849630 translateabc-1.0.5/.idea/
+-rw-rw-rw-   0        0        0      184 2023-05-23 11:40:39.000000 translateabc-1.0.5/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.850633 translateabc-1.0.5/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      174 2023-05-23 11:40:38.000000 translateabc-1.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      182 2023-05-23 11:48:08.000000 translateabc-1.0.5/.idea/misc.xml
+-rw-rw-rw-   0        0        0      283 2023-05-23 11:40:38.000000 translateabc-1.0.5/.idea/modules.xml
+-rw-rw-rw-   0        0        0      318 2023-05-23 11:48:08.000000 translateabc-1.0.5/.idea/translateabc.iml
+-rw-rw-rw-   0        0        0     4010 2023-05-23 15:34:44.000000 translateabc-1.0.5/.idea/workspace.xml
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:45:45.000000 translateabc-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-23 12:30:23.000000 translateabc-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      491 2023-05-23 15:37:00.896350 translateabc-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:45:51.000000 translateabc-1.0.5/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-23 11:45:30.000000 translateabc-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 15:37:00.896851 translateabc-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-23 15:34:44.000000 translateabc-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.832533 translateabc-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.853164 translateabc-1.0.5/src/translateabc/
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.835577 translateabc-1.0.5/src/translateabc/READMEhh/
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.860169 translateabc-1.0.5/src/translateabc/READMEhh/ai30/
+-rw-rw-rw-   0        0        0   181447 2023-05-23 14:32:40.000000 translateabc-1.0.5/src/translateabc/READMEhh/ai30/hcia3.0.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.861671 translateabc-1.0.5/src/translateabc/READMEhh/ai35/
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.870214 translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/
+-rw-rw-rw-   0        0        0     2469 2023-05-22 14:26:06.000000 translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/1.ipynb
+-rw-rw-rw-   0        0        0     5078 2023-05-22 14:26:04.000000 translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/2.ipynb
+-rw-rw-rw-   0        0        0     2661 2023-05-22 14:30:18.000000 translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/3.ipynb
+-rw-rw-rw-   0        0        0    12943 2023-05-22 14:36:23.000000 translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/4.ipynb
+-rw-rw-rw-   0        0        0     4965 2023-05-22 14:48:13.000000 translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/5.ipynb
+-rw-rw-rw-   0        0        0     3570 2023-05-22 15:10:05.000000 translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/6.ipynb
+-rw-rw-rw-   0        0        0   184064 2023-05-23 14:33:51.000000 translateabc-1.0.5/src/translateabc/READMEhh/ai35/hcia35.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.887801 translateabc-1.0.5/src/translateabc/READMEhh/moni/
+-rw-rw-rw-   0        0        0  4928289 2022-08-06 03:19:14.000000 translateabc-1.0.5/src/translateabc/READMEhh/moni/bankmarketing.csv
+-r--r--r--   0        0        0   236590 2023-05-23 13:02:38.000000 translateabc-1.0.5/src/translateabc/READMEhh/moni/bd01.ipynb
+-rw-rw-rw-   0        0        0     4281 2023-05-23 14:38:24.000000 translateabc-1.0.5/src/translateabc/READMEhh/moni/bd01.py
+-r--r--r--   0        0        0   188362 2023-05-23 13:09:26.000000 translateabc-1.0.5/src/translateabc/READMEhh/moni/bd02.ipynb
+-rw-rw-rw-   0        0        0     3980 2023-05-23 14:38:39.000000 translateabc-1.0.5/src/translateabc/READMEhh/moni/bd02.py
+-rw-rw-rw-   0        0        0   144767 2023-05-23 15:33:36.000000 translateabc-1.0.5/src/translateabc/READMEhh/moni/bd03.ipynb
+-rw-rw-rw-   0        0        0     4220 2023-05-23 15:36:22.000000 translateabc-1.0.5/src/translateabc/READMEhh/moni/bd03.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.891813 translateabc-1.0.5/src/translateabc/READMEhh/pandas-exercise/
+-rw-rw-rw-   0        0        0      124 2023-05-22 15:56:25.000000 translateabc-1.0.5/src/translateabc/READMEhh/pandas-exercise/1.csv
+-rw-rw-rw-   0        0        0     5625 2023-05-22 16:09:33.000000 translateabc-1.0.5/src/translateabc/READMEhh/pandas-exercise/1.ipynb
+-rw-rw-rw-   0        0        0       53 2023-05-22 15:56:19.000000 translateabc-1.0.5/src/translateabc/READMEhh/pandas-exercise/2.csv
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.894849 translateabc-1.0.5/src/translateabc/READMEhh/tensorflow_code/
+-rw-rw-rw-   0        0        0     5051 2023-05-05 09:52:13.000000 translateabc-1.0.5/src/translateabc/READMEhh/tensorflow_code/t.py
+-rw-rw-rw-   0        0        0      489 2023-05-03 16:18:50.000000 translateabc-1.0.5/src/translateabc/READMEhh/tensorflow_code/t1.py
+-rw-rw-rw-   0        0        0       74 2023-05-23 12:49:18.000000 translateabc-1.0.5/src/translateabc/__init__.py
+-rw-rw-rw-   0        0        0      406 2023-05-23 13:01:26.000000 translateabc-1.0.5/src/translateabc/g.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:37:00.858668 translateabc-1.0.5/src/translateabc.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-05-23 15:37:00.000000 translateabc-1.0.5/src/translateabc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1274 2023-05-23 15:37:00.000000 translateabc-1.0.5/src/translateabc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 15:37:00.000000 translateabc-1.0.5/src/translateabc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 15:37:00.000000 translateabc-1.0.5/src/translateabc.egg-info/top_level.txt
```

### Comparing `translateabc-1.0.4/.idea/workspace.xml` & `translateabc-1.0.5/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `translateabc-1.0.4/.idea/workspace.xml` & `translateabc-1.0.5/.idea/workspace.xml`

```diff
@@ -65,15 +65,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="abbb2ca3-9882-4039-a5c1-346b705212b6" name="Changes" comment=""/>
       <created>1684841815866</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1684841815866</updated>
-      <workItem from="1684841953267" duration="4174000"/>
+      <workItem from="1684841953267" duration="7486000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `translateabc-1.0.4/setup.py` & `translateabc-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="translateabc",
-    version="1.0.4",
+    version="1.0.5",
     author="Linvery",
     author_email="1253445120@qq.com",
     description="translateabc",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/pypa/sampleproject",
```

### Comparing `translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/1.ipynb` & `translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/1.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/2.ipynb` & `translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/2.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/3.ipynb` & `translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/3.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/4.ipynb` & `translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/4.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/5.ipynb` & `translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/5.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.4/src/translateabc/READMEhh/ai35/01/6.ipynb` & `translateabc-1.0.5/src/translateabc/READMEhh/ai35/01/6.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.4/src/translateabc/READMEhh/moni/bankmarketing.csv` & `translateabc-1.0.5/src/translateabc/READMEhh/moni/bankmarketing.csv`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.4/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb` & `translateabc-1.0.5/src/translateabc/READMEhh/moni/bd01.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9873511904761905%*

 * *Differences: {"'metadata'": "{'kernelspec': {'display_name': 'python-3.7.10', 'name': 'python-3.7.10'}, "*

 * *               "'language_info': {'version': '3.7.10'}}"}*

```diff
@@ -1296,27 +1296,27 @@
                 "ax.set_zlabel('campaign') \n",
                 "plt.show() "
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "python-3.7.10",
             "language": "python",
-            "name": "python3"
+            "name": "python-3.7.10"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.6"
+            "version": "3.7.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `translateabc-1.0.4/src/translateabc/READMEhh/pandas-exercise/1.ipynb` & `translateabc-1.0.5/src/translateabc/READMEhh/pandas-exercise/1.ipynb`

 * *Files identical despite different names*

