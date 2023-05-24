# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.897.tar", last modified: Tue May 23 02:16:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.898.tar", last modified: Wed May 24 01:51:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.897.tar` & `tencentcloud-sdk-python-cfs-3.0.898.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:16:57.000000 tencentcloud-sdk-python-cfs-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    14458 2023-05-23 02:16:57.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39796 2023-05-23 02:16:57.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:16:57.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)   116607 2023-05-23 02:16:57.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:16:57.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:16:57.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:16:57.000000 tencentcloud-sdk-python-cfs-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:16:58.000000 tencentcloud-sdk-python-cfs-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:34.000000 tencentcloud-sdk-python-cfs-3.0.898/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:34.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:34.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:34.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    14458 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39796 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   116710 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:34.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:51:34.000000 tencentcloud-sdk-python-cfs-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 01:51:33.000000 tencentcloud-sdk-python-cfs-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 01:51:34.000000 tencentcloud-sdk-python-cfs-3.0.898/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.897/README.rst` & `tencentcloud-sdk-python-cfs-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/cfs/v20190719/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,21 +408,21 @@
 
     """
 
     def __init__(self):
         r"""
         :param Zone: 可用区名称，例如ap-beijing-1，请参考 [概览](https://cloud.tencent.com/document/product/582/13225) 文档中的地域与可用区列表
         :type Zone: str
-        :param NetInterface: 网络类型，可选值为 VPC，BASIC，CCN；其中 VPC 为私有网络，BASIC 为基础网络, CCN 为云联网，Turbo系列当前必须选择云联网。目前基础网络已逐渐淘汰，不推荐使用。
+        :param NetInterface: 网络类型，可选值为 VPC，CCN；其中 VPC 为私有网络， CCN 为云联网。通用标准型/性能型请选择VPC，Turbo标准型/性能型请选择CCN。
         :type NetInterface: str
-        :param PGroupId: 权限组 ID，通用标准型和性能型必填，turbo系列请填写pgroupbasic
+        :param PGroupId: 权限组 ID
         :type PGroupId: str
         :param Protocol: 文件系统协议类型， 值为 NFS、CIFS、TURBO ; 若留空则默认为 NFS协议，turbo系列必须选择turbo，不支持NFS、CIFS
         :type Protocol: str
-        :param StorageType: 文件系统存储类型，默认值为 SD ；其中 SD 为通用标准型标准型存储， HP为通用性能型存储， TB为turbo标准型， TP 为turbo性能型。
+        :param StorageType: 文件系统存储类型，默认值为 SD ；其中 SD 为通用标准型存储， HP为通用性能型存储， TB为Turbo标准型， TP 为Turbo性能型。
         :type StorageType: str
         :param VpcId: 私有网络（VPC） ID，若网络类型选择的是VPC，该字段为必填。
         :type VpcId: str
         :param SubnetId: 子网 ID，若网络类型选择的是VPC，该字段为必填。
         :type SubnetId: str
         :param MountIP: 指定IP地址，仅VPC网络支持；若不填写、将在该子网下随机分配 IP，Turbo系列当前不支持指定
         :type MountIP: str
@@ -2786,28 +2786,32 @@
         :type AppId: int
         :param DeleteTime: 快照删除时间
         :type DeleteTime: str
         :param FsName: 文件系统名称
         :type FsName: str
         :param Tags: 快照标签
         :type Tags: list of TagInfo
+        :param SnapshotType: 快照类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SnapshotType: str
         """
         self.CreationTime = None
         self.SnapshotName = None
         self.SnapshotId = None
         self.Status = None
         self.RegionName = None
         self.FileSystemId = None
         self.Size = None
         self.AliveDay = None
         self.Percent = None
         self.AppId = None
         self.DeleteTime = None
         self.FsName = None
         self.Tags = None
+        self.SnapshotType = None
 
 
     def _deserialize(self, params):
         self.CreationTime = params.get("CreationTime")
         self.SnapshotName = params.get("SnapshotName")
         self.SnapshotId = params.get("SnapshotId")
         self.Status = params.get("Status")
@@ -2821,14 +2825,15 @@
         self.FsName = params.get("FsName")
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = TagInfo()
                 obj._deserialize(item)
                 self.Tags.append(obj)
+        self.SnapshotType = params.get("SnapshotType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.898/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.897/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.898/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.898/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.897/setup.py` & `tencentcloud-sdk-python-cfs-3.0.898/setup.py`

 * *Files identical despite different names*

