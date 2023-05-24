# Comparing `tmp/mtbase-4.4.202305240933-py3-none-any.whl.zip` & `tmp/mtbase-4.5.202305240940-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 93503 bytes, number of entries: 69
+Zip file size: 113950 bytes, number of entries: 75
 -rw-r--r--  2.0 unx     2172 b- defN 23-Apr-15 06:17 mt/aio/__init__.py
 -rw-r--r--  2.0 unx     4130 b- defN 23-Apr-15 06:17 mt/aio/base.py
 -rw-r--r--  2.0 unx    12618 b- defN 23-Jan-22 22:24 mt/aio/files.py
 -rw-r--r--  2.0 unx     8978 b- defN 23-Jan-22 22:24 mt/aio/multiprocessing.py
 -rw-r--r--  2.0 unx     9873 b- defN 23-Jan-24 17:12 mt/aio/path.py
 -rw-r--r--  2.0 unx     3323 b- defN 23-Jan-22 22:24 mt/aio/procedure.py
 -rw-r--r--  2.0 unx     1659 b- defN 23-Apr-15 06:08 mt/base/__init__.py
 -rw-r--r--  2.0 unx      221 b- defN 23-May-24 06:11 mt/base/aio.py
 -rw-r--r--  2.0 unx    16034 b- defN 23-Jan-22 22:24 mt/base/bg_invoke.py
 -rw-r--r--  2.0 unx     2471 b- defN 23-Jan-22 22:24 mt/base/casting.py
+-rw-r--r--  2.0 unx      259 b- defN 23-May-24 09:39 mt/base/concurrency.py
 -rw-r--r--  2.0 unx      165 b- defN 23-Jan-22 22:24 mt/base/const.py
 -rw-r--r--  2.0 unx      245 b- defN 23-Jan-22 22:24 mt/base/contextlib.py
 -rw-r--r--  2.0 unx      885 b- defN 23-Feb-26 09:07 mt/base/datatype.py
 -rw-r--r--  2.0 unx     5676 b- defN 23-Jan-22 22:24 mt/base/debug_process.py
 -rw-r--r--  2.0 unx     6863 b- defN 23-Jan-22 22:24 mt/base/deprecated.py
 -rw-r--r--  2.0 unx     1786 b- defN 23-Apr-15 06:08 mt/base/exec.py
 -rw-r--r--  2.0 unx     2655 b- defN 23-Jan-22 22:24 mt/base/filetype.py
@@ -26,22 +27,27 @@
 -rw-r--r--  2.0 unx      512 b- defN 23-Jan-22 22:24 mt/base/pyximportcpp.py
 -rw-r--r--  2.0 unx    19514 b- defN 23-Mar-17 08:13 mt/base/s3.py
 -rw-r--r--  2.0 unx    11810 b- defN 23-Feb-15 12:15 mt/base/s3transfer.py
 -rw-r--r--  2.0 unx     3363 b- defN 23-Jan-22 22:24 mt/base/str.py
 -rw-r--r--  2.0 unx      104 b- defN 23-Jan-22 22:24 mt/base/terminal.py
 -rw-r--r--  2.0 unx      110 b- defN 23-Jan-22 22:24 mt/base/threading.py
 -rw-r--r--  2.0 unx       86 b- defN 23-Jan-22 22:24 mt/base/traceback.py
--rw-r--r--  2.0 unx      396 b- defN 23-May-24 09:33 mt/base/version.py
+-rw-r--r--  2.0 unx      396 b- defN 23-May-24 09:40 mt/base/version.py
 -rw-r--r--  2.0 unx      547 b- defN 23-Jan-22 22:24 mt/base/with_utils.py
 -rw-r--r--  2.0 unx     1765 b- defN 23-Jan-22 22:24 mt/base/zipfile.py
 -rw-r--r--  2.0 unx      411 b- defN 23-May-24 06:08 mt/base/concurrency/__init__.py
 -rw-r--r--  2.0 unx    15541 b- defN 23-May-24 06:08 mt/base/concurrency/aio.py
 -rw-r--r--  2.0 unx     2442 b- defN 23-May-24 09:33 mt/base/concurrency/base.py
 -rw-r--r--  2.0 unx    41884 b- defN 23-Jan-24 17:12 mt/base/concurrency/beehive.py
 -rw-r--r--  2.0 unx    19261 b- defN 23-May-24 06:20 mt/base/concurrency/multiprocessing.py
+-rw-r--r--  2.0 unx      411 b- defN 23-May-24 06:08 mt/concurrency/__init__.py
+-rw-r--r--  2.0 unx    15541 b- defN 23-May-24 06:08 mt/concurrency/aio.py
+-rw-r--r--  2.0 unx     2442 b- defN 23-May-24 09:33 mt/concurrency/base.py
+-rw-r--r--  2.0 unx    41884 b- defN 23-Jan-24 17:12 mt/concurrency/beehive.py
+-rw-r--r--  2.0 unx    19267 b- defN 23-May-24 09:40 mt/concurrency/multiprocessing.py
 -rw-r--r--  2.0 unx      804 b- defN 23-Jan-22 22:24 mt/ctx/__init__.py
 -rw-r--r--  2.0 unx      901 b- defN 23-Mar-01 10:58 mt/jax/__init__.py
 -rw-r--r--  2.0 unx      847 b- defN 23-Mar-01 10:58 mt/jnp/__init__.py
 -rw-r--r--  2.0 unx      847 b- defN 23-Mar-01 10:58 mt/jsp/__init__.py
 -rw-r--r--  2.0 unx    20596 b- defN 23-Apr-15 05:57 mt/logg/__init__.py
 -rw-r--r--  2.0 unx      679 b- defN 23-Jan-24 17:12 mt/mpl/__init__.py
 -rw-r--r--  2.0 unx     1061 b- defN 23-Apr-20 19:15 mt/net/__init__.py
@@ -58,14 +64,14 @@
 -rw-r--r--  2.0 unx     1513 b- defN 23-Jan-22 22:24 mt/path/__init__.py
 -rw-r--r--  2.0 unx      694 b- defN 23-Jan-24 17:12 mt/plt/__init__.py
 -rw-r--r--  2.0 unx      990 b- defN 23-Jan-22 22:24 mt/shutil/__init__.py
 -rw-r--r--  2.0 unx     4994 b- defN 23-Jan-22 22:24 mt/threading/__init__.py
 -rw-r--r--  2.0 unx     2158 b- defN 23-Jan-22 22:24 mt/time/__init__.py
 -rw-r--r--  2.0 unx      521 b- defN 23-Jan-24 17:12 mt/tp/__init__.py
 -rw-r--r--  2.0 unx     1043 b- defN 23-Jan-22 22:24 mt/traceback/__init__.py
--rwxr-xr-x  2.0 unx      690 b- defN 23-May-24 09:33 mtbase-4.4.202305240933.data/scripts/path_exists
--rw-r--r--  2.0 unx     1070 b- defN 23-May-24 09:33 mtbase-4.4.202305240933.dist-info/LICENSE
--rw-r--r--  2.0 unx      776 b- defN 23-May-24 09:33 mtbase-4.4.202305240933.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 09:33 mtbase-4.4.202305240933.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-May-24 09:33 mtbase-4.4.202305240933.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5350 b- defN 23-May-24 09:33 mtbase-4.4.202305240933.dist-info/RECORD
-69 files, 306275 bytes uncompressed, 85251 bytes compressed:  72.2%
+-rwxr-xr-x  2.0 unx      690 b- defN 23-May-24 09:41 mtbase-4.5.202305240940.data/scripts/path_exists
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-24 09:41 mtbase-4.5.202305240940.dist-info/LICENSE
+-rw-r--r--  2.0 unx      776 b- defN 23-May-24 09:41 mtbase-4.5.202305240940.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 09:41 mtbase-4.5.202305240940.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-May-24 09:41 mtbase-4.5.202305240940.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5842 b- defN 23-May-24 09:41 mtbase-4.5.202305240940.dist-info/RECORD
+75 files, 386571 bytes uncompressed, 104944 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -24,14 +24,17 @@
 
 Filename: mt/base/bg_invoke.py
 Comment: 
 
 Filename: mt/base/casting.py
 Comment: 
 
+Filename: mt/base/concurrency.py
+Comment: 
+
 Filename: mt/base/const.py
 Comment: 
 
 Filename: mt/base/contextlib.py
 Comment: 
 
 Filename: mt/base/datatype.py
@@ -111,14 +114,29 @@
 
 Filename: mt/base/concurrency/beehive.py
 Comment: 
 
 Filename: mt/base/concurrency/multiprocessing.py
 Comment: 
 
+Filename: mt/concurrency/__init__.py
+Comment: 
+
+Filename: mt/concurrency/aio.py
+Comment: 
+
+Filename: mt/concurrency/base.py
+Comment: 
+
+Filename: mt/concurrency/beehive.py
+Comment: 
+
+Filename: mt/concurrency/multiprocessing.py
+Comment: 
+
 Filename: mt/ctx/__init__.py
 Comment: 
 
 Filename: mt/jax/__init__.py
 Comment: 
 
 Filename: mt/jnp/__init__.py
@@ -183,26 +201,26 @@
 
 Filename: mt/tp/__init__.py
 Comment: 
 
 Filename: mt/traceback/__init__.py
 Comment: 
 
-Filename: mtbase-4.4.202305240933.data/scripts/path_exists
+Filename: mtbase-4.5.202305240940.data/scripts/path_exists
 Comment: 
 
-Filename: mtbase-4.4.202305240933.dist-info/LICENSE
+Filename: mtbase-4.5.202305240940.dist-info/LICENSE
 Comment: 
 
-Filename: mtbase-4.4.202305240933.dist-info/METADATA
+Filename: mtbase-4.5.202305240940.dist-info/METADATA
 Comment: 
 
-Filename: mtbase-4.4.202305240933.dist-info/WHEEL
+Filename: mtbase-4.5.202305240940.dist-info/WHEEL
 Comment: 
 
-Filename: mtbase-4.4.202305240933.dist-info/top_level.txt
+Filename: mtbase-4.5.202305240940.dist-info/top_level.txt
 Comment: 
 
-Filename: mtbase-4.4.202305240933.dist-info/RECORD
+Filename: mtbase-4.5.202305240940.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/base/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
 VERSION_DAY = int('24')
 VERSION_HOUR = int('09')
-VERSION_MINUTE = int('33')
+VERSION_MINUTE = int('40')
 MAJOR_VERSION = 4
-MINOR_VERSION = 4
-PATCH_VERSION = 202305240933
-version_date = '2023/05/24 09:33'
+MINOR_VERSION = 5
+PATCH_VERSION = 202305240940
+version_date = '2023/05/24 09:40'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtbase-4.4.202305240933.data/scripts/path_exists` & `mtbase-4.5.202305240940.data/scripts/path_exists`

 * *Files identical despite different names*

## Comparing `mtbase-4.4.202305240933.dist-info/LICENSE` & `mtbase-4.5.202305240940.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtbase-4.4.202305240933.dist-info/METADATA` & `mtbase-4.5.202305240940.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtbase
-Version: 4.4.202305240933
+Version: 4.5.202305240940
 Summary: The most fundamental Python modules for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtbase
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.base/mt.base.html
 Project-URL: Source Code, https://github.com/inteplus/mtbase
 Requires-Python: >=3.6
 License-File: LICENSE
```

## Comparing `mtbase-4.4.202305240933.dist-info/RECORD` & `mtbase-4.5.202305240940.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 mt/aio/multiprocessing.py,sha256=G43P7bN10J7UqTYCsa1eh3VatJWEbLEqg1xNK3MKWdk,8978
 mt/aio/path.py,sha256=oOVNblXkChVKJCP062ynnL5YbUglyqE9WTch7NZmc_Y,9873
 mt/aio/procedure.py,sha256=eJ4AtCxqvDDxGrz-Pycred1CJRfD60VPvjUaaJ0OhYM,3323
 mt/base/__init__.py,sha256=1LzDyZSIZrxAsfgYNRHSHLUlntv47uVQ4qNOzmGTV-o,1659
 mt/base/aio.py,sha256=d-nijaZ-saqowUK1bn7HBriw5CCl9yjn_6lfuF-O2l4,221
 mt/base/bg_invoke.py,sha256=NzFNMl8fbS26dod-gi0m1f-BlQworFzWtrOTCwFT_WQ,16034
 mt/base/casting.py,sha256=yHmHDzISEsarasHQXg6MmqNYuxt1Ab4MYj8Okh2-oN8,2471
+mt/base/concurrency.py,sha256=6jjrHDdO4KxAWYYTc_8gsJ3m0yn82LZnL78yIUYVDRU,259
 mt/base/const.py,sha256=ifyavLDbeEeeAHmfsu7VDhcVpi1UcMFUg6fYL6bMPPk,165
 mt/base/contextlib.py,sha256=F-7j3hDxeyZIutD7Q7xgRER8AQSpX7KtZFcU9JPKlk8,245
 mt/base/datatype.py,sha256=psLw2Aus9kk8gCv2orY6qzM2_QFmKJe1Kzf9zC2DURo,885
 mt/base/debug_process.py,sha256=0m0TkTsg8dMvHafdK4dcXliRZ8PeZeDcOtzWQEMA7HE,5676
 mt/base/deprecated.py,sha256=RGNXdAlxjrLQj4kCCI3qhxE8bUBjn1ZtZUfsbnGjQ5M,6863
 mt/base/exec.py,sha256=npgBV9memCutw9xBOQthwCS3Tj44TN_UqVqfldVWSNU,1786
 mt/base/filetype.py,sha256=LaBEhDARcISamnNjOv90X0_Z7M-ofmpXS5YHc3NNqO4,2655
@@ -25,22 +26,27 @@
 mt/base/pyximportcpp.py,sha256=U3CHv8DcA4HndNp3ckAx-4JlHqdjstiZZTWWVp652AI,512
 mt/base/s3.py,sha256=sHGUMXUNlVUhynBkRnAYAlyf9Vb44CWAeJu9RmFs2n4,19514
 mt/base/s3transfer.py,sha256=RVdh2qL_t-EsztILt87K8D1TcA8ZydJzZ-l3Sl0hV4U,11810
 mt/base/str.py,sha256=GdEv5lBns95hMovlWohtQGVI4bt-SmoONfKRJ5qtRvk,3363
 mt/base/terminal.py,sha256=_23Kk7oihgCbe2yjJw2SQrTCqymSi-drejn1SWIS6IY,104
 mt/base/threading.py,sha256=MTVjpaTg_sbZWCksoP_5iMVYFjjUxrgpYBMOWxFY4Ms,110
 mt/base/traceback.py,sha256=Zn4oNs_f4mleJakpSaCbpMNfMt4O0gQEQrA6oChixdk,86
-mt/base/version.py,sha256=bpfWhaBMDrK8s4itZgvEaqGs7m_jONjOXUr3mo1fJ1A,396
+mt/base/version.py,sha256=8bPMPMvAdwLh7T7_NxQMPGqVwpzgCBirtsYdFtxmkLQ,396
 mt/base/with_utils.py,sha256=-7OAVtGjL1dy2bhJ0II8McJKaAG8yUWr_GhccxT15Z8,547
 mt/base/zipfile.py,sha256=SnsBCaPlPw300_mi7WYB6wSqjvW-U_g96vS2S9JwrnE,1765
 mt/base/concurrency/__init__.py,sha256=XxsRYuCXlM3fGNERLIHY0m9IrhQH06TqMVqPkOiIevU,411
 mt/base/concurrency/aio.py,sha256=z3i_89CMqCB-mwUqco6rZR1eQYqVAGmCJOBSN-ZiQic,15541
 mt/base/concurrency/base.py,sha256=psGzEzyoARWl97N5y0Hbhkjq8RnE-jkPoBK6u44PNEg,2442
 mt/base/concurrency/beehive.py,sha256=IG7mw8eKjrGW7Im7JJWSWHrZEh1JUyffERqxgka5ErA,41884
 mt/base/concurrency/multiprocessing.py,sha256=E_wTvC5Jj9gHaHrxEuDYzqmiOZXzF8xKjM8HcgdrFR4,19261
+mt/concurrency/__init__.py,sha256=XxsRYuCXlM3fGNERLIHY0m9IrhQH06TqMVqPkOiIevU,411
+mt/concurrency/aio.py,sha256=z3i_89CMqCB-mwUqco6rZR1eQYqVAGmCJOBSN-ZiQic,15541
+mt/concurrency/base.py,sha256=psGzEzyoARWl97N5y0Hbhkjq8RnE-jkPoBK6u44PNEg,2442
+mt/concurrency/beehive.py,sha256=IG7mw8eKjrGW7Im7JJWSWHrZEh1JUyffERqxgka5ErA,41884
+mt/concurrency/multiprocessing.py,sha256=Ejnt_4y2V2_Nf34ZOpt1tE_rP2mJ8JbNWJXkESL7hQU,19267
 mt/ctx/__init__.py,sha256=7V7zNr6VGNVNOxLQGZhZVmAP_jCw7JeHr77oAIwK68A,804
 mt/jax/__init__.py,sha256=H8yaQTicZJirPJAIJ59dqyUlW9HKjtSFMVhm77-n_04,901
 mt/jnp/__init__.py,sha256=ffCUR9x3KOcoHWZRFNHxL56EvcR3D-Vq3ODLIDG6Orc,847
 mt/jsp/__init__.py,sha256=JWOoWzwT_4mGyklotUbtSg4Sx5Sr_C16Nd7AvxRnQ2o,847
 mt/logg/__init__.py,sha256=w43fyKjZzeXDY9XXLml1ixdg1KFXuh4-bWYX5LNGD24,20596
 mt/mpl/__init__.py,sha256=T0xg7jVS4Ix3LXnbi1hE_tod5LUMjkKpLRwEozdRRcE,679
 mt/net/__init__.py,sha256=0SRSEqpoaq2QaunkYOWMmB7plnXLQiTrwQ6M1sXs7co,1061
@@ -57,13 +63,13 @@
 mt/path/__init__.py,sha256=7sFKV5T0nDk9lWIHhDPiDqZtE3sazKfkBBMedJrb4RA,1513
 mt/plt/__init__.py,sha256=y1RQmfTCjOYOzeAvnbnwTzw89LKiquUj28_PpwKslFg,694
 mt/shutil/__init__.py,sha256=PW9_pxVH3EVdxETupRoFc5StyyS8A8LX1lRFGVr8I4A,990
 mt/threading/__init__.py,sha256=dE7YEfeBMyxJ1DzFox28r0e2CzsSMWtm2XCvyk_ewXg,4994
 mt/time/__init__.py,sha256=lAjC0En0X0spHTu2YC120AchNlv1SzHgQlX0RmXWLEc,2158
 mt/tp/__init__.py,sha256=9yEoip3w8V2X1a49APJDC8EqVlGoa3WpR3DNXBX-cKk,521
 mt/traceback/__init__.py,sha256=7_aNd4u_CXRgWlzgfz3x7BnWta4DoAqrFFrIAiEqjJI,1043
-mtbase-4.4.202305240933.data/scripts/path_exists,sha256=9rYAZNiVEeTTi-hKM8NkQVIZOaEQkWE_WVw72avfUDo,690
-mtbase-4.4.202305240933.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
-mtbase-4.4.202305240933.dist-info/METADATA,sha256=rIxkjlyW0yILl47LVuRKG9718j4pMJRTnfZqIVMFY_Y,776
-mtbase-4.4.202305240933.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mtbase-4.4.202305240933.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtbase-4.4.202305240933.dist-info/RECORD,,
+mtbase-4.5.202305240940.data/scripts/path_exists,sha256=9rYAZNiVEeTTi-hKM8NkQVIZOaEQkWE_WVw72avfUDo,690
+mtbase-4.5.202305240940.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
+mtbase-4.5.202305240940.dist-info/METADATA,sha256=QYxlpIWt1l4t_qQmksHi8Nml3IzzuMF8LYkTh4ydSFQ,776
+mtbase-4.5.202305240940.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mtbase-4.5.202305240940.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtbase-4.5.202305240940.dist-info/RECORD,,
```

