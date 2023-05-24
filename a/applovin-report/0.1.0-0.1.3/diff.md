# Comparing `tmp/applovin_report-0.1.0.tar.gz` & `tmp/applovin_report-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "applovin_report-0.1.0.tar", max compression
+gzip compressed data, was "applovin_report-0.1.3.tar", max compression
```

## Comparing `applovin_report-0.1.0.tar` & `applovin_report-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-23 11:06:12.066537 applovin_report-0.1.0/LICENSE
--rw-r--r--   0        0        0     1154 2023-05-23 11:06:12.066537 applovin_report-0.1.0/README.md
--rw-r--r--   0        0        0      129 2023-05-23 11:06:12.066537 applovin_report-0.1.0/applovin_report/__init__.py
--rw-r--r--   0        0        0       19 2023-05-23 11:06:12.066537 applovin_report-0.1.0/applovin_report/app.py
--rw-r--r--   0        0        0     2427 2023-05-23 11:06:12.066537 applovin_report-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-23 11:06:12.066537 applovin_report-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      586 2023-05-23 11:06:12.066537 applovin_report-0.1.0/tests/test_app.py
--rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 applovin_report-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-24 07:10:10.662819 applovin_report-0.1.3/LICENSE
+-rw-r--r--   0        0        0      782 2023-05-24 07:10:10.662819 applovin_report-0.1.3/README.md
+-rw-r--r--   0        0        0      129 2023-05-24 07:10:10.662819 applovin_report-0.1.3/applovin_report/__init__.py
+-rw-r--r--   0        0        0       19 2023-05-24 07:10:10.662819 applovin_report-0.1.3/applovin_report/app.py
+-rw-r--r--   0        0        0     2502 2023-05-24 07:10:10.666819 applovin_report-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-05-24 07:10:10.666819 applovin_report-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      586 2023-05-24 07:10:10.666819 applovin_report-0.1.3/tests/test_app.py
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 applovin_report-0.1.3/PKG-INFO
```

### Comparing `applovin_report-0.1.0/LICENSE` & `applovin_report-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `applovin_report-0.1.0/pyproject.toml` & `applovin_report-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "applovin_report"
-version = "0.1.0"
+version = "0.1.3"
 homepage = "https://github.com/ikamedawn/applovin_report"
 description = "Applovin Report APIs wrapper."
 authors = ["Dawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
@@ -30,15 +30,15 @@
 pytest-cov = { version = "^4.0.0", optional = true }
 tox = { version = "^4.5.1", optional = true }
 virtualenv = { version = "^20.23.0", optional = true }
 pip = { version = "^23.1.2", optional = true }
 mkdocs = { version = "^1.4.3", optional = true }
 mkdocs-include-markdown-plugin = { version = "^4.0.4", optional = true }
 mkdocs-material = { version = "^9.1.14", optional = true }
-mkdocstrings = { version = "^0.21.2", optional = true }
+mkdocstrings-python = { version = "^1.0.0", optional = true }
 mkdocs-material-extensions = { version = "^1.0.3", optional = true }
 twine = { version = "^4.0.2", optional = true }
 mkdocs-autorefs = { version = "^0.4.1", optional = true }
 pre-commit = { version = "^3.3.2", optional = true }
 toml = { version = "^0.10.2", optional = true }
 livereload = { version = "^2.6.3", optional = true }
 pyreadline = { version = "^2.1", optional = true }
@@ -56,23 +56,26 @@
 
 dev = ["tox", "pre-commit", "virtualenv", "pip", "twine", "toml"]
 
 doc = [
     "mkdocs",
     "mkdocs-include-markdown-plugin",
     "mkdocs-material",
-    "mkdocstrings",
-    "mkdocs-material-extension",
+    "mkdocstrings-python",
+    "mkdocs-material-extensions",
     "mkdocs-autorefs",
     "mike"
 ]
 
 
 
 
+[tool.poetry.group.dev.dependencies]
+setuptools = "^67.8.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
```

### Comparing `applovin_report-0.1.0/tests/test_app.py` & `applovin_report-0.1.3/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `applovin_report-0.1.0/PKG-INFO` & `applovin_report-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6170 706c  : 2.1.Name: appl
 00000020: 6f76 696e 2d72 6570 6f72 740a 5665 7273  ovin-report.Vers
-00000030: 696f 6e3a 2030 2e31 2e30 0a53 756d 6d61  ion: 0.1.0.Summa
+00000030: 696f 6e3a 2030 2e31 2e33 0a53 756d 6d61  ion: 0.1.3.Summa
 00000040: 7279 3a20 4170 706c 6f76 696e 2052 6570  ry: Applovin Rep
 00000050: 6f72 7420 4150 4973 2077 7261 7070 6572  ort APIs wrapper
 00000060: 2e0a 486f 6d65 2d70 6167 653a 2068 7474  ..Home-page: htt
 00000070: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000080: 696b 616d 6564 6177 6e2f 6170 706c 6f76  ikamedawn/applov
 00000090: 696e 5f72 6570 6f72 740a 4c69 6365 6e73  in_report.Licens
 000000a0: 653a 204d 4954 0a41 7574 686f 723a 2044  e: MIT.Author: D
@@ -74,118 +74,96 @@
 00000490: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
 000004a0: 6373 2d6d 6174 6572 6961 6c20 283e 3d39  cs-material (>=9
 000004b0: 2e31 2e31 342c 3c31 302e 302e 3029 203b  .1.14,<10.0.0) ;
 000004c0: 2065 7874 7261 203d 3d20 2264 6f63 220a   extra == "doc".
 000004d0: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
 000004e0: 6b64 6f63 732d 6d61 7465 7269 616c 2d65  kdocs-material-e
 000004f0: 7874 656e 7369 6f6e 7320 283e 3d31 2e30  xtensions (>=1.0
-00000500: 2e33 2c3c 322e 302e 3029 0a52 6571 7569  .3,<2.0.0).Requi
-00000510: 7265 732d 4469 7374 3a20 6d6b 646f 6373  res-Dist: mkdocs
-00000520: 7472 696e 6773 2028 3e3d 302e 3231 2e32  trings (>=0.21.2
-00000530: 2c3c 302e 3232 2e30 2920 3b20 6578 7472  ,<0.22.0) ; extr
-00000540: 6120 3d3d 2022 646f 6322 0a52 6571 7569  a == "doc".Requi
-00000550: 7265 732d 4469 7374 3a20 7069 7020 283e  res-Dist: pip (>
-00000560: 3d32 332e 312e 322c 3c32 342e 302e 3029  =23.1.2,<24.0.0)
-00000570: 203b 2065 7874 7261 203d 3d20 2264 6576   ; extra == "dev
-00000580: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000590: 2070 7265 2d63 6f6d 6d69 7420 283e 3d33   pre-commit (>=3
-000005a0: 2e33 2e32 2c3c 342e 302e 3029 203b 2065  .3.2,<4.0.0) ; e
-000005b0: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
-000005c0: 7175 6972 6573 2d44 6973 743a 2070 7972  quires-Dist: pyr
-000005d0: 6561 646c 696e 6520 283e 3d32 2e31 2c3c  eadline (>=2.1,<
-000005e0: 332e 3029 0a52 6571 7569 7265 732d 4469  3.0).Requires-Di
-000005f0: 7374 3a20 7079 7465 7374 2028 3e3d 372e  st: pytest (>=7.
-00000600: 302e 312c 3c38 2e30 2e30 2920 3b20 6578  0.1,<8.0.0) ; ex
-00000610: 7472 6120 3d3d 2022 7465 7374 220a 5265  tra == "test".Re
-00000620: 7175 6972 6573 2d44 6973 743a 2070 7974  quires-Dist: pyt
-00000630: 6573 742d 636f 7620 283e 3d34 2e30 2e30  est-cov (>=4.0.0
-00000640: 2c3c 352e 302e 3029 203b 2065 7874 7261  ,<5.0.0) ; extra
-00000650: 203d 3d20 2274 6573 7422 0a52 6571 7569   == "test".Requi
-00000660: 7265 732d 4469 7374 3a20 746f 6d6c 2028  res-Dist: toml (
-00000670: 3e3d 302e 3130 2e32 2c3c 302e 3131 2e30  >=0.10.2,<0.11.0
-00000680: 2920 3b20 6578 7472 6120 3d3d 2022 6465  ) ; extra == "de
-00000690: 7622 0a52 6571 7569 7265 732d 4469 7374  v".Requires-Dist
-000006a0: 3a20 746f 7820 283e 3d34 2e35 2e31 2c3c  : tox (>=4.5.1,<
-000006b0: 352e 302e 3029 203b 2065 7874 7261 203d  5.0.0) ; extra =
-000006c0: 3d20 2264 6576 220a 5265 7175 6972 6573  = "dev".Requires
-000006d0: 2d44 6973 743a 2074 7769 6e65 2028 3e3d  -Dist: twine (>=
-000006e0: 342e 302e 322c 3c35 2e30 2e30 2920 3b20  4.0.2,<5.0.0) ; 
-000006f0: 6578 7472 6120 3d3d 2022 6465 7622 0a52  extra == "dev".R
-00000700: 6571 7569 7265 732d 4469 7374 3a20 7669  equires-Dist: vi
-00000710: 7274 7561 6c65 6e76 2028 3e3d 3230 2e32  rtualenv (>=20.2
-00000720: 332e 302c 3c32 312e 302e 3029 203b 2065  3.0,<21.0.0) ; e
-00000730: 7874 7261 203d 3d20 2264 6576 220a 4465  xtra == "dev".De
-00000740: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000750: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000760: 6b64 6f77 6e0a 0a23 2061 7070 6c6f 7669  kdown..# applovi
-00000770: 6e2d 7265 706f 7274 0a0a 0a3c 7020 616c  n-report...<p al
-00000780: 6967 6e3d 2263 656e 7465 7222 3e0a 3c61  ign="center">.<a
-00000790: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
-000007a0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
-000007b0: 7970 692f 6170 706c 6f76 696e 5f72 6570  ypi/applovin_rep
-000007c0: 6f72 7422 3e0a 2020 2020 3c69 6d67 2073  ort">.    <img s
-000007d0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-000007e0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-000007f0: 762f 6170 706c 6f76 696e 5f72 6570 6f72  v/applovin_repor
-00000800: 742e 7376 6722 0a20 2020 2020 2020 2061  t.svg".        a
-00000810: 6c74 203d 2022 5265 6c65 6173 6520 5374  lt = "Release St
-00000820: 6174 7573 223e 0a3c 2f61 3e0a 0a3c 6120  atus">.</a>..<a 
-00000830: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000840: 7468 7562 2e63 6f6d 2f69 6b61 6d65 6461  thub.com/ikameda
-00000850: 776e 2f61 7070 6c6f 7669 6e5f 7265 706f  wn/applovin_repo
-00000860: 7274 2f61 6374 696f 6e73 223e 0a20 2020  rt/actions">.   
-00000870: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000880: 3a2f 2f67 6974 6875 622e 636f 6d2f 696b  ://github.com/ik
-00000890: 616d 6564 6177 6e2f 6170 706c 6f76 696e  amedawn/applovin
-000008a0: 5f72 6570 6f72 742f 6163 7469 6f6e 732f  _report/actions/
-000008b0: 776f 726b 666c 6f77 732f 6465 762e 796d  workflows/dev.ym
-000008c0: 6c2f 6261 6467 652e 7376 6722 2061 6c74  l/badge.svg" alt
-000008d0: 3d22 6465 7622 3e0a 3c2f 613e 0a0a 3c61  ="dev">.</a>..<a
-000008e0: 2068 7265 663d 2268 7474 7073 3a2f 2f69   href="https://i
-000008f0: 6b61 6d65 6461 776e 2e67 6974 6875 622e  kamedawn.github.
-00000900: 696f 2f61 7070 6c6f 7669 6e5f 7265 706f  io/applovin_repo
-00000910: 7274 2f22 3e0a 2020 2020 3c69 6d67 2073  rt/">.    <img s
-00000920: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000930: 7368 6965 6c64 732e 696f 2f77 6562 7369  shields.io/websi
-00000940: 7465 2f68 7474 7073 2f69 6b61 6d65 6461  te/https/ikameda
-00000950: 776e 2e67 6974 6875 622e 696f 2f61 7070  wn.github.io/app
-00000960: 6c6f 7669 6e5f 7265 706f 7274 2f69 6e64  lovin_report/ind
-00000970: 6578 2e68 746d 6c2e 7376 673f 6c61 6265  ex.html.svg?labe
-00000980: 6c3d 646f 6373 2664 6f77 6e5f 6d65 7373  l=docs&down_mess
-00000990: 6167 653d 756e 6176 6169 6c61 626c 6526  age=unavailable&
-000009a0: 7570 5f6d 6573 7361 6765 3d61 7661 696c  up_message=avail
-000009b0: 6162 6c65 2220 616c 743d 2244 6f63 756d  able" alt="Docum
-000009c0: 656e 7461 7469 6f6e 2053 7461 7475 7322  entation Status"
-000009d0: 3e0a 3c2f 613e 0a0a 3c61 2068 7265 663d  >.</a>..<a href=
-000009e0: 2268 7474 7073 3a2f 2f70 7975 702e 696f  "https://pyup.io
-000009f0: 2f72 6570 6f73 2f67 6974 6875 622f 696b  /repos/github/ik
-00000a00: 616d 6564 6177 6e2f 6170 706c 6f76 696e  amedawn/applovin
-00000a10: 5f72 6570 6f72 742f 223e 0a3c 696d 6720  _report/">.<img 
-00000a20: 7372 633d 2268 7474 7073 3a2f 2f70 7975  src="https://pyu
-00000a30: 702e 696f 2f72 6570 6f73 2f67 6974 6875  p.io/repos/githu
-00000a40: 622f 696b 616d 6564 6177 6e2f 6170 706c  b/ikamedawn/appl
-00000a50: 6f76 696e 5f72 6570 6f72 742f 7368 6965  ovin_report/shie
-00000a60: 6c64 2e73 7667 2220 616c 743d 2255 7064  ld.svg" alt="Upd
-00000a70: 6174 6573 223e 0a3c 2f61 3e0a 0a3c 2f70  ates">.</a>..</p
-00000a80: 3e0a 0a0a 4170 706c 6f76 696e 2052 6570  >...Applovin Rep
-00000a90: 6f72 7420 4150 4973 2077 7261 7070 6572  ort APIs wrapper
-00000aa0: 0a0a 0a2a 2046 7265 6520 736f 6674 7761  ...* Free softwa
-00000ab0: 7265 3a20 4d49 540a 2a20 446f 6375 6d65  re: MIT.* Docume
-00000ac0: 6e74 6174 696f 6e3a 203c 6874 7470 733a  ntation: <https:
-00000ad0: 2f2f 696b 616d 6564 6177 6e2e 6769 7468  //ikamedawn.gith
-00000ae0: 7562 2e69 6f2f 6170 706c 6f76 696e 5f72  ub.io/applovin_r
-00000af0: 6570 6f72 742f 3e0a 0a0a 2323 2046 6561  eport/>...## Fea
-00000b00: 7475 7265 730a 0a2a 2054 4f44 4f0a 0a23  tures..* TODO..#
-00000b10: 2320 4372 6564 6974 730a 0a54 6869 7320  # Credits..This 
-00000b20: 7061 636b 6167 6520 7761 7320 6372 6561  package was crea
-00000b30: 7465 6420 7769 7468 2074 6865 205b 7070  ted with the [pp
-00000b40: 775d 2868 7474 7073 3a2f 2f7a 696c 6c69  w](https://zilli
-00000b50: 6f6e 6172 652e 6769 7468 7562 2e69 6f2f  onare.github.io/
-00000b60: 7079 7468 6f6e 2d70 726f 6a65 6374 2d77  python-project-w
-00000b70: 697a 6172 6429 2074 6f6f 6c2e 2046 6f72  izard) tool. For
-00000b80: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00000b90: 6e2c 2070 6c65 6173 6520 7669 7369 7420  n, please visit 
-00000ba0: 7468 6520 5b70 726f 6a65 6374 2070 6167  the [project pag
-00000bb0: 655d 2868 7474 7073 3a2f 2f7a 696c 6c69  e](https://zilli
-00000bc0: 6f6e 6172 652e 6769 7468 7562 2e69 6f2f  onare.github.io/
-00000bd0: 7079 7468 6f6e 2d70 726f 6a65 6374 2d77  python-project-w
-00000be0: 697a 6172 642f 292e 0a0a                 izard/)...
+00000500: 2e33 2c3c 322e 302e 3029 203b 2065 7874  .3,<2.0.0) ; ext
+00000510: 7261 203d 3d20 2264 6f63 220a 5265 7175  ra == "doc".Requ
+00000520: 6972 6573 2d44 6973 743a 206d 6b64 6f63  ires-Dist: mkdoc
+00000530: 7374 7269 6e67 732d 7079 7468 6f6e 2028  strings-python (
+00000540: 3e3d 312e 302e 302c 3c32 2e30 2e30 2920  >=1.0.0,<2.0.0) 
+00000550: 3b20 6578 7472 6120 3d3d 2022 646f 6322  ; extra == "doc"
+00000560: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000570: 7069 7020 283e 3d32 332e 312e 322c 3c32  pip (>=23.1.2,<2
+00000580: 342e 302e 3029 203b 2065 7874 7261 203d  4.0.0) ; extra =
+00000590: 3d20 2264 6576 220a 5265 7175 6972 6573  = "dev".Requires
+000005a0: 2d44 6973 743a 2070 7265 2d63 6f6d 6d69  -Dist: pre-commi
+000005b0: 7420 283e 3d33 2e33 2e32 2c3c 342e 302e  t (>=3.3.2,<4.0.
+000005c0: 3029 203b 2065 7874 7261 203d 3d20 2264  0) ; extra == "d
+000005d0: 6576 220a 5265 7175 6972 6573 2d44 6973  ev".Requires-Dis
+000005e0: 743a 2070 7972 6561 646c 696e 6520 283e  t: pyreadline (>
+000005f0: 3d32 2e31 2c3c 332e 3029 0a52 6571 7569  =2.1,<3.0).Requi
+00000600: 7265 732d 4469 7374 3a20 7079 7465 7374  res-Dist: pytest
+00000610: 2028 3e3d 372e 302e 312c 3c38 2e30 2e30   (>=7.0.1,<8.0.0
+00000620: 2920 3b20 6578 7472 6120 3d3d 2022 7465  ) ; extra == "te
+00000630: 7374 220a 5265 7175 6972 6573 2d44 6973  st".Requires-Dis
+00000640: 743a 2070 7974 6573 742d 636f 7620 283e  t: pytest-cov (>
+00000650: 3d34 2e30 2e30 2c3c 352e 302e 3029 203b  =4.0.0,<5.0.0) ;
+00000660: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
+00000670: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000680: 746f 6d6c 2028 3e3d 302e 3130 2e32 2c3c  toml (>=0.10.2,<
+00000690: 302e 3131 2e30 2920 3b20 6578 7472 6120  0.11.0) ; extra 
+000006a0: 3d3d 2022 6465 7622 0a52 6571 7569 7265  == "dev".Require
+000006b0: 732d 4469 7374 3a20 746f 7820 283e 3d34  s-Dist: tox (>=4
+000006c0: 2e35 2e31 2c3c 352e 302e 3029 203b 2065  .5.1,<5.0.0) ; e
+000006d0: 7874 7261 203d 3d20 2264 6576 220a 5265  xtra == "dev".Re
+000006e0: 7175 6972 6573 2d44 6973 743a 2074 7769  quires-Dist: twi
+000006f0: 6e65 2028 3e3d 342e 302e 322c 3c35 2e30  ne (>=4.0.2,<5.0
+00000700: 2e30 2920 3b20 6578 7472 6120 3d3d 2022  .0) ; extra == "
+00000710: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000720: 7374 3a20 7669 7274 7561 6c65 6e76 2028  st: virtualenv (
+00000730: 3e3d 3230 2e32 332e 302c 3c32 312e 302e  >=20.23.0,<21.0.
+00000740: 3029 203b 2065 7874 7261 203d 3d20 2264  0) ; extra == "d
+00000750: 6576 220a 4465 7363 7269 7074 696f 6e2d  ev".Description-
+00000760: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+00000770: 7874 2f6d 6172 6b64 6f77 6e0a 0a23 2061  xt/markdown..# a
+00000780: 7070 6c6f 7669 6e2d 7265 706f 7274 0a0a  pplovin-report..
+00000790: 5b21 5b72 656c 6561 7365 5d28 6874 7470  [![release](http
+000007a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000007b0: 696f 2f70 7970 692f 762f 6170 706c 6f76  io/pypi/v/applov
+000007c0: 696e 5f72 6570 6f72 742e 7376 6729 5d28  in_report.svg)](
+000007d0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000007e0: 2f70 726f 6a65 6374 2f61 7070 6c6f 7669  /project/applovi
+000007f0: 6e2d 7265 706f 7274 2f29 0a5b 215b 646f  n-report/).[![do
+00000800: 6373 5d28 6874 7470 733a 2f2f 696d 672e  cs](https://img.
+00000810: 7368 6965 6c64 732e 696f 2f77 6562 7369  shields.io/websi
+00000820: 7465 2f68 7474 7073 2f69 6b61 6d65 6461  te/https/ikameda
+00000830: 776e 2e67 6974 6875 622e 696f 2f61 7070  wn.github.io/app
+00000840: 6c6f 7669 6e5f 7265 706f 7274 2f69 6e64  lovin_report/ind
+00000850: 6578 2e68 746d 6c2e 7376 673f 6c61 6265  ex.html.svg?labe
+00000860: 6c3d 646f 6373 2664 6f77 6e5f 6d65 7373  l=docs&down_mess
+00000870: 6167 653d 756e 6176 6169 6c61 626c 6526  age=unavailable&
+00000880: 7570 5f6d 6573 7361 6765 3d61 7661 696c  up_message=avail
+00000890: 6162 6c65 295d 2868 7474 7073 3a2f 2f69  able)](https://i
+000008a0: 6b61 6d65 6461 776e 2e67 6974 6875 622e  kamedawn.github.
+000008b0: 696f 2f61 7070 6c6f 7669 6e5f 7265 706f  io/applovin_repo
+000008c0: 7274 290a 5b21 5b64 6576 656c 6f70 5d28  rt).[![develop](
+000008d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000008e0: 6f6d 2f69 6b61 6d65 6461 776e 2f61 7070  om/ikamedawn/app
+000008f0: 6c6f 7669 6e5f 7265 706f 7274 2f61 6374  lovin_report/act
+00000900: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f64  ions/workflows/d
+00000910: 6576 2e79 6d6c 2f62 6164 6765 2e73 7667  ev.yml/badge.svg
+00000920: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000930: 622e 636f 6d2f 696b 616d 6564 6177 6e2f  b.com/ikamedawn/
+00000940: 6170 706c 6f76 696e 5f72 6570 6f72 742f  applovin_report/
+00000950: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000960: 732f 6465 762e 796d 6c29 0a5b 215b 6d61  s/dev.yml).[![ma
+00000970: 696e 5d28 6874 7470 733a 2f2f 6769 7468  in](https://gith
+00000980: 7562 2e63 6f6d 2f69 6b61 6d65 6461 776e  ub.com/ikamedawn
+00000990: 2f61 7070 6c6f 7669 6e5f 7265 706f 7274  /applovin_report
+000009a0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+000009b0: 7773 2f72 656c 6561 7365 2e79 6d6c 2f62  ws/release.yml/b
+000009c0: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+000009d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 696b  ://github.com/ik
+000009e0: 616d 6564 6177 6e2f 6170 706c 6f76 696e  amedawn/applovin
+000009f0: 5f72 6570 6f72 742f 6163 7469 6f6e 732f  _report/actions/
+00000a00: 776f 726b 666c 6f77 732f 7265 6c65 6173  workflows/releas
+00000a10: 652e 796d 6c29 0a0a 4170 706c 6f76 696e  e.yml)..Applovin
+00000a20: 2052 6570 6f72 7420 4150 4973 2077 7261   Report APIs wra
+00000a30: 7070 6572 0a0a 2a20 446f 6375 6d65 6e74  pper..* Document
+00000a40: 6174 696f 6e3a 203c 6874 7470 733a 2f2f  ation: <https://
+00000a50: 696b 616d 6564 6177 6e2e 6769 7468 7562  ikamedawn.github
+00000a60: 2e69 6f2f 6170 706c 6f76 696e 5f72 6570  .io/applovin_rep
+00000a70: 6f72 742f 3e0a 0a23 2320 4665 6174 7572  ort/>..## Featur
+00000a80: 6573 0a0a 2a20 544f 444f 0a0a            es..* TODO..
```

