# Comparing `tmp/tencentcloud-sdk-python-live-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.897.tar", last modified: Tue May 23 02:26:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.898.tar", last modified: Wed May 24 02:00:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.897.tar` & `tencentcloud-sdk-python-live-3.0.898.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   137459 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18117 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   431326 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:26:03.000000 tencentcloud-sdk-python-live-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-24 02:00:48.000000 tencentcloud-sdk-python-live-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   137459 2023-05-24 02:00:48.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18117 2023-05-24 02:00:48.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:00:48.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   431811 2023-05-24 02:00:48.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:00:48.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 02:00:48.000000 tencentcloud-sdk-python-live-3.0.898/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-24 02:00:48.000000 tencentcloud-sdk-python-live-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 02:00:49.000000 tencentcloud-sdk-python-live-3.0.898/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.897/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.898/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.897/README.rst` & `tencentcloud-sdk-python-live-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/v20180801/live_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.897/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.898/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3702,17 +3702,23 @@
 class DescribeCallbackRecordsListRequest(AbstractModel):
     """DescribeCallbackRecordsList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param StartTime: 起始时间点，格式为yyyy-mm-dd HH:MM:SS。
+        :param StartTime: 起始时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
         :type StartTime: str
-        :param EndTime: 结束时间点，格式为yyyy-mm-dd HH:MM:SS，起始和结束时间跨度不支持超过1天。
+        :param EndTime: 结束时间点，接口查询支持两种时间格式：
+1）YYYY-MM-DDThh:mm:ssZ：UTC时间格式，详见IOS日期格式说明文档: https://cloud.tencent.com/document/product/266/11732#I
+2）YYYY-MM-DD hh:mm:ss：使用此格式时，默认代表北京时间。
+
+查询的起始和结束时间跨度不支持超过1天。仅支持查询最近14天的数据。
         :type EndTime: str
         :param StreamName: 流名称，精确匹配。
         :type StreamName: str
         :param PageNum: 页码。
         :type PageNum: int
         :param PageSize: 每页条数。
         :type PageSize: int
```

### Comparing `tencentcloud-sdk-python-live-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.898/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.898/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.897/setup.py` & `tencentcloud-sdk-python-live-3.0.898/setup.py`

 * *Files identical despite different names*

