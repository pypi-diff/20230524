# Comparing `tmp/tencentcloud-sdk-python-chdfs-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-chdfs-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-chdfs-3.0.897.tar", last modified: Tue May 23 02:17:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-chdfs-3.0.898.tar", last modified: Wed May 24 01:51:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-chdfs-3.0.897.tar` & `tencentcloud-sdk-python-chdfs-3.0.898.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20190718/
--rw-r--r--   0 root         (0) root         (0)     3280 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20190718/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20190718/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51568 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20190718/models.py
--rw-r--r--   0 root         (0) root         (0)    28022 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20190718/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20201112/
--rw-r--r--   0 root         (0) root         (0)     3600 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20201112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20201112/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57610 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20201112/models.py
--rw-r--r--   0 root         (0) root         (0)    27286 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20201112/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud_sdk_python_chdfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud_sdk_python_chdfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud_sdk_python_chdfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:17:11.000000 tencentcloud-sdk-python-chdfs-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20190718/
+-rw-r--r--   0 root         (0) root         (0)     3280 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20190718/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20190718/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51568 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20190718/models.py
+-rw-r--r--   0 root         (0) root         (0)    28022 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20190718/chdfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20201112/
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20201112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20201112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60294 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20201112/models.py
+-rw-r--r--   0 root         (0) root         (0)    27286 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20201112/chdfs_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud_sdk_python_chdfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud_sdk_python_chdfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud_sdk_python_chdfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 01:51:48.000000 tencentcloud-sdk-python-chdfs-3.0.898/setup.cfg
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/README.rst` & `tencentcloud-sdk-python-chdfs-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20190718/errorcodes.py` & `tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20190718/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20190718/models.py` & `tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20190718/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20190718/chdfs_client.py` & `tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20190718/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20201112/errorcodes.py` & `tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20201112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20201112/models.py` & `tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20201112/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1365,35 +1365,45 @@
         :type Path: str
         :param Transitions: 生命周期规则转换列表
         :type Transitions: list of Transition
         :param Status: 生命周期规则状态（1：打开；2：关闭）
         :type Status: int
         :param CreateTime: 创建时间
         :type CreateTime: str
+        :param Summary: 生命周期规则当前路径具体存储量
+        :type Summary: :class:`tencentcloud.chdfs.v20201112.models.Summary`
+        :param LastSummaryTime: Summary更新时间
+        :type LastSummaryTime: str
         """
         self.LifeCycleRuleId = None
         self.LifeCycleRuleName = None
         self.Path = None
         self.Transitions = None
         self.Status = None
         self.CreateTime = None
+        self.Summary = None
+        self.LastSummaryTime = None
 
 
     def _deserialize(self, params):
         self.LifeCycleRuleId = params.get("LifeCycleRuleId")
         self.LifeCycleRuleName = params.get("LifeCycleRuleName")
         self.Path = params.get("Path")
         if params.get("Transitions") is not None:
             self.Transitions = []
             for item in params.get("Transitions"):
                 obj = Transition()
                 obj._deserialize(item)
                 self.Transitions.append(obj)
         self.Status = params.get("Status")
         self.CreateTime = params.get("CreateTime")
+        if params.get("Summary") is not None:
+            self.Summary = Summary()
+            self.Summary._deserialize(params.get("Summary"))
+        self.LastSummaryTime = params.get("LastSummaryTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1791,14 +1801,64 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class Summary(AbstractModel):
+    """生命周期规则当前路径具体存储量信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CapacityUsed: 总存储量（单位byte）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CapacityUsed: int
+        :param StandardCapacityUsed: 标准存储量（单位byte）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StandardCapacityUsed: int
+        :param DegradeCapacityUsed: 低频存储量（单位byte）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DegradeCapacityUsed: int
+        :param ArchiveCapacityUsed: 归档存储量（单位byte）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ArchiveCapacityUsed: int
+        :param DeepArchiveCapacityUsed: 深度归档存储量（单位byte）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeepArchiveCapacityUsed: int
+        :param IntelligentCapacityUsed: 智能分层存储量（单位byte）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IntelligentCapacityUsed: int
+        """
+        self.CapacityUsed = None
+        self.StandardCapacityUsed = None
+        self.DegradeCapacityUsed = None
+        self.ArchiveCapacityUsed = None
+        self.DeepArchiveCapacityUsed = None
+        self.IntelligentCapacityUsed = None
+
+
+    def _deserialize(self, params):
+        self.CapacityUsed = params.get("CapacityUsed")
+        self.StandardCapacityUsed = params.get("StandardCapacityUsed")
+        self.DegradeCapacityUsed = params.get("DegradeCapacityUsed")
+        self.ArchiveCapacityUsed = params.get("ArchiveCapacityUsed")
+        self.DeepArchiveCapacityUsed = params.get("DeepArchiveCapacityUsed")
+        self.IntelligentCapacityUsed = params.get("IntelligentCapacityUsed")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class Tag(AbstractModel):
     """资源标签。
 
     """
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/chdfs/v20201112/chdfs_client.py` & `tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/chdfs/v20201112/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud_sdk_python_chdfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-chdfs-3.0.898/tencentcloud_sdk_python_chdfs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-chdfs
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Chdfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-chdfs-3.0.898/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-chdfs
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Chdfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-chdfs-3.0.897/setup.py` & `tencentcloud-sdk-python-chdfs-3.0.898/setup.py`

 * *Files identical despite different names*

