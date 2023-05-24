# Comparing `tmp/foliage-1.5.5.tar.gz` & `tmp/foliage-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliage-1.5.5.tar", last modified: Thu Mar  9 19:00:23 2023, max compression
+gzip compressed data, was "foliage-1.6.0.tar", last modified: Wed May 24 00:17:27 2023, max compression
```

## Comparing `foliage-1.5.5.tar` & `foliage-1.6.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2023-03-09 19:00:23.420907 foliage-1.5.5/
--rw-r--r--   0 mhucka     (511) staff       (20)     1528 2023-03-09 18:22:28.000000 foliage-1.5.5/LICENSE
--rw-r--r--   0 mhucka     (511) staff       (20)     6892 2023-03-09 19:00:23.421027 foliage-1.5.5/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)     5880 2023-03-09 18:23:01.000000 foliage-1.5.5/README.md
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2023-03-09 19:00:23.418521 foliage-1.5.5/foliage/
--rw-r--r--   0 mhucka     (511) staff       (20)     1428 2023-03-09 18:58:04.000000 foliage-1.5.5/foliage/__init__.py
--rw-r--r--   0 mhucka     (511) staff       (20)    29345 2022-09-26 21:07:49.000000 foliage-1.5.5/foliage/__main__.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1049 2022-09-26 20:23:23.000000 foliage-1.5.5/foliage/base_tab.py
--rw-r--r--   0 mhucka     (511) staff       (20)    27938 2022-09-26 23:52:13.000000 foliage-1.5.5/foliage/change_tab.py
--rw-r--r--   0 mhucka     (511) staff       (20)    10808 2022-09-26 23:50:59.000000 foliage-1.5.5/foliage/clean_tab.py
--rw-r--r--   0 mhucka     (511) staff       (20)    10569 2022-09-29 02:13:23.000000 foliage-1.5.5/foliage/credentials.py
--rw-r--r--   0 mhucka     (511) staff       (20)    14007 2022-09-27 20:09:06.000000 foliage-1.5.5/foliage/delete_tab.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1075 2022-09-26 20:45:48.000000 foliage-1.5.5/foliage/enum_utils.py
--rw-r--r--   0 mhucka     (511) staff       (20)      984 2022-09-26 20:45:56.000000 foliage-1.5.5/foliage/exceptions.py
--rw-r--r--   0 mhucka     (511) staff       (20)     5467 2022-09-26 23:28:06.000000 foliage-1.5.5/foliage/export.py
--rw-r--r--   0 mhucka     (511) staff       (20)    53664 2022-09-27 20:10:02.000000 foliage-1.5.5/foliage/folio.py
--rw-r--r--   0 mhucka     (511) staff       (20)     7677 2022-09-26 21:01:33.000000 foliage-1.5.5/foliage/list_tab.py
--rw-r--r--   0 mhucka     (511) staff       (20)    22737 2023-03-09 03:58:14.000000 foliage-1.5.5/foliage/lookup_tab.py
--rw-r--r--   0 mhucka     (511) staff       (20)     4753 2022-09-26 21:04:52.000000 foliage-1.5.5/foliage/other_tab.py
--rw-r--r--   0 mhucka     (511) staff       (20)    14672 2022-09-26 21:05:40.000000 foliage-1.5.5/foliage/system_widget.py
--rw-r--r--   0 mhucka     (511) staff       (20)    15937 2022-12-02 23:20:45.000000 foliage-1.5.5/foliage/ui.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2023-03-09 19:00:23.420727 foliage-1.5.5/foliage.egg-info/
--rw-r--r--   0 mhucka     (511) staff       (20)     6892 2023-03-09 19:00:23.000000 foliage-1.5.5/foliage.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)      583 2023-03-09 19:00:23.000000 foliage-1.5.5/foliage.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2023-03-09 19:00:23.000000 foliage-1.5.5/foliage.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (511) staff       (20)       67 2023-03-09 19:00:23.000000 foliage-1.5.5/foliage.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2023-03-09 18:57:53.000000 foliage-1.5.5/foliage.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (511) staff       (20)      920 2023-03-09 19:00:23.000000 foliage-1.5.5/foliage.egg-info/requires.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        8 2023-03-09 19:00:23.000000 foliage-1.5.5/foliage.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (511) staff       (20)     1116 2023-03-09 19:00:23.421529 foliage-1.5.5/setup.cfg
--rwxr-xr-x   0 mhucka     (511) staff       (20)     1683 2022-07-11 17:48:24.000000 foliage-1.5.5/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 00:17:27.122722 foliage-1.6.0/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1528 2023-03-09 18:22:28.000000 foliage-1.6.0/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)     6872 2023-05-24 00:17:27.122787 foliage-1.6.0/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)     5880 2023-03-09 18:23:01.000000 foliage-1.6.0/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 00:17:27.121361 foliage-1.6.0/foliage/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1428 2023-05-24 00:16:24.000000 foliage-1.6.0/foliage/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    29345 2022-09-26 21:07:49.000000 foliage-1.6.0/foliage/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1049 2022-09-26 20:23:23.000000 foliage-1.6.0/foliage/base_tab.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    27938 2022-09-26 23:52:13.000000 foliage-1.6.0/foliage/change_tab.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    10808 2022-09-26 23:50:59.000000 foliage-1.6.0/foliage/clean_tab.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    11072 2023-05-02 22:56:36.000000 foliage-1.6.0/foliage/credentials.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14007 2022-09-27 20:09:06.000000 foliage-1.6.0/foliage/delete_tab.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1075 2022-09-26 20:45:48.000000 foliage-1.6.0/foliage/enum_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      984 2022-09-26 20:45:56.000000 foliage-1.6.0/foliage/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5467 2023-05-23 21:54:21.000000 foliage-1.6.0/foliage/export.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    54048 2023-05-02 22:49:37.000000 foliage-1.6.0/foliage/folio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     7677 2023-05-03 01:10:04.000000 foliage-1.6.0/foliage/list_tab.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    27582 2023-05-23 22:42:42.000000 foliage-1.6.0/foliage/lookup_tab.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4753 2022-09-26 21:04:52.000000 foliage-1.6.0/foliage/other_tab.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14672 2022-09-26 21:05:40.000000 foliage-1.6.0/foliage/system_widget.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15937 2022-12-02 23:20:45.000000 foliage-1.6.0/foliage/ui.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 00:17:27.122254 foliage-1.6.0/foliage.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)     6872 2023-05-24 00:17:27.000000 foliage-1.6.0/foliage.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      648 2023-05-24 00:17:27.000000 foliage-1.6.0/foliage.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-24 00:17:27.000000 foliage-1.6.0/foliage.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       66 2023-05-24 00:17:27.000000 foliage-1.6.0/foliage.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-24 00:17:20.000000 foliage-1.6.0/foliage.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      929 2023-05-24 00:17:27.000000 foliage-1.6.0/foliage.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        8 2023-05-24 00:17:27.000000 foliage-1.6.0/foliage.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1116 2023-05-24 00:17:27.123069 foliage-1.6.0/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1683 2022-07-11 17:48:24.000000 foliage-1.6.0/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-24 00:17:27.122619 foliage-1.6.0/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1439 2022-09-29 02:16:15.000000 foliage-1.6.0/tests/test_credentials.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2549 2022-09-29 18:11:27.000000 foliage-1.6.0/tests/test_folio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      270 2022-09-29 00:03:20.000000 foliage-1.6.0/tests/test_init.py
```

### Comparing `foliage-1.5.5/LICENSE` & `foliage-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/PKG-INFO` & `foliage-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: foliage
-Version: 1.5.5
+Version: 1.6.0
 Summary: Foliage: a tool to do bulk changes in FOLIO using the OKAPI API
 Home-page: https://github.com/caltechlibrary/foliage
 Author: Mike Hucka
 Author-email: helpdesk@library.caltech.edu
 License: BSD 3-clause license
 Project-URL: Source Code, https://github.com/caltechlibrary/foliage
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/foliage/issues
 Keywords: Python,applications
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
@@ -126,9 +125,7 @@
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
     <img width="100" height="100" src="https://raw.githubusercontent.com/caltechlibrary/foliage/main/.graphics/caltech-round.png">
   </a>
 </div>
-
-
```

### Comparing `foliage-1.5.5/README.md` & `foliage-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/__init__.py` & `foliage-1.6.0/foliage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '1.5.5'
+__version__     = '1.6.0'
 __description__ = 'Foliage: a tool to do bulk changes in FOLIO using the OKAPI API'
 __url__         = 'https://github.com/caltechlibrary/foliage'
 __author__      = 'Mike Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'BSD 3-clause license'
```

### Comparing `foliage-1.5.5/foliage/__main__.py` & `foliage-1.6.0/foliage/__main__.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/base_tab.py` & `foliage-1.6.0/foliage/base_tab.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/change_tab.py` & `foliage-1.6.0/foliage/change_tab.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/clean_tab.py` & `foliage-1.6.0/foliage/clean_tab.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/credentials.py` & `foliage-1.6.0/foliage/credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,534 +128,565 @@
 000007f0: 2e6f 7574 7075 7420 696d 706f 7274 2070  .output import p
 00000800: 7574 5f6c 6f61 6469 6e67 0a66 726f 6d20  ut_loading.from 
 00000810: 2020 7079 7765 6269 6f2e 7069 6e20 696d    pywebio.pin im
 00000820: 706f 7274 2070 696e 2c20 7075 745f 696e  port pin, put_in
 00000830: 7075 740a 6672 6f6d 2020 2073 6964 6574  put.from   sidet
 00000840: 7261 636b 2069 6d70 6f72 7420 6c6f 670a  rack import log.
 00000850: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
-00000860: 7420 7468 7265 6164 696e 670a 0a69 6620  t threading..if 
-00000870: 7379 732e 706c 6174 666f 726d 2e73 7461  sys.platform.sta
-00000880: 7274 7377 6974 6828 2777 696e 2729 3a0a  rtswith('win'):.
-00000890: 2020 2020 696d 706f 7274 206b 6579 7269      import keyri
-000008a0: 6e67 2e62 6163 6b65 6e64 730a 2020 2020  ng.backends.    
-000008b0: 6672 6f6d 206b 6579 7269 6e67 2e62 6163  from keyring.bac
-000008c0: 6b65 6e64 732e 5769 6e64 6f77 7320 696d  kends.Windows im
-000008d0: 706f 7274 2057 696e 5661 756c 744b 6579  port WinVaultKey
-000008e0: 7269 6e67 0a69 6620 7379 732e 706c 6174  ring.if sys.plat
-000008f0: 666f 726d 2e73 7461 7274 7377 6974 6828  form.startswith(
-00000900: 2764 6172 7769 6e27 293a 0a20 2020 2069  'darwin'):.    i
-00000910: 6d70 6f72 7420 6b65 7972 696e 672e 6261  mport keyring.ba
-00000920: 636b 656e 6473 0a20 2020 2066 726f 6d20  ckends.    from 
-00000930: 6b65 7972 696e 672e 6261 636b 656e 6473  keyring.backends
-00000940: 2e4f 535f 5820 696d 706f 7274 204b 6579  .OS_X import Key
-00000950: 7269 6e67 0a0a 6672 6f6d 2066 6f6c 6961  ring..from folia
-00000960: 6765 2e66 6f6c 696f 2069 6d70 6f72 7420  ge.folio import 
-00000970: 466f 6c69 6f0a 6672 6f6d 2066 6f6c 6961  Folio.from folia
-00000980: 6765 2e75 6920 696d 706f 7274 2063 6f6e  ge.ui import con
-00000990: 6669 726d 2c20 6e6f 7465 5f69 6e66 6f2c  firm, note_info,
-000009a0: 206e 6f74 6966 790a 0a0c 0a23 2050 7269   notify....# Pri
-000009b0: 7661 7465 2063 6f6e 7374 616e 7473 2e0a  vate constants..
-000009c0: 2320 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  # ..............
-000009d0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-000009e0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000860: 7420 7468 7265 6164 696e 670a 6672 6f6d  t threading.from
+00000870: 2020 2076 616c 6964 6174 6f72 732e 7572     validators.ur
+00000880: 6c20 696d 706f 7274 2075 726c 2061 7320  l import url as 
+00000890: 7661 6c69 645f 7572 6c0a 0a69 6620 7379  valid_url..if sy
+000008a0: 732e 706c 6174 666f 726d 2e73 7461 7274  s.platform.start
+000008b0: 7377 6974 6828 2777 696e 2729 3a0a 2020  swith('win'):.  
+000008c0: 2020 696d 706f 7274 206b 6579 7269 6e67    import keyring
+000008d0: 2e62 6163 6b65 6e64 730a 2020 2020 6672  .backends.    fr
+000008e0: 6f6d 206b 6579 7269 6e67 2e62 6163 6b65  om keyring.backe
+000008f0: 6e64 732e 5769 6e64 6f77 7320 696d 706f  nds.Windows impo
+00000900: 7274 2057 696e 5661 756c 744b 6579 7269  rt WinVaultKeyri
+00000910: 6e67 0a69 6620 7379 732e 706c 6174 666f  ng.if sys.platfo
+00000920: 726d 2e73 7461 7274 7377 6974 6828 2764  rm.startswith('d
+00000930: 6172 7769 6e27 293a 0a20 2020 2069 6d70  arwin'):.    imp
+00000940: 6f72 7420 6b65 7972 696e 672e 6261 636b  ort keyring.back
+00000950: 656e 6473 0a20 2020 2066 726f 6d20 6b65  ends.    from ke
+00000960: 7972 696e 672e 6261 636b 656e 6473 2e4f  yring.backends.O
+00000970: 535f 5820 696d 706f 7274 204b 6579 7269  S_X import Keyri
+00000980: 6e67 0a0a 6672 6f6d 2066 6f6c 6961 6765  ng..from foliage
+00000990: 2e66 6f6c 696f 2069 6d70 6f72 7420 466f  .folio import Fo
+000009a0: 6c69 6f0a 6672 6f6d 2066 6f6c 6961 6765  lio.from foliage
+000009b0: 2e75 6920 696d 706f 7274 2063 6f6e 6669  .ui import confi
+000009c0: 726d 2c20 6e6f 7465 5f69 6e66 6f2c 206e  rm, note_info, n
+000009d0: 6f74 6966 790a 0a0c 0a23 2050 7269 7661  otify....# Priva
+000009e0: 7465 2063 6f6e 7374 616e 7473 2e0a 2320  te constants..# 
 000009f0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000a00: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e0a  ................
-00000a10: 0a5f 4b45 5952 494e 4720 3d20 6627 6f72  ._KEYRING = f'or
-00000a20: 672e 6361 6c74 6563 686c 6962 7261 7279  g.caltechlibrary
-00000a30: 2e7b 5f5f 7061 636b 6167 655f 5f7d 270a  .{__package__}'.
-00000a40: 2727 2754 6865 206e 616d 6520 6f66 2074  '''The name of t
-00000a50: 6865 206b 6579 7269 6e67 2075 7365 6420  he keyring used 
-00000a60: 746f 2073 746f 7265 2073 6572 7665 7220  to store server 
-00000a70: 6163 6365 7373 2063 7265 6465 6e74 6961  access credentia
-00000a80: 6c73 2c20 6966 2061 6e79 2e27 2727 0a0a  ls, if any.'''..
-00000a90: 0c0a 2320 5075 626c 6963 2064 6174 6120  ..# Public data 
-00000aa0: 7479 7065 732e 0a23 202e 2e2e 2e2e 2e2e  types..# .......
-00000ab0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000ac0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000ad0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000a00: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000a10: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000a20: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000a30: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e0a 0a5f  ..............._
+00000a40: 4b45 5952 494e 4720 3d20 6627 6f72 672e  KEYRING = f'org.
+00000a50: 6361 6c74 6563 686c 6962 7261 7279 2e7b  caltechlibrary.{
+00000a60: 5f5f 7061 636b 6167 655f 5f7d 270a 2727  __package__}'.''
+00000a70: 2754 6865 206e 616d 6520 6f66 2074 6865  'The name of the
+00000a80: 206b 6579 7269 6e67 2075 7365 6420 746f   keyring used to
+00000a90: 2073 746f 7265 2073 6572 7665 7220 6163   store server ac
+00000aa0: 6365 7373 2063 7265 6465 6e74 6961 6c73  cess credentials
+00000ab0: 2c20 6966 2061 6e79 2e27 2727 0a0a 0c0a  , if any.'''....
+00000ac0: 2320 5075 626c 6963 2064 6174 6120 7479  # Public data ty
+00000ad0: 7065 732e 0a23 202e 2e2e 2e2e 2e2e 2e2e  pes..# .........
 00000ae0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000af0: 2e2e 2e2e 2e2e 0a0a 4372 6564 656e 7469  ........Credenti
-00000b00: 616c 7320 3d20 6e61 6d65 6474 7570 6c65  als = namedtuple
-00000b10: 2827 4372 6564 656e 7469 616c 7327 2c20  ('Credentials', 
-00000b20: 2775 726c 2074 656e 616e 745f 6964 2074  'url tenant_id t
-00000b30: 6f6b 656e 2729 0a0a 0c0a 2320 5075 626c  oken')....# Publ
-00000b40: 6963 2066 756e 6374 696f 6e73 2e0a 2320  ic functions..# 
-00000b50: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000b60: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000b70: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000af0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000b00: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000b10: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000b20: 2e2e 2e2e 0a0a 4372 6564 656e 7469 616c  ......Credential
+00000b30: 7320 3d20 6e61 6d65 6474 7570 6c65 2827  s = namedtuple('
+00000b40: 4372 6564 656e 7469 616c 7327 2c20 2775  Credentials', 'u
+00000b50: 726c 2074 656e 616e 745f 6964 2074 6f6b  rl tenant_id tok
+00000b60: 656e 2729 0a0a 0c0a 2320 5075 626c 6963  en')....# Public
+00000b70: 2066 756e 6374 696f 6e73 2e0a 2320 2e2e   functions..# ..
 00000b80: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000b90: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e0a 0a64  ...............d
-00000ba0: 6566 2063 7265 6465 6e74 6961 6c73 5f66  ef credentials_f
-00000bb0: 726f 6d5f 6669 6c65 2863 7265 6473 5f66  rom_file(creds_f
-00000bc0: 696c 6529 3a0a 2020 2020 2727 2752 6574  ile):.    '''Ret
-00000bd0: 7572 6e20 6120 4372 6564 656e 7469 616c  urn a Credential
-00000be0: 7320 6f62 6a65 6374 2063 7265 6174 6564  s object created
-00000bf0: 2066 726f 6d20 7661 6c75 6573 2069 6e20   from values in 
-00000c00: 6372 6564 735f 6669 6c65 2e0a 0a20 2020  creds_file...   
-00000c10: 2054 6865 2063 7265 6465 6e74 6961 6c73   The credentials
-00000c20: 2066 696c 6520 6d75 7374 2062 6520 696e   file must be in
-00000c30: 2022 2e69 6e69 2220 666f 726d 6174 2c20   ".ini" format, 
-00000c40: 6c69 6b65 2074 6869 733a 0a0a 2020 2020  like this:..    
-00000c50: 5b73 6574 7469 6e67 735d 0a20 2020 2046  [settings].    F
-00000c60: 4f4c 494f 5f4f 4b41 5049 5f55 524c 203d  OLIO_OKAPI_URL =
-00000c70: 202e 2e2e 2e2e 0a20 2020 2046 4f4c 494f   ......    FOLIO
-00000c80: 5f4f 4b41 5049 5f54 454e 414e 545f 4944  _OKAPI_TENANT_ID
-00000c90: 203d 202e 2e2e 2e2e 0a20 2020 2046 4f4c   = ......    FOL
-00000ca0: 494f 5f4f 4b41 5049 5f54 4f4b 454e 203d  IO_OKAPI_TOKEN =
-00000cb0: 202e 2e2e 2e2e 0a20 2020 2027 2727 0a20   ......    '''. 
-00000cc0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00000cd0: 636f 6e66 6967 5f66 696c 6520 3d20 436f  config_file = Co
-00000ce0: 6e66 6967 2852 6570 6f73 6974 6f72 7949  nfig(RepositoryI
-00000cf0: 6e69 2873 6f75 7263 6520 3d20 6372 6564  ni(source = cred
-00000d00: 735f 6669 6c65 2929 0a20 2020 2065 7863  s_file)).    exc
-00000d10: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00000d20: 2065 783a 2020 2020 2020 2020 2020 2020   ex:            
-00000d30: 2023 206e 6f71 613a 2050 4945 3738 360a   # noqa: PIE786.
-00000d40: 2020 2020 2020 2020 6c6f 6728 2775 6e61          log('una
-00000d50: 626c 6520 746f 2072 6561 6420 6769 7665  ble to read give
-00000d60: 6e20 6372 6564 7320 6669 6c65 3a20 2720  n creds file: ' 
-00000d70: 2b20 7374 7228 6578 2929 0a20 2020 2020  + str(ex)).     
-00000d80: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00000d90: 2020 2072 6574 7572 6e20 5f63 7265 6473     return _creds
-00000da0: 5f66 726f 6d5f 736f 7572 6365 2863 6f6e  _from_source(con
-00000db0: 6669 675f 6669 6c65 2c20 7374 7228 6372  fig_file, str(cr
-00000dc0: 6564 735f 6669 6c65 2929 0a0a 0a64 6566  eds_file))...def
-00000dd0: 2063 7265 6465 6e74 6961 6c73 5f66 726f   credentials_fro
-00000de0: 6d5f 656e 7628 293a 0a20 2020 2027 2727  m_env():.    '''
-00000df0: 5265 7475 726e 2061 2043 7265 6465 6e74  Return a Credent
-00000e00: 6961 6c73 206f 626a 6563 7420 6372 6561  ials object crea
-00000e10: 7465 6420 6672 6f6d 2065 6e76 6972 6f6e  ted from environ
-00000e20: 6d65 6e74 2076 6172 6961 626c 6573 2e0a  ment variables..
-00000e30: 0a20 2020 2054 6869 7320 6368 6563 6b73  .    This checks
-00000e40: 2066 6f72 2074 6865 2066 6f6c 6c6f 7769   for the followi
-00000e50: 6e67 2065 6e76 6972 6f6e 6d65 6e74 2076  ng environment v
-00000e60: 6172 6961 626c 6573 3a0a 0a20 2020 2020  ariables:..     
-00000e70: 2046 4f4c 494f 5f4f 4b41 5049 5f55 524c   FOLIO_OKAPI_URL
-00000e80: 0a20 2020 2020 2046 4f4c 494f 5f4f 4b41  .      FOLIO_OKA
-00000e90: 5049 5f54 454e 414e 545f 4944 0a20 2020  PI_TENANT_ID.   
-00000ea0: 2020 2046 4f4c 494f 5f4f 4b41 5049 5f54     FOLIO_OKAPI_T
-00000eb0: 4f4b 454e 0a20 2020 2027 2727 0a20 2020  OKEN.    '''.   
-00000ec0: 2072 6574 7572 6e20 5f63 7265 6473 5f66   return _creds_f
-00000ed0: 726f 6d5f 736f 7572 6365 2843 6f6e 6669  rom_source(Confi
-00000ee0: 6728 5265 706f 7369 746f 7279 456d 7074  g(RepositoryEmpt
-00000ef0: 7928 2929 2c20 2765 6e76 6972 6f6e 6d65  y()), 'environme
-00000f00: 6e74 2729 0a0a 0a64 6566 2063 7265 6465  nt')...def crede
-00000f10: 6e74 6961 6c73 5f66 726f 6d5f 7573 6572  ntials_from_user
-00000f20: 2877 6172 6e5f 656d 7074 7920 3d20 5472  (warn_empty = Tr
-00000f30: 7565 2c20 696e 6974 6961 6c5f 6372 6564  ue, initial_cred
-00000f40: 7320 3d20 4e6f 6e65 293a 0a20 2020 2027  s = None):.    '
-00000f50: 2727 4173 6b20 7573 6572 2066 6f72 2069  ''Ask user for i
-00000f60: 6e66 6f20 6e65 6564 6564 2074 6f20 6372  nfo needed to cr
-00000f70: 6561 7465 2061 2074 6f6b 656e 2026 2072  eate a token & r
-00000f80: 6574 7572 6e20 6120 4372 6564 656e 7469  eturn a Credenti
-00000f90: 616c 7320 6f62 6a2e 2727 270a 0a20 2020  als obj.'''..   
-00000fa0: 2065 7665 6e74 203d 2074 6872 6561 6469   event = threadi
-00000fb0: 6e67 2e45 7665 6e74 2829 0a20 2020 2063  ng.Event().    c
-00000fc0: 6c69 636b 6564 5f6f 6b20 3d20 4661 6c73  licked_ok = Fals
-00000fd0: 650a 0a20 2020 2064 6566 2063 6c6b 2876  e..    def clk(v
-00000fe0: 616c 293a 0a20 2020 2020 2020 206e 6f6e  al):.        non
-00000ff0: 6c6f 6361 6c20 636c 6963 6b65 645f 6f6b  local clicked_ok
-00001000: 0a20 2020 2020 2020 2063 6c69 636b 6564  .        clicked
-00001010: 5f6f 6b20 3d20 7661 6c0a 2020 2020 2020  _ok = val.      
-00001020: 2020 6576 656e 742e 7365 7428 290a 0a20    event.set().. 
-00001030: 2020 206c 6f67 2827 6173 6b69 6e67 2075     log('asking u
-00001040: 7365 7220 666f 7220 6372 6564 656e 7469  ser for credenti
-00001050: 616c 7327 290a 2020 2020 6375 7272 656e  als').    curren
-00001060: 7420 3d20 696e 6974 6961 6c5f 6372 6564  t = initial_cred
-00001070: 7320 6f72 2043 7265 6465 6e74 6961 6c73  s or Credentials
-00001080: 2827 272c 2027 272c 2027 2729 0a20 2020  ('', '', '').   
-00001090: 2070 696e 7320 3d20 5b0a 2020 2020 2020   pins = [.      
-000010a0: 2020 7075 745f 6d61 726b 646f 776e 2827    put_markdown('
-000010b0: 5f54 6869 7320 696e 666f 726d 6174 696f  _This informatio
-000010c0: 6e20 6973 206e 6565 6465 6420 746f 2063  n is needed to c
-000010d0: 7265 6174 6520 6120 464f 4c49 4f20 4150  reate a FOLIO AP
-000010e0: 4920 746f 6b65 6e2e 270a 2020 2020 2020  I token.'.      
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001100: 2059 6f75 7220 464f 4c49 4f20 6c6f 6769   Your FOLIO logi
-00001110: 6e20 2620 7061 7373 776f 7264 2077 696c  n & password wil
-00001120: 6c5f 270a 2020 2020 2020 2020 2020 2020  l_'.            
-00001130: 2020 2020 2020 2020 2027 202a 2a6e 6f74           ' **not
-00001140: 2a2a 205f 6265 2073 746f 7265 6420 6166  ** _be stored af
-00001150: 7465 7220 7468 6973 2066 6f72 6d20 6469  ter this form di
-00001160: 7361 7070 6561 7273 3b20 6f6e 6c79 270a  sappears; only'.
-00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001180: 2020 2020 2027 2074 6865 2074 6f6b 656e       ' the token
-00001190: 2c20 5552 4c20 616e 6420 7465 6e61 6e74  , URL and tenant
-000011a0: 2069 6420 7769 6c6c 2062 6520 7374 6f72   id will be stor
-000011b0: 6564 2e5f 2729 2c0a 2020 2020 2020 2020  ed._'),.        
-000011c0: 7075 745f 696e 7075 7428 2775 7365 7227  put_input('user'
-000011d0: 2c20 2020 2020 206c 6162 656c 203d 2027  ,      label = '
-000011e0: 464f 4c49 4f20 7573 6572 206e 616d 6527  FOLIO user name'
-000011f0: 292c 0a20 2020 2020 2020 2070 7574 5f69  ),.        put_i
-00001200: 6e70 7574 2827 7061 7373 776f 7264 272c  nput('password',
-00001210: 2020 6c61 6265 6c20 3d20 2746 4f4c 494f    label = 'FOLIO
-00001220: 2070 6173 7377 6f72 6427 2c20 7479 7065   password', type
-00001230: 203d 2027 7061 7373 776f 7264 2729 2c0a   = 'password'),.
-00001240: 2020 2020 2020 2020 7075 745f 696e 7075          put_inpu
-00001250: 7428 2775 726c 272c 2020 2020 2020 206c  t('url',       l
-00001260: 6162 656c 203d 2027 4f4b 4150 4920 5552  abel = 'OKAPI UR
-00001270: 4c27 2c20 7661 6c75 6520 3d20 6375 7272  L', value = curr
-00001280: 656e 742e 7572 6c29 2c0a 2020 2020 2020  ent.url),.      
-00001290: 2020 7075 745f 696e 7075 7428 2774 656e    put_input('ten
-000012a0: 616e 745f 6964 272c 206c 6162 656c 203d  ant_id', label =
-000012b0: 2027 5465 6e61 6e74 2069 6427 2c20 7661   'Tenant id', va
-000012c0: 6c75 6520 3d20 6375 7272 656e 742e 7465  lue = current.te
-000012d0: 6e61 6e74 5f69 6429 2c0a 2020 2020 2020  nant_id),.      
-000012e0: 2020 7075 745f 6275 7474 6f6e 7328 5b0a    put_buttons([.
-000012f0: 2020 2020 2020 2020 2020 2020 7b27 6c61              {'la
-00001300: 6265 6c27 3a20 2753 7562 6d69 7427 2c20  bel': 'Submit', 
-00001310: 2776 616c 7565 273a 2054 7275 657d 2c0a  'value': True},.
-00001320: 2020 2020 2020 2020 2020 2020 7b27 6c61              {'la
-00001330: 6265 6c27 3a20 2743 616e 6365 6c27 2c20  bel': 'Cancel', 
-00001340: 2776 616c 7565 273a 2046 616c 7365 2c20  'value': False, 
-00001350: 2763 6f6c 6f72 273a 2027 6461 6e67 6572  'color': 'danger
-00001360: 277d 2c0a 2020 2020 2020 2020 5d2c 206f  '},.        ], o
-00001370: 6e63 6c69 636b 203d 2063 6c6b 292e 7374  nclick = clk).st
-00001380: 796c 6528 2766 6c6f 6174 3a20 7269 6768  yle('float: righ
-00001390: 7427 290a 2020 2020 5d0a 2020 2020 706f  t').    ].    po
-000013a0: 7075 7028 7469 746c 6520 3d20 2746 4f4c  pup(title = 'FOL
-000013b0: 494f 2063 7265 6465 6e74 6961 6c73 272c  IO credentials',
-000013c0: 2063 6f6e 7465 6e74 203d 2070 696e 732c   content = pins,
-000013d0: 2073 697a 6520 3d20 276d 6564 6975 6d27   size = 'medium'
-000013e0: 2c0a 2020 2020 2020 2020 2020 636c 6f73  ,.          clos
-000013f0: 6162 6c65 203d 2046 616c 7365 290a 0a20  able = False).. 
-00001400: 2020 2065 7665 6e74 2e77 6169 7428 290a     event.wait().
-00001410: 2020 2020 636c 6f73 655f 706f 7075 7028      close_popup(
-00001420: 290a 2020 2020 7761 6974 2830 2e35 2920  ).    wait(0.5) 
-00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001440: 2020 2020 2020 2020 2020 2320 4769 7665            # Give
-00001450: 2074 696d 6520 666f 7220 706f 7075 7020   time for popup 
-00001460: 746f 2067 6f20 6177 6179 2e0a 0a20 2020  to go away...   
-00001470: 2069 6620 6e6f 7420 636c 6963 6b65 645f   if not clicked_
-00001480: 6f6b 3a0a 2020 2020 2020 2020 6c6f 6728  ok:.        log(
-00001490: 2775 7365 7220 6361 6e63 656c 6c65 6420  'user cancelled 
-000014a0: 6f75 7420 6f66 2063 7265 6465 6e74 6961  out of credentia
-000014b0: 6c73 2064 6961 6c6f 6727 290a 2020 2020  ls dialog').    
-000014c0: 2020 2020 7265 7475 726e 2069 6e69 7469      return initi
-000014d0: 616c 5f63 7265 6473 0a0a 2020 2020 6966  al_creds..    if
-000014e0: 2070 696e 2e75 726c 3a20 2020 2020 2020   pin.url:       
-000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001500: 2020 2320 5265 6d6f 7665 2027 2f27 2069    # Remove '/' i
-00001510: 6620 7468 6520 7573 6572 2069 6e63 6c75  f the user inclu
-00001520: 6465 6420 6974 2e0a 2020 2020 2020 2020  ded it..        
-00001530: 7069 6e2e 7572 6c20 3d20 7069 6e2e 7572  pin.url = pin.ur
-00001540: 6c2e 7273 7472 6970 2827 2f27 290a 0a20  l.rstrip('/').. 
-00001550: 2020 2069 6620 6e6f 7420 616c 6c28 5b70     if not all([p
-00001560: 696e 2e75 726c 2c20 7069 6e2e 7465 6e61  in.url, pin.tena
-00001570: 6e74 5f69 642c 2070 696e 2e75 7365 722c  nt_id, pin.user,
-00001580: 2070 696e 2e70 6173 7377 6f72 645d 293a   pin.password]):
-00001590: 0a20 2020 2020 2020 2069 6620 7761 726e  .        if warn
-000015a0: 5f65 6d70 7479 3a0a 2020 2020 2020 2020  _empty:.        
-000015b0: 2020 2020 6c6f 6728 2775 7365 7220 7072      log('user pr
-000015c0: 6f76 6964 6564 2069 6e63 6f6d 706c 6574  ovided incomplet
-000015d0: 6520 6372 6564 656e 7469 616c 7327 290a  e credentials').
-000015e0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-000015f0: 6f6e 6669 726d 2827 4361 6e6e 6f74 2070  onfirm('Cannot p
-00001600: 726f 6365 6564 2077 6974 686f 7574 2061  roceed without a
-00001610: 6c6c 2063 7265 6465 6e74 6961 6c73 2e20  ll credentials. 
-00001620: 5472 7920 6167 6169 6e3f 2729 3a0a 2020  Try again?'):.  
-00001630: 2020 2020 2020 2020 2020 2020 2020 746d                tm
-00001640: 7020 3d20 4372 6564 656e 7469 616c 7328  p = Credentials(
-00001650: 7572 6c20 3d20 7069 6e2e 7572 6c2c 2074  url = pin.url, t
-00001660: 656e 616e 745f 6964 203d 2070 696e 2e74  enant_id = pin.t
-00001670: 656e 616e 745f 6964 2c20 746f 6b65 6e20  enant_id, token 
-00001680: 3d20 4e6f 6e65 290a 2020 2020 2020 2020  = None).        
-00001690: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-000016a0: 7265 6465 6e74 6961 6c73 5f66 726f 6d5f  redentials_from_
-000016b0: 7573 6572 2869 6e69 7469 616c 5f63 7265  user(initial_cre
-000016c0: 6473 203d 2074 6d70 290a 2020 2020 2020  ds = tmp).      
-000016d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000016e0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-000016f0: 0a20 2020 2077 6974 6820 7075 745f 6c6f  .    with put_lo
-00001700: 6164 696e 6728 293a 0a20 2020 2020 2020  ading():.       
-00001710: 2074 6f6b 656e 2c20 6572 726f 7220 3d20   token, error = 
-00001720: 466f 6c69 6f2e 6e65 775f 746f 6b65 6e28  Folio.new_token(
-00001730: 7572 6c20 3d20 7069 6e2e 7572 6c2c 2074  url = pin.url, t
-00001740: 656e 616e 745f 6964 203d 2070 696e 2e74  enant_id = pin.t
-00001750: 656e 616e 745f 6964 2c0a 2020 2020 2020  enant_id,.      
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001780: 2075 7365 7220 3d20 7069 6e2e 7573 6572   user = pin.user
-00001790: 2c20 7061 7373 776f 7264 203d 2070 696e  , password = pin
-000017a0: 2e70 6173 7377 6f72 6429 0a0a 2020 2020  .password)..    
-000017b0: 6966 2065 7272 6f72 3a0a 2020 2020 2020  if error:.      
-000017c0: 2020 6e6f 7469 6679 2827 4661 696c 6564    notify('Failed
-000017d0: 2074 6f20 6765 7420 6120 746f 6b65 6e3a   to get a token:
-000017e0: 2027 202b 2065 7272 6f72 202b 2027 2e27   ' + error + '.'
-000017f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00001800: 204e 6f6e 650a 2020 2020 656c 7365 3a0a   None.    else:.
-00001810: 2020 2020 2020 2020 6e6f 7465 5f69 6e66          note_inf
-00001820: 6f28 274e 6577 2046 4f4c 494f 2041 5049  o('New FOLIO API
-00001830: 2074 6f6b 656e 206f 6274 6169 6e65 642e   token obtained.
-00001840: 2729 0a0a 2020 2020 6c6f 6728 2767 6f74  ')..    log('got
-00001850: 2063 7265 6465 6e74 6961 6c73 2066 726f   credentials fro
-00001860: 6d20 7573 6572 2729 0a20 2020 2072 6574  m user').    ret
-00001870: 7572 6e20 4372 6564 656e 7469 616c 7328  urn Credentials(
-00001880: 7572 6c20 3d20 7069 6e2e 7572 6c2c 2074  url = pin.url, t
-00001890: 656e 616e 745f 6964 203d 2070 696e 2e74  enant_id = pin.t
-000018a0: 656e 616e 745f 6964 2c20 746f 6b65 6e20  enant_id, token 
-000018b0: 3d20 746f 6b65 6e29 0a0a 0a23 2045 7870  = token)...# Exp
-000018c0: 6c61 6e61 7469 6f6e 2061 626f 7574 2074  lanation about t
-000018d0: 6865 2077 6569 7264 2077 6179 2074 6869  he weird way thi
-000018e0: 7320 6973 2064 6f6e 653a 2074 6865 2050  s is done: the P
-000018f0: 7974 686f 6e20 6b65 7972 696e 6720 6d6f  ython keyring mo
-00001900: 6475 6c65 0a23 206f 6e6c 7920 6f66 6665  dule.# only offe
-00001910: 7273 2061 2073 696e 676c 6520 6675 6e63  rs a single func
-00001920: 7469 6f6e 2066 6f72 2073 6574 7469 6e67  tion for setting
-00001930: 2061 2076 616c 7565 3b20 6f73 7465 6e73   a value; ostens
-00001940: 6962 6c79 2c20 7468 6973 2069 730a 2320  ibly, this is.# 
-00001950: 696e 7465 6e64 6564 2074 6f20 7374 6f72  intended to stor
-00001960: 6520 6120 7061 7373 776f 7264 2061 7373  e a password ass
-00001970: 6f63 6961 7465 6420 7769 7468 2061 6e20  ociated with an 
-00001980: 6964 656e 7469 6669 6572 2028 6120 7573  identifier (a us
-00001990: 6572 206e 616d 6529 2c0a 2320 616e 6420  er name),.# and 
-000019a0: 7468 6973 2069 6465 6e74 6966 6965 7220  this identifier 
-000019b0: 6973 2065 7870 6563 7465 6420 746f 2062  is expected to b
-000019c0: 6520 6f62 7461 696e 6564 2073 6f6d 6520  e obtained some 
-000019d0: 6f74 6865 7220 7761 792c 2073 7563 6820  other way, such 
-000019e0: 6173 2062 790a 2320 7573 696e 6720 7468  as by.# using th
-000019f0: 6520 6375 7272 656e 7420 7573 6572 2773  e current user's
-00001a00: 2063 6f6d 7075 7465 7220 6c6f 6769 6e20   computer login 
-00001a10: 6e61 6d65 2e20 2042 7574 2c20 696e 206f  name.  But, in o
-00001a20: 7572 2073 6974 7561 7469 6f6e 2c20 7765  ur situation, we
-00001a30: 0a23 2068 6176 6520 6d75 6c74 6970 6c65  .# have multiple
-00001a40: 2070 6965 6365 7320 6f66 2069 6e66 6f72   pieces of infor
-00001a50: 6d61 7469 6f6e 2077 6520 6861 7665 2074  mation we have t
-00001a60: 6f20 7374 6f72 6520 2861 2075 7365 7220  o store (a user 
-00001a70: 6964 2061 6e64 2061 6e20 6170 690a 2320  id and an api.# 
-00001a80: 6b65 7929 2e20 2054 6865 2068 6163 6b61  key).  The hacka
-00001a90: 6369 6f75 7320 736f 6c75 7469 6f6e 2074  cious solution t
-00001aa0: 616b 656e 2068 6572 6520 6973 2074 6f20  aken here is to 
-00001ab0: 636f 6e63 6174 656e 6174 6520 7468 6520  concatenate the 
-00001ac0: 7661 6c75 6573 2069 6e74 6f0a 2320 6120  values into.# a 
-00001ad0: 7369 6e67 6c65 2073 7472 696e 6720 7573  single string us
-00001ae0: 6564 2061 7320 7468 6520 6163 7475 616c  ed as the actual
-00001af0: 2076 616c 7565 2073 746f 7265 642e 2020   value stored.  
-00001b00: 5468 6520 696e 6469 7669 6475 616c 2076  The individual v
-00001b10: 616c 7565 7320 6172 650a 2320 7365 7061  alues are.# sepa
-00001b20: 7261 7465 6420 6279 2061 2063 6861 7261  rated by a chara
-00001b30: 6374 6572 2074 6861 7420 6973 2075 6e6c  cter that is unl
-00001b40: 696b 656c 7920 746f 2062 6520 7061 7274  ikely to be part
-00001b50: 206f 6620 616e 7920 7573 6572 2d74 7970   of any user-typ
-00001b60: 6564 2076 616c 7565 2e0a 0a64 6566 2063  ed value...def c
-00001b70: 7265 6465 6e74 6961 6c73 5f66 726f 6d5f  redentials_from_
-00001b80: 6b65 7972 696e 6728 7061 7274 6961 6c5f  keyring(partial_
-00001b90: 6f6b 203d 2046 616c 7365 2c20 7269 6e67  ok = False, ring
-00001ba0: 203d 205f 4b45 5952 494e 4729 3a0a 2020   = _KEYRING):.  
-00001bb0: 2020 2727 274c 6f6f 6b20 7570 2074 6865    '''Look up the
-00001bc0: 2075 7365 7227 7320 6372 6564 656e 7469   user's credenti
-00001bd0: 616c 732e 0a20 2020 2049 6620 7061 7274  als..    If part
-00001be0: 6961 6c5f 6f6b 2069 7320 4661 6c73 652c  ial_ok is False,
-00001bf0: 2072 6574 7572 6e20 4e6f 6e65 2069 6620   return None if 
-00001c00: 7468 6520 6b65 7972 696e 6720 7661 6c75  the keyring valu
-00001c10: 6520 6973 2069 6e63 6f6d 706c 6574 652e  e is incomplete.
-00001c20: 2727 270a 2020 2020 6966 2073 7973 2e70  '''.    if sys.p
-00001c30: 6c61 7466 6f72 6d2e 7374 6172 7473 7769  latform.startswi
-00001c40: 7468 2827 7769 6e27 293a 0a20 2020 2020  th('win'):.     
-00001c50: 2020 206c 6f67 2827 7573 696e 6720 7769     log('using wi
-00001c60: 6e64 6f77 7320 6b65 7972 696e 6720 7661  ndows keyring va
-00001c70: 756c 7427 290a 2020 2020 2020 2020 6b65  ult').        ke
-00001c80: 7972 696e 672e 7365 745f 6b65 7972 696e  yring.set_keyrin
-00001c90: 6728 5769 6e56 6175 6c74 4b65 7972 696e  g(WinVaultKeyrin
-00001ca0: 6728 2929 0a20 2020 2069 6620 7379 732e  g()).    if sys.
-00001cb0: 706c 6174 666f 726d 2e73 7461 7274 7377  platform.startsw
-00001cc0: 6974 6828 2764 6172 7769 6e27 293a 0a20  ith('darwin'):. 
-00001cd0: 2020 2020 2020 206c 6f67 2827 7573 696e         log('usin
-00001ce0: 6720 6d61 636f 7320 6b65 7972 696e 6727  g macos keyring'
-00001cf0: 290a 2020 2020 2020 2020 6b65 7972 696e  ).        keyrin
-00001d00: 672e 7365 745f 6b65 7972 696e 6728 4b65  g.set_keyring(Ke
-00001d10: 7972 696e 6728 2929 0a20 2020 206c 6f67  yring()).    log
-00001d20: 2866 2774 7279 696e 6720 746f 2072 6561  (f'trying to rea
-00001d30: 6420 7661 6c75 6520 6672 6f6d 207b 7269  d value from {ri
-00001d40: 6e67 7d27 290a 2020 2020 7472 793a 0a20  ng}').    try:. 
-00001d50: 2020 2020 2020 2076 616c 7565 203d 206b         value = k
-00001d60: 6579 7269 6e67 2e67 6574 5f70 6173 7377  eyring.get_passw
-00001d70: 6f72 6428 7269 6e67 2c20 6765 7470 6173  ord(ring, getpas
-00001d80: 732e 6765 7475 7365 7228 2929 0a20 2020  s.getuser()).   
-00001d90: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00001da0: 6e20 6173 2065 783a 2020 2020 2020 2020  n as ex:        
-00001db0: 2020 2020 2023 206e 6f71 613a 2050 4945       # noqa: PIE
-00001dc0: 3738 360a 2020 2020 2020 2020 6c6f 6728  786.        log(
-00001dd0: 2765 7863 6570 7469 6f6e 2074 7279 696e  'exception tryin
-00001de0: 6720 746f 2067 6574 2070 6173 7377 6f72  g to get passwor
-00001df0: 6420 6672 6f6d 206b 6579 7269 6e67 3a20  d from keyring: 
-00001e00: 2720 2b20 7374 7228 6578 2929 0a20 2020  ' + str(ex)).   
-00001e10: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00001e20: 0a20 2020 2069 6620 7661 6c75 653a 0a20  .    if value:. 
-00001e30: 2020 2020 2020 206c 6f67 2866 2767 6f74         log(f'got
-00001e40: 2063 7265 6465 6e74 6961 6c73 2066 726f   credentials fro
-00001e50: 6d20 6b65 7972 696e 6720 7b72 696e 677d  m keyring {ring}
-00001e60: 2729 0a20 2020 2020 2020 2070 6172 7473  ').        parts
-00001e70: 203d 205f 6465 636f 6465 6428 7661 6c75   = _decoded(valu
-00001e80: 6529 0a20 2020 2020 2020 2069 6620 616c  e).        if al
-00001e90: 6c28 7061 7274 7329 206f 7220 7061 7274  l(parts) or part
-00001ea0: 6961 6c5f 6f6b 3a0a 2020 2020 2020 2020  ial_ok:.        
-00001eb0: 2020 2020 7265 7475 726e 2043 7265 6465      return Crede
-00001ec0: 6e74 6961 6c73 2875 726c 203d 2070 6172  ntials(url = par
-00001ed0: 7473 5b30 5d2c 2074 656e 616e 745f 6964  ts[0], tenant_id
-00001ee0: 203d 2070 6172 7473 5b31 5d2c 2074 6f6b   = parts[1], tok
-00001ef0: 656e 203d 2070 6172 7473 5b32 5d29 0a20  en = parts[2]). 
-00001f00: 2020 206c 6f67 2866 2764 6964 206e 6f74     log(f'did not
-00001f10: 2066 696e 6420 6120 7661 6c75 6520 696e   find a value in
-00001f20: 206b 6579 7269 6e67 207b 7269 6e67 7d27   keyring {ring}'
-00001f30: 290a 2020 2020 7265 7475 726e 204e 6f6e  ).    return Non
-00001f40: 650a 0a0a 6465 6620 7573 655f 6372 6564  e...def use_cred
-00001f50: 656e 7469 616c 7328 6372 6564 7329 3a0a  entials(creds):.
-00001f60: 2020 2020 2727 2753 6574 2072 756e 2d74      '''Set run-t
-00001f70: 696d 6520 656e 7669 726f 6e6d 656e 7420  ime environment 
-00001f80: 6372 6564 656e 7469 616c 7320 616e 6420  credentials and 
-00001f90: 7361 7665 2074 6865 6d20 746f 2074 6865  save them to the
-00001fa0: 206b 6579 7269 6e67 2e27 2727 0a20 2020   keyring.'''.   
-00001fb0: 206c 6f67 2827 7365 7474 696e 6720 656e   log('setting en
-00001fc0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00001fd0: 6c65 7320 666f 7220 6372 6564 656e 7469  les for credenti
-00001fe0: 616c 7327 290a 2020 2020 6f73 2e65 6e76  als').    os.env
-00001ff0: 6972 6f6e 5b27 464f 4c49 4f5f 4f4b 4150  iron['FOLIO_OKAP
-00002000: 495f 5552 4c27 5d20 2020 2020 2020 3d20  I_URL']       = 
-00002010: 6372 6564 732e 7572 6c0a 2020 2020 6f73  creds.url.    os
-00002020: 2e65 6e76 6972 6f6e 5b27 464f 4c49 4f5f  .environ['FOLIO_
-00002030: 4f4b 4150 495f 5445 4e41 4e54 5f49 4427  OKAPI_TENANT_ID'
-00002040: 5d20 3d20 6372 6564 732e 7465 6e61 6e74  ] = creds.tenant
-00002050: 5f69 640a 2020 2020 6f73 2e65 6e76 6972  _id.    os.envir
-00002060: 6f6e 5b27 464f 4c49 4f5f 4f4b 4150 495f  on['FOLIO_OKAPI_
-00002070: 544f 4b45 4e27 5d20 2020 2020 3d20 6372  TOKEN']     = cr
-00002080: 6564 732e 746f 6b65 6e0a 2020 2020 6966  eds.token.    if
-00002090: 2063 6f6e 6669 6728 2755 5345 5f4b 4559   config('USE_KEY
-000020a0: 5249 4e47 272c 2063 6173 7420 3d20 626f  RING', cast = bo
-000020b0: 6f6c 293a 0a20 2020 2020 2020 206b 6579  ol):.        key
-000020c0: 7269 6e67 5f63 7265 6473 203d 2063 7265  ring_creds = cre
-000020d0: 6465 6e74 6961 6c73 5f66 726f 6d5f 6b65  dentials_from_ke
-000020e0: 7972 696e 6728 290a 2020 2020 2020 2020  yring().        
-000020f0: 6966 2063 7265 6473 2021 3d20 6b65 7972  if creds != keyr
-00002100: 696e 675f 6372 6564 733a 0a20 2020 2020  ing_creds:.     
-00002110: 2020 2020 2020 205f 7374 6f72 655f 6372         _store_cr
-00002120: 6564 656e 7469 616c 7328 6372 6564 7329  edentials(creds)
-00002130: 0a0a 0a64 6566 2063 7572 7265 6e74 5f63  ...def current_c
-00002140: 7265 6465 6e74 6961 6c73 2829 3a0a 2020  redentials():.  
-00002150: 2020 7572 6c20 2020 2020 2020 3d20 636f    url       = co
-00002160: 6e66 6967 2827 464f 4c49 4f5f 4f4b 4150  nfig('FOLIO_OKAP
-00002170: 495f 5552 4c27 2c20 6465 6661 756c 7420  I_URL', default 
-00002180: 3d20 4e6f 6e65 290a 2020 2020 7465 6e61  = None).    tena
-00002190: 6e74 5f69 6420 3d20 636f 6e66 6967 2827  nt_id = config('
-000021a0: 464f 4c49 4f5f 4f4b 4150 495f 5445 4e41  FOLIO_OKAPI_TENA
-000021b0: 4e54 5f49 4427 2c20 6465 6661 756c 7420  NT_ID', default 
-000021c0: 3d20 4e6f 6e65 290a 2020 2020 746f 6b65  = None).    toke
-000021d0: 6e20 2020 2020 3d20 636f 6e66 6967 2827  n     = config('
-000021e0: 464f 4c49 4f5f 4f4b 4150 495f 544f 4b45  FOLIO_OKAPI_TOKE
-000021f0: 4e27 2c20 6465 6661 756c 7420 3d20 4e6f  N', default = No
-00002200: 6e65 290a 2020 2020 7265 7475 726e 2043  ne).    return C
-00002210: 7265 6465 6e74 6961 6c73 2875 726c 203d  redentials(url =
-00002220: 2075 726c 2c20 7465 6e61 6e74 5f69 6420   url, tenant_id 
-00002230: 3d20 7465 6e61 6e74 5f69 642c 2074 6f6b  = tenant_id, tok
-00002240: 656e 203d 2074 6f6b 656e 290a 0a0a 6465  en = token)...de
-00002250: 6620 6372 6564 656e 7469 616c 735f 636f  f credentials_co
-00002260: 6d70 6c65 7465 2863 7265 6473 293a 0a20  mplete(creds):. 
-00002270: 2020 2027 2727 5265 7475 726e 2054 7275     '''Return Tru
-00002280: 6520 6966 2074 6865 2067 6976 656e 2063  e if the given c
-00002290: 7265 6465 6e74 6961 6c73 2061 7265 2063  redentials are c
-000022a0: 6f6d 706c 6574 652e 2727 270a 2020 2020  omplete.'''.    
-000022b0: 7265 7475 726e 2028 6372 6564 7320 616e  return (creds an
-000022c0: 6420 6372 6564 732e 7572 6c20 616e 6420  d creds.url and 
-000022d0: 6372 6564 732e 7465 6e61 6e74 5f69 6420  creds.tenant_id 
-000022e0: 616e 6420 6372 6564 732e 746f 6b65 6e29  and creds.token)
-000022f0: 0a0a 0c0a 2320 5072 6976 6174 6520 6865  ....# Private he
-00002300: 6c70 6572 2066 756e 6374 696f 6e73 2e0a  lper functions..
-00002310: 2320 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  # ..............
-00002320: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00002330: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00002340: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00002350: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e0a  ................
-00002360: 0a5f 5345 5020 3d20 2703 270a 2727 2743  ._SEP = '.'.'''C
-00002370: 6861 7261 6374 6572 2075 7365 6420 746f  haracter used to
-00002380: 2073 6570 6172 6174 6520 6d75 6c74 6970   separate multip
-00002390: 6c65 2061 6374 7561 6c20 7661 6c75 6573  le actual values
-000023a0: 2073 746f 7265 6420 6173 2061 2073 696e   stored as a sin
-000023b0: 676c 650a 656e 636f 6465 6420 7661 6c75  gle.encoded valu
-000023c0: 6520 7374 7269 6e67 2e20 2054 6869 7320  e string.  This 
-000023d0: 6368 6172 6163 7465 7220 6973 2064 656c  character is del
-000023e0: 6962 6572 6174 656c 7920 6368 6f73 656e  iberately chosen
-000023f0: 2074 6f20 6265 2073 6f6d 6574 6869 6e67   to be something
-00002400: 0a76 6572 7920 756e 6c69 6b65 6c79 2074  .very unlikely t
-00002410: 6f20 6265 2070 6172 7420 6f66 2061 206c  o be part of a l
-00002420: 6567 6974 696d 6174 6520 7374 7269 6e67  egitimate string
-00002430: 2076 616c 7565 2074 7970 6564 2062 7920   value typed by 
-00002440: 7573 6572 2061 7420 610a 7368 656c 6c20  user at a.shell 
-00002450: 7072 6f6d 7074 2c20 6265 6361 7573 6520  prompt, because 
-00002460: 636f 6e74 726f 6c2d 6320 6973 206e 6f72  control-c is nor
-00002470: 6d61 6c6c 7920 7573 6564 2074 6f20 696e  mally used to in
-00002480: 7465 7272 7570 7420 7072 6f67 7261 6d73  terrupt programs
-00002490: 2e0a 2727 270a 0a0a 6465 6620 5f65 6e63  ..'''...def _enc
-000024a0: 6f64 6564 2875 726c 2c20 7465 6e61 6e74  oded(url, tenant
-000024b0: 5f69 642c 2074 6f6b 656e 293a 0a20 2020  _id, token):.   
-000024c0: 2072 6574 7572 6e20 6627 7b75 726c 7d7b   return f'{url}{
-000024d0: 5f53 4550 7d7b 7465 6e61 6e74 5f69 647d  _SEP}{tenant_id}
-000024e0: 7b5f 5345 507d 7b74 6f6b 656e 7d27 0a0a  {_SEP}{token}'..
-000024f0: 0a64 6566 205f 6465 636f 6465 6428 7661  .def _decoded(va
-00002500: 6c75 655f 7374 7269 6e67 293a 0a20 2020  lue_string):.   
-00002510: 2072 6574 7572 6e20 7475 706c 6528 7661   return tuple(va
-00002520: 6c75 655f 7374 7269 6e67 2e73 706c 6974  lue_string.split
-00002530: 285f 5345 5029 290a 0a0a 6465 6620 5f63  (_SEP))...def _c
-00002540: 7265 6473 5f66 726f 6d5f 736f 7572 6365  reds_from_source
-00002550: 2873 6f75 7263 6520 3d20 4e6f 6e65 2c20  (source = None, 
-00002560: 7768 6572 6520 3d20 2727 293a 0a20 2020  where = ''):.   
-00002570: 2069 6620 6e6f 7420 736f 7572 6365 3a0a   if not source:.
-00002580: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00002590: 6f6e 650a 2020 2020 7572 6c20 2020 2020  one.    url     
-000025a0: 2020 3d20 736f 7572 6365 2e67 6574 2827    = source.get('
-000025b0: 464f 4c49 4f5f 4f4b 4150 495f 5552 4c27  FOLIO_OKAPI_URL'
-000025c0: 2c20 6465 6661 756c 7420 3d20 4e6f 6e65  , default = None
-000025d0: 290a 2020 2020 7465 6e61 6e74 5f69 6420  ).    tenant_id 
-000025e0: 3d20 736f 7572 6365 2e67 6574 2827 464f  = source.get('FO
-000025f0: 4c49 4f5f 4f4b 4150 495f 5445 4e41 4e54  LIO_OKAPI_TENANT
-00002600: 5f49 4427 2c20 6465 6661 756c 7420 3d20  _ID', default = 
-00002610: 4e6f 6e65 290a 2020 2020 746f 6b65 6e20  None).    token 
-00002620: 2020 2020 3d20 736f 7572 6365 2e67 6574      = source.get
-00002630: 2827 464f 4c49 4f5f 4f4b 4150 495f 544f  ('FOLIO_OKAPI_TO
-00002640: 4b45 4e27 2c20 6465 6661 756c 7420 3d20  KEN', default = 
-00002650: 4e6f 6e65 290a 2020 2020 6966 206e 6f74  None).    if not
-00002660: 2061 6e79 285b 7572 6c2c 2074 656e 616e   any([url, tenan
-00002670: 745f 6964 2c20 746f 6b65 6e5d 293a 0a20  t_id, token]):. 
-00002680: 2020 2020 2020 206c 6f67 2866 276e 6f20         log(f'no 
-00002690: 6372 6564 656e 7469 616c 7320 666f 756e  credentials foun
-000026a0: 6420 696e 207b 7768 6572 657d 2729 0a20  d in {where}'). 
-000026b0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-000026c0: 6e65 0a20 2020 2063 7265 6473 203d 2043  ne.    creds = C
-000026d0: 7265 6465 6e74 6961 6c73 2875 726c 203d  redentials(url =
-000026e0: 2075 726c 2c20 7465 6e61 6e74 5f69 6420   url, tenant_id 
-000026f0: 3d20 7465 6e61 6e74 5f69 642c 2074 6f6b  = tenant_id, tok
-00002700: 656e 203d 2074 6f6b 656e 290a 2020 2020  en = token).    
-00002710: 636f 6d70 6c65 7465 203d 2027 636f 6d70  complete = 'comp
-00002720: 6c65 7465 2720 6966 2063 7265 6465 6e74  lete' if credent
-00002730: 6961 6c73 5f63 6f6d 706c 6574 6528 6372  ials_complete(cr
-00002740: 6564 7329 2065 6c73 6520 276e 6f74 2063  eds) else 'not c
-00002750: 6f6d 706c 6574 6527 0a20 2020 206c 6f67  omplete'.    log
-00002760: 2866 2763 7265 6465 6e74 6961 6c73 2069  (f'credentials i
-00002770: 6e20 7b77 6865 7265 7d20 6172 6520 7b63  n {where} are {c
-00002780: 6f6d 706c 6574 657d 2729 0a20 2020 2072  omplete}').    r
-00002790: 6574 7572 6e20 6372 6564 730a 0a0a 6465  eturn creds...de
-000027a0: 6620 5f73 746f 7265 5f63 7265 6465 6e74  f _store_credent
-000027b0: 6961 6c73 2863 7265 6473 2c20 7269 6e67  ials(creds, ring
-000027c0: 203d 205f 4b45 5952 494e 4729 3a0a 2020   = _KEYRING):.  
-000027d0: 2020 2727 2753 6176 6520 7468 6520 7573    '''Save the us
-000027e0: 6572 2773 2063 7265 6465 6e74 6961 6c73  er's credentials
-000027f0: 2e27 2727 0a20 2020 2069 6620 7379 732e  .'''.    if sys.
-00002800: 706c 6174 666f 726d 2e73 7461 7274 7377  platform.startsw
-00002810: 6974 6828 2777 696e 2729 3a0a 2020 2020  ith('win'):.    
-00002820: 2020 2020 6b65 7972 696e 672e 7365 745f      keyring.set_
-00002830: 6b65 7972 696e 6728 5769 6e56 6175 6c74  keyring(WinVault
-00002840: 4b65 7972 696e 6728 2929 0a20 2020 2069  Keyring()).    i
-00002850: 6620 7379 732e 706c 6174 666f 726d 2e73  f sys.platform.s
-00002860: 7461 7274 7377 6974 6828 2764 6172 7769  tartswith('darwi
-00002870: 6e27 293a 0a20 2020 2020 2020 206b 6579  n'):.        key
-00002880: 7269 6e67 2e73 6574 5f6b 6579 7269 6e67  ring.set_keyring
-00002890: 284b 6579 7269 6e67 2829 290a 2020 2020  (Keyring()).    
-000028a0: 7661 6c75 6520 3d20 5f65 6e63 6f64 6564  value = _encoded
-000028b0: 2863 7265 6473 2e75 726c 2c20 6372 6564  (creds.url, cred
-000028c0: 732e 7465 6e61 6e74 5f69 642c 2063 7265  s.tenant_id, cre
-000028d0: 6473 2e74 6f6b 656e 290a 2020 2020 6c6f  ds.token).    lo
-000028e0: 6728 6627 7374 6f72 696e 6720 6372 6564  g(f'storing cred
-000028f0: 656e 7469 616c 7320 746f 206b 6579 7269  entials to keyri
-00002900: 6e67 207b 5f4b 4559 5249 4e47 7d27 290a  ng {_KEYRING}').
-00002910: 2020 2020 6b65 7972 696e 672e 7365 745f      keyring.set_
-00002920: 7061 7373 776f 7264 2872 696e 672c 2067  password(ring, g
-00002930: 6574 7061 7373 2e67 6574 7573 6572 2829  etpass.getuser()
-00002940: 2c20 7661 6c75 6529 0a                   , value).
+00000b90: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000ba0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000bb0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000bc0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e0a 0a64 6566  .............def
+00000bd0: 2063 7265 6465 6e74 6961 6c73 5f66 726f   credentials_fro
+00000be0: 6d5f 6669 6c65 2863 7265 6473 5f66 696c  m_file(creds_fil
+00000bf0: 6529 3a0a 2020 2020 2727 2752 6574 7572  e):.    '''Retur
+00000c00: 6e20 6120 4372 6564 656e 7469 616c 7320  n a Credentials 
+00000c10: 6f62 6a65 6374 2063 7265 6174 6564 2066  object created f
+00000c20: 726f 6d20 7661 6c75 6573 2069 6e20 6372  rom values in cr
+00000c30: 6564 735f 6669 6c65 2e0a 0a20 2020 2054  eds_file...    T
+00000c40: 6865 2063 7265 6465 6e74 6961 6c73 2066  he credentials f
+00000c50: 696c 6520 6d75 7374 2062 6520 696e 2022  ile must be in "
+00000c60: 2e69 6e69 2220 666f 726d 6174 2c20 6c69  .ini" format, li
+00000c70: 6b65 2074 6869 733a 0a0a 2020 2020 5b73  ke this:..    [s
+00000c80: 6574 7469 6e67 735d 0a20 2020 2046 4f4c  ettings].    FOL
+00000c90: 494f 5f4f 4b41 5049 5f55 524c 203d 202e  IO_OKAPI_URL = .
+00000ca0: 2e2e 2e2e 0a20 2020 2046 4f4c 494f 5f4f  .....    FOLIO_O
+00000cb0: 4b41 5049 5f54 454e 414e 545f 4944 203d  KAPI_TENANT_ID =
+00000cc0: 202e 2e2e 2e2e 0a20 2020 2046 4f4c 494f   ......    FOLIO
+00000cd0: 5f4f 4b41 5049 5f54 4f4b 454e 203d 202e  _OKAPI_TOKEN = .
+00000ce0: 2e2e 2e2e 0a20 2020 2027 2727 0a20 2020  .....    '''.   
+00000cf0: 2074 7279 3a0a 2020 2020 2020 2020 636f   try:.        co
+00000d00: 6e66 6967 5f66 696c 6520 3d20 436f 6e66  nfig_file = Conf
+00000d10: 6967 2852 6570 6f73 6974 6f72 7949 6e69  ig(RepositoryIni
+00000d20: 2873 6f75 7263 6520 3d20 6372 6564 735f  (source = creds_
+00000d30: 6669 6c65 2929 0a20 2020 2065 7863 6570  file)).    excep
+00000d40: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00000d50: 783a 2020 2020 2020 2020 2020 2020 2023  x:             #
+00000d60: 206e 6f71 613a 2050 4945 3738 360a 2020   noqa: PIE786.  
+00000d70: 2020 2020 2020 6c6f 6728 2775 6e61 626c        log('unabl
+00000d80: 6520 746f 2072 6561 6420 6769 7665 6e20  e to read given 
+00000d90: 6372 6564 7320 6669 6c65 3a20 2720 2b20  creds file: ' + 
+00000da0: 7374 7228 6578 2929 0a20 2020 2020 2020  str(ex)).       
+00000db0: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
+00000dc0: 2072 6574 7572 6e20 5f63 7265 6473 5f66   return _creds_f
+00000dd0: 726f 6d5f 736f 7572 6365 2863 6f6e 6669  rom_source(confi
+00000de0: 675f 6669 6c65 2c20 7374 7228 6372 6564  g_file, str(cred
+00000df0: 735f 6669 6c65 2929 0a0a 0a64 6566 2063  s_file))...def c
+00000e00: 7265 6465 6e74 6961 6c73 5f66 726f 6d5f  redentials_from_
+00000e10: 656e 7628 293a 0a20 2020 2027 2727 5265  env():.    '''Re
+00000e20: 7475 726e 2061 2043 7265 6465 6e74 6961  turn a Credentia
+00000e30: 6c73 206f 626a 6563 7420 6372 6561 7465  ls object create
+00000e40: 6420 6672 6f6d 2065 6e76 6972 6f6e 6d65  d from environme
+00000e50: 6e74 2076 6172 6961 626c 6573 2e0a 0a20  nt variables... 
+00000e60: 2020 2054 6869 7320 6368 6563 6b73 2066     This checks f
+00000e70: 6f72 2074 6865 2066 6f6c 6c6f 7769 6e67  or the following
+00000e80: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00000e90: 6961 626c 6573 3a0a 0a20 2020 2020 2046  iables:..      F
+00000ea0: 4f4c 494f 5f4f 4b41 5049 5f55 524c 0a20  OLIO_OKAPI_URL. 
+00000eb0: 2020 2020 2046 4f4c 494f 5f4f 4b41 5049       FOLIO_OKAPI
+00000ec0: 5f54 454e 414e 545f 4944 0a20 2020 2020  _TENANT_ID.     
+00000ed0: 2046 4f4c 494f 5f4f 4b41 5049 5f54 4f4b   FOLIO_OKAPI_TOK
+00000ee0: 454e 0a20 2020 2027 2727 0a20 2020 2072  EN.    '''.    r
+00000ef0: 6574 7572 6e20 5f63 7265 6473 5f66 726f  eturn _creds_fro
+00000f00: 6d5f 736f 7572 6365 2843 6f6e 6669 6728  m_source(Config(
+00000f10: 5265 706f 7369 746f 7279 456d 7074 7928  RepositoryEmpty(
+00000f20: 2929 2c20 2765 6e76 6972 6f6e 6d65 6e74  )), 'environment
+00000f30: 2729 0a0a 0a64 6566 2063 7265 6465 6e74  ')...def credent
+00000f40: 6961 6c73 5f66 726f 6d5f 7573 6572 2877  ials_from_user(w
+00000f50: 6172 6e5f 656d 7074 7920 3d20 5472 7565  arn_empty = True
+00000f60: 2c20 696e 6974 6961 6c5f 6372 6564 7320  , initial_creds 
+00000f70: 3d20 4e6f 6e65 293a 0a20 2020 2027 2727  = None):.    '''
+00000f80: 4173 6b20 7573 6572 2066 6f72 2069 6e66  Ask user for inf
+00000f90: 6f20 6e65 6564 6564 2074 6f20 6372 6561  o needed to crea
+00000fa0: 7465 2061 2074 6f6b 656e 2026 2072 6574  te a token & ret
+00000fb0: 7572 6e20 6120 4372 6564 656e 7469 616c  urn a Credential
+00000fc0: 7320 6f62 6a2e 2727 270a 0a20 2020 2065  s obj.'''..    e
+00000fd0: 7665 6e74 203d 2074 6872 6561 6469 6e67  vent = threading
+00000fe0: 2e45 7665 6e74 2829 0a20 2020 2063 6c69  .Event().    cli
+00000ff0: 636b 6564 5f6f 6b20 3d20 4661 6c73 650a  cked_ok = False.
+00001000: 0a20 2020 2064 6566 2063 6c6b 2876 616c  .    def clk(val
+00001010: 293a 0a20 2020 2020 2020 206e 6f6e 6c6f  ):.        nonlo
+00001020: 6361 6c20 636c 6963 6b65 645f 6f6b 0a20  cal clicked_ok. 
+00001030: 2020 2020 2020 2063 6c69 636b 6564 5f6f         clicked_o
+00001040: 6b20 3d20 7661 6c0a 2020 2020 2020 2020  k = val.        
+00001050: 6576 656e 742e 7365 7428 290a 0a20 2020  event.set()..   
+00001060: 206c 6f67 2827 6173 6b69 6e67 2075 7365   log('asking use
+00001070: 7220 666f 7220 6372 6564 656e 7469 616c  r for credential
+00001080: 7327 290a 2020 2020 6375 7272 656e 7420  s').    current 
+00001090: 3d20 696e 6974 6961 6c5f 6372 6564 7320  = initial_creds 
+000010a0: 6f72 2043 7265 6465 6e74 6961 6c73 2827  or Credentials('
+000010b0: 272c 2027 272c 2027 2729 0a20 2020 2070  ', '', '').    p
+000010c0: 696e 7320 3d20 5b0a 2020 2020 2020 2020  ins = [.        
+000010d0: 7075 745f 6d61 726b 646f 776e 2827 5f54  put_markdown('_T
+000010e0: 6869 7320 696e 666f 726d 6174 696f 6e20  his information 
+000010f0: 6973 206e 6565 6465 6420 746f 2063 7265  is needed to cre
+00001100: 6174 6520 6120 464f 4c49 4f20 4150 4920  ate a FOLIO API 
+00001110: 746f 6b65 6e2e 270a 2020 2020 2020 2020  token.'.        
+00001120: 2020 2020 2020 2020 2020 2020 2027 2059               ' Y
+00001130: 6f75 7220 464f 4c49 4f20 6c6f 6769 6e20  our FOLIO login 
+00001140: 2620 7061 7373 776f 7264 2077 696c 6c5f  & password will_
+00001150: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00001160: 2020 2020 2020 2027 202a 2a6e 6f74 2a2a         ' **not**
+00001170: 205f 6265 2073 746f 7265 6420 6166 7465   _be stored afte
+00001180: 7220 7468 6973 2066 6f72 6d20 6469 7361  r this form disa
+00001190: 7070 6561 7273 3b20 6f6e 6c79 270a 2020  ppears; only'.  
+000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011b0: 2020 2027 2074 6865 2074 6f6b 656e 2c20     ' the token, 
+000011c0: 5552 4c20 616e 6420 7465 6e61 6e74 2069  URL and tenant i
+000011d0: 6420 7769 6c6c 2062 6520 7374 6f72 6564  d will be stored
+000011e0: 2e5f 2729 2c0a 2020 2020 2020 2020 7075  ._'),.        pu
+000011f0: 745f 696e 7075 7428 2775 7365 7227 2c20  t_input('user', 
+00001200: 2020 2020 206c 6162 656c 203d 2027 464f       label = 'FO
+00001210: 4c49 4f20 7573 6572 206e 616d 6527 292c  LIO user name'),
+00001220: 0a20 2020 2020 2020 2070 7574 5f69 6e70  .        put_inp
+00001230: 7574 2827 7061 7373 776f 7264 272c 2020  ut('password',  
+00001240: 6c61 6265 6c20 3d20 2746 4f4c 494f 2070  label = 'FOLIO p
+00001250: 6173 7377 6f72 6427 2c20 7479 7065 203d  assword', type =
+00001260: 2027 7061 7373 776f 7264 2729 2c0a 2020   'password'),.  
+00001270: 2020 2020 2020 7075 745f 696e 7075 7428        put_input(
+00001280: 2775 726c 272c 2020 2020 2020 206c 6162  'url',       lab
+00001290: 656c 203d 2027 4f4b 4150 4920 5552 4c27  el = 'OKAPI URL'
+000012a0: 2c20 7661 6c75 6520 3d20 6375 7272 656e  , value = curren
+000012b0: 742e 7572 6c29 2c0a 2020 2020 2020 2020  t.url),.        
+000012c0: 7075 745f 696e 7075 7428 2774 656e 616e  put_input('tenan
+000012d0: 745f 6964 272c 206c 6162 656c 203d 2027  t_id', label = '
+000012e0: 5465 6e61 6e74 2069 6427 2c20 7661 6c75  Tenant id', valu
+000012f0: 6520 3d20 6375 7272 656e 742e 7465 6e61  e = current.tena
+00001300: 6e74 5f69 6429 2c0a 2020 2020 2020 2020  nt_id),.        
+00001310: 7075 745f 6275 7474 6f6e 7328 5b0a 2020  put_buttons([.  
+00001320: 2020 2020 2020 2020 2020 7b27 6c61 6265            {'labe
+00001330: 6c27 3a20 2753 7562 6d69 7427 2c20 2776  l': 'Submit', 'v
+00001340: 616c 7565 273a 2054 7275 657d 2c0a 2020  alue': True},.  
+00001350: 2020 2020 2020 2020 2020 7b27 6c61 6265            {'labe
+00001360: 6c27 3a20 2743 616e 6365 6c27 2c20 2776  l': 'Cancel', 'v
+00001370: 616c 7565 273a 2046 616c 7365 2c20 2763  alue': False, 'c
+00001380: 6f6c 6f72 273a 2027 6461 6e67 6572 277d  olor': 'danger'}
+00001390: 2c0a 2020 2020 2020 2020 5d2c 206f 6e63  ,.        ], onc
+000013a0: 6c69 636b 203d 2063 6c6b 292e 7374 796c  lick = clk).styl
+000013b0: 6528 2766 6c6f 6174 3a20 7269 6768 7427  e('float: right'
+000013c0: 290a 2020 2020 5d0a 2020 2020 706f 7075  ).    ].    popu
+000013d0: 7028 7469 746c 6520 3d20 2746 4f4c 494f  p(title = 'FOLIO
+000013e0: 2063 7265 6465 6e74 6961 6c73 272c 2063   credentials', c
+000013f0: 6f6e 7465 6e74 203d 2070 696e 732c 2073  ontent = pins, s
+00001400: 697a 6520 3d20 276d 6564 6975 6d27 2c0a  ize = 'medium',.
+00001410: 2020 2020 2020 2020 2020 636c 6f73 6162            closab
+00001420: 6c65 203d 2046 616c 7365 290a 0a20 2020  le = False)..   
+00001430: 2065 7665 6e74 2e77 6169 7428 290a 2020   event.wait().  
+00001440: 2020 636c 6f73 655f 706f 7075 7028 290a    close_popup().
+00001450: 2020 2020 7761 6974 2830 2e35 2920 2020      wait(0.5)   
+00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001470: 2020 2020 2020 2020 2320 4769 7665 2074          # Give t
+00001480: 696d 6520 666f 7220 706f 7075 7020 746f  ime for popup to
+00001490: 2067 6f20 6177 6179 2e0a 0a20 2020 2069   go away...    i
+000014a0: 6620 6e6f 7420 636c 6963 6b65 645f 6f6b  f not clicked_ok
+000014b0: 3a0a 2020 2020 2020 2020 6c6f 6728 2775  :.        log('u
+000014c0: 7365 7220 6361 6e63 656c 6c65 6420 6f75  ser cancelled ou
+000014d0: 7420 6f66 2063 7265 6465 6e74 6961 6c73  t of credentials
+000014e0: 2064 6961 6c6f 6727 290a 2020 2020 2020   dialog').      
+000014f0: 2020 7265 7475 726e 2069 6e69 7469 616c    return initial
+00001500: 5f63 7265 6473 0a0a 2020 2020 6966 2070  _creds..    if p
+00001510: 696e 2e75 726c 3a20 2020 2020 2020 2020  in.url:         
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2320 5265 6d6f 7665 2027 2f27 2069 6620  # Remove '/' if 
+00001540: 7468 6520 7573 6572 2069 6e63 6c75 6465  the user include
+00001550: 6420 6974 2e0a 2020 2020 2020 2020 7069  d it..        pi
+00001560: 6e2e 7572 6c20 3d20 7069 6e2e 7572 6c2e  n.url = pin.url.
+00001570: 7273 7472 6970 2827 2f27 290a 0a20 2020  rstrip('/')..   
+00001580: 2069 6620 6e6f 7420 616c 6c28 5b70 696e   if not all([pin
+00001590: 2e75 726c 2c20 7069 6e2e 7465 6e61 6e74  .url, pin.tenant
+000015a0: 5f69 642c 2070 696e 2e75 7365 722c 2070  _id, pin.user, p
+000015b0: 696e 2e70 6173 7377 6f72 645d 293a 0a20  in.password]):. 
+000015c0: 2020 2020 2020 2069 6620 7761 726e 5f65         if warn_e
+000015d0: 6d70 7479 3a0a 2020 2020 2020 2020 2020  mpty:.          
+000015e0: 2020 6c6f 6728 2775 7365 7220 7072 6f76    log('user prov
+000015f0: 6964 6564 2069 6e63 6f6d 706c 6574 6520  ided incomplete 
+00001600: 6372 6564 656e 7469 616c 7327 290a 2020  credentials').  
+00001610: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
+00001620: 6669 726d 2827 4361 6e6e 6f74 2070 726f  firm('Cannot pro
+00001630: 6365 6564 2077 6974 686f 7574 2061 6c6c  ceed without all
+00001640: 2063 7265 6465 6e74 6961 6c73 2e20 5472   credentials. Tr
+00001650: 7920 6167 6169 6e3f 2729 3a0a 2020 2020  y again?'):.    
+00001660: 2020 2020 2020 2020 2020 2020 746d 7020              tmp 
+00001670: 3d20 4372 6564 656e 7469 616c 7328 7572  = Credentials(ur
+00001680: 6c20 3d20 7069 6e2e 7572 6c2c 2074 656e  l = pin.url, ten
+00001690: 616e 745f 6964 203d 2070 696e 2e74 656e  ant_id = pin.ten
+000016a0: 616e 745f 6964 2c20 746f 6b65 6e20 3d20  ant_id, token = 
+000016b0: 4e6f 6e65 290a 2020 2020 2020 2020 2020  None).          
+000016c0: 2020 2020 2020 7265 7475 726e 2063 7265        return cre
+000016d0: 6465 6e74 6961 6c73 5f66 726f 6d5f 7573  dentials_from_us
+000016e0: 6572 2869 6e69 7469 616c 5f63 7265 6473  er(initial_creds
+000016f0: 203d 2074 6d70 290a 2020 2020 2020 2020   = tmp).        
+00001700: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00001710: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00001720: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001730: 204e 6f6e 650a 0a20 2020 2069 6620 6e6f   None..    if no
+00001740: 7420 7661 6c69 645f 7572 6c28 7069 6e2e  t valid_url(pin.
+00001750: 7572 6c29 3a0a 2020 2020 2020 2020 6c6f  url):.        lo
+00001760: 6728 2767 6976 656e 2055 524c 2074 6861  g('given URL tha
+00001770: 7420 646f 6573 6e5c 2774 206c 6f6f 6b20  t doesn\'t look 
+00001780: 6c69 6b65 2061 2075 524c 3a20 2720 2b20  like a uRL: ' + 
+00001790: 7069 6e2e 7572 6c29 0a20 2020 2020 2020  pin.url).       
+000017a0: 2069 6620 636f 6e66 6972 6d28 2754 6869   if confirm('Thi
+000017b0: 7320 646f 6573 206e 6f74 206c 6f6f 6b20  s does not look 
+000017c0: 6c69 6b65 2061 2055 524c 3a20 2227 202b  like a URL: "' +
+000017d0: 2070 696e 2e75 726c 202b 2027 2227 0a20   pin.url + '"'. 
+000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017f0: 2020 2b20 2720 e280 9320 776f 756c 6420    + ' ... would 
+00001800: 796f 7520 6c69 6b65 2074 6f20 6564 6974  you like to edit
+00001810: 2074 6865 2076 616c 7565 2061 6e64 2074   the value and t
+00001820: 7279 2061 6761 696e 3f27 293a 0a20 2020  ry again?'):.   
+00001830: 2020 2020 2020 2020 2074 6d70 203d 2043           tmp = C
+00001840: 7265 6465 6e74 6961 6c73 2875 726c 203d  redentials(url =
+00001850: 2070 696e 2e75 726c 2c20 7465 6e61 6e74   pin.url, tenant
+00001860: 5f69 6420 3d20 7069 6e2e 7465 6e61 6e74  _id = pin.tenant
+00001870: 5f69 642c 2074 6f6b 656e 203d 204e 6f6e  _id, token = Non
+00001880: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
+00001890: 6574 7572 6e20 6372 6564 656e 7469 616c  eturn credential
+000018a0: 735f 6672 6f6d 5f75 7365 7228 696e 6974  s_from_user(init
+000018b0: 6961 6c5f 6372 6564 7320 3d20 746d 7029  ial_creds = tmp)
+000018c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000018d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000018e0: 6e20 4e6f 6e65 0a0a 2020 2020 7769 7468  n None..    with
+000018f0: 2070 7574 5f6c 6f61 6469 6e67 2829 3a0a   put_loading():.
+00001900: 2020 2020 2020 2020 746f 6b65 6e2c 2065          token, e
+00001910: 7272 6f72 203d 2046 6f6c 696f 2e6e 6577  rror = Folio.new
+00001920: 5f74 6f6b 656e 2875 726c 203d 2070 696e  _token(url = pin
+00001930: 2e75 726c 2c20 7465 6e61 6e74 5f69 6420  .url, tenant_id 
+00001940: 3d20 7069 6e2e 7465 6e61 6e74 5f69 642c  = pin.tenant_id,
+00001950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2020 2020 2020 7573 6572 203d 2070          user = p
+00001980: 696e 2e75 7365 722c 2070 6173 7377 6f72  in.user, passwor
+00001990: 6420 3d20 7069 6e2e 7061 7373 776f 7264  d = pin.password
+000019a0: 290a 0a20 2020 2069 6620 6572 726f 723a  )..    if error:
+000019b0: 0a20 2020 2020 2020 206e 6f74 6966 7928  .        notify(
+000019c0: 2746 6169 6c65 6420 746f 2067 6574 2061  'Failed to get a
+000019d0: 2074 6f6b 656e 2e20 2720 2b20 6572 726f   token. ' + erro
+000019e0: 7220 2b20 272e 2729 0a20 2020 2020 2020  r + '.').       
+000019f0: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
+00001a00: 2065 6c73 653a 0a20 2020 2020 2020 206e   else:.        n
+00001a10: 6f74 655f 696e 666f 2827 4e65 7720 464f  ote_info('New FO
+00001a20: 4c49 4f20 4150 4920 746f 6b65 6e20 6f62  LIO API token ob
+00001a30: 7461 696e 6564 2e27 290a 0a20 2020 206c  tained.')..    l
+00001a40: 6f67 2827 676f 7420 6372 6564 656e 7469  og('got credenti
+00001a50: 616c 7320 6672 6f6d 2075 7365 7227 290a  als from user').
+00001a60: 2020 2020 7265 7475 726e 2043 7265 6465      return Crede
+00001a70: 6e74 6961 6c73 2875 726c 203d 2070 696e  ntials(url = pin
+00001a80: 2e75 726c 2c20 7465 6e61 6e74 5f69 6420  .url, tenant_id 
+00001a90: 3d20 7069 6e2e 7465 6e61 6e74 5f69 642c  = pin.tenant_id,
+00001aa0: 2074 6f6b 656e 203d 2074 6f6b 656e 290a   token = token).
+00001ab0: 0a0a 2320 4578 706c 616e 6174 696f 6e20  ..# Explanation 
+00001ac0: 6162 6f75 7420 7468 6520 7765 6972 6420  about the weird 
+00001ad0: 7761 7920 7468 6973 2069 7320 646f 6e65  way this is done
+00001ae0: 3a20 7468 6520 5079 7468 6f6e 206b 6579  : the Python key
+00001af0: 7269 6e67 206d 6f64 756c 650a 2320 6f6e  ring module.# on
+00001b00: 6c79 206f 6666 6572 7320 6120 7369 6e67  ly offers a sing
+00001b10: 6c65 2066 756e 6374 696f 6e20 666f 7220  le function for 
+00001b20: 7365 7474 696e 6720 6120 7661 6c75 653b  setting a value;
+00001b30: 206f 7374 656e 7369 626c 792c 2074 6869   ostensibly, thi
+00001b40: 7320 6973 0a23 2069 6e74 656e 6465 6420  s is.# intended 
+00001b50: 746f 2073 746f 7265 2061 2070 6173 7377  to store a passw
+00001b60: 6f72 6420 6173 736f 6369 6174 6564 2077  ord associated w
+00001b70: 6974 6820 616e 2069 6465 6e74 6966 6965  ith an identifie
+00001b80: 7220 2861 2075 7365 7220 6e61 6d65 292c  r (a user name),
+00001b90: 0a23 2061 6e64 2074 6869 7320 6964 656e  .# and this iden
+00001ba0: 7469 6669 6572 2069 7320 6578 7065 6374  tifier is expect
+00001bb0: 6564 2074 6f20 6265 206f 6274 6169 6e65  ed to be obtaine
+00001bc0: 6420 736f 6d65 206f 7468 6572 2077 6179  d some other way
+00001bd0: 2c20 7375 6368 2061 7320 6279 0a23 2075  , such as by.# u
+00001be0: 7369 6e67 2074 6865 2063 7572 7265 6e74  sing the current
+00001bf0: 2075 7365 7227 7320 636f 6d70 7574 6572   user's computer
+00001c00: 206c 6f67 696e 206e 616d 652e 2020 4275   login name.  Bu
+00001c10: 742c 2069 6e20 6f75 7220 7369 7475 6174  t, in our situat
+00001c20: 696f 6e2c 2077 650a 2320 6861 7665 206d  ion, we.# have m
+00001c30: 756c 7469 706c 6520 7069 6563 6573 206f  ultiple pieces o
+00001c40: 6620 696e 666f 726d 6174 696f 6e20 7765  f information we
+00001c50: 2068 6176 6520 746f 2073 746f 7265 2028   have to store (
+00001c60: 6120 7573 6572 2069 6420 616e 6420 616e  a user id and an
+00001c70: 2061 7069 0a23 206b 6579 292e 2020 5468   api.# key).  Th
+00001c80: 6520 6861 636b 6163 696f 7573 2073 6f6c  e hackacious sol
+00001c90: 7574 696f 6e20 7461 6b65 6e20 6865 7265  ution taken here
+00001ca0: 2069 7320 746f 2063 6f6e 6361 7465 6e61   is to concatena
+00001cb0: 7465 2074 6865 2076 616c 7565 7320 696e  te the values in
+00001cc0: 746f 0a23 2061 2073 696e 676c 6520 7374  to.# a single st
+00001cd0: 7269 6e67 2075 7365 6420 6173 2074 6865  ring used as the
+00001ce0: 2061 6374 7561 6c20 7661 6c75 6520 7374   actual value st
+00001cf0: 6f72 6564 2e20 2054 6865 2069 6e64 6976  ored.  The indiv
+00001d00: 6964 7561 6c20 7661 6c75 6573 2061 7265  idual values are
+00001d10: 0a23 2073 6570 6172 6174 6564 2062 7920  .# separated by 
+00001d20: 6120 6368 6172 6163 7465 7220 7468 6174  a character that
+00001d30: 2069 7320 756e 6c69 6b65 6c79 2074 6f20   is unlikely to 
+00001d40: 6265 2070 6172 7420 6f66 2061 6e79 2075  be part of any u
+00001d50: 7365 722d 7479 7065 6420 7661 6c75 652e  ser-typed value.
+00001d60: 0a0a 6465 6620 6372 6564 656e 7469 616c  ..def credential
+00001d70: 735f 6672 6f6d 5f6b 6579 7269 6e67 2870  s_from_keyring(p
+00001d80: 6172 7469 616c 5f6f 6b20 3d20 4661 6c73  artial_ok = Fals
+00001d90: 652c 2072 696e 6720 3d20 5f4b 4559 5249  e, ring = _KEYRI
+00001da0: 4e47 293a 0a20 2020 2027 2727 4c6f 6f6b  NG):.    '''Look
+00001db0: 2075 7020 7468 6520 7573 6572 2773 2063   up the user's c
+00001dc0: 7265 6465 6e74 6961 6c73 2e0a 2020 2020  redentials..    
+00001dd0: 4966 2070 6172 7469 616c 5f6f 6b20 6973  If partial_ok is
+00001de0: 2046 616c 7365 2c20 7265 7475 726e 204e   False, return N
+00001df0: 6f6e 6520 6966 2074 6865 206b 6579 7269  one if the keyri
+00001e00: 6e67 2076 616c 7565 2069 7320 696e 636f  ng value is inco
+00001e10: 6d70 6c65 7465 2e27 2727 0a20 2020 2069  mplete.'''.    i
+00001e20: 6620 7379 732e 706c 6174 666f 726d 2e73  f sys.platform.s
+00001e30: 7461 7274 7377 6974 6828 2777 696e 2729  tartswith('win')
+00001e40: 3a0a 2020 2020 2020 2020 6c6f 6728 2775  :.        log('u
+00001e50: 7369 6e67 2077 696e 646f 7773 206b 6579  sing windows key
+00001e60: 7269 6e67 2076 6175 6c74 2729 0a20 2020  ring vault').   
+00001e70: 2020 2020 206b 6579 7269 6e67 2e73 6574       keyring.set
+00001e80: 5f6b 6579 7269 6e67 2857 696e 5661 756c  _keyring(WinVaul
+00001e90: 744b 6579 7269 6e67 2829 290a 2020 2020  tKeyring()).    
+00001ea0: 6966 2073 7973 2e70 6c61 7466 6f72 6d2e  if sys.platform.
+00001eb0: 7374 6172 7473 7769 7468 2827 6461 7277  startswith('darw
+00001ec0: 696e 2729 3a0a 2020 2020 2020 2020 6c6f  in'):.        lo
+00001ed0: 6728 2775 7369 6e67 206d 6163 6f73 206b  g('using macos k
+00001ee0: 6579 7269 6e67 2729 0a20 2020 2020 2020  eyring').       
+00001ef0: 206b 6579 7269 6e67 2e73 6574 5f6b 6579   keyring.set_key
+00001f00: 7269 6e67 284b 6579 7269 6e67 2829 290a  ring(Keyring()).
+00001f10: 2020 2020 6c6f 6728 6627 7472 7969 6e67      log(f'trying
+00001f20: 2074 6f20 7265 6164 2076 616c 7565 2066   to read value f
+00001f30: 726f 6d20 7b72 696e 677d 2729 0a20 2020  rom {ring}').   
+00001f40: 2074 7279 3a0a 2020 2020 2020 2020 7661   try:.        va
+00001f50: 6c75 6520 3d20 6b65 7972 696e 672e 6765  lue = keyring.ge
+00001f60: 745f 7061 7373 776f 7264 2872 696e 672c  t_password(ring,
+00001f70: 2067 6574 7061 7373 2e67 6574 7573 6572   getpass.getuser
+00001f80: 2829 290a 2020 2020 6578 6365 7074 2045  ()).    except E
+00001f90: 7863 6570 7469 6f6e 2061 7320 6578 3a20  xception as ex: 
+00001fa0: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
+00001fb0: 7161 3a20 5049 4537 3836 0a20 2020 2020  qa: PIE786.     
+00001fc0: 2020 206c 6f67 2827 6578 6365 7074 696f     log('exceptio
+00001fd0: 6e20 7472 7969 6e67 2074 6f20 6765 7420  n trying to get 
+00001fe0: 7061 7373 776f 7264 2066 726f 6d20 6b65  password from ke
+00001ff0: 7972 696e 673a 2027 202b 2073 7472 2865  yring: ' + str(e
+00002000: 7829 290a 2020 2020 2020 2020 7265 7475  x)).        retu
+00002010: 726e 204e 6f6e 650a 2020 2020 6966 2076  rn None.    if v
+00002020: 616c 7565 3a0a 2020 2020 2020 2020 6c6f  alue:.        lo
+00002030: 6728 6627 676f 7420 6372 6564 656e 7469  g(f'got credenti
+00002040: 616c 7320 6672 6f6d 206b 6579 7269 6e67  als from keyring
+00002050: 207b 7269 6e67 7d27 290a 2020 2020 2020   {ring}').      
+00002060: 2020 7061 7274 7320 3d20 5f64 6563 6f64    parts = _decod
+00002070: 6564 2876 616c 7565 290a 2020 2020 2020  ed(value).      
+00002080: 2020 6966 2061 6c6c 2870 6172 7473 2920    if all(parts) 
+00002090: 6f72 2070 6172 7469 616c 5f6f 6b3a 0a20  or partial_ok:. 
+000020a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000020b0: 6e20 4372 6564 656e 7469 616c 7328 7572  n Credentials(ur
+000020c0: 6c20 3d20 7061 7274 735b 305d 2c20 7465  l = parts[0], te
+000020d0: 6e61 6e74 5f69 6420 3d20 7061 7274 735b  nant_id = parts[
+000020e0: 315d 2c20 746f 6b65 6e20 3d20 7061 7274  1], token = part
+000020f0: 735b 325d 290a 2020 2020 6c6f 6728 6627  s[2]).    log(f'
+00002100: 6469 6420 6e6f 7420 6669 6e64 2061 2076  did not find a v
+00002110: 616c 7565 2069 6e20 6b65 7972 696e 6720  alue in keyring 
+00002120: 7b72 696e 677d 2729 0a20 2020 2072 6574  {ring}').    ret
+00002130: 7572 6e20 4e6f 6e65 0a0a 0a64 6566 2075  urn None...def u
+00002140: 7365 5f63 7265 6465 6e74 6961 6c73 2863  se_credentials(c
+00002150: 7265 6473 293a 0a20 2020 2027 2727 5365  reds):.    '''Se
+00002160: 7420 7275 6e2d 7469 6d65 2065 6e76 6972  t run-time envir
+00002170: 6f6e 6d65 6e74 2063 7265 6465 6e74 6961  onment credentia
+00002180: 6c73 2061 6e64 2073 6176 6520 7468 656d  ls and save them
+00002190: 2074 6f20 7468 6520 6b65 7972 696e 672e   to the keyring.
+000021a0: 2727 270a 2020 2020 6c6f 6728 2773 6574  '''.    log('set
+000021b0: 7469 6e67 2065 6e76 6972 6f6e 6d65 6e74  ting environment
+000021c0: 2076 6172 6961 626c 6573 2066 6f72 2063   variables for c
+000021d0: 7265 6465 6e74 6961 6c73 2729 0a20 2020  redentials').   
+000021e0: 206f 732e 656e 7669 726f 6e5b 2746 4f4c   os.environ['FOL
+000021f0: 494f 5f4f 4b41 5049 5f55 524c 275d 2020  IO_OKAPI_URL']  
+00002200: 2020 2020 203d 2063 7265 6473 2e75 726c       = creds.url
+00002210: 0a20 2020 206f 732e 656e 7669 726f 6e5b  .    os.environ[
+00002220: 2746 4f4c 494f 5f4f 4b41 5049 5f54 454e  'FOLIO_OKAPI_TEN
+00002230: 414e 545f 4944 275d 203d 2063 7265 6473  ANT_ID'] = creds
+00002240: 2e74 656e 616e 745f 6964 0a20 2020 206f  .tenant_id.    o
+00002250: 732e 656e 7669 726f 6e5b 2746 4f4c 494f  s.environ['FOLIO
+00002260: 5f4f 4b41 5049 5f54 4f4b 454e 275d 2020  _OKAPI_TOKEN']  
+00002270: 2020 203d 2063 7265 6473 2e74 6f6b 656e     = creds.token
+00002280: 0a20 2020 2069 6620 636f 6e66 6967 2827  .    if config('
+00002290: 5553 455f 4b45 5952 494e 4727 2c20 6361  USE_KEYRING', ca
+000022a0: 7374 203d 2062 6f6f 6c29 3a0a 2020 2020  st = bool):.    
+000022b0: 2020 2020 6b65 7972 696e 675f 6372 6564      keyring_cred
+000022c0: 7320 3d20 6372 6564 656e 7469 616c 735f  s = credentials_
+000022d0: 6672 6f6d 5f6b 6579 7269 6e67 2829 0a20  from_keyring(). 
+000022e0: 2020 2020 2020 2069 6620 6372 6564 7320         if creds 
+000022f0: 213d 206b 6579 7269 6e67 5f63 7265 6473  != keyring_creds
+00002300: 3a0a 2020 2020 2020 2020 2020 2020 5f73  :.            _s
+00002310: 746f 7265 5f63 7265 6465 6e74 6961 6c73  tore_credentials
+00002320: 2863 7265 6473 290a 0a0a 6465 6620 6375  (creds)...def cu
+00002330: 7272 656e 745f 6372 6564 656e 7469 616c  rrent_credential
+00002340: 7328 293a 0a20 2020 2075 726c 2020 2020  s():.    url    
+00002350: 2020 203d 2063 6f6e 6669 6728 2746 4f4c     = config('FOL
+00002360: 494f 5f4f 4b41 5049 5f55 524c 272c 2064  IO_OKAPI_URL', d
+00002370: 6566 6175 6c74 203d 204e 6f6e 6529 0a20  efault = None). 
+00002380: 2020 2074 656e 616e 745f 6964 203d 2063     tenant_id = c
+00002390: 6f6e 6669 6728 2746 4f4c 494f 5f4f 4b41  onfig('FOLIO_OKA
+000023a0: 5049 5f54 454e 414e 545f 4944 272c 2064  PI_TENANT_ID', d
+000023b0: 6566 6175 6c74 203d 204e 6f6e 6529 0a20  efault = None). 
+000023c0: 2020 2074 6f6b 656e 2020 2020 203d 2063     token     = c
+000023d0: 6f6e 6669 6728 2746 4f4c 494f 5f4f 4b41  onfig('FOLIO_OKA
+000023e0: 5049 5f54 4f4b 454e 272c 2064 6566 6175  PI_TOKEN', defau
+000023f0: 6c74 203d 204e 6f6e 6529 0a20 2020 2072  lt = None).    r
+00002400: 6574 7572 6e20 4372 6564 656e 7469 616c  eturn Credential
+00002410: 7328 7572 6c20 3d20 7572 6c2c 2074 656e  s(url = url, ten
+00002420: 616e 745f 6964 203d 2074 656e 616e 745f  ant_id = tenant_
+00002430: 6964 2c20 746f 6b65 6e20 3d20 746f 6b65  id, token = toke
+00002440: 6e29 0a0a 0a64 6566 2063 7265 6465 6e74  n)...def credent
+00002450: 6961 6c73 5f63 6f6d 706c 6574 6528 6372  ials_complete(cr
+00002460: 6564 7329 3a0a 2020 2020 2727 2752 6574  eds):.    '''Ret
+00002470: 7572 6e20 5472 7565 2069 6620 7468 6520  urn True if the 
+00002480: 6769 7665 6e20 6372 6564 656e 7469 616c  given credential
+00002490: 7320 6172 6520 636f 6d70 6c65 7465 2e27  s are complete.'
+000024a0: 2727 0a20 2020 2072 6574 7572 6e20 2863  ''.    return (c
+000024b0: 7265 6473 2061 6e64 2063 7265 6473 2e75  reds and creds.u
+000024c0: 726c 2061 6e64 2063 7265 6473 2e74 656e  rl and creds.ten
+000024d0: 616e 745f 6964 2061 6e64 2063 7265 6473  ant_id and creds
+000024e0: 2e74 6f6b 656e 290a 0a0c 0a23 2050 7269  .token)....# Pri
+000024f0: 7661 7465 2068 656c 7065 7220 6675 6e63  vate helper func
+00002500: 7469 6f6e 732e 0a23 202e 2e2e 2e2e 2e2e  tions..# .......
+00002510: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00002520: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00002530: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00002540: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00002550: 2e2e 2e2e 2e2e 0a0a 5f53 4550 203d 2027  ........_SEP = '
+00002560: 0327 0a27 2727 4368 6172 6163 7465 7220  .'.'''Character 
+00002570: 7573 6564 2074 6f20 7365 7061 7261 7465  used to separate
+00002580: 206d 756c 7469 706c 6520 6163 7475 616c   multiple actual
+00002590: 2076 616c 7565 7320 7374 6f72 6564 2061   values stored a
+000025a0: 7320 6120 7369 6e67 6c65 0a65 6e63 6f64  s a single.encod
+000025b0: 6564 2076 616c 7565 2073 7472 696e 672e  ed value string.
+000025c0: 2020 5468 6973 2063 6861 7261 6374 6572    This character
+000025d0: 2069 7320 6465 6c69 6265 7261 7465 6c79   is deliberately
+000025e0: 2063 686f 7365 6e20 746f 2062 6520 736f   chosen to be so
+000025f0: 6d65 7468 696e 670a 7665 7279 2075 6e6c  mething.very unl
+00002600: 696b 656c 7920 746f 2062 6520 7061 7274  ikely to be part
+00002610: 206f 6620 6120 6c65 6769 7469 6d61 7465   of a legitimate
+00002620: 2073 7472 696e 6720 7661 6c75 6520 7479   string value ty
+00002630: 7065 6420 6279 2075 7365 7220 6174 2061  ped by user at a
+00002640: 0a73 6865 6c6c 2070 726f 6d70 742c 2062  .shell prompt, b
+00002650: 6563 6175 7365 2063 6f6e 7472 6f6c 2d63  ecause control-c
+00002660: 2069 7320 6e6f 726d 616c 6c79 2075 7365   is normally use
+00002670: 6420 746f 2069 6e74 6572 7275 7074 2070  d to interrupt p
+00002680: 726f 6772 616d 732e 0a27 2727 0a0a 0a64  rograms..'''...d
+00002690: 6566 205f 656e 636f 6465 6428 7572 6c2c  ef _encoded(url,
+000026a0: 2074 656e 616e 745f 6964 2c20 746f 6b65   tenant_id, toke
+000026b0: 6e29 3a0a 2020 2020 7265 7475 726e 2066  n):.    return f
+000026c0: 277b 7572 6c7d 7b5f 5345 507d 7b74 656e  '{url}{_SEP}{ten
+000026d0: 616e 745f 6964 7d7b 5f53 4550 7d7b 746f  ant_id}{_SEP}{to
+000026e0: 6b65 6e7d 270a 0a0a 6465 6620 5f64 6563  ken}'...def _dec
+000026f0: 6f64 6564 2876 616c 7565 5f73 7472 696e  oded(value_strin
+00002700: 6729 3a0a 2020 2020 7265 7475 726e 2074  g):.    return t
+00002710: 7570 6c65 2876 616c 7565 5f73 7472 696e  uple(value_strin
+00002720: 672e 7370 6c69 7428 5f53 4550 2929 0a0a  g.split(_SEP))..
+00002730: 0a64 6566 205f 6372 6564 735f 6672 6f6d  .def _creds_from
+00002740: 5f73 6f75 7263 6528 736f 7572 6365 203d  _source(source =
+00002750: 204e 6f6e 652c 2077 6865 7265 203d 2027   None, where = '
+00002760: 2729 3a0a 2020 2020 6966 206e 6f74 2073  '):.    if not s
+00002770: 6f75 7263 653a 0a20 2020 2020 2020 2072  ource:.        r
+00002780: 6574 7572 6e20 4e6f 6e65 0a20 2020 2075  eturn None.    u
+00002790: 726c 2020 2020 2020 203d 2073 6f75 7263  rl       = sourc
+000027a0: 652e 6765 7428 2746 4f4c 494f 5f4f 4b41  e.get('FOLIO_OKA
+000027b0: 5049 5f55 524c 272c 2064 6566 6175 6c74  PI_URL', default
+000027c0: 203d 204e 6f6e 6529 0a20 2020 2074 656e   = None).    ten
+000027d0: 616e 745f 6964 203d 2073 6f75 7263 652e  ant_id = source.
+000027e0: 6765 7428 2746 4f4c 494f 5f4f 4b41 5049  get('FOLIO_OKAPI
+000027f0: 5f54 454e 414e 545f 4944 272c 2064 6566  _TENANT_ID', def
+00002800: 6175 6c74 203d 204e 6f6e 6529 0a20 2020  ault = None).   
+00002810: 2074 6f6b 656e 2020 2020 203d 2073 6f75   token     = sou
+00002820: 7263 652e 6765 7428 2746 4f4c 494f 5f4f  rce.get('FOLIO_O
+00002830: 4b41 5049 5f54 4f4b 454e 272c 2064 6566  KAPI_TOKEN', def
+00002840: 6175 6c74 203d 204e 6f6e 6529 0a20 2020  ault = None).   
+00002850: 2069 6620 6e6f 7420 616e 7928 5b75 726c   if not any([url
+00002860: 2c20 7465 6e61 6e74 5f69 642c 2074 6f6b  , tenant_id, tok
+00002870: 656e 5d29 3a0a 2020 2020 2020 2020 6c6f  en]):.        lo
+00002880: 6728 6627 6e6f 2063 7265 6465 6e74 6961  g(f'no credentia
+00002890: 6c73 2066 6f75 6e64 2069 6e20 7b77 6865  ls found in {whe
+000028a0: 7265 7d27 290a 2020 2020 2020 2020 7265  re}').        re
+000028b0: 7475 726e 204e 6f6e 650a 2020 2020 6372  turn None.    cr
+000028c0: 6564 7320 3d20 4372 6564 656e 7469 616c  eds = Credential
+000028d0: 7328 7572 6c20 3d20 7572 6c2c 2074 656e  s(url = url, ten
+000028e0: 616e 745f 6964 203d 2074 656e 616e 745f  ant_id = tenant_
+000028f0: 6964 2c20 746f 6b65 6e20 3d20 746f 6b65  id, token = toke
+00002900: 6e29 0a20 2020 2063 6f6d 706c 6574 6520  n).    complete 
+00002910: 3d20 2763 6f6d 706c 6574 6527 2069 6620  = 'complete' if 
+00002920: 6372 6564 656e 7469 616c 735f 636f 6d70  credentials_comp
+00002930: 6c65 7465 2863 7265 6473 2920 656c 7365  lete(creds) else
+00002940: 2027 6e6f 7420 636f 6d70 6c65 7465 270a   'not complete'.
+00002950: 2020 2020 6c6f 6728 6627 6372 6564 656e      log(f'creden
+00002960: 7469 616c 7320 696e 207b 7768 6572 657d  tials in {where}
+00002970: 2061 7265 207b 636f 6d70 6c65 7465 7d27   are {complete}'
+00002980: 290a 2020 2020 7265 7475 726e 2063 7265  ).    return cre
+00002990: 6473 0a0a 0a64 6566 205f 7374 6f72 655f  ds...def _store_
+000029a0: 6372 6564 656e 7469 616c 7328 6372 6564  credentials(cred
+000029b0: 732c 2072 696e 6720 3d20 5f4b 4559 5249  s, ring = _KEYRI
+000029c0: 4e47 293a 0a20 2020 2027 2727 5361 7665  NG):.    '''Save
+000029d0: 2074 6865 2075 7365 7227 7320 6372 6564   the user's cred
+000029e0: 656e 7469 616c 732e 2727 270a 2020 2020  entials.'''.    
+000029f0: 6966 2073 7973 2e70 6c61 7466 6f72 6d2e  if sys.platform.
+00002a00: 7374 6172 7473 7769 7468 2827 7769 6e27  startswith('win'
+00002a10: 293a 0a20 2020 2020 2020 206b 6579 7269  ):.        keyri
+00002a20: 6e67 2e73 6574 5f6b 6579 7269 6e67 2857  ng.set_keyring(W
+00002a30: 696e 5661 756c 744b 6579 7269 6e67 2829  inVaultKeyring()
+00002a40: 290a 2020 2020 6966 2073 7973 2e70 6c61  ).    if sys.pla
+00002a50: 7466 6f72 6d2e 7374 6172 7473 7769 7468  tform.startswith
+00002a60: 2827 6461 7277 696e 2729 3a0a 2020 2020  ('darwin'):.    
+00002a70: 2020 2020 6b65 7972 696e 672e 7365 745f      keyring.set_
+00002a80: 6b65 7972 696e 6728 4b65 7972 696e 6728  keyring(Keyring(
+00002a90: 2929 0a20 2020 2076 616c 7565 203d 205f  )).    value = _
+00002aa0: 656e 636f 6465 6428 6372 6564 732e 7572  encoded(creds.ur
+00002ab0: 6c2c 2063 7265 6473 2e74 656e 616e 745f  l, creds.tenant_
+00002ac0: 6964 2c20 6372 6564 732e 746f 6b65 6e29  id, creds.token)
+00002ad0: 0a20 2020 206c 6f67 2866 2773 746f 7269  .    log(f'stori
+00002ae0: 6e67 2063 7265 6465 6e74 6961 6c73 2074  ng credentials t
+00002af0: 6f20 6b65 7972 696e 6720 7b5f 4b45 5952  o keyring {_KEYR
+00002b00: 494e 477d 2729 0a20 2020 206b 6579 7269  ING}').    keyri
+00002b10: 6e67 2e73 6574 5f70 6173 7377 6f72 6428  ng.set_password(
+00002b20: 7269 6e67 2c20 6765 7470 6173 732e 6765  ring, getpass.ge
+00002b30: 7475 7365 7228 292c 2076 616c 7565 290a  tuser(), value).
```

### Comparing `foliage-1.5.5/foliage/delete_tab.py` & `foliage-1.6.0/foliage/delete_tab.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/enum_utils.py` & `foliage-1.6.0/foliage/enum_utils.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/exceptions.py` & `foliage-1.6.0/foliage/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/export.py` & `foliage-1.6.0/foliage/export.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/folio.py` & `foliage-1.6.0/foliage/folio.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,23 @@
             request_url = url + '/authn/login'
             (resp, error) = net('post', request_url, headers = headers, data = data)
             if resp.status_code == 201:
                 token = resp.headers['x-okapi-token']
                 log(f'got new token from FOLIO: {token}')
                 return token, None
             elif resp.status_code == 422:
-                return None, 'FOLIO rejected the information given'
+                msg = 'FOLIO rejected the information given'
+                try:
+                    if errors := json.loads(resp.text).get('errors', []):
+                        text = errors[0].get('message', '')
+                        if text:
+                            msg += (': ' + text)
+                except json.JSONDecodeError:
+                    log('could not extract error message from FOLIO reply')
+                return None, msg
             elif isinstance(error, Interrupted):
                 raise_for_interrupts()
             elif error:
                 return None, 'FOLIO returned an error: ' + str(error)
             else:
                 return None, f'FOLIO returned unknown code {str(resp.status_code)}'
         except Interrupted:
```

### Comparing `foliage-1.5.5/foliage/list_tab.py` & `foliage-1.6.0/foliage/list_tab.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/lookup_tab.py` & `foliage-1.6.0/foliage/lookup_tab.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from   pywebio.session import eval_js
 from   sidetrack import log
 import threading
 
 from   foliage.base_tab import FoliageTab
 from   foliage.export import export_records
 from   foliage.folio import Folio, RecordKind, IdKind, TypeKind
-from   foliage.folio import unique_identifiers
+from   foliage.folio import unique_identifiers, Record
 from   foliage.ui import user_file, stop_processbar
 from   foliage.ui import tell_success, tell_warning, tell_failure
 from   foliage.ui import note_error, PROGRESS_BOX
 
 
 # Tab definition class.
 # .............................................................................
@@ -42,14 +42,16 @@
     def pin_watchers(self):
         return {}
 
 
 # Tab layout.
 # .............................................................................
 
+column_widths = '54% 46%'
+
 def tab_contents():
     log('generating lookup tab contents')
     return [
         put_grid([[
             put_markdown('Input one or more item barcode, item id, item hrid,'
                          ' instance id, instance hrid, instance accession'
                          ' number, loan id, loan hrid, user id, or user'
@@ -68,30 +70,31 @@
                                  ('User', RecordKind.USER)]),
             put_checkbox("open_loans", inline = True,
                          options = [('Search open loans only', True, True)],
                          help_text = ('When searching for loans (and users,'
                                       ' based on loans), limit searches to'
                                       ' open loans only. Deselect'
                                       ' to search all loans.')),
-        ]], cell_widths = '54% 46%'),
+        ]], cell_widths = column_widths),
         put_grid([[
             put_grid([[
                 put_text('Format in which to display records:'),
             ], [
                 put_radio('show_raw', inline = True,
                           options = [('Summary', 'summary', True),
+                                     ('Enhanced summary', 'enhanced'),
                                      ('Raw data', 'json')]),
             ]]),
             put_checkbox("inventory_api", inline = True,
-                         options = [('Use inventory API for items and instances',
+                         options = [('Use FOLIO "inventory" API',
                                      True, True)],
                          help_text = ("FOLIO's Inventory API shows more fields but"
                                       ' some values are computed. Deselect to'
                                       ' get pure records from the storage API.')),
-        ]], cell_widths = '54% 46%'),
+        ]], cell_widths = column_widths),
         put_row([
             put_button('Look up records', onclick = lambda: do_find()),
             put_text(''),    # Adds a column, pushing next item to the right.
             put_button('Clear', outline = True,
                        onclick = lambda: clear_tab()).style('text-align: right')
         ])
     ]
@@ -104,30 +107,41 @@
 _running = False
 _last_textbox = ''
 _last_results = {}
 _last_kind = None
 _last_inventory_api = True
 _last_open_loans = True
 _location_map = None
+_loan_map = None
 
 
 def load_file():
     log('user requesting file upload')
     if (contents := user_file('Upload a file containing identifiers')):
         pin.textbox_find = contents
 
 
 def init_location_map():
     global _location_map
     if _location_map is None:
+        log('building map of location names')
         folio = Folio()
         _location_map = {x.data['id']: x.data['name']
                          for x in folio.types(TypeKind.LOCATION)}
 
 
+def init_loan_map():
+    global _loan_map
+    if _loan_map is None:
+        log('building map of loan types')
+        folio = Folio()
+        _loan_map = {x.data['id']: x.data['name']
+                     for x in folio.types(TypeKind.LOAN)}
+
+
 def inputs_are_unchanged():
     global _last_textbox
     global _last_kind
     global _last_inventory_api
     global _last_open_loans
     unchanged = (pin.textbox_find == _last_textbox
                  and pin.select_kind == _last_kind
@@ -194,14 +208,37 @@
             wait(1)
             wait_count -= 1
         except Interrupted:
             continue
     enable_lookup_button(True)
 
 
+def nonexistent_record_stub(id_, id_kind):
+    data = {'id': ''}
+
+    if id_kind in [IdKind.ITEM_BARCODE, IdKind.USER_BARCODE]:
+        data['barcode'] = id_
+    elif id_kind in [IdKind.ITEM_ID, IdKind.HOLDINGS_ID, IdKind.INSTANCE_ID,
+                     IdKind.USER_ID, IdKind.LOAN_ID, IdKind.TYPE_ID,
+                     IdKind.ACCESSION]:
+        data['id'] = id_
+    elif id_kind in [IdKind.ITEM_HRID, IdKind.HOLDINGS_HRID, IdKind.INSTANCE_HRID]:
+        data['hrid'] = id_
+
+    if id_kind in [IdKind.INSTANCE_ID, IdKind.INSTANCE_HRID]:
+        data['title'] = ''
+    # Item records from the storage API don't have 'title', so we don't add it
+    # unless we're using the inventory API.
+    if pin.inventory_api and id_kind in [IdKind.ITEM_BARCODE, IdKind.ITEM_ID,
+                                         IdKind.ITEM_HRID]:
+        data['title'] = ''
+
+    return Record(id_, id_kind, data)
+
+
 # Summary of the basic flow of control:
 #
 # User clicks "look up records", thus invoking do_find().
 # We show progress bar & stop button while lookup is running.
 # Possible scenarios:
 #   1) process finishes normally
 #   2) user clicks stop button
@@ -236,15 +273,14 @@
     _last_textbox = pin.textbox_find
     _last_kind = pin.select_kind
     _last_inventory_api = pin.inventory_api
     _last_open_loans = pin.open_loans
     kind_wanted = pin.select_kind
     steps = len(identifiers) + 1
     folio = Folio()
-    init_location_map()
     total_found = 0
     with use_scope('output', clear = True):
         put_grid([[
             put_scope('current_activity', [
                 put_markdown('_Certain lookups take a long time. Please be patient._'
                              ).style('color: DarkOrange; margin-bottom: 0')]),
         ], [
@@ -264,29 +300,32 @@
                     tell_failure(f'Unrecognized identifier: **{id_}**.')
                     continue
                 if reuse_results:
                     records = _last_results.get(id_)
                 else:
                     records = folio.related_records(id_, id_kind, kind_wanted,
                                                     pin.inventory_api, pin.open_loans)
-                    _last_results[id_] = records
-                if not records or len(records) == 0:
-                    tell_failure(f'No {kind_wanted} record(s) found for {id_kind} **{id_}**.')
-                    continue
+                    if not records or len(records) == 0:
+                        tell_failure(f'No {kind_wanted} record(s) found for'
+                                     f' {id_kind} **{id_}**.')
+                        _last_results[id_] = [nonexistent_record_stub(id_, id_kind)]
+                        continue
+                    else:
+                        _last_results[id_] = records
 
                 # Report the results & how we got them.
                 source = 'storage'
                 if pin.inventory_api and kind_wanted in ['item', 'instance']:
                     source = 'inventory'
                 this = pluralized(kind_wanted + f' {source} record', records, True)
                 how = f'by searching for {id_kind} **{id_}**.'
                 tell_success(f'Found {this} {how}')
                 show_index = (len(records) > 1)
                 for index, record in enumerate(records, start = 1):
-                    print_record(record, id_, index, show_index, pin.show_raw == 'json')
+                    print_record(record, id_, index, show_index, pin.show_raw)
                 total_found += len(records)
             except Interrupted:
                 log('stopping due to interruption')
                 _interrupted = True
             except Exception as ex:     # noqa: PIE786
                 import traceback
                 log('Exception info: ' + str(ex) + '\n' + traceback.format_exc())
@@ -324,26 +363,30 @@
         value = record.data[field_name]
     if isinstance(value, list) and list_joiner:
         return list_joiner.join(str(x) for x in value)
     else:
         return str(value)
 
 
-def location(record, field_name):
-    global _location_map
+def location(record, field_name, include_id=True):
     if field_name not in record.data:
         return ''
     location_data = record.data[field_name]
     if isinstance(location_data, dict):
         if 'name' in location_data:
-            return f'{location_data["name"]}  ({location_data["id"]})'
+            id_info = f' ({location_data["id"]})' if include_id else ''
+            return f'{location_data["name"]}{id_info}'
         else:
             return location_data["id"]
-    elif location_data and location_data in _location_map:
-        return f'{_location_map[location_data]}  ({location_data})'
+    elif location_data:
+        global _location_map
+        init_location_map()
+        if location_data in _location_map:
+            id_info = f' ({location_data})' if include_id else ''
+            return f'{_location_map[location_data]}{id_info}'
     return '(unknown location)'
 
 
 def notes(record, field_name):
     if field_name not in record.data:
         return ''
     notes = record.data[field_name]
@@ -356,137 +399,223 @@
             return '\n'.join(filter(None, [n.get('note', '') for n in notes]))
         else:
             return '\n'.join(str(note) for note in notes)
     else:
         return notes
 
 
-def print_record(record, identifier, index, show_index, show_raw):
+def loan_type(record, field_name):
+    if field_name not in record.data:
+        return ''
+    loan_type = record.data[field_name]
+    if isinstance(loan_type, dict):
+        if 'name' in loan_type:
+            return f'{loan_type["name"]}  ({loan_type["id"]})'
+        else:
+            return loan_type["id"]
+    elif loan_type:
+        global _loan_map
+        init_loan_map()
+        if loan_type in _loan_map:
+            return f'{_loan_map[loan_type]}  ({loan_type})'
+    return '(unknown loan type)'
+
+
+def print_record(record, identifier, index, show_index, format):
     log(f'printing {record.kind} record {record.id}')
     if show_index:
         put_markdown(f'{record.kind.title()} record #{index}:')
-
-    if show_raw:
+    if format == 'json':
         put_code(pformat(record.data, indent = 2))
-    elif record.kind is RecordKind.ITEM:
-        # Caution: left-hand values contain nonbreaking spaces (invisible here).
+        return
+    # Caution: left-hand values contain nonbreaking spaces (invisible here).
+    if record.kind is RecordKind.ITEM:
         if 'title' in record.data:
             # Inventory record version.
-            put_table([
+            table = [
                 ['Title'                     , field(record, 'title')],
                 ['Barcode'                   , field(record, 'barcode')],
                 ['Call number'               , field(record, 'callNumber')],
                 [f'{record.kind.title()} id' , field(record, 'id')],
                 ['Effective location'        , location(record, 'effectiveLocation')],
                 ['Permanent location'        , location(record, 'permanentLocation')],
+                ['Loan type'                 , loan_type(record, 'permanentLoanType')],
                 ['Status'                    , field(record, 'status', 'name')],
                 ['Tags'                      , field(record, 'tags', 'tagsList')],
                 ['Notes'                     , notes(record, 'notes')],
                 ['HRID'                      , field(record, 'hrid')],
                 ['Created'                   , field(record, 'metadata', 'createdDate')],
                 ['Updated'                   , field(record, 'metadata', 'updatedDate')],
-            ]).style('font-size: 90%; margin: auto 17px 1.5em 17px')
+            ]
         else:
             # Storage record version.
-            put_table([
+            table = [
                 ['Barcode'                   , field(record, 'barcode')],
                 ['Call number'               , field(record, 'itemLevelCallNumber')],
                 [f'{record.kind.title()} id' , field(record, 'id')],
                 ['Effective location'        , location(record, 'effectiveLocationId')],
                 ['Permanent location'        , location(record, 'permanentLocationId')],
+                ['Loan type'                 , loan_type(record, 'permanentLoanTypeId')],
                 ['Tags'                      , field(record, 'tags', 'tagsList')],
                 ['Notes'                     , notes(record, 'notes')],
                 ['HRID'                      , field(record, 'hrid')],
                 ['Created'                   , field(record, 'metadata', 'createdDate')],
                 ['Updated'                   , field(record, 'metadata', 'updatedDate')],
-            ]).style('font-size: 90%; margin: auto 17px 1.5em 17px')
+            ]
     elif record.kind is RecordKind.INSTANCE:
-        # Caution: left-hand values contain nonbreaking spaces (invisible here).
+        call_number = ''
         if field(record, 'classifications'):
             call_number = record.data['classifications'][0]['classificationNumber']
-        else:
-            call_number = ''
         if 'tags' in record.data:
-            put_table([
+            table = [
                 ['Title'                     , field(record, 'title')],
                 ['Call number'               , call_number],
                 [f'{record.kind.title()} id' , field(record, 'id')],
                 ['Tags'                      , field(record, 'tags', 'tagsList')],
                 ['Notes'                     , notes(record, 'notes')],
                 ['HRID'                      , field(record, 'hrid')],
                 ['Created'                   , field(record, 'metadata', 'createdDate')],
                 ['Updated'                   , field(record, 'metadata', 'updatedDate')],
-            ]).style('font-size: 90%; margin: auto 17px 1.5em 17px')
+            ]
         else:
-            put_table([
+            table = [
                 ['Title'                     , field(record, 'title')],
                 ['Call number'               , call_number],
                 [f'{record.kind.title()} id' , field(record, 'id')],
                 ['HRID'                      , field(record, 'hrid')],
                 ['Notes'                     , notes(record, 'notes')],
                 ['Created'                   , field(record, 'metadata', 'createdDate')],
                 ['Updated'                   , field(record, 'metadata', 'updatedDate')],
-            ]).style('font-size: 90%; margin: auto 17px 1.5em 17px')
+            ]
     elif record.kind is RecordKind.HOLDINGS:
-        # Caution: left-hand values contain nonbreaking spaces (invisible here).
         if 'effectiveLocationId' in record.data:
-            put_table([
+            table = [
                 [f'{record.kind.title()} id' , field(record, 'id')],
                 ['HRID'                      , field(record, 'hrid')],
                 ['Holdings type id'          , field(record, 'holdingsTypeId')],
                 ['Instance id'               , field(record, 'instanceId')],
                 ['Effective location'        , location(record, 'effectiveLocationId')],
                 ['Permanent location'        , location(record, 'permanentLocationId')],
                 ['Created'                   , field(record, 'metadata', 'createdDate')],
                 ['Updated'                   , field(record, 'metadata', 'updatedDate')],
-            ]).style('font-size: 90%; margin: auto 17px 1.5em 17px')
+            ]
         else:
-            put_table([
+            table = [
                 [f'{record.kind.title()} id' , field(record, 'id')],
                 ['HRID'                      , field(record, 'hrid')],
                 ['Holdings type id'          , field(record, 'holdingsTypeId')],
                 ['Instance id'               , field(record, 'instanceId')],
                 ['Effective location'        , ''],
                 ['Permanent location'        , location(record, 'permanentLocationId')],
                 ['Created'                   , field(record, 'metadata', 'createdDate')],
                 ['Updated'                   , field(record, 'metadata', 'updatedDate')],
-            ]).style('font-size: 90%; margin: auto 17px 1.5em 17px')
+            ]
     elif record.kind is RecordKind.USER:
-        # Caution: left-hand values contain nonbreaking spaces (invisible here).
-        put_table([
+        table = [
             ['Username'                  , field(record, 'username')],
             ['Barcode'                   , field(record, 'barcode')],
             [f'{record.kind.title()} id' , field(record, 'id')],
             ['Patron group'              , field(record, 'patronGroup')],
             ['Created'                   , field(record, 'metadata', 'createdDate')],
             ['Updated'                   , field(record, 'metadata', 'updatedDate')],
-        ]).style('font-size: 90%; margin: auto 17px 1.5em 17px')
+        ]
     elif record.kind is RecordKind.LOAN:
         if 'userId' in record.data:
-            put_table([
+            table = [
                 [f'{record.kind.title()} id' , field(record, 'id')],
                 ['Status'                    , field(record, 'status', 'name')],
                 ['User id'                   , field(record, 'userId')],
                 ['Item id'                   , field(record, 'itemId')],
                 ['Loan date'                 , field(record, 'loanDate')],
                 ['Due date'                  , field(record, 'dueDate')],
                 ['Created'                   , field(record, 'metadata', 'createdDate')],
                 ['Updated'                   , field(record, 'metadata', 'updatedDate')],
-            ]).style('font-size: 90%; margin: auto 17px 1.5em 17px')
+            ]
         else:
-            put_table([
+            table = [
                 [f'{record.kind.title()} id' , field(record, 'id')],
                 ['Status'                    , field(record, 'status', 'name')],
                 ['User id'                   , ''],
                 ['Item id'                   , field(record, 'itemId')],
                 ['Loan date'                 , field(record, 'loanDate')],
                 ['Due date'                  , field(record, 'dueDate')],
                 ['Created'                   , field(record, 'metadata', 'createdDate')],
                 ['Updated'                   , field(record, 'metadata', 'updatedDate')],
-            ]).style('font-size: 90%; margin: auto 17px 1.5em 17px')
+            ]
+
+    # Define some helpers for the enhanced format.
+    def item_info(hid):
+        folio = Folio()
+        items = folio.related_records(hid, IdKind.HOLDINGS_ID, RecordKind.ITEM)
+        num_items = len(items)
+        text = str(num_items)
+        if num_items > 1:
+            if record.kind == RecordKind.ITEM:
+                text += ' (including this item)'
+        else:
+            if record.kind == RecordKind.ITEM:
+                text += ' (this is the only item on the holdings record)'
+        return text
+
+    def holdings_info(iid):
+        folio = Folio()
+        holdings = folio.related_records(iid, IdKind.INSTANCE_ID, RecordKind.HOLDINGS)
+        num_holdings = len(holdings)
+        if num_holdings > 1:
+            prefix = '<br>&nbsp;&nbsp;&bull;&nbsp;'
+            holdings_list = []
+            for h in holdings:
+                if 'effectiveLocationId' in h.data:
+                    loc = location(h, 'effectiveLocationId', False)
+                else:
+                    loc = location(h, 'permanentLocationId', False)
+                holdings_list.append(loc + f' (holdings record: {h.id})')
+            locations = prefix + prefix.join(holdings_list)
+            return put_html(f'{num_holdings} holdings records in total:{locations}')
+        else:
+            if record.kind == RecordKind.HOLDINGS:
+                return '1 (there are no other holdings records on the instance)'
+            else:
+                return '1 (including this holdings record)'
+
+    # Add additional info when doing an enhanced summary.
+    if format == 'enhanced' and record.kind == RecordKind.ITEM:
+        folio = Folio()
+        hid = record.data['holdingsRecordId']
+        instances = folio.related_records(hid, IdKind.HOLDINGS_ID, RecordKind.INSTANCE)
+        instance = instances[0]
+        iid = instance.id
+        total_items = item_info(hid)
+        total_holdings = holdings_info(iid)
+
+        table.append(['Parent holdings record'             , hid])
+        table.append(['Total items on the holdings record' , total_items])
+        table.append(['Parent instance record'             , iid])
+        table.append(['Total holdings records on the instance', total_holdings])
+
+        additions = {'parentHoldingsRecord'                 : hid,
+                     'totalItemsOnHoldingsRecord'           : total_items,
+                     'parentInstanceRecord'                 : iid,
+                     'totalHoldingsRecordsOnParentInstance' : total_holdings}
+        record.data['computedByFoliage'] = additions
+    elif format == 'enhanced' and record.kind == RecordKind.HOLDINGS:
+        folio = Folio()
+        hid = record.id
+        iid = record.data['instanceId']
+        total_items = item_info(hid)
+        total_holdings = holdings_info(iid)
+
+        # The summary table for holdings already has the holdings & instance id's.
+        table.append(['Total items on this holdings record'   , total_items])
+        table.append(['Total holdings records on the instance', total_holdings])
+
+        additions = {'totalItemsOnThisHoldingsRecord': total_items,
+                     'totalHoldingsRecordsOnParentInstance': total_holdings}
+        record.data['computedByFoliage'] = additions
+    put_table(table).style('font-size: 90%; margin: auto 17px 1.5em 17px')
 
 
 def user_wants_reuse():
     event = threading.Event()
     answer = False
 
     def clk(val):
```

### Comparing `foliage-1.5.5/foliage/other_tab.py` & `foliage-1.6.0/foliage/other_tab.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/system_widget.py` & `foliage-1.6.0/foliage/system_widget.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage/ui.py` & `foliage-1.6.0/foliage/ui.py`

 * *Files identical despite different names*

### Comparing `foliage-1.5.5/foliage.egg-info/PKG-INFO` & `foliage-1.6.0/foliage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: foliage
-Version: 1.5.5
+Version: 1.6.0
 Summary: Foliage: a tool to do bulk changes in FOLIO using the OKAPI API
 Home-page: https://github.com/caltechlibrary/foliage
 Author: Mike Hucka
 Author-email: helpdesk@library.caltech.edu
 License: BSD 3-clause license
 Project-URL: Source Code, https://github.com/caltechlibrary/foliage
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/foliage/issues
 Keywords: Python,applications
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
@@ -126,9 +125,7 @@
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
     <img width="100" height="100" src="https://raw.githubusercontent.com/caltechlibrary/foliage/main/.graphics/caltech-round.png">
   </a>
 </div>
-
-
```

### Comparing `foliage-1.5.5/foliage.egg-info/SOURCES.txt` & `foliage-1.6.0/foliage.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -20,8 +20,11 @@
 foliage/ui.py
 foliage.egg-info/PKG-INFO
 foliage.egg-info/SOURCES.txt
 foliage.egg-info/dependency_links.txt
 foliage.egg-info/entry_points.txt
 foliage.egg-info/not-zip-safe
 foliage.egg-info/requires.txt
-foliage.egg-info/top_level.txt
+foliage.egg-info/top_level.txt
+tests/test_credentials.py
+tests/test_folio.py
+tests/test_init.py
```

### Comparing `foliage-1.5.5/setup.cfg` & `foliage-1.6.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foliage
-version = 1.5.5
+version = 1.6.0
 description = Foliage: a tool to do bulk changes in FOLIO using the OKAPI API
 author = Mike Hucka
 author_email = helpdesk@library.caltech.edu
 license = BSD 3-clause license
 license_files = LICENSE
 url = https://github.com/caltechlibrary/foliage
 project_urls =
```

### Comparing `foliage-1.5.5/setup.py` & `foliage-1.6.0/setup.py`

 * *Files identical despite different names*

