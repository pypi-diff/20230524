# Comparing `tmp/enebootools-2.0.3.tar.gz` & `tmp/enebootools-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enebootools-2.0.3.tar", last modified: Wed May 24 09:03:14 2023, max compression
+gzip compressed data, was "enebootools-2.0.4.tar", last modified: Wed May 24 09:22:19 2023, max compression
```

## Comparing `enebootools-2.0.3.tar` & `enebootools-2.0.4.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.123237 enebootools-2.0.3/
--rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.3/AUTHORS
--rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.3/LICENSE.gplv3
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 09:03:14.123237 enebootools-2.0.3/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.3/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.115237 enebootools-2.0.3/enebootools/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-24 09:02:26.000000 enebootools-2.0.3/enebootools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.3/enebootools/__init__.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.115237 enebootools-2.0.3/enebootools/assembler/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.3/enebootools/assembler/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/assembler/config.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-22 17:15:33.000000 enebootools-2.0.3/enebootools/assembler/database.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/assembler/databasemodels.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.3/enebootools/assembler/featureconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25310 2023-05-24 09:01:44.000000 enebootools-2.0.3/enebootools/assembler/kobjects.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/assembler/mypeewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.3/enebootools/assembler/save_auto.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.115237 enebootools-2.0.3/enebootools/autoconfig/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.3/enebootools/autoconfig/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.3/enebootools/autoconfig/autoconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/autoconfig/parsers.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.115237 enebootools-2.0.3/enebootools/config/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.3/enebootools/config/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.115237 enebootools-2.0.3/enebootools/crypto/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/crypto/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.119237 enebootools-2.0.3/enebootools/crypto/certificates/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/crypto/certificates/CA_Test_Partners.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/crypto/certificates/Partner_Test.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/crypto/certificates/Partner_Test.pem
--rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/crypto/certificates/README.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/crypto/certificates/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.3/enebootools/crypto/main.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.119237 enebootools-2.0.3/enebootools/databaseadmin/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.3/enebootools/databaseadmin/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.119237 enebootools-2.0.3/enebootools/databaseadmin/dblayer/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/databaseadmin/dblayer/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/databaseadmin/dblayer/drivers.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.3/enebootools/entry_points.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.119237 enebootools-2.0.3/enebootools/extracttool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/extracttool/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/extracttool/extractfunctions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.119237 enebootools-2.0.3/enebootools/lib/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.3/enebootools/lib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.119237 enebootools-2.0.3/enebootools/lib/etree/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.3/enebootools/lib/etree/ElementInclude.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/lib/etree/ElementPath.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/lib/etree/ElementTree.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.3/enebootools/lib/etree/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.3/enebootools/lib/etree/cElementTree.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/lib/peewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/lib/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.119237 enebootools-2.0.3/enebootools/mergetool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.3/enebootools/mergetool/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.119237 enebootools-2.0.3/enebootools/mergetool/etc/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/mergetool/etc/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.119237 enebootools-2.0.3/enebootools/mergetool/etc/formats/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/mergetool/etc/formats/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/mergetool/etc/formats/aq23-kut.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.3/enebootools/mergetool/etc/formats/aq23-mtd.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/mergetool/etc/formats/aq23-xml.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/mergetool/etc/formats/qt3-ts.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/mergetool/etc/formats/qt3-ui.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/mergetool/etc/index.xml
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.123237 enebootools-2.0.3/enebootools/mergetool/etc/patch-styles/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/mergetool/etc/patch-styles/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
--rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/mergetool/etc/patch-styles/legacy1.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.3/enebootools/mergetool/etc/patch-styles/semantic1.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76872 2023-05-17 19:00:59.000000 enebootools-2.0.3/enebootools/mergetool/flpatchapipy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31275 2023-05-24 08:29:21.000000 enebootools-2.0.3/enebootools/mergetool/flpatchdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44111 2023-05-24 08:29:10.000000 enebootools-2.0.3/enebootools/mergetool/flpatchlxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-2.0.3/enebootools/mergetool/flpatchmodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-09 12:25:44.000000 enebootools-2.0.3/enebootools/mergetool/flpatchpy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-24 08:26:10.000000 enebootools-2.0.3/enebootools/mergetool/flpatchqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.3/enebootools/mergetool/flpatchtest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/mergetool/flpatchxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3708 2023-05-22 15:27:23.000000 enebootools-2.0.3/enebootools/mergetool/projectbuilder.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.123237 enebootools-2.0.3/enebootools/mergetool/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.3/enebootools/mergetool/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.3/enebootools/mergetool/test/test_mergetool.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.123237 enebootools-2.0.3/enebootools/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.3/enebootools/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.3/enebootools/packager/pkgjoiner.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/packager/pkgsplitter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.3/enebootools/parseargs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.3/enebootools/parseargs.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.123237 enebootools-2.0.3/enebootools/parser/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.3/enebootools/parser/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.123237 enebootools-2.0.3/enebootools/vcsworkflow/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.3/enebootools/vcsworkflow/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:03:14.115237 enebootools-2.0.3/enebootools.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 09:03:13.000000 enebootools-2.0.3/enebootools.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-24 09:03:14.000000 enebootools-2.0.3/enebootools.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-24 09:03:13.000000 enebootools-2.0.3/enebootools.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-24 09:03:13.000000 enebootools-2.0.3/enebootools.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-24 09:03:13.000000 enebootools-2.0.3/enebootools.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-24 09:03:13.000000 enebootools-2.0.3/enebootools.egg-info/top_level.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-24 09:03:14.123237 enebootools-2.0.3/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.3/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.4/AUTHORS
+-rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.4/LICENSE.gplv3
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 09:22:19.448222 enebootools-2.0.4/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.4/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.440222 enebootools-2.0.4/enebootools/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-24 09:19:34.000000 enebootools-2.0.4/enebootools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.4/enebootools/__init__.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/assembler/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.4/enebootools/assembler/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/assembler/config.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-22 17:15:33.000000 enebootools-2.0.4/enebootools/assembler/database.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/assembler/databasemodels.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.4/enebootools/assembler/featureconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25310 2023-05-24 09:01:44.000000 enebootools-2.0.4/enebootools/assembler/kobjects.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/assembler/mypeewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.4/enebootools/assembler/save_auto.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/autoconfig/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/autoconfig/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.4/enebootools/autoconfig/autoconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/autoconfig/parsers.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/config/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/config/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/crypto/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/crypto/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/crypto/certificates/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/CA_Test_Partners.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/Partner_Test.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/Partner_Test.pem
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/crypto/certificates/README.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/crypto/certificates/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.4/enebootools/crypto/main.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/databaseadmin/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/databaseadmin/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/databaseadmin/dblayer/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/databaseadmin/dblayer/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/databaseadmin/dblayer/drivers.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.4/enebootools/entry_points.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/extracttool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/extracttool/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/extracttool/extractfunctions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/lib/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/lib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools/lib/etree/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.4/enebootools/lib/etree/ElementInclude.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/lib/etree/ElementPath.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/lib/etree/ElementTree.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.4/enebootools/lib/etree/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.4/enebootools/lib/etree/cElementTree.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/lib/peewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/lib/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.4/enebootools/mergetool/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/etc/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/mergetool/etc/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/etc/formats/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-kut.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-mtd.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-xml.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/qt3-ts.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/formats/qt3-ui.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/index.xml
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/legacy1.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/semantic1.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76872 2023-05-17 19:00:59.000000 enebootools-2.0.4/enebootools/mergetool/flpatchapipy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31644 2023-05-24 09:19:21.000000 enebootools-2.0.4/enebootools/mergetool/flpatchdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44111 2023-05-24 08:29:10.000000 enebootools-2.0.4/enebootools/mergetool/flpatchlxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-2.0.4/enebootools/mergetool/flpatchmodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-09 12:25:44.000000 enebootools-2.0.4/enebootools/mergetool/flpatchpy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    80758 2023-05-24 08:26:10.000000 enebootools-2.0.4/enebootools/mergetool/flpatchqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.4/enebootools/mergetool/flpatchtest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/mergetool/flpatchxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3708 2023-05-22 15:27:23.000000 enebootools-2.0.4/enebootools/mergetool/projectbuilder.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/mergetool/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.4/enebootools/mergetool/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.4/enebootools/mergetool/test/test_mergetool.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.4/enebootools/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.4/enebootools/packager/pkgjoiner.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/packager/pkgsplitter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.4/enebootools/parseargs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.4/enebootools/parseargs.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/parser/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.4/enebootools/parser/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.448222 enebootools-2.0.4/enebootools/vcsworkflow/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.4/enebootools/vcsworkflow/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-24 09:22:19.444222 enebootools-2.0.4/enebootools.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-24 09:22:19.000000 enebootools-2.0.4/enebootools.egg-info/top_level.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-24 09:22:19.448222 enebootools-2.0.4/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.4/setup.py
```

### Comparing `enebootools-2.0.3/LICENSE.gplv3` & `enebootools-2.0.4/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/PKG-INFO` & `enebootools-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.3
+Version: 2.0.4
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.3/README.rst` & `enebootools-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/__init__.py` & `enebootools-2.0.4/enebootools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os.path
 import sys
 import traceback
 from pprint import pformat
 import enebootools.parseargs as pa
 
 
-__VERSION__ = "2.0.3"
+__VERSION__ = "2.0.4"
 QS_EXTEND_MODE = "legacy"
 
 
 def ustr(value):
     """Ustr."""
     if isinstance(value, str):
         return value
```

### Comparing `enebootools-2.0.3/enebootools/__init__.pyc` & `enebootools-2.0.4/enebootools/__init__.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/assembler/__init__.py` & `enebootools-2.0.4/enebootools/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/assembler/config.py` & `enebootools-2.0.4/enebootools/assembler/config.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/assembler/database.py` & `enebootools-2.0.4/enebootools/assembler/database.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/assembler/databasemodels.py` & `enebootools-2.0.4/enebootools/assembler/databasemodels.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/assembler/featureconfig.py` & `enebootools-2.0.4/enebootools/assembler/featureconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/assembler/kobjects.py` & `enebootools-2.0.4/enebootools/assembler/kobjects.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/assembler/mypeewee.py` & `enebootools-2.0.4/enebootools/assembler/mypeewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/assembler/save_auto.py` & `enebootools-2.0.4/enebootools/assembler/save_auto.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/autoconfig/autoconfig.py` & `enebootools-2.0.4/enebootools/autoconfig/autoconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/autoconfig/parsers.py` & `enebootools-2.0.4/enebootools/autoconfig/parsers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/crypto/__init__.py` & `enebootools-2.0.4/enebootools/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt` & `enebootools-2.0.4/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/crypto/certificates/CA_Test_Partners.crt` & `enebootools-2.0.4/enebootools/crypto/certificates/CA_Test_Partners.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt` & `enebootools-2.0.4/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/crypto/certificates/Partner_Test.crt` & `enebootools-2.0.4/enebootools/crypto/certificates/Partner_Test.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/crypto/certificates/Partner_Test.pem` & `enebootools-2.0.4/enebootools/crypto/certificates/Partner_Test.pem`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/crypto/certificates/README.txt` & `enebootools-2.0.4/enebootools/crypto/certificates/README.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/crypto/main.py` & `enebootools-2.0.4/enebootools/crypto/main.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/databaseadmin/dblayer/drivers.py` & `enebootools-2.0.4/enebootools/databaseadmin/dblayer/drivers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/entry_points.py` & `enebootools-2.0.4/enebootools/entry_points.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/extracttool/__init__.py` & `enebootools-2.0.4/enebootools/extracttool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/extracttool/extractfunctions.py` & `enebootools-2.0.4/enebootools/extracttool/extractfunctions.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/lib/etree/ElementInclude.py` & `enebootools-2.0.4/enebootools/lib/etree/ElementInclude.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/lib/etree/ElementPath.py` & `enebootools-2.0.4/enebootools/lib/etree/ElementPath.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/lib/etree/ElementTree.py` & `enebootools-2.0.4/enebootools/lib/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/lib/etree/__init__.py` & `enebootools-2.0.4/enebootools/lib/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/lib/peewee.py` & `enebootools-2.0.4/enebootools/lib/peewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/lib/utils.py` & `enebootools-2.0.4/enebootools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/__init__.py` & `enebootools-2.0.4/enebootools/mergetool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/etc/formats/aq23-kut.xml` & `enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-kut.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/etc/formats/aq23-mtd.xml` & `enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-mtd.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/etc/formats/aq23-xml.xml` & `enebootools-2.0.4/enebootools/mergetool/etc/formats/aq23-xml.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/etc/formats/qt3-ts.xml` & `enebootools-2.0.4/enebootools/mergetool/etc/formats/qt3-ts.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/etc/formats/qt3-ui.xml` & `enebootools-2.0.4/enebootools/mergetool/etc/formats/qt3-ui.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/etc/index.xml` & `enebootools-2.0.4/enebootools/mergetool/etc/index.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl` & `enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/etc/patch-styles/legacy1.xml` & `enebootools-2.0.4/enebootools/mergetool/etc/patch-styles/legacy1.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/flpatchapipy.py` & `enebootools-2.0.4/enebootools/mergetool/flpatchapipy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/flpatchdir.py` & `enebootools-2.0.4/enebootools/mergetool/flpatchdir.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     def replace_file(self, replacefile, folder):
         path = replacefile.get("path")
         filename = replacefile.get("name")
 
         pathname = os.path.join(path, filename)
         dst = os.path.join(folder, pathname)
         if not os.path.exists(dst):
-            self.iface.warn(
+            self.iface.debug(
                 "Ignorando reemplazo de fichero para %s (el fichero no existe)" % filename
             )
             return
 
         self.iface.debug("Reemplazando fichero %s . . ." % filename)
         src = os.path.join(self.patch_dir, filename)
         os.unlink(dst)
@@ -760,17 +760,27 @@
         os.remove(final_file)
 
     return True
 
 
 def update_xml_patch(iface, fpatch, basedir):
     patch_xml_file = os.path.join(fpatch.patchdir, fpatch.patch_name + ".xml")
-    iface.info("Calculando cambios en %s" % patch_xml_file)
-
-    current_et = etree.parse(patch_xml_file)
+    iface.warn("Calculando cambios en %s" % patch_xml_file)
+    try:
+        encoding = "iso-8859-15"
+        parser = etree.XMLParser(
+            ns_clean=False,
+            encoding=encoding,
+            # .. recover funciona y parsea cuasi cualquier cosa.
+            recover=True,
+            remove_blank_text=True,
+        )
+        current_et = etree.parse(patch_xml_file, parser)
+    except IOError as e:
+        iface.error("No se pudo leer el parche: " + str(e))
     current_root = current_et.getroot()
 
     found_changes = False
 
     for action in fpatch.root:
         found_changes = True
         new_path = action.get("path")
```

### Comparing `enebootools-2.0.3/enebootools/mergetool/flpatchlxml.py` & `enebootools-2.0.4/enebootools/mergetool/flpatchlxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/flpatchmodel.py` & `enebootools-2.0.4/enebootools/mergetool/flpatchmodel.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/flpatchpy.py` & `enebootools-2.0.4/enebootools/mergetool/flpatchpy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/flpatchqs.py` & `enebootools-2.0.4/enebootools/mergetool/flpatchqs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/flpatchtest.py` & `enebootools-2.0.4/enebootools/mergetool/flpatchtest.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/flpatchxml.py` & `enebootools-2.0.4/enebootools/mergetool/flpatchxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/projectbuilder.py` & `enebootools-2.0.4/enebootools/mergetool/projectbuilder.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/test/__init__.py` & `enebootools-2.0.4/enebootools/mergetool/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/mergetool/test/test_mergetool.py` & `enebootools-2.0.4/enebootools/mergetool/test/test_mergetool.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/packager/__init__.py` & `enebootools-2.0.4/enebootools/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/packager/pkgjoiner.py` & `enebootools-2.0.4/enebootools/packager/pkgjoiner.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/packager/pkgsplitter.py` & `enebootools-2.0.4/enebootools/packager/pkgsplitter.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/parseargs.py` & `enebootools-2.0.4/enebootools/parseargs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools/parseargs.pyc` & `enebootools-2.0.4/enebootools/parseargs.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/enebootools.egg-info/PKG-INFO` & `enebootools-2.0.4/enebootools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.3
+Version: 2.0.4
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.3/enebootools.egg-info/SOURCES.txt` & `enebootools-2.0.4/enebootools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.3/setup.py` & `enebootools-2.0.4/setup.py`

 * *Files identical despite different names*

