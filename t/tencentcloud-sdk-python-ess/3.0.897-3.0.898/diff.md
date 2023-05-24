# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.897.tar", last modified: Tue May 23 02:22:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.898.tar", last modified: Wed May 24 01:57:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.897.tar` & `tencentcloud-sdk-python-ess-3.0.898.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    50900 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23810 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223352 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:22:28.000000 tencentcloud-sdk-python-ess-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    51121 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23810 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223352 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.897/README.rst` & `tencentcloud-sdk-python-ess-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.898/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.897'
+__version__ = '3.0.898'
```

### Comparing `tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,14 +349,15 @@
 
 
     def CreateFlowSignUrl(self, request):
         """创建个人H5签署链接，请联系客户经理申请使用 <br/>
         该接口用于发起合同后，生成C端签署人的签署链接 <br/>
         注意：该接口目前签署人类型仅支持个人签署方（PERSON） <br/>
         注意：该接口可生成签署链接的C端签署人必须仅有手写签名和时间类型的签署控件<br/>
+        注意：该接口返回的签署链接是用于APP集成的场景，支持APP打开或浏览器直接打开，不支持微信小程序嵌入。微信小程序请使用小程序跳转或半屏弹窗的方式<br/>
 
         :param request: Request instance for CreateFlowSignUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowSignUrlRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowSignUrlResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.897/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.897/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.898/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.897/setup.py` & `tencentcloud-sdk-python-ess-3.0.898/setup.py`

 * *Files identical despite different names*

