# Comparing `tmp/packagetenssor-0.6.tar.gz` & `tmp/packagetenssor-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packagetenssor-0.6.tar", last modified: Wed May 24 04:32:29 2023, max compression
+gzip compressed data, was "packagetenssor-0.7.tar", last modified: Wed May 24 05:49:41 2023, max compression
```

## Comparing `packagetenssor-0.6.tar` & `packagetenssor-0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 ankit.sharma10 (101996570) 1493847943        0 2023-05-24 04:32:29.888619 packagetenssor-0.6/
--rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      215 2023-05-24 04:32:29.887427 packagetenssor-0.6/PKG-INFO
-drwxr-xr-x   0 ankit.sharma10 (101996570) 1493847943        0 2023-05-24 04:32:29.875800 packagetenssor-0.6/packagetenssor.egg-info/
--rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      215 2023-05-24 04:32:29.000000 packagetenssor-0.6/packagetenssor.egg-info/PKG-INFO
--rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      180 2023-05-24 04:32:29.000000 packagetenssor-0.6/packagetenssor.egg-info/SOURCES.txt
--rw-r--r--   0 ankit.sharma10 (101996570) 1493847943        1 2023-05-24 04:32:29.000000 packagetenssor-0.6/packagetenssor.egg-info/dependency_links.txt
--rw-r--r--   0 ankit.sharma10 (101996570) 1493847943        8 2023-05-24 04:32:29.000000 packagetenssor-0.6/packagetenssor.egg-info/top_level.txt
--rw-r--r--   0 ankit.sharma10 (101996570) 1493847943       38 2023-05-24 04:32:29.888827 packagetenssor-0.6/setup.cfg
--rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      258 2023-05-24 04:32:17.000000 packagetenssor-0.6/setup.py
-drwxr-xr-x   0 ankit.sharma10 (101996570) 1493847943        0 2023-05-24 04:32:29.886046 packagetenssor-0.6/tenssor/
--rw-r--r--   0 ankit.sharma10 (101996570) 1493847943    34142 2023-05-24 04:29:50.000000 packagetenssor-0.6/tenssor/__init__.py
+drwxr-xr-x   0 ankit.sharma10 (101996570) 1493847943        0 2023-05-24 05:49:41.696277 packagetenssor-0.7/
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      215 2023-05-24 05:49:41.695859 packagetenssor-0.7/PKG-INFO
+drwxr-xr-x   0 ankit.sharma10 (101996570) 1493847943        0 2023-05-24 05:49:41.693282 packagetenssor-0.7/packagetenssor.egg-info/
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      215 2023-05-24 05:49:41.000000 packagetenssor-0.7/packagetenssor.egg-info/PKG-INFO
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      180 2023-05-24 05:49:41.000000 packagetenssor-0.7/packagetenssor.egg-info/SOURCES.txt
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943        1 2023-05-24 05:49:41.000000 packagetenssor-0.7/packagetenssor.egg-info/dependency_links.txt
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943        8 2023-05-24 05:49:41.000000 packagetenssor-0.7/packagetenssor.egg-info/top_level.txt
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943       38 2023-05-24 05:49:41.696331 packagetenssor-0.7/setup.cfg
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      258 2023-05-24 05:49:33.000000 packagetenssor-0.7/setup.py
+drwxr-xr-x   0 ankit.sharma10 (101996570) 1493847943        0 2023-05-24 05:49:41.694557 packagetenssor-0.7/tenssor/
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943    57942 2023-05-24 05:48:37.000000 packagetenssor-0.7/tenssor/__init__.py
```

