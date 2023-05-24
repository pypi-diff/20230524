# Comparing `tmp/bocfx-0.7.9.tar.gz` & `tmp/bocfx-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bocfx-0.7.9.tar", last modified: Sat Jun  4 10:53:25 2022, max compression
+gzip compressed data, was "bocfx-0.8.0.tar", last modified: Tue May 23 16:27:57 2023, max compression
```

## Comparing `bocfx-0.7.9.tar` & `bocfx-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2022-06-04 10:53:25.817248 bocfx-0.7.9/
--rw-r--r--   0 bob        (501) staff       (20)     1073 2019-02-20 22:13:33.000000 bocfx-0.7.9/LICENSE
--rw-r--r--   0 bob        (501) staff       (20)    17496 2022-06-04 10:53:25.816471 bocfx-0.7.9/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)    17076 2020-10-31 18:08:35.000000 bocfx-0.7.9/README.md
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2022-06-04 10:53:25.814123 bocfx-0.7.9/bocfx/
--rwxr-xr-x   0 bob        (501) staff       (20)      417 2020-03-22 14:42:55.000000 bocfx-0.7.9/bocfx/__init__.py
--rw-r--r--   0 bob        (501) staff       (20)    11348 2022-06-04 10:46:08.000000 bocfx-0.7.9/bocfx/__main__.py
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2022-06-04 10:53:25.816053 bocfx-0.7.9/bocfx.egg-info/
--rw-r--r--   0 bob        (501) staff       (20)    17496 2022-06-04 10:53:25.000000 bocfx-0.7.9/bocfx.egg-info/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)      238 2022-06-04 10:53:25.000000 bocfx-0.7.9/bocfx.egg-info/SOURCES.txt
--rw-r--r--   0 bob        (501) staff       (20)        1 2022-06-04 10:53:25.000000 bocfx-0.7.9/bocfx.egg-info/dependency_links.txt
--rw-r--r--   0 bob        (501) staff       (20)       39 2022-06-04 10:53:25.000000 bocfx-0.7.9/bocfx.egg-info/entry_points.txt
--rw-r--r--   0 bob        (501) staff       (20)       50 2022-06-04 10:53:25.000000 bocfx-0.7.9/bocfx.egg-info/requires.txt
--rw-r--r--   0 bob        (501) staff       (20)        6 2022-06-04 10:53:25.000000 bocfx-0.7.9/bocfx.egg-info/top_level.txt
--rw-r--r--   0 bob        (501) staff       (20)       38 2022-06-04 10:53:25.817348 bocfx-0.7.9/setup.cfg
--rwxr-xr-x   0 bob        (501) staff       (20)      880 2022-06-04 10:49:28.000000 bocfx-0.7.9/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-23 16:27:57.561104 bocfx-0.8.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-05-23 16:00:18.000000 bocfx-0.8.0/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17323 2023-05-23 16:27:57.557104 bocfx-0.8.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16903 2023-05-23 16:11:35.000000 bocfx-0.8.0/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-23 16:27:57.557104 bocfx-0.8.0/bocfx/
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)      417 2023-05-23 16:00:18.000000 bocfx-0.8.0/bocfx/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11484 2023-05-23 16:25:11.000000 bocfx-0.8.0/bocfx/__main__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-23 16:27:57.557104 bocfx-0.8.0/bocfx.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17323 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      238 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       39 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-05-23 16:27:57.000000 bocfx-0.8.0/bocfx.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-23 16:27:57.561104 bocfx-0.8.0/setup.cfg
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)      880 2023-05-23 16:26:11.000000 bocfx-0.8.0/setup.py
```

### Comparing `bocfx-0.7.9/LICENSE` & `bocfx-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bocfx-0.7.9/PKG-INFO` & `bocfx-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,22 @@
-Metadata-Version: 2.1
-Name: bocfx
-Version: 0.7.9
-Summary: Easy API to get foreign exchange rate from Bank of China.
-Home-page: https://github.com/bobleer/bocfx
-Author: bobleer
-Author-email: liwenbo628@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.7.7-ffd242.svg)
+# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.8.0-ffd242.svg)
 An easy-to-use python package for getting foreign exchange rate from Bank of China (BOC).  
 一个帮你快速获取中国银行外汇牌价的 Python 爬虫（也可作外汇牌价实时查询API)。  
 Author: [**Bob Lee**](https://boblee.cn)
 
 <br>
 
 # Features
 # 特点
 
 * [x] **Multithreading 多线程**
 * [x] **As a command-line application 支持命令行应用模式**
 * [x] **As a python module 支持模块导入模式（import到你自己的项目里就能作API了）**
 * [x] **Foreign exchange selection 支持多种外汇币种同时输出（默认是英、欧、美、加、澳）**
-* [x] **Foreign exchange quotation filter 支持外汇牌价种类同时输出（买入、卖出、现钞、现汇）**
+* [x] **Foreign exchange quotation filter 支持外汇牌价种类同时输出（买入、卖出、现钞、现汇、中行折算价）**
 * [x] **Date selection (Realtime/History) 支持仅输出最新牌价 或 输出指定时间段内全部牌价变动**
 * [x] **Line graph generation 支持生成历史波动曲线**
 * [x] **.csv generation 支持导出csv格式表格文件**
 * [x] **Set output path 支持导出到指定路径**
 * [x] **Show or close loading bar 支持显示或关闭进度条**
 * [x] **Export to database 支持导出到数据库（可使用Pandas的df.to_sql()）**
 
@@ -79,55 +66,53 @@
 # 基本用法 (输出最新的牌价)
 <br>
 
 ## As a command-line application
 ## 作为命令行工具使用
 
 ```
-❯ bocfx                        
-100%|████████████████████████████████████████████| 5/5 [00:00<00:00, 471.66it/s]
+❯ bocfx
+
 
-+-----+--------+--------+--------+--------+---------------------+
-|  5  | SE_BID | BN_BID | SE_ASK | BN_ASK |         Time        |
-+-----+--------+--------+--------+--------+---------------------+
-| GBP | 873.53 | 846.38 | 879.96 | 882.1  | 2019-02-25 09:25:37 |
-| EUR | 758.54 | 734.97 | 764.14 | 765.83 | 2019-02-25 09:25:37 |
-| USD | 669.44 | 663.99 | 672.28 | 672.28 | 2019-02-25 09:25:37 |
-| CAD | 509.1  | 493.03 | 512.86 | 514.1  | 2019-02-25 09:25:37 |
-| AUD | 476.19 | 461.4  | 479.69 | 480.87 | 2019-02-25 10:10:35 |
-+-----+--------+--------+--------+--------+---------------------+
++-----+--------+--------+--------+--------+----------+---------------------+
+|  5  | SE_BID | BN_BID | SE_ASK | BN_ASK | BOC_CONV |         Time        |
++-----+--------+--------+--------+--------+----------+---------------------+
+| GBP | 873.01 | 845.88 | 879.44 | 883.32 |  874.54  | 2023-05-23 23:09:35 |
+| EUR | 757.61 | 734.07 | 763.19 | 765.65 |  760.31  | 2023-05-23 23:09:35 |
+| USD | 703.77 | 698.05 | 706.76 | 706.76 |  703.26  | 2023-05-23 23:09:35 |
+| CAD | 520.43 |  504   | 524.27 | 526.58 |  520.83  | 2023-05-23 23:09:35 |
+| AUD | 465.18 | 450.73 | 468.6  | 470.68 |  467.72  | 2023-05-23 23:09:35 |
++-----+--------+--------+--------+--------+----------+---------------------+
 (SE = Spot Exchange, BN = Banknote)
 ```
 
 ```
 ❯ bocfx -f USD                
 
 
-+-----+--------+--------+--------+--------+---------------------+
-|  1  | SE_BID | BN_BID | SE_ASK | BN_ASK |         Time        |
-+-----+--------+--------+--------+--------+---------------------+
-| USD | 682.91 | 677.36 | 685.81 | 685.81 | 2020-09-06 10:30:00 |
-+-----+--------+--------+--------+--------+---------------------+
++-----+--------+--------+--------+--------+----------+---------------------+
+|  1  | SE_BID | BN_BID | SE_ASK | BN_ASK | BOC_CONV |         Time        |
++-----+--------+--------+--------+--------+----------+---------------------+
+| USD | 703.77 | 698.05 | 706.76 | 706.76 |  703.26  | 2023-05-23 23:25:12 |
++-----+--------+--------+--------+--------+----------+---------------------+
 (SE = Spot Exchange, BN = Banknote)
 ```
 
 <br>
 <br>
 
 ## As a Python module
 ## 作为 Python 模块导入使用
 
 ```
 >>> from bocfx import bocfx
 
 >>> output = bocfx('GBP,USD','SE,ASK') # 选择了英镑和美元，现汇卖出价
-100%|████████████████████████████████████████████| 5/5 [00:00<00:00, 532.87it/s]
-
 >>> output # The latest foreign exchange rate | 英镑和美元，现汇卖出价 (最新的牌价)
-['879.96', '672.28'] 
+['879.22', '706.76'] 
 ```
 <br>
 <br>
 
 # Advanced Usage
 # 进阶用法
 <br>
@@ -264,15 +249,15 @@
 `加拿大元` | `CAD` | Canadian Dollar | `CA` 
 `澳大利亚元` | `AUD` | Australian Dollar | `AU` 
 `欧元` | `EUR` | Euro | `EU` 
 `澳门元` | `MOP` | Macao Pataca | `MO`
 `菲律宾比索` | `PHP` | Philippine Peso | 
 `泰国铢` | `THB` | Thai Baht | 
 `新西兰元` | `NZD` | New Zealand Dollar | `KIWI` 
-`韩元` | `WON` | South Korean Won | `SK` 
+`韩国元` | `WON` | South Korean Won | `SK` 
 `卢布` | `RUB` | Russian Ruble | `RU` 
 `林吉特` | `MYR` | Malaysia Ringgit | `SEN` 
 `新台币` | `NTD` | New Taiwan Dollar | `TW` 
 `西班牙比塞塔` | `ESP` | Spain Peseta | 
 `意大利里拉` | `ITL` | Italian Lira | 
 `荷兰盾` | `ANG` | Nederlandse Gulden | 
 `比利时法郎` | `BEF` | Belgian Franc | 
@@ -283,15 +268,15 @@
 `阿联酋迪拉姆` | `AED` | United Arab Emirates Dirham | 
 `南非兰特` | `ZAF` | South African Rand | 
 `沙特里亚尔` | `SAR` | Saudi Arabian Riyal | 
 `土耳其里拉` | `TRY` | Yeni Türk Lirası | `YTL` 
   
 FX, ISO and Alias can be used as values of this option, e.g. `英镑`, `GBP`, `UK` are all correct.  
 This parameter is case-insensitive, e.g. `GBP`, `gBp`, `UK`, `uk` will get same output.  
-If not using this option, the default parameter will be `GBP, EUR, USD, CAD, AUD`.  
+If not setting this parameter, the default value of parameter will be `GBP, EUR, USD, CAD, AUD`.  
 <br>
 <br>
 
 #### Example:
 
 ```
 ~
```

### Comparing `bocfx-0.7.9/README.md` & `bocfx-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,35 @@
-# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.7.7-ffd242.svg)
+Metadata-Version: 2.1
+Name: bocfx
+Version: 0.8.0
+Summary: Easy API to get foreign exchange rate from Bank of China.
+Home-page: https://github.com/bobleer/bocfx
+Author: bobleer
+Author-email: liwenbo628@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.8.0-ffd242.svg)
 An easy-to-use python package for getting foreign exchange rate from Bank of China (BOC).  
 一个帮你快速获取中国银行外汇牌价的 Python 爬虫（也可作外汇牌价实时查询API)。  
 Author: [**Bob Lee**](https://boblee.cn)
 
 <br>
 
 # Features
 # 特点
 
 * [x] **Multithreading 多线程**
 * [x] **As a command-line application 支持命令行应用模式**
 * [x] **As a python module 支持模块导入模式（import到你自己的项目里就能作API了）**
 * [x] **Foreign exchange selection 支持多种外汇币种同时输出（默认是英、欧、美、加、澳）**
-* [x] **Foreign exchange quotation filter 支持外汇牌价种类同时输出（买入、卖出、现钞、现汇）**
+* [x] **Foreign exchange quotation filter 支持外汇牌价种类同时输出（买入、卖出、现钞、现汇、中行折算价）**
 * [x] **Date selection (Realtime/History) 支持仅输出最新牌价 或 输出指定时间段内全部牌价变动**
 * [x] **Line graph generation 支持生成历史波动曲线**
 * [x] **.csv generation 支持导出csv格式表格文件**
 * [x] **Set output path 支持导出到指定路径**
 * [x] **Show or close loading bar 支持显示或关闭进度条**
 * [x] **Export to database 支持导出到数据库（可使用Pandas的df.to_sql()）**
 
@@ -66,55 +79,53 @@
 # 基本用法 (输出最新的牌价)
 <br>
 
 ## As a command-line application
 ## 作为命令行工具使用
 
 ```
-❯ bocfx                        
-100%|████████████████████████████████████████████| 5/5 [00:00<00:00, 471.66it/s]
+❯ bocfx
+
 
-+-----+--------+--------+--------+--------+---------------------+
-|  5  | SE_BID | BN_BID | SE_ASK | BN_ASK |         Time        |
-+-----+--------+--------+--------+--------+---------------------+
-| GBP | 873.53 | 846.38 | 879.96 | 882.1  | 2019-02-25 09:25:37 |
-| EUR | 758.54 | 734.97 | 764.14 | 765.83 | 2019-02-25 09:25:37 |
-| USD | 669.44 | 663.99 | 672.28 | 672.28 | 2019-02-25 09:25:37 |
-| CAD | 509.1  | 493.03 | 512.86 | 514.1  | 2019-02-25 09:25:37 |
-| AUD | 476.19 | 461.4  | 479.69 | 480.87 | 2019-02-25 10:10:35 |
-+-----+--------+--------+--------+--------+---------------------+
++-----+--------+--------+--------+--------+----------+---------------------+
+|  5  | SE_BID | BN_BID | SE_ASK | BN_ASK | BOC_CONV |         Time        |
++-----+--------+--------+--------+--------+----------+---------------------+
+| GBP | 873.01 | 845.88 | 879.44 | 883.32 |  874.54  | 2023-05-23 23:09:35 |
+| EUR | 757.61 | 734.07 | 763.19 | 765.65 |  760.31  | 2023-05-23 23:09:35 |
+| USD | 703.77 | 698.05 | 706.76 | 706.76 |  703.26  | 2023-05-23 23:09:35 |
+| CAD | 520.43 |  504   | 524.27 | 526.58 |  520.83  | 2023-05-23 23:09:35 |
+| AUD | 465.18 | 450.73 | 468.6  | 470.68 |  467.72  | 2023-05-23 23:09:35 |
++-----+--------+--------+--------+--------+----------+---------------------+
 (SE = Spot Exchange, BN = Banknote)
 ```
 
 ```
 ❯ bocfx -f USD                
 
 
-+-----+--------+--------+--------+--------+---------------------+
-|  1  | SE_BID | BN_BID | SE_ASK | BN_ASK |         Time        |
-+-----+--------+--------+--------+--------+---------------------+
-| USD | 682.91 | 677.36 | 685.81 | 685.81 | 2020-09-06 10:30:00 |
-+-----+--------+--------+--------+--------+---------------------+
++-----+--------+--------+--------+--------+----------+---------------------+
+|  1  | SE_BID | BN_BID | SE_ASK | BN_ASK | BOC_CONV |         Time        |
++-----+--------+--------+--------+--------+----------+---------------------+
+| USD | 703.77 | 698.05 | 706.76 | 706.76 |  703.26  | 2023-05-23 23:25:12 |
++-----+--------+--------+--------+--------+----------+---------------------+
 (SE = Spot Exchange, BN = Banknote)
 ```
 
 <br>
 <br>
 
 ## As a Python module
 ## 作为 Python 模块导入使用
 
 ```
 >>> from bocfx import bocfx
 
 >>> output = bocfx('GBP,USD','SE,ASK') # 选择了英镑和美元，现汇卖出价
-100%|████████████████████████████████████████████| 5/5 [00:00<00:00, 532.87it/s]
-
 >>> output # The latest foreign exchange rate | 英镑和美元，现汇卖出价 (最新的牌价)
-['879.96', '672.28'] 
+['879.22', '706.76'] 
 ```
 <br>
 <br>
 
 # Advanced Usage
 # 进阶用法
 <br>
@@ -251,15 +262,15 @@
 `加拿大元` | `CAD` | Canadian Dollar | `CA` 
 `澳大利亚元` | `AUD` | Australian Dollar | `AU` 
 `欧元` | `EUR` | Euro | `EU` 
 `澳门元` | `MOP` | Macao Pataca | `MO`
 `菲律宾比索` | `PHP` | Philippine Peso | 
 `泰国铢` | `THB` | Thai Baht | 
 `新西兰元` | `NZD` | New Zealand Dollar | `KIWI` 
-`韩元` | `WON` | South Korean Won | `SK` 
+`韩国元` | `WON` | South Korean Won | `SK` 
 `卢布` | `RUB` | Russian Ruble | `RU` 
 `林吉特` | `MYR` | Malaysia Ringgit | `SEN` 
 `新台币` | `NTD` | New Taiwan Dollar | `TW` 
 `西班牙比塞塔` | `ESP` | Spain Peseta | 
 `意大利里拉` | `ITL` | Italian Lira | 
 `荷兰盾` | `ANG` | Nederlandse Gulden | 
 `比利时法郎` | `BEF` | Belgian Franc | 
@@ -270,15 +281,15 @@
 `阿联酋迪拉姆` | `AED` | United Arab Emirates Dirham | 
 `南非兰特` | `ZAF` | South African Rand | 
 `沙特里亚尔` | `SAR` | Saudi Arabian Riyal | 
 `土耳其里拉` | `TRY` | Yeni Türk Lirası | `YTL` 
   
 FX, ISO and Alias can be used as values of this option, e.g. `英镑`, `GBP`, `UK` are all correct.  
 This parameter is case-insensitive, e.g. `GBP`, `gBp`, `UK`, `uk` will get same output.  
-If not using this option, the default parameter will be `GBP, EUR, USD, CAD, AUD`.  
+If not setting this parameter, the default value of parameter will be `GBP, EUR, USD, CAD, AUD`.  
 <br>
 <br>
 
 #### Example:
 
 ```
 ~
```

### Comparing `bocfx-0.7.9/bocfx/__main__.py` & `bocfx-0.8.0/bocfx/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # coding: utf-8
 # Author: Bob Lee
 # Blog: https://boblee.cn
-# Version: 0.7.8
-# Date: 2020-11-01
+# Version: 0.8.0
+# Date: 2023-05-24 00:12:05
 
 import getopt
 import sys
 import time as tm
 import os
 import requests
 
@@ -88,14 +88,15 @@
     html = r.text
     for row in range(2,end):
         try:
             SE_B = Selector(text=html).xpath('//tr[%i]/td[2]/text()' % (row)).extract()[0].strip('\r\n\t ')
             BN_B = Selector(text=html).xpath('//tr[%i]/td[3]/text()' % (row)).extract()[0].strip('\r\n\t ')
             SE_A = Selector(text=html).xpath('//tr[%i]/td[4]/text()' % (row)).extract()[0].strip('\r\n\t ')
             BN_A = Selector(text=html).xpath('//tr[%i]/td[5]/text()' % (row)).extract()[0].strip('\r\n\t ')
+            BOC_C = Selector(text=html).xpath('//tr[%i]/td[6]/text()' % (row)).extract()[0].strip('\r\n\t ')
             time = Selector(text=html).xpath('//tr[%i]/td[7]/text()' % (row)).extract()[0].replace('.','-').strip('\r\n\t ')
             output.append(eval(sort))
 
         except IndexError:
             break
 
 
@@ -156,16 +157,16 @@
             sort = '(FX_or[i],SE_A,BN_A,time)'
             output = [(len(FX),'SE_ASK','BN_ASK','Time')]
         else:
             print("Sort Value error!")
             exit()
 
     else:
-        sort = '(FX_or[i],SE_B,BN_B,SE_A,BN_A,time)'
-        output = [(len(FX),'SE_BID','BN_BID','SE_ASK','BN_ASK','Time')]
+        sort = '(FX_or[i],SE_B,BN_B,SE_A,BN_A,BOC_C,time)'
+        output = [(len(FX),'SE_BID','BN_BID','SE_ASK','BN_ASK', 'BOC_CONV','Time')]
 
 
     if time != -1:
         if len(str(time)) < 5:
             today_nof = datetime.date.today()
             tegart_nof = today_nof - datetime.timedelta(days=int(time))
             erectDate = str(tegart_nof)
```

### Comparing `bocfx-0.7.9/bocfx.egg-info/PKG-INFO` & `bocfx-0.8.0/bocfx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: bocfx
-Version: 0.7.9
+Version: 0.8.0
 Summary: Easy API to get foreign exchange rate from Bank of China.
 Home-page: https://github.com/bobleer/bocfx
 Author: bobleer
 Author-email: liwenbo628@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.7.7-ffd242.svg)
+# bocfx ![](https://img.shields.io/badge/License-MIT-green.svg) ![](https://img.shields.io/badge/Python-3-3776ab.svg) ![](https://img.shields.io/badge/PyPI-0.8.0-ffd242.svg)
 An easy-to-use python package for getting foreign exchange rate from Bank of China (BOC).  
 一个帮你快速获取中国银行外汇牌价的 Python 爬虫（也可作外汇牌价实时查询API)。  
 Author: [**Bob Lee**](https://boblee.cn)
 
 <br>
 
 # Features
 # 特点
 
 * [x] **Multithreading 多线程**
 * [x] **As a command-line application 支持命令行应用模式**
 * [x] **As a python module 支持模块导入模式（import到你自己的项目里就能作API了）**
 * [x] **Foreign exchange selection 支持多种外汇币种同时输出（默认是英、欧、美、加、澳）**
-* [x] **Foreign exchange quotation filter 支持外汇牌价种类同时输出（买入、卖出、现钞、现汇）**
+* [x] **Foreign exchange quotation filter 支持外汇牌价种类同时输出（买入、卖出、现钞、现汇、中行折算价）**
 * [x] **Date selection (Realtime/History) 支持仅输出最新牌价 或 输出指定时间段内全部牌价变动**
 * [x] **Line graph generation 支持生成历史波动曲线**
 * [x] **.csv generation 支持导出csv格式表格文件**
 * [x] **Set output path 支持导出到指定路径**
 * [x] **Show or close loading bar 支持显示或关闭进度条**
 * [x] **Export to database 支持导出到数据库（可使用Pandas的df.to_sql()）**
 
@@ -79,55 +79,53 @@
 # 基本用法 (输出最新的牌价)
 <br>
 
 ## As a command-line application
 ## 作为命令行工具使用
 
 ```
-❯ bocfx                        
-100%|████████████████████████████████████████████| 5/5 [00:00<00:00, 471.66it/s]
+❯ bocfx
 
-+-----+--------+--------+--------+--------+---------------------+
-|  5  | SE_BID | BN_BID | SE_ASK | BN_ASK |         Time        |
-+-----+--------+--------+--------+--------+---------------------+
-| GBP | 873.53 | 846.38 | 879.96 | 882.1  | 2019-02-25 09:25:37 |
-| EUR | 758.54 | 734.97 | 764.14 | 765.83 | 2019-02-25 09:25:37 |
-| USD | 669.44 | 663.99 | 672.28 | 672.28 | 2019-02-25 09:25:37 |
-| CAD | 509.1  | 493.03 | 512.86 | 514.1  | 2019-02-25 09:25:37 |
-| AUD | 476.19 | 461.4  | 479.69 | 480.87 | 2019-02-25 10:10:35 |
-+-----+--------+--------+--------+--------+---------------------+
+
++-----+--------+--------+--------+--------+----------+---------------------+
+|  5  | SE_BID | BN_BID | SE_ASK | BN_ASK | BOC_CONV |         Time        |
++-----+--------+--------+--------+--------+----------+---------------------+
+| GBP | 873.01 | 845.88 | 879.44 | 883.32 |  874.54  | 2023-05-23 23:09:35 |
+| EUR | 757.61 | 734.07 | 763.19 | 765.65 |  760.31  | 2023-05-23 23:09:35 |
+| USD | 703.77 | 698.05 | 706.76 | 706.76 |  703.26  | 2023-05-23 23:09:35 |
+| CAD | 520.43 |  504   | 524.27 | 526.58 |  520.83  | 2023-05-23 23:09:35 |
+| AUD | 465.18 | 450.73 | 468.6  | 470.68 |  467.72  | 2023-05-23 23:09:35 |
++-----+--------+--------+--------+--------+----------+---------------------+
 (SE = Spot Exchange, BN = Banknote)
 ```
 
 ```
 ❯ bocfx -f USD                
 
 
-+-----+--------+--------+--------+--------+---------------------+
-|  1  | SE_BID | BN_BID | SE_ASK | BN_ASK |         Time        |
-+-----+--------+--------+--------+--------+---------------------+
-| USD | 682.91 | 677.36 | 685.81 | 685.81 | 2020-09-06 10:30:00 |
-+-----+--------+--------+--------+--------+---------------------+
++-----+--------+--------+--------+--------+----------+---------------------+
+|  1  | SE_BID | BN_BID | SE_ASK | BN_ASK | BOC_CONV |         Time        |
++-----+--------+--------+--------+--------+----------+---------------------+
+| USD | 703.77 | 698.05 | 706.76 | 706.76 |  703.26  | 2023-05-23 23:25:12 |
++-----+--------+--------+--------+--------+----------+---------------------+
 (SE = Spot Exchange, BN = Banknote)
 ```
 
 <br>
 <br>
 
 ## As a Python module
 ## 作为 Python 模块导入使用
 
 ```
 >>> from bocfx import bocfx
 
 >>> output = bocfx('GBP,USD','SE,ASK') # 选择了英镑和美元，现汇卖出价
-100%|████████████████████████████████████████████| 5/5 [00:00<00:00, 532.87it/s]
-
 >>> output # The latest foreign exchange rate | 英镑和美元，现汇卖出价 (最新的牌价)
-['879.96', '672.28'] 
+['879.22', '706.76'] 
 ```
 <br>
 <br>
 
 # Advanced Usage
 # 进阶用法
 <br>
@@ -264,15 +262,15 @@
 `加拿大元` | `CAD` | Canadian Dollar | `CA` 
 `澳大利亚元` | `AUD` | Australian Dollar | `AU` 
 `欧元` | `EUR` | Euro | `EU` 
 `澳门元` | `MOP` | Macao Pataca | `MO`
 `菲律宾比索` | `PHP` | Philippine Peso | 
 `泰国铢` | `THB` | Thai Baht | 
 `新西兰元` | `NZD` | New Zealand Dollar | `KIWI` 
-`韩元` | `WON` | South Korean Won | `SK` 
+`韩国元` | `WON` | South Korean Won | `SK` 
 `卢布` | `RUB` | Russian Ruble | `RU` 
 `林吉特` | `MYR` | Malaysia Ringgit | `SEN` 
 `新台币` | `NTD` | New Taiwan Dollar | `TW` 
 `西班牙比塞塔` | `ESP` | Spain Peseta | 
 `意大利里拉` | `ITL` | Italian Lira | 
 `荷兰盾` | `ANG` | Nederlandse Gulden | 
 `比利时法郎` | `BEF` | Belgian Franc | 
@@ -283,15 +281,15 @@
 `阿联酋迪拉姆` | `AED` | United Arab Emirates Dirham | 
 `南非兰特` | `ZAF` | South African Rand | 
 `沙特里亚尔` | `SAR` | Saudi Arabian Riyal | 
 `土耳其里拉` | `TRY` | Yeni Türk Lirası | `YTL` 
   
 FX, ISO and Alias can be used as values of this option, e.g. `英镑`, `GBP`, `UK` are all correct.  
 This parameter is case-insensitive, e.g. `GBP`, `gBp`, `UK`, `uk` will get same output.  
-If not using this option, the default parameter will be `GBP, EUR, USD, CAD, AUD`.  
+If not setting this parameter, the default value of parameter will be `GBP, EUR, USD, CAD, AUD`.  
 <br>
 <br>
 
 #### Example:
 
 ```
 ~
```

### Comparing `bocfx-0.7.9/setup.py` & `bocfx-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bocfx",
-    version="0.7.9",
+    version="0.8.0",
     author="bobleer",
     author_email="liwenbo628@gmail.com",
     description="Easy API to get foreign exchange rate from Bank of China.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bobleer/bocfx",
     packages=setuptools.find_packages(),
```

