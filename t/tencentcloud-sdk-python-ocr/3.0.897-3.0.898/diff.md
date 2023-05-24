# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.897.tar", last modified: Tue May 23 02:28:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.898.tar", last modified: Wed May 24 02:02:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.897.tar` & `tencentcloud-sdk-python-ocr-3.0.898.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   113504 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505982 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:28:02.000000 tencentcloud-sdk-python-ocr-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   113613 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   506230 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.897/README.rst` & `tencentcloud-sdk-python-ocr-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,16 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CarInvoiceOCR(self, request):
         """本接口支持机动车销售统一发票和二手车销售统一发票的识别，包括发票号码、发票代码、合计金额、合计税额等二十多个字段。
 
+        默认接口请求频率限制：5次/秒。
+
         :param request: Request instance for CarInvoiceOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.CarInvoiceOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.CarInvoiceOCRResponse`
 
         """
         try:
             params = request._serialize()
@@ -1428,15 +1430,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RecognizeGeneralInvoice(self, request):
-        """本接口支持 PDF多页（最多30页）、一页中单张、多张、类型票据的混合识别，同时支持单选识别某类票据，已支持票种包括：增值税发票（专票、普票、卷票、区块链发票、通行费发票）、全电发票（专票、普票）、非税发票（通用票据、统一缴纳书）、定额发票、通用机打发票、购车发票（机动车销售发票、二手车发票）、火车票、出租车发票、机票行程单、汽车票、轮船票、过路过桥费发票共14种标准报销发票，并支持非上述类型的其他发票的智能识别。
+        """本接口支持 PDF多页（最多30页）、一页中单张、多张、类型票据的混合识别，同时支持单选识别某类票据，已支持票种包括：增值税发票（专票、普票、卷票、区块链发票、通行费发票）、全电发票（专票、普票）、非税发票（通用票据、统一缴纳书）、定额发票、通用机打发票、购车发票（机动车销售发票、二手车发票）、火车票、出租车发票、机票行程单、汽车票、轮船票、过路过桥费发票共14种标准报销发票，并支持非上述类型的其他发票的智能识别，点击[立即试用](https://cloud.tencent.com/product/ocr)。
 
         默认接口请求频率限制：5次/秒。
 
 
         支持返回的细项目子票种SubType、子票种中文TypeDescription、以及对应所属大类票种Type 的说明如下列表：
         <table style="width:715px">
               <thead>
@@ -1469,15 +1471,15 @@
                 </tr>
                 <tr>
                   <td> VatElectronicInvoiceBlockchain</td>
                   <td> 区块链电子发票 </td>
                   <td> 3 </td>
                 </tr>
                 <tr>
-                  <td> VatElectronicSpecialInvoiceFull</td>
+                  <td> VatElectronicInvoiceToll</td>
                   <td> 增值税电子普通发票(通行费)</td>
                   <td> 3 </td>
                 </tr>
                 <tr>
                   <td> VatElectronicSpecialInvoiceFull</td>
                   <td> 电子发票(专用发票)</td>
                   <td> 16 </td>
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1345,29 +1345,33 @@
         r"""
         :param FileList: 多个文件的URL列表
         :type FileList: list of SmartFormFileUrl
         :param FirstNotes: 备注信息1
         :type FirstNotes: str
         :param SecondNotes: 备注信息2
         :type SecondNotes: str
+        :param FileType: 文件类型
+        :type FileType: int
         """
         self.FileList = None
         self.FirstNotes = None
         self.SecondNotes = None
+        self.FileType = None
 
 
     def _deserialize(self, params):
         if params.get("FileList") is not None:
             self.FileList = []
             for item in params.get("FileList"):
                 obj = SmartFormFileUrl()
                 obj._deserialize(item)
                 self.FileList.append(obj)
         self.FirstNotes = params.get("FirstNotes")
         self.SecondNotes = params.get("SecondNotes")
+        self.FileType = params.get("FileType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6519,19 +6523,21 @@
     """
 
     def __init__(self):
         r"""
         :param ImageBase64: 图片的 Base64 值。
 支持的图片格式：PNG、JPG、JPEG、PDF，暂不支持 GIF 格式。
 支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
+支持的图片像素：需介于20-10000px之间。
 图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
         :type ImageBase64: str
         :param ImageUrl: 图片的 Url 地址。
 支持的图片格式：PNG、JPG、JPEG、PDF，暂不支持 GIF 格式。
 支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。
+支持的图片像素：需介于20-10000px之间。
 图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
 非腾讯云存储的 Url 速度和稳定性可能受一定影响。
         :type ImageUrl: str
         :param Types: 需要识别的票据类型列表，为空或不填表示识别全部类型。
 0：出租车发票
 1：定额发票
 2：火车票
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.898/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.897/setup.py` & `tencentcloud-sdk-python-ocr-3.0.898/setup.py`

 * *Files identical despite different names*

