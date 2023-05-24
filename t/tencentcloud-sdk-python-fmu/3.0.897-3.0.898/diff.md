# Comparing `tmp/tencentcloud-sdk-python-fmu-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-fmu-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.897.tar", last modified: Tue May 23 02:22:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.898.tar", last modified: Wed May 24 01:57:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-fmu-3.0.897.tar` & `tencentcloud-sdk-python-fmu-3.0.898.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/v20191213/
--rw-r--r--   0 root         (0) root         (0)    10489 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/v20191213/fmu_client.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/v20191213/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/v20191213/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31049 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/v20191213/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud_sdk_python_fmu.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:22:53.000000 tencentcloud-sdk-python-fmu-3.0.897/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/
+-rw-r--r--   0 root         (0) root         (0)    10552 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/fmu_client.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31049 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.897/README.rst` & `tencentcloud-sdk-python-fmu-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/v20191213/fmu_client.py` & `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/fmu_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class FmuClient(AbstractClient):
     _apiVersion = '2019-12-13'
     _endpoint = 'fmu.tencentcloudapi.com'
     _service = 'fmu'
 
 
     def BeautifyPic(self, request):
-        """用户上传一张人脸图片，精准定位五官，实现美肤、亮肤、祛痘等美颜功能。
+        """用户上传一张人脸图片（最多能处理一张图片中最大的五张人脸信息），精准定位五官，实现美肤、亮肤、祛痘等美颜功能。
 
         :param request: Request instance for BeautifyPic.
         :type request: :class:`tencentcloud.fmu.v20191213.models.BeautifyPicRequest`
         :rtype: :class:`tencentcloud.fmu.v20191213.models.BeautifyPicResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/v20191213/errorcodes.py` & `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.897/tencentcloud/fmu/v20191213/models.py` & `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.898/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.897/setup.py` & `tencentcloud-sdk-python-fmu-3.0.898/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.897/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

