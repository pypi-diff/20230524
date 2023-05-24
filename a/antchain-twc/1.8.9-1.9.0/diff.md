# Comparing `tmp/antchain_twc-1.8.9.tar.gz` & `tmp/antchain_twc-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_twc-1.8.9.tar", last modified: Fri Nov 25 06:09:07 2022, max compression
+gzip compressed data, was "dist/antchain_twc-1.9.0.tar", last modified: Wed May 24 03:05:49 2023, max compression
```

## Comparing `antchain_twc-1.8.9.tar` & `antchain_twc-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/
--rw-r--r--   0 root         (0) root         (0)      213 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2162 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_sdk_twc/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/antchain_sdk_twc/__init__.py
--rw-r--r--   0 root         (0) root         (0)   682400 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/antchain_sdk_twc/client.py
--rw-r--r--   0 root         (0) root         (0)  1823714 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/antchain_sdk_twc/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2162 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      336 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/antchain_twc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-25 06:09:07.000000 antchain_twc-1.8.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2022-11-25 06:09:05.000000 antchain_twc-1.8.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_sdk_twc/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/antchain_sdk_twc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   736938 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/antchain_sdk_twc/client.py
+-rw-r--r--   0 root         (0) root         (0)  1932157 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/antchain_sdk_twc/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/antchain_twc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 03:05:49.000000 antchain_twc-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-05-24 03:05:48.000000 antchain_twc-1.9.0/setup.py
```

### Comparing `antchain_twc-1.8.9/LICENSE` & `antchain_twc-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_twc-1.8.9/PKG-INFO` & `antchain_twc-1.9.0/antchain_twc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_twc
-Version: 1.8.9
+Name: antchain-twc
+Version: 1.9.0
 Summary: Ant Chain TWC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_twc-1.8.9/README-CN.md` & `antchain_twc-1.9.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_twc-1.8.9/README.md` & `antchain_twc-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_twc-1.8.9/antchain_sdk_twc/client.py` & `antchain_twc-1.9.0/antchain_sdk_twc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.9',
+                    'sdk_version': '1.9.0',
                     '_prod_code': 'TWC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'twc-openapi.antchain.antgroup.com'),
@@ -198,15 +198,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.9',
+                    'sdk_version': '1.9.0',
                     '_prod_code': 'TWC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'twc-openapi.antchain.antgroup.com'),
@@ -6159,14 +6159,462 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             twc_models.ExecContractPayResponse(),
             await self.do_request_async('1.0', 'twc.notary.contract.pay.exec', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def unbind_contract_pay(
+        self,
+        request: twc_models.UnbindContractPayRequest,
+    ) -> twc_models.UnbindContractPayResponse:
+        """
+        Description: 强制帮用户接触代扣协议，未执行成功的代扣会被取消，已执行成功的代扣不变。
+        Summary: 代扣强制解约
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.unbind_contract_pay_ex(request, headers, runtime)
+
+    async def unbind_contract_pay_async(
+        self,
+        request: twc_models.UnbindContractPayRequest,
+    ) -> twc_models.UnbindContractPayResponse:
+        """
+        Description: 强制帮用户接触代扣协议，未执行成功的代扣会被取消，已执行成功的代扣不变。
+        Summary: 代扣强制解约
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.unbind_contract_pay_ex_async(request, headers, runtime)
+
+    def unbind_contract_pay_ex(
+        self,
+        request: twc_models.UnbindContractPayRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UnbindContractPayResponse:
+        """
+        Description: 强制帮用户接触代扣协议，未执行成功的代扣会被取消，已执行成功的代扣不变。
+        Summary: 代扣强制解约
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UnbindContractPayResponse(),
+            self.do_request('1.0', 'twc.notary.contract.pay.unbind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def unbind_contract_pay_ex_async(
+        self,
+        request: twc_models.UnbindContractPayRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UnbindContractPayResponse:
+        """
+        Description: 强制帮用户接触代扣协议，未执行成功的代扣会被取消，已执行成功的代扣不变。
+        Summary: 代扣强制解约
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UnbindContractPayResponse(),
+            await self.do_request_async('1.0', 'twc.notary.contract.pay.unbind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_contract_complain(
+        self,
+        request: twc_models.QueryContractComplainRequest,
+    ) -> twc_models.QueryContractComplainResponse:
+        """
+        Description: 商户每次收到客户投诉回调通知，商户端均需要通过此接口来查询投诉数据。
+        Summary: 投诉数据查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_contract_complain_ex(request, headers, runtime)
+
+    async def query_contract_complain_async(
+        self,
+        request: twc_models.QueryContractComplainRequest,
+    ) -> twc_models.QueryContractComplainResponse:
+        """
+        Description: 商户每次收到客户投诉回调通知，商户端均需要通过此接口来查询投诉数据。
+        Summary: 投诉数据查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_contract_complain_ex_async(request, headers, runtime)
+
+    def query_contract_complain_ex(
+        self,
+        request: twc_models.QueryContractComplainRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.QueryContractComplainResponse:
+        """
+        Description: 商户每次收到客户投诉回调通知，商户端均需要通过此接口来查询投诉数据。
+        Summary: 投诉数据查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.QueryContractComplainResponse(),
+            self.do_request('1.0', 'twc.notary.contract.complain.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_contract_complain_ex_async(
+        self,
+        request: twc_models.QueryContractComplainRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.QueryContractComplainResponse:
+        """
+        Description: 商户每次收到客户投诉回调通知，商户端均需要通过此接口来查询投诉数据。
+        Summary: 投诉数据查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.QueryContractComplainResponse(),
+            await self.do_request_async('1.0', 'twc.notary.contract.complain.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def send_contract_complainfeedback(
+        self,
+        request: twc_models.SendContractComplainfeedbackRequest,
+    ) -> twc_models.SendContractComplainfeedbackResponse:
+        """
+        Description: 商家收到用户投诉后，可通过此接口进行投诉反馈。注意，只有当投诉单状态为MERCHANT_PROCESSING时，才允许商家进行投诉反馈。
+        Summary: 投诉反馈
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.send_contract_complainfeedback_ex(request, headers, runtime)
+
+    async def send_contract_complainfeedback_async(
+        self,
+        request: twc_models.SendContractComplainfeedbackRequest,
+    ) -> twc_models.SendContractComplainfeedbackResponse:
+        """
+        Description: 商家收到用户投诉后，可通过此接口进行投诉反馈。注意，只有当投诉单状态为MERCHANT_PROCESSING时，才允许商家进行投诉反馈。
+        Summary: 投诉反馈
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.send_contract_complainfeedback_ex_async(request, headers, runtime)
+
+    def send_contract_complainfeedback_ex(
+        self,
+        request: twc_models.SendContractComplainfeedbackRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.SendContractComplainfeedbackResponse:
+        """
+        Description: 商家收到用户投诉后，可通过此接口进行投诉反馈。注意，只有当投诉单状态为MERCHANT_PROCESSING时，才允许商家进行投诉反馈。
+        Summary: 投诉反馈
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.SendContractComplainfeedbackResponse(),
+            self.do_request('1.0', 'twc.notary.contract.complainfeedback.send', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def send_contract_complainfeedback_ex_async(
+        self,
+        request: twc_models.SendContractComplainfeedbackRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.SendContractComplainfeedbackResponse:
+        """
+        Description: 商家收到用户投诉后，可通过此接口进行投诉反馈。注意，只有当投诉单状态为MERCHANT_PROCESSING时，才允许商家进行投诉反馈。
+        Summary: 投诉反馈
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.SendContractComplainfeedbackResponse(),
+            await self.do_request_async('1.0', 'twc.notary.contract.complainfeedback.send', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def upload_contract_complainimage(
+        self,
+        request: twc_models.UploadContractComplainimageRequest,
+    ) -> twc_models.UploadContractComplainimageResponse:
+        """
+        Description: 商户上传处理图片
+        Summary: 商户上传处理图片
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_contract_complainimage_ex(request, headers, runtime)
+
+    async def upload_contract_complainimage_async(
+        self,
+        request: twc_models.UploadContractComplainimageRequest,
+    ) -> twc_models.UploadContractComplainimageResponse:
+        """
+        Description: 商户上传处理图片
+        Summary: 商户上传处理图片
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_contract_complainimage_ex_async(request, headers, runtime)
+
+    def upload_contract_complainimage_ex(
+        self,
+        request: twc_models.UploadContractComplainimageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UploadContractComplainimageResponse:
+        """
+        Description: 商户上传处理图片
+        Summary: 商户上传处理图片
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UploadContractComplainimageResponse(),
+            self.do_request('1.0', 'twc.notary.contract.complainimage.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_contract_complainimage_ex_async(
+        self,
+        request: twc_models.UploadContractComplainimageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UploadContractComplainimageResponse:
+        """
+        Description: 商户上传处理图片
+        Summary: 商户上传处理图片
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UploadContractComplainimageResponse(),
+            await self.do_request_async('1.0', 'twc.notary.contract.complainimage.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_contract_complaineventids(
+        self,
+        request: twc_models.QueryContractComplaineventidsRequest,
+    ) -> twc_models.QueryContractComplaineventidsResponse:
+        """
+        Description: 根据起止日期查询体验宝投诉工单
+        Summary: 根据起止日期查询体验宝投诉工单
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_contract_complaineventids_ex(request, headers, runtime)
+
+    async def query_contract_complaineventids_async(
+        self,
+        request: twc_models.QueryContractComplaineventidsRequest,
+    ) -> twc_models.QueryContractComplaineventidsResponse:
+        """
+        Description: 根据起止日期查询体验宝投诉工单
+        Summary: 根据起止日期查询体验宝投诉工单
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_contract_complaineventids_ex_async(request, headers, runtime)
+
+    def query_contract_complaineventids_ex(
+        self,
+        request: twc_models.QueryContractComplaineventidsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.QueryContractComplaineventidsResponse:
+        """
+        Description: 根据起止日期查询体验宝投诉工单
+        Summary: 根据起止日期查询体验宝投诉工单
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.QueryContractComplaineventidsResponse(),
+            self.do_request('1.0', 'twc.notary.contract.complaineventids.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_contract_complaineventids_ex_async(
+        self,
+        request: twc_models.QueryContractComplaineventidsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.QueryContractComplaineventidsResponse:
+        """
+        Description: 根据起止日期查询体验宝投诉工单
+        Summary: 根据起止日期查询体验宝投诉工单
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.QueryContractComplaineventidsResponse(),
+            await self.do_request_async('1.0', 'twc.notary.contract.complaineventids.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def push_digitalcontent_usage(
+        self,
+        request: twc_models.PushDigitalcontentUsageRequest,
+    ) -> twc_models.PushDigitalcontentUsageResponse:
+        """
+        Description: 用户使用mp4内容，集成方通过该openAPI进行使用上报。
+        Summary: 集成方通过该接口进行使用mp4上报
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.push_digitalcontent_usage_ex(request, headers, runtime)
+
+    async def push_digitalcontent_usage_async(
+        self,
+        request: twc_models.PushDigitalcontentUsageRequest,
+    ) -> twc_models.PushDigitalcontentUsageResponse:
+        """
+        Description: 用户使用mp4内容，集成方通过该openAPI进行使用上报。
+        Summary: 集成方通过该接口进行使用mp4上报
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.push_digitalcontent_usage_ex_async(request, headers, runtime)
+
+    def push_digitalcontent_usage_ex(
+        self,
+        request: twc_models.PushDigitalcontentUsageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.PushDigitalcontentUsageResponse:
+        """
+        Description: 用户使用mp4内容，集成方通过该openAPI进行使用上报。
+        Summary: 集成方通过该接口进行使用mp4上报
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.PushDigitalcontentUsageResponse(),
+            self.do_request('1.0', 'twc.notary.digitalcontent.usage.push', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def push_digitalcontent_usage_ex_async(
+        self,
+        request: twc_models.PushDigitalcontentUsageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.PushDigitalcontentUsageResponse:
+        """
+        Description: 用户使用mp4内容，集成方通过该openAPI进行使用上报。
+        Summary: 集成方通过该接口进行使用mp4上报
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.PushDigitalcontentUsageResponse(),
+            await self.do_request_async('1.0', 'twc.notary.digitalcontent.usage.push', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def apply_digitalcontent_order(
+        self,
+        request: twc_models.ApplyDigitalcontentOrderRequest,
+    ) -> twc_models.ApplyDigitalcontentOrderResponse:
+        """
+        Description: 用户使用apk内容，集成方通过该openAPI申请该使用的订单id。
+        Summary: 集成方通过该接口申请apk订单id
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.apply_digitalcontent_order_ex(request, headers, runtime)
+
+    async def apply_digitalcontent_order_async(
+        self,
+        request: twc_models.ApplyDigitalcontentOrderRequest,
+    ) -> twc_models.ApplyDigitalcontentOrderResponse:
+        """
+        Description: 用户使用apk内容，集成方通过该openAPI申请该使用的订单id。
+        Summary: 集成方通过该接口申请apk订单id
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.apply_digitalcontent_order_ex_async(request, headers, runtime)
+
+    def apply_digitalcontent_order_ex(
+        self,
+        request: twc_models.ApplyDigitalcontentOrderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.ApplyDigitalcontentOrderResponse:
+        """
+        Description: 用户使用apk内容，集成方通过该openAPI申请该使用的订单id。
+        Summary: 集成方通过该接口申请apk订单id
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.ApplyDigitalcontentOrderResponse(),
+            self.do_request('1.0', 'twc.notary.digitalcontent.order.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def apply_digitalcontent_order_ex_async(
+        self,
+        request: twc_models.ApplyDigitalcontentOrderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.ApplyDigitalcontentOrderResponse:
+        """
+        Description: 用户使用apk内容，集成方通过该openAPI申请该使用的订单id。
+        Summary: 集成方通过该接口申请apk订单id
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.ApplyDigitalcontentOrderResponse(),
+            await self.do_request_async('1.0', 'twc.notary.digitalcontent.order.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def submit_digitalcontent_order(
+        self,
+        request: twc_models.SubmitDigitalcontentOrderRequest,
+    ) -> twc_models.SubmitDigitalcontentOrderResponse:
+        """
+        Description: 用户使用apk内容支付后，集成方通过订单id和支付id反馈支付结果，并申请交互token。
+        Summary: 集成方反馈apk订单支付结果
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_digitalcontent_order_ex(request, headers, runtime)
+
+    async def submit_digitalcontent_order_async(
+        self,
+        request: twc_models.SubmitDigitalcontentOrderRequest,
+    ) -> twc_models.SubmitDigitalcontentOrderResponse:
+        """
+        Description: 用户使用apk内容支付后，集成方通过订单id和支付id反馈支付结果，并申请交互token。
+        Summary: 集成方反馈apk订单支付结果
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_digitalcontent_order_ex_async(request, headers, runtime)
+
+    def submit_digitalcontent_order_ex(
+        self,
+        request: twc_models.SubmitDigitalcontentOrderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.SubmitDigitalcontentOrderResponse:
+        """
+        Description: 用户使用apk内容支付后，集成方通过订单id和支付id反馈支付结果，并申请交互token。
+        Summary: 集成方反馈apk订单支付结果
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.SubmitDigitalcontentOrderResponse(),
+            self.do_request('1.0', 'twc.notary.digitalcontent.order.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_digitalcontent_order_ex_async(
+        self,
+        request: twc_models.SubmitDigitalcontentOrderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.SubmitDigitalcontentOrderResponse:
+        """
+        Description: 用户使用apk内容支付后，集成方通过订单id和支付id反馈支付结果，并申请交互token。
+        Summary: 集成方反馈apk订单支付结果
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.SubmitDigitalcontentOrderResponse(),
+            await self.do_request_async('1.0', 'twc.notary.digitalcontent.order.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def sync_inner_trans(
         self,
         request: twc_models.SyncInnerTransRequest,
     ) -> twc_models.SyncInnerTransResponse:
         """
         Description: baas-notary向notarycore同步生成的事务数据，仅做数据同步使用
         Summary: 向notarycore同步事务数据
@@ -8735,14 +9183,238 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             twc_models.QueryJusticeCommoncaseinfoResponse(),
             await self.do_request_async('1.0', 'twc.notary.justice.commoncaseinfo.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def create_justice_agentcase(
+        self,
+        request: twc_models.CreateJusticeAgentcaseRequest,
+    ) -> twc_models.CreateJusticeAgentcaseResponse:
+        """
+        Description: 1级商户为2级商户进件
+        Summary: 代理二级商户进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_justice_agentcase_ex(request, headers, runtime)
+
+    async def create_justice_agentcase_async(
+        self,
+        request: twc_models.CreateJusticeAgentcaseRequest,
+    ) -> twc_models.CreateJusticeAgentcaseResponse:
+        """
+        Description: 1级商户为2级商户进件
+        Summary: 代理二级商户进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_justice_agentcase_ex_async(request, headers, runtime)
+
+    def create_justice_agentcase_ex(
+        self,
+        request: twc_models.CreateJusticeAgentcaseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateJusticeAgentcaseResponse:
+        """
+        Description: 1级商户为2级商户进件
+        Summary: 代理二级商户进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateJusticeAgentcaseResponse(),
+            self.do_request('1.0', 'twc.notary.justice.agentcase.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_justice_agentcase_ex_async(
+        self,
+        request: twc_models.CreateJusticeAgentcaseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateJusticeAgentcaseResponse:
+        """
+        Description: 1级商户为2级商户进件
+        Summary: 代理二级商户进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateJusticeAgentcaseResponse(),
+            await self.do_request_async('1.0', 'twc.notary.justice.agentcase.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_justice_rights(
+        self,
+        request: twc_models.QueryJusticeRightsRequest,
+    ) -> twc_models.QueryJusticeRightsResponse:
+        """
+        Description: isv机构-案件要素查询
+        Summary: isv机构-案件要素查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_justice_rights_ex(request, headers, runtime)
+
+    async def query_justice_rights_async(
+        self,
+        request: twc_models.QueryJusticeRightsRequest,
+    ) -> twc_models.QueryJusticeRightsResponse:
+        """
+        Description: isv机构-案件要素查询
+        Summary: isv机构-案件要素查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_justice_rights_ex_async(request, headers, runtime)
+
+    def query_justice_rights_ex(
+        self,
+        request: twc_models.QueryJusticeRightsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.QueryJusticeRightsResponse:
+        """
+        Description: isv机构-案件要素查询
+        Summary: isv机构-案件要素查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.QueryJusticeRightsResponse(),
+            self.do_request('1.0', 'twc.notary.justice.rights.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_justice_rights_ex_async(
+        self,
+        request: twc_models.QueryJusticeRightsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.QueryJusticeRightsResponse:
+        """
+        Description: isv机构-案件要素查询
+        Summary: isv机构-案件要素查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.QueryJusticeRightsResponse(),
+            await self.do_request_async('1.0', 'twc.notary.justice.rights.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def update_justice_rights(
+        self,
+        request: twc_models.UpdateJusticeRightsRequest,
+    ) -> twc_models.UpdateJusticeRightsResponse:
+        """
+        Description: isv机构-维权状态更新
+        Summary: isv机构-维权状态更新
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_justice_rights_ex(request, headers, runtime)
+
+    async def update_justice_rights_async(
+        self,
+        request: twc_models.UpdateJusticeRightsRequest,
+    ) -> twc_models.UpdateJusticeRightsResponse:
+        """
+        Description: isv机构-维权状态更新
+        Summary: isv机构-维权状态更新
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_justice_rights_ex_async(request, headers, runtime)
+
+    def update_justice_rights_ex(
+        self,
+        request: twc_models.UpdateJusticeRightsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UpdateJusticeRightsResponse:
+        """
+        Description: isv机构-维权状态更新
+        Summary: isv机构-维权状态更新
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UpdateJusticeRightsResponse(),
+            self.do_request('1.0', 'twc.notary.justice.rights.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def update_justice_rights_ex_async(
+        self,
+        request: twc_models.UpdateJusticeRightsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UpdateJusticeRightsResponse:
+        """
+        Description: isv机构-维权状态更新
+        Summary: isv机构-维权状态更新
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UpdateJusticeRightsResponse(),
+            await self.do_request_async('1.0', 'twc.notary.justice.rights.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def notify_justice_rightspayment(
+        self,
+        request: twc_models.NotifyJusticeRightspaymentRequest,
+    ) -> twc_models.NotifyJusticeRightspaymentResponse:
+        """
+        Description: isv机构-案件缴费通知接口
+        Summary: isv机构-案件缴费通知接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.notify_justice_rightspayment_ex(request, headers, runtime)
+
+    async def notify_justice_rightspayment_async(
+        self,
+        request: twc_models.NotifyJusticeRightspaymentRequest,
+    ) -> twc_models.NotifyJusticeRightspaymentResponse:
+        """
+        Description: isv机构-案件缴费通知接口
+        Summary: isv机构-案件缴费通知接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.notify_justice_rightspayment_ex_async(request, headers, runtime)
+
+    def notify_justice_rightspayment_ex(
+        self,
+        request: twc_models.NotifyJusticeRightspaymentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.NotifyJusticeRightspaymentResponse:
+        """
+        Description: isv机构-案件缴费通知接口
+        Summary: isv机构-案件缴费通知接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.NotifyJusticeRightspaymentResponse(),
+            self.do_request('1.0', 'twc.notary.justice.rightspayment.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def notify_justice_rightspayment_ex_async(
+        self,
+        request: twc_models.NotifyJusticeRightspaymentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.NotifyJusticeRightspaymentResponse:
+        """
+        Description: isv机构-案件缴费通知接口
+        Summary: isv机构-案件缴费通知接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.NotifyJusticeRightspaymentResponse(),
+            await self.do_request_async('1.0', 'twc.notary.justice.rightspayment.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_lease_productinfo(
         self,
         request: twc_models.CreateLeaseProductinfoRequest,
     ) -> twc_models.CreateLeaseProductinfoResponse:
         """
         Description: 融资服务平台上传商品类别信息
         Summary: 融资服务平台上传商品类别信息
@@ -15287,14 +15959,518 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             twc_models.GetInternalFileResponse(),
             await self.do_request_async('1.0', 'twc.notary.internal.file.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def create_dataflow_text(
+        self,
+        request: twc_models.CreateDataflowTextRequest,
+    ) -> twc_models.CreateDataflowTextResponse:
+        """
+        Description: 数据流转文本存证
+        Summary: 数据流转文本存证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_dataflow_text_ex(request, headers, runtime)
+
+    async def create_dataflow_text_async(
+        self,
+        request: twc_models.CreateDataflowTextRequest,
+    ) -> twc_models.CreateDataflowTextResponse:
+        """
+        Description: 数据流转文本存证
+        Summary: 数据流转文本存证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_dataflow_text_ex_async(request, headers, runtime)
+
+    def create_dataflow_text_ex(
+        self,
+        request: twc_models.CreateDataflowTextRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateDataflowTextResponse:
+        """
+        Description: 数据流转文本存证
+        Summary: 数据流转文本存证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateDataflowTextResponse(),
+            self.do_request('1.0', 'twc.notary.dataflow.text.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_dataflow_text_ex_async(
+        self,
+        request: twc_models.CreateDataflowTextRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateDataflowTextResponse:
+        """
+        Description: 数据流转文本存证
+        Summary: 数据流转文本存证
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateDataflowTextResponse(),
+            await self.do_request_async('1.0', 'twc.notary.dataflow.text.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_dataflow_text(
+        self,
+        request: twc_models.GetDataflowTextRequest,
+    ) -> twc_models.GetDataflowTextResponse:
+        """
+        Description: 查询数据流转文本存证内容
+        Summary: 查询数据流转文本存证内容
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_dataflow_text_ex(request, headers, runtime)
+
+    async def get_dataflow_text_async(
+        self,
+        request: twc_models.GetDataflowTextRequest,
+    ) -> twc_models.GetDataflowTextResponse:
+        """
+        Description: 查询数据流转文本存证内容
+        Summary: 查询数据流转文本存证内容
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_dataflow_text_ex_async(request, headers, runtime)
+
+    def get_dataflow_text_ex(
+        self,
+        request: twc_models.GetDataflowTextRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.GetDataflowTextResponse:
+        """
+        Description: 查询数据流转文本存证内容
+        Summary: 查询数据流转文本存证内容
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.GetDataflowTextResponse(),
+            self.do_request('1.0', 'twc.notary.dataflow.text.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_dataflow_text_ex_async(
+        self,
+        request: twc_models.GetDataflowTextRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.GetDataflowTextResponse:
+        """
+        Description: 查询数据流转文本存证内容
+        Summary: 查询数据流转文本存证内容
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.GetDataflowTextResponse(),
+            await self.do_request_async('1.0', 'twc.notary.dataflow.text.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_dataflow_trans(
+        self,
+        request: twc_models.CreateDataflowTransRequest,
+    ) -> twc_models.CreateDataflowTransResponse:
+        """
+        Description: 数据流转存证创建存证事务
+        Summary: 数据流转存证创建存证事务
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_dataflow_trans_ex(request, headers, runtime)
+
+    async def create_dataflow_trans_async(
+        self,
+        request: twc_models.CreateDataflowTransRequest,
+    ) -> twc_models.CreateDataflowTransResponse:
+        """
+        Description: 数据流转存证创建存证事务
+        Summary: 数据流转存证创建存证事务
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_dataflow_trans_ex_async(request, headers, runtime)
+
+    def create_dataflow_trans_ex(
+        self,
+        request: twc_models.CreateDataflowTransRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateDataflowTransResponse:
+        """
+        Description: 数据流转存证创建存证事务
+        Summary: 数据流转存证创建存证事务
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateDataflowTransResponse(),
+            self.do_request('1.0', 'twc.notary.dataflow.trans.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_dataflow_trans_ex_async(
+        self,
+        request: twc_models.CreateDataflowTransRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateDataflowTransResponse:
+        """
+        Description: 数据流转存证创建存证事务
+        Summary: 数据流转存证创建存证事务
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateDataflowTransResponse(),
+            await self.do_request_async('1.0', 'twc.notary.dataflow.trans.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def deploy_dataflow_contract(
+        self,
+        request: twc_models.DeployDataflowContractRequest,
+    ) -> twc_models.DeployDataflowContractResponse:
+        """
+        Description: 数据流转存证需要通过存证合约进行授权和流转的管理，存证方可以通过本接口发起管理合约的部署。
+        Summary: 发起管理合约部署
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.deploy_dataflow_contract_ex(request, headers, runtime)
+
+    async def deploy_dataflow_contract_async(
+        self,
+        request: twc_models.DeployDataflowContractRequest,
+    ) -> twc_models.DeployDataflowContractResponse:
+        """
+        Description: 数据流转存证需要通过存证合约进行授权和流转的管理，存证方可以通过本接口发起管理合约的部署。
+        Summary: 发起管理合约部署
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.deploy_dataflow_contract_ex_async(request, headers, runtime)
+
+    def deploy_dataflow_contract_ex(
+        self,
+        request: twc_models.DeployDataflowContractRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.DeployDataflowContractResponse:
+        """
+        Description: 数据流转存证需要通过存证合约进行授权和流转的管理，存证方可以通过本接口发起管理合约的部署。
+        Summary: 发起管理合约部署
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.DeployDataflowContractResponse(),
+            self.do_request('1.0', 'twc.notary.dataflow.contract.deploy', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def deploy_dataflow_contract_ex_async(
+        self,
+        request: twc_models.DeployDataflowContractRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.DeployDataflowContractResponse:
+        """
+        Description: 数据流转存证需要通过存证合约进行授权和流转的管理，存证方可以通过本接口发起管理合约的部署。
+        Summary: 发起管理合约部署
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.DeployDataflowContractResponse(),
+            await self.do_request_async('1.0', 'twc.notary.dataflow.contract.deploy', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_dataflow_authorize(
+        self,
+        request: twc_models.CreateDataflowAuthorizeRequest,
+    ) -> twc_models.CreateDataflowAuthorizeResponse:
+        """
+        Description: 存证方对证据的使用方进行各类型的权限授予，允许使用方调用存证合约中的对应方法。
+        Summary: 发起授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_dataflow_authorize_ex(request, headers, runtime)
+
+    async def create_dataflow_authorize_async(
+        self,
+        request: twc_models.CreateDataflowAuthorizeRequest,
+    ) -> twc_models.CreateDataflowAuthorizeResponse:
+        """
+        Description: 存证方对证据的使用方进行各类型的权限授予，允许使用方调用存证合约中的对应方法。
+        Summary: 发起授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_dataflow_authorize_ex_async(request, headers, runtime)
+
+    def create_dataflow_authorize_ex(
+        self,
+        request: twc_models.CreateDataflowAuthorizeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateDataflowAuthorizeResponse:
+        """
+        Description: 存证方对证据的使用方进行各类型的权限授予，允许使用方调用存证合约中的对应方法。
+        Summary: 发起授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateDataflowAuthorizeResponse(),
+            self.do_request('1.0', 'twc.notary.dataflow.authorize.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_dataflow_authorize_ex_async(
+        self,
+        request: twc_models.CreateDataflowAuthorizeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateDataflowAuthorizeResponse:
+        """
+        Description: 存证方对证据的使用方进行各类型的权限授予，允许使用方调用存证合约中的对应方法。
+        Summary: 发起授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateDataflowAuthorizeResponse(),
+            await self.do_request_async('1.0', 'twc.notary.dataflow.authorize.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def cancel_dataflow_authorize(
+        self,
+        request: twc_models.CancelDataflowAuthorizeRequest,
+    ) -> twc_models.CancelDataflowAuthorizeResponse:
+        """
+        Description: 存证方对撤销已经发起的权限授予。
+        Summary: 撤销授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.cancel_dataflow_authorize_ex(request, headers, runtime)
+
+    async def cancel_dataflow_authorize_async(
+        self,
+        request: twc_models.CancelDataflowAuthorizeRequest,
+    ) -> twc_models.CancelDataflowAuthorizeResponse:
+        """
+        Description: 存证方对撤销已经发起的权限授予。
+        Summary: 撤销授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.cancel_dataflow_authorize_ex_async(request, headers, runtime)
+
+    def cancel_dataflow_authorize_ex(
+        self,
+        request: twc_models.CancelDataflowAuthorizeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CancelDataflowAuthorizeResponse:
+        """
+        Description: 存证方对撤销已经发起的权限授予。
+        Summary: 撤销授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CancelDataflowAuthorizeResponse(),
+            self.do_request('1.0', 'twc.notary.dataflow.authorize.cancel', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def cancel_dataflow_authorize_ex_async(
+        self,
+        request: twc_models.CancelDataflowAuthorizeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CancelDataflowAuthorizeResponse:
+        """
+        Description: 存证方对撤销已经发起的权限授予。
+        Summary: 撤销授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CancelDataflowAuthorizeResponse(),
+            await self.do_request_async('1.0', 'twc.notary.dataflow.authorize.cancel', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_dataflow_action(
+        self,
+        request: twc_models.QueryDataflowActionRequest,
+    ) -> twc_models.QueryDataflowActionResponse:
+        """
+        Description: 查询存证管理合约的部署/授权/撤销授权/密钥上传等操作的执行结果。
+        Summary: 查询对存证合约的各类操作执行结果
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_dataflow_action_ex(request, headers, runtime)
+
+    async def query_dataflow_action_async(
+        self,
+        request: twc_models.QueryDataflowActionRequest,
+    ) -> twc_models.QueryDataflowActionResponse:
+        """
+        Description: 查询存证管理合约的部署/授权/撤销授权/密钥上传等操作的执行结果。
+        Summary: 查询对存证合约的各类操作执行结果
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_dataflow_action_ex_async(request, headers, runtime)
+
+    def query_dataflow_action_ex(
+        self,
+        request: twc_models.QueryDataflowActionRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.QueryDataflowActionResponse:
+        """
+        Description: 查询存证管理合约的部署/授权/撤销授权/密钥上传等操作的执行结果。
+        Summary: 查询对存证合约的各类操作执行结果
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.QueryDataflowActionResponse(),
+            self.do_request('1.0', 'twc.notary.dataflow.action.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_dataflow_action_ex_async(
+        self,
+        request: twc_models.QueryDataflowActionRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.QueryDataflowActionResponse:
+        """
+        Description: 查询存证管理合约的部署/授权/撤销授权/密钥上传等操作的执行结果。
+        Summary: 查询对存证合约的各类操作执行结果
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.QueryDataflowActionResponse(),
+            await self.do_request_async('1.0', 'twc.notary.dataflow.action.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def upload_dataflow_pubkey(
+        self,
+        request: twc_models.UploadDataflowPubkeyRequest,
+    ) -> twc_models.UploadDataflowPubkeyResponse:
+        """
+        Description: 存证的使用方，在获得密钥上传（PUBKEY_UPLOAD）授权后，使用本接口上传信封密钥，后续查询存证时，会使用此信封密钥对存证原文加密，将密文返回，保障数据安全。
+        Summary: 发起信封密钥上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_dataflow_pubkey_ex(request, headers, runtime)
+
+    async def upload_dataflow_pubkey_async(
+        self,
+        request: twc_models.UploadDataflowPubkeyRequest,
+    ) -> twc_models.UploadDataflowPubkeyResponse:
+        """
+        Description: 存证的使用方，在获得密钥上传（PUBKEY_UPLOAD）授权后，使用本接口上传信封密钥，后续查询存证时，会使用此信封密钥对存证原文加密，将密文返回，保障数据安全。
+        Summary: 发起信封密钥上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_dataflow_pubkey_ex_async(request, headers, runtime)
+
+    def upload_dataflow_pubkey_ex(
+        self,
+        request: twc_models.UploadDataflowPubkeyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UploadDataflowPubkeyResponse:
+        """
+        Description: 存证的使用方，在获得密钥上传（PUBKEY_UPLOAD）授权后，使用本接口上传信封密钥，后续查询存证时，会使用此信封密钥对存证原文加密，将密文返回，保障数据安全。
+        Summary: 发起信封密钥上传
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UploadDataflowPubkeyResponse(),
+            self.do_request('1.0', 'twc.notary.dataflow.pubkey.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_dataflow_pubkey_ex_async(
+        self,
+        request: twc_models.UploadDataflowPubkeyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UploadDataflowPubkeyResponse:
+        """
+        Description: 存证的使用方，在获得密钥上传（PUBKEY_UPLOAD）授权后，使用本接口上传信封密钥，后续查询存证时，会使用此信封密钥对存证原文加密，将密文返回，保障数据安全。
+        Summary: 发起信封密钥上传
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UploadDataflowPubkeyResponse(),
+            await self.do_request_async('1.0', 'twc.notary.dataflow.pubkey.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_dataflow_account(
+        self,
+        request: twc_models.CreateDataflowAccountRequest,
+    ) -> twc_models.CreateDataflowAccountResponse:
+        """
+        Description: 数据流转存证创建链上账户
+        Summary: 数据流转存证创建链上账户
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_dataflow_account_ex(request, headers, runtime)
+
+    async def create_dataflow_account_async(
+        self,
+        request: twc_models.CreateDataflowAccountRequest,
+    ) -> twc_models.CreateDataflowAccountResponse:
+        """
+        Description: 数据流转存证创建链上账户
+        Summary: 数据流转存证创建链上账户
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_dataflow_account_ex_async(request, headers, runtime)
+
+    def create_dataflow_account_ex(
+        self,
+        request: twc_models.CreateDataflowAccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateDataflowAccountResponse:
+        """
+        Description: 数据流转存证创建链上账户
+        Summary: 数据流转存证创建链上账户
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateDataflowAccountResponse(),
+            self.do_request('1.0', 'twc.notary.dataflow.account.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_dataflow_account_ex_async(
+        self,
+        request: twc_models.CreateDataflowAccountRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateDataflowAccountResponse:
+        """
+        Description: 数据流转存证创建链上账户
+        Summary: 数据流转存证创建链上账户
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateDataflowAccountResponse(),
+            await self.do_request_async('1.0', 'twc.notary.dataflow.account.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_flow_instance(
         self,
         request: twc_models.CreateFlowInstanceRequest,
     ) -> twc_models.CreateFlowInstanceResponse:
         """
         Description: 创建存证流程实例
         Summary: 创建存证流程实例
@@ -16462,7 +17638,119 @@
         Summary: 查询合约核验结果
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             twc_models.QueryContractStatusResponse(),
             await self.do_request_async('1.0', 'twc.notary.contract.status.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def create_traffic_traceid(
+        self,
+        request: twc_models.CreateTrafficTraceidRequest,
+    ) -> twc_models.CreateTrafficTraceidResponse:
+        """
+        Description: 根据业务场景码创建raceId
+        Summary: traceId创建接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_traffic_traceid_ex(request, headers, runtime)
+
+    async def create_traffic_traceid_async(
+        self,
+        request: twc_models.CreateTrafficTraceidRequest,
+    ) -> twc_models.CreateTrafficTraceidResponse:
+        """
+        Description: 根据业务场景码创建raceId
+        Summary: traceId创建接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_traffic_traceid_ex_async(request, headers, runtime)
+
+    def create_traffic_traceid_ex(
+        self,
+        request: twc_models.CreateTrafficTraceidRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateTrafficTraceidResponse:
+        """
+        Description: 根据业务场景码创建raceId
+        Summary: traceId创建接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateTrafficTraceidResponse(),
+            self.do_request('1.0', 'twc.notary.traffic.traceid.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_traffic_traceid_ex_async(
+        self,
+        request: twc_models.CreateTrafficTraceidRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.CreateTrafficTraceidResponse:
+        """
+        Description: 根据业务场景码创建raceId
+        Summary: traceId创建接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.CreateTrafficTraceidResponse(),
+            await self.do_request_async('1.0', 'twc.notary.traffic.traceid.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def upload_traffic_operatelog(
+        self,
+        request: twc_models.UploadTrafficOperatelogRequest,
+    ) -> twc_models.UploadTrafficOperatelogResponse:
+        """
+        Description: 业务方操作行为日志传入
+        Summary: 操作行为日志传入
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_traffic_operatelog_ex(request, headers, runtime)
+
+    async def upload_traffic_operatelog_async(
+        self,
+        request: twc_models.UploadTrafficOperatelogRequest,
+    ) -> twc_models.UploadTrafficOperatelogResponse:
+        """
+        Description: 业务方操作行为日志传入
+        Summary: 操作行为日志传入
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_traffic_operatelog_ex_async(request, headers, runtime)
+
+    def upload_traffic_operatelog_ex(
+        self,
+        request: twc_models.UploadTrafficOperatelogRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UploadTrafficOperatelogResponse:
+        """
+        Description: 业务方操作行为日志传入
+        Summary: 操作行为日志传入
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UploadTrafficOperatelogResponse(),
+            self.do_request('1.0', 'twc.notary.traffic.operatelog.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_traffic_operatelog_ex_async(
+        self,
+        request: twc_models.UploadTrafficOperatelogRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> twc_models.UploadTrafficOperatelogResponse:
+        """
+        Description: 业务方操作行为日志传入
+        Summary: 操作行为日志传入
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            twc_models.UploadTrafficOperatelogResponse(),
+            await self.do_request_async('1.0', 'twc.notary.traffic.operatelog.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_twc-1.8.9/antchain_sdk_twc/models.py` & `antchain_twc-1.9.0/antchain_sdk_twc/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,19 +204,27 @@
 
 
 class FileInfo(TeaModel):
     def __init__(
         self,
         file_key: str = None,
         file_name: str = None,
+        file_type: str = None,
     ):
         # 文件key
         self.file_key = file_key
         # 文件名称
         self.file_name = file_name
+        # 文件类型(枚举)
+        # CASE_NOTICE: 立案通知书
+        # CASE_VERDICT: 仲裁裁决书
+        # CASE_EFFECT_PROVE: 裁决书司法生效证明
+        # CASE_SERVED_NOTICE: 电子送达通知
+        # PAYMETN_INFO: 缴费相关文件
+        self.file_type = file_type
 
     def validate(self):
         self.validate_required(self.file_key, 'file_key')
         self.validate_required(self.file_name, 'file_name')
 
     def to_map(self):
         _map = super().to_map()
@@ -224,22 +232,26 @@
             return _map
 
         result = dict()
         if self.file_key is not None:
             result['file_key'] = self.file_key
         if self.file_name is not None:
             result['file_name'] = self.file_name
+        if self.file_type is not None:
+            result['file_type'] = self.file_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('file_key') is not None:
             self.file_key = m.get('file_key')
         if m.get('file_name') is not None:
             self.file_name = m.get('file_name')
+        if m.get('file_type') is not None:
+            self.file_type = m.get('file_type')
         return self
 
 
 class RentalInstallmentPerformance(TeaModel):
     def __init__(
         self,
         repayment_period: int = None,
@@ -1021,15 +1033,14 @@
         self.job_certification = job_certification
         # 性别， 0-男，1-女
         self.sex = sex
         # 联系邮件地址
         self.email = email
 
     def validate(self):
-        self.validate_required(self.name, 'name')
         if self.identity_certification:
             self.identity_certification.validate()
         if self.job_certification:
             self.job_certification.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -4112,27 +4123,30 @@
         self,
         rec_bank_area_code: str = None,
         account_no: str = None,
         bank_name: str = None,
         account_name: str = None,
         cnaps: str = None,
         identify_no: str = None,
+        bank_code: str = None,
     ):
         # 银行区域代码，可网上查询各银行最新对应的区域代码，比如杭州的区域代码为：3301
         self.rec_bank_area_code = rec_bank_area_code
         # 投保人收款账号
         self.account_no = account_no
         # 完整银行名称，不需要具体到分行
         self.bank_name = bank_name
         # 投保人户名
         self.account_name = account_name
         # 联行号
         self.cnaps = cnaps
         # 统一社会信用代码
         self.identify_no = identify_no
+        # 银行代码
+        self.bank_code = bank_code
 
     def validate(self):
         self.validate_required(self.rec_bank_area_code, 'rec_bank_area_code')
         if self.rec_bank_area_code is not None:
             self.validate_max_length(self.rec_bank_area_code, 'rec_bank_area_code', 8)
         self.validate_required(self.account_no, 'account_no')
         if self.account_no is not None:
@@ -4145,14 +4159,17 @@
             self.validate_max_length(self.account_name, 'account_name', 64)
         self.validate_required(self.cnaps, 'cnaps')
         if self.cnaps is not None:
             self.validate_max_length(self.cnaps, 'cnaps', 16)
         self.validate_required(self.identify_no, 'identify_no')
         if self.identify_no is not None:
             self.validate_max_length(self.identify_no, 'identify_no', 32)
+        self.validate_required(self.bank_code, 'bank_code')
+        if self.bank_code is not None:
+            self.validate_max_length(self.bank_code, 'bank_code', 16)
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -4164,14 +4181,16 @@
             result['bank_name'] = self.bank_name
         if self.account_name is not None:
             result['account_name'] = self.account_name
         if self.cnaps is not None:
             result['cnaps'] = self.cnaps
         if self.identify_no is not None:
             result['identify_no'] = self.identify_no
+        if self.bank_code is not None:
+            result['bank_code'] = self.bank_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('rec_bank_area_code') is not None:
             self.rec_bank_area_code = m.get('rec_bank_area_code')
         if m.get('account_no') is not None:
@@ -4180,14 +4199,16 @@
             self.bank_name = m.get('bank_name')
         if m.get('account_name') is not None:
             self.account_name = m.get('account_name')
         if m.get('cnaps') is not None:
             self.cnaps = m.get('cnaps')
         if m.get('identify_no') is not None:
             self.identify_no = m.get('identify_no')
+        if m.get('bank_code') is not None:
+            self.bank_code = m.get('bank_code')
         return self
 
 
 class JudicialEventOperateInfo(TeaModel):
     def __init__(
         self,
         operate_type: str = None,
@@ -7395,14 +7416,58 @@
         if m.get('width') is not None:
             self.width = m.get('width')
         if m.get('auto_execute') is not None:
             self.auto_execute = m.get('auto_execute')
         return self
 
 
+class PaymentInfo(TeaModel):
+    def __init__(
+        self,
+        account_name: str = None,
+        bank_name: str = None,
+        bank_num: str = None,
+    ):
+        # 收款账户-户名 不超过64字符
+        self.account_name = account_name
+        # 收款账户-开户银行 不超过64字符
+        self.bank_name = bank_name
+        # 收款账户-收款账户银行账号 不超过64字符
+        self.bank_num = bank_num
+
+    def validate(self):
+        self.validate_required(self.account_name, 'account_name')
+        self.validate_required(self.bank_name, 'bank_name')
+        self.validate_required(self.bank_num, 'bank_num')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_name is not None:
+            result['account_name'] = self.account_name
+        if self.bank_name is not None:
+            result['bank_name'] = self.bank_name
+        if self.bank_num is not None:
+            result['bank_num'] = self.bank_num
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('account_name') is not None:
+            self.account_name = m.get('account_name')
+        if m.get('bank_name') is not None:
+            self.bank_name = m.get('bank_name')
+        if m.get('bank_num') is not None:
+            self.bank_num = m.get('bank_num')
+        return self
+
+
 class ContractNotaryInitInfo(TeaModel):
     def __init__(
         self,
         content: str = None,
         file_num: int = None,
         initiator: str = None,
         signatories: str = None,
@@ -7847,14 +7912,79 @@
         if m.get('seal_type') is not None:
             self.seal_type = m.get('seal_type')
         if m.get('signfield_id') is not None:
             self.signfield_id = m.get('signfield_id')
         return self
 
 
+class ReplayDetailInfo(TeaModel):
+    def __init__(
+        self,
+        replier_name: str = None,
+        replier_role: str = None,
+        gmt_create: str = None,
+        content: str = None,
+        images: List[str] = None,
+    ):
+        # 回复人名称
+        self.replier_name = replier_name
+        # 回复人角色
+        # 用户：USER
+        # 商家：MERCHANT
+        # 系统：SYSTEM
+        # 审核小二：AUDITOR
+        # 政府单位：GOVERNMENT
+        self.replier_role = replier_role
+        # 回复时间
+        self.gmt_create = gmt_create
+        # 回复内容
+        self.content = content
+        # 回复图片
+        self.images = images
+
+    def validate(self):
+        self.validate_required(self.replier_name, 'replier_name')
+        self.validate_required(self.replier_role, 'replier_role')
+        self.validate_required(self.gmt_create, 'gmt_create')
+        self.validate_required(self.content, 'content')
+        self.validate_required(self.images, 'images')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.replier_name is not None:
+            result['replier_name'] = self.replier_name
+        if self.replier_role is not None:
+            result['replier_role'] = self.replier_role
+        if self.gmt_create is not None:
+            result['gmt_create'] = self.gmt_create
+        if self.content is not None:
+            result['content'] = self.content
+        if self.images is not None:
+            result['images'] = self.images
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('replier_name') is not None:
+            self.replier_name = m.get('replier_name')
+        if m.get('replier_role') is not None:
+            self.replier_role = m.get('replier_role')
+        if m.get('gmt_create') is not None:
+            self.gmt_create = m.get('gmt_create')
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('images') is not None:
+            self.images = m.get('images')
+        return self
+
+
 class ContractTemplateStructComponent(TeaModel):
     def __init__(
         self,
         font: int = None,
         font_size: str = None,
         height: str = None,
         id: str = None,
@@ -19253,14 +19383,15 @@
         result_code: str = None,
         result_msg: str = None,
         out_trade_no: str = None,
         deduct_time: str = None,
         pay_date: str = None,
         pay_money: int = None,
         status: str = None,
+        pay_index: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -19280,14 +19411,16 @@
         # TRADE_REFUNDED 已发生退款
         # TRADE_CLOSED 交易终止（未成功）
         # TRADE_SUCCESS 扣款成功
         # PAY_FAIL 扣款失败
         # TRADE_FINISHED 交易终止（扣款成功）
         # TRADE_CANCEL 代扣取消
         self.status = status
+        # 唯一订单号
+        self.pay_index = pay_index
 
     def validate(self):
         if self.deduct_time is not None:
             self.validate_pattern(self.deduct_time, 'deduct_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
         if self.pay_date is not None:
             self.validate_pattern(self.pay_date, 'pay_date', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
 
@@ -19309,14 +19442,16 @@
             result['deduct_time'] = self.deduct_time
         if self.pay_date is not None:
             result['pay_date'] = self.pay_date
         if self.pay_money is not None:
             result['pay_money'] = self.pay_money
         if self.status is not None:
             result['status'] = self.status
+        if self.pay_index is not None:
+            result['pay_index'] = self.pay_index
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -19329,29 +19464,34 @@
             self.deduct_time = m.get('deduct_time')
         if m.get('pay_date') is not None:
             self.pay_date = m.get('pay_date')
         if m.get('pay_money') is not None:
             self.pay_money = m.get('pay_money')
         if m.get('status') is not None:
             self.status = m.get('status')
+        if m.get('pay_index') is not None:
+            self.pay_index = m.get('pay_index')
         return self
 
 
 class QueryContractRefundRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         refund_id: str = None,
+        flow_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 退款ID，用户调用退款接口时传入的自定义第三方id
         self.refund_id = refund_id
+        # 合同流程id
+        self.flow_id = flow_id
 
     def validate(self):
         self.validate_required(self.refund_id, 'refund_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -19360,24 +19500,28 @@
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.refund_id is not None:
             result['refund_id'] = self.refund_id
+        if self.flow_id is not None:
+            result['flow_id'] = self.flow_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('refund_id') is not None:
             self.refund_id = m.get('refund_id')
+        if m.get('flow_id') is not None:
+            self.flow_id = m.get('flow_id')
         return self
 
 
 class QueryContractRefundResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -21566,15 +21710,14 @@
         self.user = user
         # 用户类型
         # 个人：PERSON；
         # 机构：ORGANIZATION
         self.user_type = user_type
 
     def validate(self):
-        self.validate_required(self.organization, 'organization')
         if self.organization:
             self.organization.validate()
         self.validate_required(self.user, 'user')
         if self.user:
             self.user.validate()
         self.validate_required(self.user_type, 'user_type')
 
@@ -22230,14 +22373,1016 @@
         if m.get('code') is not None:
             self.code = m.get('code')
         if m.get('msg') is not None:
             self.msg = m.get('msg')
         return self
 
 
+class UnbindContractPayRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        user_tuid: str = None,
+        external_agreement_no: str = None,
+        allow_unsign: bool = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 用户id，平台方用户创建时生成的id。用户解约失败时该字段会通过解约申请消息透传给商家。
+        self.user_tuid = user_tuid
+        # 外部代扣协议号，用户解约失败时该字段会通过解约申请消息透传给商家。
+        self.external_agreement_no = external_agreement_no
+        # 是否允许解约
+        self.allow_unsign = allow_unsign
+
+    def validate(self):
+        self.validate_required(self.user_tuid, 'user_tuid')
+        self.validate_required(self.external_agreement_no, 'external_agreement_no')
+        self.validate_required(self.allow_unsign, 'allow_unsign')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.user_tuid is not None:
+            result['user_tuid'] = self.user_tuid
+        if self.external_agreement_no is not None:
+            result['external_agreement_no'] = self.external_agreement_no
+        if self.allow_unsign is not None:
+            result['allow_unsign'] = self.allow_unsign
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('user_tuid') is not None:
+            self.user_tuid = m.get('user_tuid')
+        if m.get('external_agreement_no') is not None:
+            self.external_agreement_no = m.get('external_agreement_no')
+        if m.get('allow_unsign') is not None:
+            self.allow_unsign = m.get('allow_unsign')
+        return self
+
+
+class UnbindContractPayResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        unsign_success: bool = None,
+        code: str = None,
+        msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否解约成功
+        self.unsign_success = unsign_success
+        # 业务处理结果码
+        self.code = code
+        # 业务结果描述
+        self.msg = msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.unsign_success is not None:
+            result['unsign_success'] = self.unsign_success
+        if self.code is not None:
+            result['code'] = self.code
+        if self.msg is not None:
+            result['msg'] = self.msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('unsign_success') is not None:
+            self.unsign_success = m.get('unsign_success')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('msg') is not None:
+            self.msg = m.get('msg')
+        return self
+
+
+class QueryContractComplainRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        complain_event_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 投诉单号
+        self.complain_event_id = complain_event_id
+
+    def validate(self):
+        self.validate_required(self.complain_event_id, 'complain_event_id')
+        if self.complain_event_id is not None:
+            self.validate_max_length(self.complain_event_id, 'complain_event_id', 64)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.complain_event_id is not None:
+            result['complain_event_id'] = self.complain_event_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('complain_event_id') is not None:
+            self.complain_event_id = m.get('complain_event_id')
+        return self
+
+
+class QueryContractComplainResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        complain_event_id: str = None,
+        status: str = None,
+        trade_no: str = None,
+        merchant_order_no: str = None,
+        gmt_create: str = None,
+        gmt_modified: str = None,
+        gmt_finished: str = None,
+        leaf_category_name: str = None,
+        complain_reason: str = None,
+        content: str = None,
+        images: List[str] = None,
+        phone_no: str = None,
+        trade_amount: str = None,
+        reply_detail_infos: List[ReplayDetailInfo] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 投诉单号
+        self.complain_event_id = complain_event_id
+        # 投诉单状态
+        # 商家处理中：MERCHANT_PROCESSING
+        # 商家已反馈：MERCHANT_FEEDBACKED
+        # 投诉已完结：FINISHED
+        # 投诉已撤销：CANCELLED
+        # 平台处理中：PLATFORM_PROCESSING
+        # 平台处理完结：PLATFORM_FINISH
+        # 系统关闭：CLOSED
+        self.status = status
+        # 支付宝交易号
+        self.trade_no = trade_no
+        # 商家订单号
+        self.merchant_order_no = merchant_order_no
+        # 投诉单创建时间
+        self.gmt_create = gmt_create
+        # 投诉单修改时间
+        self.gmt_modified = gmt_modified
+        # 投诉单完结时间
+        self.gmt_finished = gmt_finished
+        # 用户投诉诉求
+        self.leaf_category_name = leaf_category_name
+        # 用户投诉原因
+        self.complain_reason = complain_reason
+        # 用户投诉内容
+        self.content = content
+        # 投诉图片
+        self.images = images
+        # 投诉人电话号码
+        self.phone_no = phone_no
+        # 交易金额，单位元
+        self.trade_amount = trade_amount
+        # 用户与商家之间的协商记录
+        self.reply_detail_infos = reply_detail_infos
+
+    def validate(self):
+        if self.reply_detail_infos:
+            for k in self.reply_detail_infos:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.complain_event_id is not None:
+            result['complain_event_id'] = self.complain_event_id
+        if self.status is not None:
+            result['status'] = self.status
+        if self.trade_no is not None:
+            result['trade_no'] = self.trade_no
+        if self.merchant_order_no is not None:
+            result['merchant_order_no'] = self.merchant_order_no
+        if self.gmt_create is not None:
+            result['gmt_create'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['gmt_modified'] = self.gmt_modified
+        if self.gmt_finished is not None:
+            result['gmt_finished'] = self.gmt_finished
+        if self.leaf_category_name is not None:
+            result['leaf_category_name'] = self.leaf_category_name
+        if self.complain_reason is not None:
+            result['complain_reason'] = self.complain_reason
+        if self.content is not None:
+            result['content'] = self.content
+        if self.images is not None:
+            result['images'] = self.images
+        if self.phone_no is not None:
+            result['phone_no'] = self.phone_no
+        if self.trade_amount is not None:
+            result['trade_amount'] = self.trade_amount
+        result['reply_detail_infos'] = []
+        if self.reply_detail_infos is not None:
+            for k in self.reply_detail_infos:
+                result['reply_detail_infos'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('complain_event_id') is not None:
+            self.complain_event_id = m.get('complain_event_id')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('trade_no') is not None:
+            self.trade_no = m.get('trade_no')
+        if m.get('merchant_order_no') is not None:
+            self.merchant_order_no = m.get('merchant_order_no')
+        if m.get('gmt_create') is not None:
+            self.gmt_create = m.get('gmt_create')
+        if m.get('gmt_modified') is not None:
+            self.gmt_modified = m.get('gmt_modified')
+        if m.get('gmt_finished') is not None:
+            self.gmt_finished = m.get('gmt_finished')
+        if m.get('leaf_category_name') is not None:
+            self.leaf_category_name = m.get('leaf_category_name')
+        if m.get('complain_reason') is not None:
+            self.complain_reason = m.get('complain_reason')
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('images') is not None:
+            self.images = m.get('images')
+        if m.get('phone_no') is not None:
+            self.phone_no = m.get('phone_no')
+        if m.get('trade_amount') is not None:
+            self.trade_amount = m.get('trade_amount')
+        self.reply_detail_infos = []
+        if m.get('reply_detail_infos') is not None:
+            for k in m.get('reply_detail_infos'):
+                temp_model = ReplayDetailInfo()
+                self.reply_detail_infos.append(temp_model.from_map(k))
+        return self
+
+
+class SendContractComplainfeedbackRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        complain_event_id: str = None,
+        feedback_code: str = None,
+        feedback_content: str = None,
+        feedback_images: str = None,
+        operator: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 支付宝侧投诉单号
+        self.complain_event_id = complain_event_id
+        # 反馈类目ID
+        # 00:使用体验保障金退款；
+        # 02:通过其他方式退款;
+        # 03:已发货;
+        # 04:其他;
+        # 05:已完成售后服务;
+        # 06:非我方责任范围；
+        self.feedback_code = feedback_code
+        # 反馈内容，字数不超过200个字
+        self.feedback_content = feedback_content
+        # 商家处理投诉时反馈凭证的图片id，多个逗号隔开（图片id可以通过"商户上传处理图片"接口获取）
+        self.feedback_images = feedback_images
+        # 处理投诉人，字数不超过6个字
+        self.operator = operator
+
+    def validate(self):
+        self.validate_required(self.complain_event_id, 'complain_event_id')
+        if self.complain_event_id is not None:
+            self.validate_max_length(self.complain_event_id, 'complain_event_id', 64)
+        self.validate_required(self.feedback_code, 'feedback_code')
+        if self.feedback_code is not None:
+            self.validate_max_length(self.feedback_code, 'feedback_code', 32)
+        self.validate_required(self.feedback_content, 'feedback_content')
+        if self.feedback_content is not None:
+            self.validate_max_length(self.feedback_content, 'feedback_content', 200)
+        if self.operator is not None:
+            self.validate_max_length(self.operator, 'operator', 32)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.complain_event_id is not None:
+            result['complain_event_id'] = self.complain_event_id
+        if self.feedback_code is not None:
+            result['feedback_code'] = self.feedback_code
+        if self.feedback_content is not None:
+            result['feedback_content'] = self.feedback_content
+        if self.feedback_images is not None:
+            result['feedback_images'] = self.feedback_images
+        if self.operator is not None:
+            result['operator'] = self.operator
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('complain_event_id') is not None:
+            self.complain_event_id = m.get('complain_event_id')
+        if m.get('feedback_code') is not None:
+            self.feedback_code = m.get('feedback_code')
+        if m.get('feedback_content') is not None:
+            self.feedback_content = m.get('feedback_content')
+        if m.get('feedback_images') is not None:
+            self.feedback_images = m.get('feedback_images')
+        if m.get('operator') is not None:
+            self.operator = m.get('operator')
+        return self
+
+
+class SendContractComplainfeedbackResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        submit_success: bool = None,
+        code: str = None,
+        msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否反馈成功
+        self.submit_success = submit_success
+        # 业务处理结果码
+        self.code = code
+        # 业务结果描述
+        self.msg = msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.submit_success is not None:
+            result['submit_success'] = self.submit_success
+        if self.code is not None:
+            result['code'] = self.code
+        if self.msg is not None:
+            result['msg'] = self.msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('submit_success') is not None:
+            self.submit_success = m.get('submit_success')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('msg') is not None:
+            self.msg = m.get('msg')
+        return self
+
+
+class UploadContractComplainimageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        file_name: str = None,
+        content: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 图片名称，支持后缀格式：jpg、jpeg、png
+        self.file_name = file_name
+        # 图片二进制字节流
+        self.content = content
+
+    def validate(self):
+        self.validate_required(self.file_name, 'file_name')
+        if self.file_name is not None:
+            self.validate_max_length(self.file_name, 'file_name', 32)
+        self.validate_required(self.content, 'content')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.file_name is not None:
+            result['file_name'] = self.file_name
+        if self.content is not None:
+            result['content'] = self.content
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('file_name') is not None:
+            self.file_name = m.get('file_name')
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        return self
+
+
+class UploadContractComplainimageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        image_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 图片id
+        self.image_id = image_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.image_id is not None:
+            result['image_id'] = self.image_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('image_id') is not None:
+            self.image_id = m.get('image_id')
+        return self
+
+
+class QueryContractComplaineventidsRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        complain_start_date: str = None,
+        complain_end_date: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 客诉单创建开始日期
+        self.complain_start_date = complain_start_date
+        # 客诉单创建开始日期
+        self.complain_end_date = complain_end_date
+
+    def validate(self):
+        self.validate_required(self.complain_start_date, 'complain_start_date')
+        self.validate_required(self.complain_end_date, 'complain_end_date')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.complain_start_date is not None:
+            result['complain_start_date'] = self.complain_start_date
+        if self.complain_end_date is not None:
+            result['complain_end_date'] = self.complain_end_date
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('complain_start_date') is not None:
+            self.complain_start_date = m.get('complain_start_date')
+        if m.get('complain_end_date') is not None:
+            self.complain_end_date = m.get('complain_end_date')
+        return self
+
+
+class QueryContractComplaineventidsResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        complain_event_ids: List[str] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 投诉单id列表
+        self.complain_event_ids = complain_event_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.complain_event_ids is not None:
+            result['complain_event_ids'] = self.complain_event_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('complain_event_ids') is not None:
+            self.complain_event_ids = m.get('complain_event_ids')
+        return self
+
+
+class PushDigitalcontentUsageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        content_id: str = None,
+        device_id: str = None,
+        usage: str = None,
+        client_token: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 内容id
+        self.content_id = content_id
+        # 设备id
+        self.device_id = device_id
+        # 使用量，按次使用需要为数字
+        self.usage = usage
+        # 客户端幂等token
+        self.client_token = client_token
+
+    def validate(self):
+        self.validate_required(self.content_id, 'content_id')
+        self.validate_required(self.device_id, 'device_id')
+        self.validate_required(self.usage, 'usage')
+        self.validate_required(self.client_token, 'client_token')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.content_id is not None:
+            result['content_id'] = self.content_id
+        if self.device_id is not None:
+            result['device_id'] = self.device_id
+        if self.usage is not None:
+            result['usage'] = self.usage
+        if self.client_token is not None:
+            result['client_token'] = self.client_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('content_id') is not None:
+            self.content_id = m.get('content_id')
+        if m.get('device_id') is not None:
+            self.device_id = m.get('device_id')
+        if m.get('usage') is not None:
+            self.usage = m.get('usage')
+        if m.get('client_token') is not None:
+            self.client_token = m.get('client_token')
+        return self
+
+
+class PushDigitalcontentUsageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        order_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 上报成功返回的订单id
+        self.order_id = order_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        return self
+
+
+class ApplyDigitalcontentOrderRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        content_id: str = None,
+        device_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 内容id
+        self.content_id = content_id
+        # 设备id
+        self.device_id = device_id
+
+    def validate(self):
+        self.validate_required(self.content_id, 'content_id')
+        self.validate_required(self.device_id, 'device_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.content_id is not None:
+            result['content_id'] = self.content_id
+        if self.device_id is not None:
+            result['device_id'] = self.device_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('content_id') is not None:
+            self.content_id = m.get('content_id')
+        if m.get('device_id') is not None:
+            self.device_id = m.get('device_id')
+        return self
+
+
+class ApplyDigitalcontentOrderResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        order_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 生成的订单id
+        self.order_id = order_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        return self
+
+
+class SubmitDigitalcontentOrderRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        order_id: str = None,
+        payment_id: str = None,
+        payment_type: str = None,
+        usage: str = None,
+        client_token: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 订单id
+        self.order_id = order_id
+        # 支付id
+        self.payment_id = payment_id
+        # 付款方式
+        # ●AliPay，支付宝
+        # ● WeChatPay，微信支付
+        # ● Bank，银行卡支付
+        # ● Other，其他
+        self.payment_type = payment_type
+        # 按次使用时需要为整数
+        self.usage = usage
+        # 用作幂等，防重调用
+        self.client_token = client_token
+
+    def validate(self):
+        self.validate_required(self.order_id, 'order_id')
+        self.validate_required(self.payment_id, 'payment_id')
+        self.validate_required(self.payment_type, 'payment_type')
+        self.validate_required(self.usage, 'usage')
+        self.validate_required(self.client_token, 'client_token')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        if self.payment_id is not None:
+            result['payment_id'] = self.payment_id
+        if self.payment_type is not None:
+            result['payment_type'] = self.payment_type
+        if self.usage is not None:
+            result['usage'] = self.usage
+        if self.client_token is not None:
+            result['client_token'] = self.client_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        if m.get('payment_id') is not None:
+            self.payment_id = m.get('payment_id')
+        if m.get('payment_type') is not None:
+            self.payment_type = m.get('payment_type')
+        if m.get('usage') is not None:
+            self.usage = m.get('usage')
+        if m.get('client_token') is not None:
+            self.client_token = m.get('client_token')
+        return self
+
+
+class SubmitDigitalcontentOrderResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        token: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 传递给apk使用的token
+        self.token = token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.token is not None:
+            result['token'] = self.token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('token') is not None:
+            self.token = m.get('token')
+        return self
+
+
 class SyncInnerTransRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         id: int = None,
         transaction_id: str = None,
@@ -26955,14 +28100,16 @@
         auth_token: str = None,
         product_instance_id: str = None,
         party_id: int = None,
         party_type: str = None,
         party_organization_info: JudicialOrgInfo = None,
         coordinator_person_info: JudicialPersonInfo = None,
         coordinator_bank_info: JudicialBankInfo = None,
+        sub_tenant_id: str = None,
+        agent_create_party: bool = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 委托申请方配置ID
         self.party_id = party_id
         # 委托申请方类型,目前仅支持企业.
@@ -26972,14 +28119,19 @@
         # 企业信息实体;
         # 当申请方类型为企业时,该字段必填;
         self.party_organization_info = party_organization_info
         # 案件协同工作联系人信息实体
         self.coordinator_person_info = coordinator_person_info
         # 案件协同人银行账户信息
         self.coordinator_bank_info = coordinator_bank_info
+        # adsada
+        self.sub_tenant_id = sub_tenant_id
+        # 默认为空,true表示为二级商户创建或者修改申请人,sub_tenant_id不能为空,
+        # false表示为当前商户创建或者修改申请人,sub_tenant_id为空
+        self.agent_create_party = agent_create_party
 
     def validate(self):
         self.validate_required(self.party_type, 'party_type')
         if self.party_organization_info:
             self.party_organization_info.validate()
         if self.coordinator_person_info:
             self.coordinator_person_info.validate()
@@ -27002,14 +28154,18 @@
             result['party_type'] = self.party_type
         if self.party_organization_info is not None:
             result['party_organization_info'] = self.party_organization_info.to_map()
         if self.coordinator_person_info is not None:
             result['coordinator_person_info'] = self.coordinator_person_info.to_map()
         if self.coordinator_bank_info is not None:
             result['coordinator_bank_info'] = self.coordinator_bank_info.to_map()
+        if self.sub_tenant_id is not None:
+            result['sub_tenant_id'] = self.sub_tenant_id
+        if self.agent_create_party is not None:
+            result['agent_create_party'] = self.agent_create_party
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -27023,14 +28179,18 @@
             self.party_organization_info = temp_model.from_map(m['party_organization_info'])
         if m.get('coordinator_person_info') is not None:
             temp_model = JudicialPersonInfo()
             self.coordinator_person_info = temp_model.from_map(m['coordinator_person_info'])
         if m.get('coordinator_bank_info') is not None:
             temp_model = JudicialBankInfo()
             self.coordinator_bank_info = temp_model.from_map(m['coordinator_bank_info'])
+        if m.get('sub_tenant_id') is not None:
+            self.sub_tenant_id = m.get('sub_tenant_id')
+        if m.get('agent_create_party') is not None:
+            self.agent_create_party = m.get('agent_create_party')
         return self
 
 
 class SaveJusticePartyResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -27097,42 +28257,45 @@
         case_desc: str = None,
         case_biz_element_info: str = None,
         party_id: int = None,
         pleader_type: str = None,
         pleader_person_info: JudicialPersonInfo = None,
         use_template: bool = None,
         business_info: str = None,
+        evidence_info: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 案由
         self.case_reason = case_reason
         # 业务类型
         # LEASE- 租赁
         # HB_FINANCIAL - HB金融
         self.case_type = case_type
         # 外部业务ID
         self.external_biz_id = external_biz_id
         # 业务描述,用于案件的补充描述; 没有则不填
         self.case_desc = case_desc
-        # 针对对应业务类型的证据要素补充.
+        # 针对对应业务类型的案件要素补充.
         self.case_biz_element_info = case_biz_element_info
         # 当事人(申请人)ID, 案件填充信息返回
         self.party_id = party_id
         # 答辩人类型, 目前仅支持个人.
         # PERSON , 个人
         # ORG , 机构
         self.pleader_type = pleader_type
         # 答辩人(自然人)信息, 类型为个人时必填
         self.pleader_person_info = pleader_person_info
         # 是否使用模板
         self.use_template = use_template
         # 使用模板时必填，根据案件要素模板对应提供要素信息
         self.business_info = business_info
+        # 使用模板时必填，根据案件要素模板对应提供证据信息
+        self.evidence_info = evidence_info
 
     def validate(self):
         self.validate_required(self.case_reason, 'case_reason')
         self.validate_required(self.case_type, 'case_type')
         self.validate_required(self.external_biz_id, 'external_biz_id')
         self.validate_required(self.party_id, 'party_id')
         if self.pleader_person_info:
@@ -27164,14 +28327,16 @@
             result['pleader_type'] = self.pleader_type
         if self.pleader_person_info is not None:
             result['pleader_person_info'] = self.pleader_person_info.to_map()
         if self.use_template is not None:
             result['use_template'] = self.use_template
         if self.business_info is not None:
             result['business_info'] = self.business_info
+        if self.evidence_info is not None:
+            result['evidence_info'] = self.evidence_info
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -27193,14 +28358,16 @@
         if m.get('pleader_person_info') is not None:
             temp_model = JudicialPersonInfo()
             self.pleader_person_info = temp_model.from_map(m['pleader_person_info'])
         if m.get('use_template') is not None:
             self.use_template = m.get('use_template')
         if m.get('business_info') is not None:
             self.business_info = m.get('business_info')
+        if m.get('evidence_info') is not None:
+            self.evidence_info = m.get('evidence_info')
         return self
 
 
 class CreateJusticeNormalcaseResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -28101,70 +29268,86 @@
 
 class GetJusticeFileuploadurlRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         file_name: str = None,
+        file_md_5: str = None,
+        file_type: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 上传文件全名
         self.file_name = file_name
+        # 文件Md5值，用于上传后的文件校验
+        self.file_md_5 = file_md_5
+        # 枚举值：案件证据文件：EVIDENCE
+        self.file_type = file_type
 
     def validate(self):
         self.validate_required(self.file_name, 'file_name')
+        self.validate_required(self.file_md_5, 'file_md_5')
+        self.validate_required(self.file_type, 'file_type')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.file_name is not None:
             result['file_name'] = self.file_name
+        if self.file_md_5 is not None:
+            result['file_md5'] = self.file_md_5
+        if self.file_type is not None:
+            result['file_type'] = self.file_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('file_name') is not None:
             self.file_name = m.get('file_name')
+        if m.get('file_md5') is not None:
+            self.file_md_5 = m.get('file_md5')
+        if m.get('file_type') is not None:
+            self.file_type = m.get('file_type')
         return self
 
 
 class GetJusticeFileuploadurlResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         file_key: str = None,
         upload_url: str = None,
-        expired_time: str = None,
+        expired_time: int = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 获取的文件key, 请妥善保存, 用于后续接口调用.
         self.file_key = file_key
         # 文件上传链接url
         self.upload_url = upload_url
-        # 链接失效日期: "yyyy-MM-dd HH:mm:ss"
+        # 链接失效时间戳（毫秒）
         self.expired_time = expired_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28399,25 +29582,28 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         business_info: str = None,
         case_no: str = None,
+        biz_type: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 要素信息
         self.business_info = business_info
         # 查询的案件编号
         self.case_no = case_no
+        # 业务类型
+        self.biz_type = biz_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -28430,28 +29616,560 @@
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         if self.business_info is not None:
             result['business_info'] = self.business_info
         if self.case_no is not None:
             result['case_no'] = self.case_no
+        if self.biz_type is not None:
+            result['biz_type'] = self.biz_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('business_info') is not None:
             self.business_info = m.get('business_info')
         if m.get('case_no') is not None:
             self.case_no = m.get('case_no')
+        if m.get('biz_type') is not None:
+            self.biz_type = m.get('biz_type')
+        return self
+
+
+class CreateJusticeAgentcaseRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        case_reason: str = None,
+        biz_type: str = None,
+        sub_tenant_id: str = None,
+        external_biz_id: str = None,
+        case_desc: str = None,
+        business_info: str = None,
+        evidence_info: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 案由
+        self.case_reason = case_reason
+        # 业务类型，LEASE- 租赁 ，HB_FINANCIAL - HB金融， 模板创建的其他业务类型
+        self.biz_type = biz_type
+        # 二级商户租户ID，八位字母
+        self.sub_tenant_id = sub_tenant_id
+        # 外部业务ID
+        self.external_biz_id = external_biz_id
+        # 业务描述,用于案件的补充描述; 没有则不填
+        self.case_desc = case_desc
+        # 根据案件要素模板对应提供要素信息
+        self.business_info = business_info
+        # 根据案件要素模板对应提供证据信息
+        self.evidence_info = evidence_info
+
+    def validate(self):
+        self.validate_required(self.case_reason, 'case_reason')
+        self.validate_required(self.biz_type, 'biz_type')
+        self.validate_required(self.sub_tenant_id, 'sub_tenant_id')
+        self.validate_required(self.external_biz_id, 'external_biz_id')
+        self.validate_required(self.business_info, 'business_info')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.case_reason is not None:
+            result['case_reason'] = self.case_reason
+        if self.biz_type is not None:
+            result['biz_type'] = self.biz_type
+        if self.sub_tenant_id is not None:
+            result['sub_tenant_id'] = self.sub_tenant_id
+        if self.external_biz_id is not None:
+            result['external_biz_id'] = self.external_biz_id
+        if self.case_desc is not None:
+            result['case_desc'] = self.case_desc
+        if self.business_info is not None:
+            result['business_info'] = self.business_info
+        if self.evidence_info is not None:
+            result['evidence_info'] = self.evidence_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('case_reason') is not None:
+            self.case_reason = m.get('case_reason')
+        if m.get('biz_type') is not None:
+            self.biz_type = m.get('biz_type')
+        if m.get('sub_tenant_id') is not None:
+            self.sub_tenant_id = m.get('sub_tenant_id')
+        if m.get('external_biz_id') is not None:
+            self.external_biz_id = m.get('external_biz_id')
+        if m.get('case_desc') is not None:
+            self.case_desc = m.get('case_desc')
+        if m.get('business_info') is not None:
+            self.business_info = m.get('business_info')
+        if m.get('evidence_info') is not None:
+            self.evidence_info = m.get('evidence_info')
+        return self
+
+
+class CreateJusticeAgentcaseResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        case_id: int = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 案件创建是否成功
+        self.success = success
+        # 案件ID, 创建成功后, 返回的案件ID
+        self.case_id = case_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.case_id is not None:
+            result['case_id'] = self.case_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('case_id') is not None:
+            self.case_id = m.get('case_id')
+        return self
+
+
+class QueryJusticeRightsRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        record_id: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 案件维权记录编号
+        self.record_id = record_id
+
+    def validate(self):
+        self.validate_required(self.record_id, 'record_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.record_id is not None:
+            result['record_id'] = self.record_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('record_id') is not None:
+            self.record_id = m.get('record_id')
+        return self
+
+
+class QueryJusticeRightsResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        business_info: str = None,
+        evidence_info: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 案件业务信息(申请人,被申请人,业务要素),示例查看对接文档
+        self.business_info = business_info
+        # 证据信息,示例查看对接文档
+        self.evidence_info = evidence_info
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.business_info is not None:
+            result['business_info'] = self.business_info
+        if self.evidence_info is not None:
+            result['evidence_info'] = self.evidence_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('business_info') is not None:
+            self.business_info = m.get('business_info')
+        if m.get('evidence_info') is not None:
+            self.evidence_info = m.get('evidence_info')
+        return self
+
+
+class UpdateJusticeRightsRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        record_id: int = None,
+        case_status: str = None,
+        status_ext: str = None,
+        status_file_infos: List[FileInfo] = None,
+        case_status_date: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 案件维权记录编号
+        self.record_id = record_id
+        # 案件状态(枚举)
+        self.case_status = case_status
+        # 状态扩展信息示例查看对接文档
+        self.status_ext = status_ext
+        # 文件信息,示例查看对接文档
+        self.status_file_infos = status_file_infos
+        # 案件状态对应的实际时间
+        self.case_status_date = case_status_date
+
+    def validate(self):
+        self.validate_required(self.record_id, 'record_id')
+        self.validate_required(self.case_status, 'case_status')
+        if self.status_file_infos:
+            for k in self.status_file_infos:
+                if k:
+                    k.validate()
+        self.validate_required(self.case_status_date, 'case_status_date')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.record_id is not None:
+            result['record_id'] = self.record_id
+        if self.case_status is not None:
+            result['case_status'] = self.case_status
+        if self.status_ext is not None:
+            result['status_ext'] = self.status_ext
+        result['status_file_infos'] = []
+        if self.status_file_infos is not None:
+            for k in self.status_file_infos:
+                result['status_file_infos'].append(k.to_map() if k else None)
+        if self.case_status_date is not None:
+            result['case_status_date'] = self.case_status_date
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('record_id') is not None:
+            self.record_id = m.get('record_id')
+        if m.get('case_status') is not None:
+            self.case_status = m.get('case_status')
+        if m.get('status_ext') is not None:
+            self.status_ext = m.get('status_ext')
+        self.status_file_infos = []
+        if m.get('status_file_infos') is not None:
+            for k in m.get('status_file_infos'):
+                temp_model = FileInfo()
+                self.status_file_infos.append(temp_model.from_map(k))
+        if m.get('case_status_date') is not None:
+            self.case_status_date = m.get('case_status_date')
+        return self
+
+
+class UpdateJusticeRightsResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否处理成功
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class NotifyJusticeRightspaymentRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        record_id: int = None,
+        amount: str = None,
+        payment_type: str = None,
+        payment_status: str = None,
+        payment_remark: str = None,
+        payment_file_infos: List[FileInfo] = None,
+        payment_info: PaymentInfo = None,
+        payment_status_success_date: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 案件维权记录编号
+        self.record_id = record_id
+        # 缴费金额(支持两位小数)
+        self.amount = amount
+        # 费用类型(枚举)
+        # ARBITRATION: 仲裁案件受理费
+        self.payment_type = payment_type
+        # 缴费状态(枚举)
+        # WAIT_FEE: 待缴费
+        # SUCCESS: 成功
+        # FAIL: 失败
+        self.payment_status = payment_status
+        # 缴费失败的描述(不是缴费完成时,必填)
+        # 不超过500字符
+        self.payment_remark = payment_remark
+        # 相关的文件信息列表,示例查看对接文档
+        self.payment_file_infos = payment_file_infos
+        # 缴费账户信息(待缴费时必填),示例查看对接文档
+        self.payment_info = payment_info
+        # 缴费状态(SUCCESS)实际对应时间
+        self.payment_status_success_date = payment_status_success_date
+
+    def validate(self):
+        self.validate_required(self.record_id, 'record_id')
+        self.validate_required(self.amount, 'amount')
+        self.validate_required(self.payment_type, 'payment_type')
+        self.validate_required(self.payment_status, 'payment_status')
+        if self.payment_file_infos:
+            for k in self.payment_file_infos:
+                if k:
+                    k.validate()
+        if self.payment_info:
+            self.payment_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.record_id is not None:
+            result['record_id'] = self.record_id
+        if self.amount is not None:
+            result['amount'] = self.amount
+        if self.payment_type is not None:
+            result['payment_type'] = self.payment_type
+        if self.payment_status is not None:
+            result['payment_status'] = self.payment_status
+        if self.payment_remark is not None:
+            result['payment_remark'] = self.payment_remark
+        result['payment_file_infos'] = []
+        if self.payment_file_infos is not None:
+            for k in self.payment_file_infos:
+                result['payment_file_infos'].append(k.to_map() if k else None)
+        if self.payment_info is not None:
+            result['payment_info'] = self.payment_info.to_map()
+        if self.payment_status_success_date is not None:
+            result['payment_status_success_date'] = self.payment_status_success_date
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('record_id') is not None:
+            self.record_id = m.get('record_id')
+        if m.get('amount') is not None:
+            self.amount = m.get('amount')
+        if m.get('payment_type') is not None:
+            self.payment_type = m.get('payment_type')
+        if m.get('payment_status') is not None:
+            self.payment_status = m.get('payment_status')
+        if m.get('payment_remark') is not None:
+            self.payment_remark = m.get('payment_remark')
+        self.payment_file_infos = []
+        if m.get('payment_file_infos') is not None:
+            for k in m.get('payment_file_infos'):
+                temp_model = FileInfo()
+                self.payment_file_infos.append(temp_model.from_map(k))
+        if m.get('payment_info') is not None:
+            temp_model = PaymentInfo()
+            self.payment_info = temp_model.from_map(m['payment_info'])
+        if m.get('payment_status_success_date') is not None:
+            self.payment_status_success_date = m.get('payment_status_success_date')
+        return self
+
+
+class NotifyJusticeRightspaymentResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否处理成功
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
 class CreateLeaseProductinfoRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -32707,14 +34425,15 @@
         result_code: str = None,
         result_msg: str = None,
         status: str = None,
         policy_no: str = None,
         srd_premium: str = None,
         code: str = None,
         message: str = None,
+        repay_flag: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -32724,14 +34443,16 @@
         self.policy_no = policy_no
         # 退还保费，单位：分
         self.srd_premium = srd_premium
         # 结果码，00表示成功
         self.code = code
         # 结果描述
         self.message = message
+        # 是否为实收保单退保
+        self.repay_flag = repay_flag
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -32750,14 +34471,16 @@
             result['policy_no'] = self.policy_no
         if self.srd_premium is not None:
             result['srd_premium'] = self.srd_premium
         if self.code is not None:
             result['code'] = self.code
         if self.message is not None:
             result['message'] = self.message
+        if self.repay_flag is not None:
+            result['repay_flag'] = self.repay_flag
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -32770,14 +34493,16 @@
             self.policy_no = m.get('policy_no')
         if m.get('srd_premium') is not None:
             self.srd_premium = m.get('srd_premium')
         if m.get('code') is not None:
             self.code = m.get('code')
         if m.get('message') is not None:
             self.message = m.get('message')
+        if m.get('repay_flag') is not None:
+            self.repay_flag = m.get('repay_flag')
         return self
 
 
 class PushRefinanceInvalidorderRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -32942,27 +34667,30 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         paas: str = None,
         risk_id: str = None,
+        risk_version: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 风控结果
         # SUCCESS：通过
         # FAIL：不通过
         self.paas = paas
         # 风控识别id，与订单id对应
         self.risk_id = risk_id
+        # 风控规则对应的版本号
+        self.risk_version = risk_version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -32975,28 +34703,32 @@
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         if self.paas is not None:
             result['paas'] = self.paas
         if self.risk_id is not None:
             result['risk_id'] = self.risk_id
+        if self.risk_version is not None:
+            result['risk_version'] = self.risk_version
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('paas') is not None:
             self.paas = m.get('paas')
         if m.get('risk_id') is not None:
             self.risk_id = m.get('risk_id')
+        if m.get('risk_version') is not None:
+            self.risk_version = m.get('risk_version')
         return self
 
 
 class CreateLeaseAsyncverifyinfoRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -33070,14 +34802,16 @@
         if self.lease_corp_id is not None:
             self.validate_max_length(self.lease_corp_id, 'lease_corp_id', 50)
         if self.lease_corp_name is not None:
             self.validate_max_length(self.lease_corp_name, 'lease_corp_name', 50)
         if self.lease_corp_owner_name is not None:
             self.validate_max_length(self.lease_corp_owner_name, 'lease_corp_owner_name', 50)
         self.validate_required(self.lease_id, 'lease_id')
+        if self.lease_id is not None:
+            self.validate_max_length(self.lease_id, 'lease_id', 32)
         self.validate_required(self.order_id, 'order_id')
         if self.order_id is not None:
             self.validate_max_length(self.order_id, 'order_id', 50)
         if self.user_name is not None:
             self.validate_max_length(self.user_name, 'user_name', 10)
         self.validate_required(self.verify_result, 'verify_result')
 
@@ -33298,21 +35032,29 @@
         # 归还日，格式为"2019-07-31 12:00:00"
         self.return_time = return_time
         # 归还日，格式为"2019-07-31 12:00:00"
         self.return_time_list = return_time_list
 
     def validate(self):
         self.validate_required(self.lease_id, 'lease_id')
+        if self.lease_id is not None:
+            self.validate_max_length(self.lease_id, 'lease_id', 32)
         self.validate_required(self.order_id, 'order_id')
         if self.order_id is not None:
             self.validate_max_length(self.order_id, 'order_id', 50)
         self.validate_required(self.pay_in_advance_time_list, 'pay_in_advance_time_list')
         self.validate_required(self.promise_hash, 'promise_hash')
+        if self.promise_hash is not None:
+            self.validate_max_length(self.promise_hash, 'promise_hash', 70)
         self.validate_required(self.promise_tx_hash, 'promise_tx_hash')
+        if self.promise_tx_hash is not None:
+            self.validate_max_length(self.promise_tx_hash, 'promise_tx_hash', 70)
         self.validate_required(self.return_money_list, 'return_money_list')
+        if self.return_rate is not None:
+            self.validate_minimum(self.return_rate, 'return_rate', 0)
         self.validate_required(self.return_time_list, 'return_time_list')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
@@ -33514,15 +35256,20 @@
         self.validate_required(self.lease_id, 'lease_id')
         if self.lease_id is not None:
             self.validate_max_length(self.lease_id, 'lease_id', 50)
         self.validate_required(self.order_id, 'order_id')
         if self.order_id is not None:
             self.validate_max_length(self.order_id, 'order_id', 50)
         self.validate_required(self.return_index, 'return_index')
+        if self.return_index is not None:
+            self.validate_maximum(self.return_index, 'return_index', 1024)
+            self.validate_minimum(self.return_index, 'return_index', 1)
         self.validate_required(self.start_time, 'start_time')
+        if self.memo is not None:
+            self.validate_max_length(self.memo, 'memo', 128)
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -33734,24 +35481,37 @@
         self.validate_required(self.lease_id, 'lease_id')
         if self.lease_id is not None:
             self.validate_max_length(self.lease_id, 'lease_id', 50)
         self.validate_required(self.order_id, 'order_id')
         if self.order_id is not None:
             self.validate_max_length(self.order_id, 'order_id', 50)
         self.validate_required(self.remain_return_money, 'remain_return_money')
+        if self.remain_return_money is not None:
+            self.validate_minimum(self.remain_return_money, 'remain_return_money', 0)
         self.validate_required(self.remain_return_term, 'remain_return_term')
+        if self.remain_return_term is not None:
+            self.validate_maximum(self.remain_return_term, 'remain_return_term', 1024)
+            self.validate_minimum(self.remain_return_term, 'remain_return_term', 0)
         self.validate_required(self.repayment_unique_id, 'repayment_unique_id')
         self.validate_required(self.return_description, 'return_description')
         if self.return_description is not None:
             self.validate_max_length(self.return_description, 'return_description', 256)
         self.validate_required(self.return_index, 'return_index')
+        if self.return_index is not None:
+            self.validate_maximum(self.return_index, 'return_index', 1024)
+            self.validate_minimum(self.return_index, 'return_index', 1)
         self.validate_required(self.return_money, 'return_money')
+        if self.return_money is not None:
+            self.validate_minimum(self.return_money, 'return_money', 0)
         self.validate_required(self.return_status, 'return_status')
         self.validate_required(self.return_time, 'return_time')
         self.validate_required(self.source, 'source')
+        if self.source is not None:
+            self.validate_maximum(self.source, 'source', 2)
+            self.validate_minimum(self.source, 'source', 1)
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -34440,17 +36200,17 @@
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         status: str = None,
         tx_hash: str = None,
         chain_fail_message: str = None,
-        response_data: str = None,
         code: str = None,
         message: str = None,
+        response_data: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -34459,20 +36219,20 @@
         # CHAINING（上链中）SUCCESS(上链成功)
         # FAIL(上链失败)
         self.status = status
         # 成功的时候返回txHash
         self.tx_hash = tx_hash
         # 上链失败信息，status为FAIL时返回
         self.chain_fail_message = chain_fail_message
-        # 对应的加密后的具体信息,异步查询场景会有值
-        self.response_data = response_data
         # 结果码，OK表示成功
         self.code = code
         # 结果描述
         self.message = message
+        # 查询对应的具体的数据
+        self.response_data = response_data
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -34487,20 +36247,20 @@
             result['result_msg'] = self.result_msg
         if self.status is not None:
             result['status'] = self.status
         if self.tx_hash is not None:
             result['tx_hash'] = self.tx_hash
         if self.chain_fail_message is not None:
             result['chain_fail_message'] = self.chain_fail_message
-        if self.response_data is not None:
-            result['response_data'] = self.response_data
         if self.code is not None:
             result['code'] = self.code
         if self.message is not None:
             result['message'] = self.message
+        if self.response_data is not None:
+            result['response_data'] = self.response_data
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -34509,20 +36269,20 @@
             self.result_msg = m.get('result_msg')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('tx_hash') is not None:
             self.tx_hash = m.get('tx_hash')
         if m.get('chain_fail_message') is not None:
             self.chain_fail_message = m.get('chain_fail_message')
-        if m.get('response_data') is not None:
-            self.response_data = m.get('response_data')
         if m.get('code') is not None:
             self.code = m.get('code')
         if m.get('message') is not None:
             self.message = m.get('message')
+        if m.get('response_data') is not None:
+            self.response_data = m.get('response_data')
         return self
 
 
 class CreateWitnessFlowRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -46548,14 +48308,977 @@
         if m.get('file_hash') is not None:
             self.file_hash = m.get('file_hash')
         if m.get('hash_algorithm') is not None:
             self.hash_algorithm = m.get('hash_algorithm')
         return self
 
 
+class CreateDataflowTextRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        notary_content: str = None,
+        phase: str = None,
+        transaction_id: str = None,
+        properties: str = None,
+        text_notary_type: str = None,
+        hash_algorithm: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 用户本地加密后的存证内容
+        self.notary_content = notary_content
+        # 存证阶段
+        self.phase = phase
+        # 存证事务id
+        self.transaction_id = transaction_id
+        # 存证拓展信息
+        self.properties = properties
+        # 存证类型，支持
+        # ● TEXT_HASH：文本哈希
+        # ● TEXT_RAW：源文本（默认）
+        self.text_notary_type = text_notary_type
+        # 哈希算法，当存证类型为TEXT_HASH时必填，目前支持两种
+        # ● SHA256
+        # ● SM3
+        self.hash_algorithm = hash_algorithm
+
+    def validate(self):
+        self.validate_required(self.notary_content, 'notary_content')
+        self.validate_required(self.phase, 'phase')
+        self.validate_required(self.transaction_id, 'transaction_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.notary_content is not None:
+            result['notary_content'] = self.notary_content
+        if self.phase is not None:
+            result['phase'] = self.phase
+        if self.transaction_id is not None:
+            result['transaction_id'] = self.transaction_id
+        if self.properties is not None:
+            result['properties'] = self.properties
+        if self.text_notary_type is not None:
+            result['text_notary_type'] = self.text_notary_type
+        if self.hash_algorithm is not None:
+            result['hash_algorithm'] = self.hash_algorithm
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('notary_content') is not None:
+            self.notary_content = m.get('notary_content')
+        if m.get('phase') is not None:
+            self.phase = m.get('phase')
+        if m.get('transaction_id') is not None:
+            self.transaction_id = m.get('transaction_id')
+        if m.get('properties') is not None:
+            self.properties = m.get('properties')
+        if m.get('text_notary_type') is not None:
+            self.text_notary_type = m.get('text_notary_type')
+        if m.get('hash_algorithm') is not None:
+            self.hash_algorithm = m.get('hash_algorithm')
+        return self
+
+
+class CreateDataflowTextResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        tx_hash: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 交易哈希，链上存证地址
+        self.tx_hash = tx_hash
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.tx_hash is not None:
+            result['tx_hash'] = self.tx_hash
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('tx_hash') is not None:
+            self.tx_hash = m.get('tx_hash')
+        return self
+
+
+class GetDataflowTextRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tx_hash: str = None,
+        target_tenant_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 存证地址
+        self.tx_hash = tx_hash
+        # 存证方使用的8位英文租户id，当存证地址来自其他存证方用户时必填
+        self.target_tenant_id = target_tenant_id
+
+    def validate(self):
+        self.validate_required(self.tx_hash, 'tx_hash')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.tx_hash is not None:
+            result['tx_hash'] = self.tx_hash
+        if self.target_tenant_id is not None:
+            result['target_tenant_id'] = self.target_tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tx_hash') is not None:
+            self.tx_hash = m.get('tx_hash')
+        if m.get('target_tenant_id') is not None:
+            self.target_tenant_id = m.get('target_tenant_id')
+        return self
+
+
+class GetDataflowTextResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        content: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 存证内容
+        self.content = content
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.content is not None:
+            result['content'] = self.content
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        return self
+
+
+class CreateDataflowTransRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        customer: str = None,
+        sub_biz_id: str = None,
+        properties: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 存证主体信息，使用存证公钥加密
+        self.customer = customer
+        # 子业务ID，选填
+        self.sub_biz_id = sub_biz_id
+        # 扩展属性信息，使用存证公钥加密，选填
+        self.properties = properties
+
+    def validate(self):
+        self.validate_required(self.customer, 'customer')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.customer is not None:
+            result['customer'] = self.customer
+        if self.sub_biz_id is not None:
+            result['sub_biz_id'] = self.sub_biz_id
+        if self.properties is not None:
+            result['properties'] = self.properties
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('customer') is not None:
+            self.customer = m.get('customer')
+        if m.get('sub_biz_id') is not None:
+            self.sub_biz_id = m.get('sub_biz_id')
+        if m.get('properties') is not None:
+            self.properties = m.get('properties')
+        return self
+
+
+class CreateDataflowTransResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        transaction_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 存证事务id
+        self.transaction_id = transaction_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.transaction_id is not None:
+            result['transaction_id'] = self.transaction_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('transaction_id') is not None:
+            self.transaction_id = m.get('transaction_id')
+        return self
+
+
+class DeployDataflowContractRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        pubkey: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 信封密钥。存证方本地自行派生一堆非对称密钥，将公钥作为信封密钥。存证方用户后续读取链上信息（如存证密钥、存证数据原文）时，为避免链上明文信息泄漏，会使用该信封密钥对所有链上数据进行加密后再返回，保障数据安全。
+        self.pubkey = pubkey
+
+    def validate(self):
+        self.validate_required(self.pubkey, 'pubkey')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.pubkey is not None:
+            result['pubkey'] = self.pubkey
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('pubkey') is not None:
+            self.pubkey = m.get('pubkey')
+        return self
+
+
+class DeployDataflowContractResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        order_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 发起部署的请求回执，用于后续做部署结果查询。
+        self.order_id = order_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        return self
+
+
+class CreateDataflowAuthorizeRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        target_tenant: str = None,
+        auth_type: str = None,
+        auth_scope: str = None,
+        tx_hash_list: List[str] = None,
+        expire_time: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 被授权账户的租户ID
+        self.target_tenant = target_tenant
+        # 授权类型：
+        # 1. PUBKEY_UPLOAD：上传信封公钥
+        # 2. GET_NOTARY：查询存证原文
+        # 3. CHECK_NOTARY：核验存证信息
+        self.auth_type = auth_type
+        # 授权范围，授权类型为GET_NOTARY或者CHECK_NOTARY时必填，取值为：
+        # 1. TXHASH：交易哈希维度授权
+        # 2. ACCOUNT：账号维度授权
+        self.auth_scope = auth_scope
+        # 授权的目标存证地址，当授权类型为GET_NOTARY或者CHECK_NOTARY，且授权范围为TXHASH时必填，最多20个
+        self.tx_hash_list = tx_hash_list
+        # 授权有效的时间戳
+        self.expire_time = expire_time
+
+    def validate(self):
+        self.validate_required(self.target_tenant, 'target_tenant')
+        self.validate_required(self.auth_type, 'auth_type')
+        self.validate_required(self.expire_time, 'expire_time')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.target_tenant is not None:
+            result['target_tenant'] = self.target_tenant
+        if self.auth_type is not None:
+            result['auth_type'] = self.auth_type
+        if self.auth_scope is not None:
+            result['auth_scope'] = self.auth_scope
+        if self.tx_hash_list is not None:
+            result['tx_hash_list'] = self.tx_hash_list
+        if self.expire_time is not None:
+            result['expire_time'] = self.expire_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('target_tenant') is not None:
+            self.target_tenant = m.get('target_tenant')
+        if m.get('auth_type') is not None:
+            self.auth_type = m.get('auth_type')
+        if m.get('auth_scope') is not None:
+            self.auth_scope = m.get('auth_scope')
+        if m.get('tx_hash_list') is not None:
+            self.tx_hash_list = m.get('tx_hash_list')
+        if m.get('expire_time') is not None:
+            self.expire_time = m.get('expire_time')
+        return self
+
+
+class CreateDataflowAuthorizeResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        order_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 发起授权的请求回执，用于后续做发起授权结果查询。
+        self.order_id = order_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        return self
+
+
+class CancelDataflowAuthorizeRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        target_tenant: str = None,
+        auth_type: str = None,
+        auth_scope: str = None,
+        tx_hash_list: List[str] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 目标租户ID
+        self.target_tenant = target_tenant
+        # 授权类型： 1. PUBKEY_UPLOAD：上传信封公钥 2. GET_NOTARY：查询存证原文 3. CHECK_NOTARY：核验存证信息
+        self.auth_type = auth_type
+        # 授权范围，授权类型为GET_NOTARY或者CHECK_NOTARY时必填，取值为： 1. TXHASH：交易哈希维度授权 2. ACCOUNT：账号维度授权
+        self.auth_scope = auth_scope
+        # 授权的目标存证地址，当授权类型为GET_NOTARY或者CHECK_NOTARY，且授权范围为TXHASH时必填，最多20个
+        self.tx_hash_list = tx_hash_list
+
+    def validate(self):
+        self.validate_required(self.target_tenant, 'target_tenant')
+        self.validate_required(self.auth_type, 'auth_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.target_tenant is not None:
+            result['target_tenant'] = self.target_tenant
+        if self.auth_type is not None:
+            result['auth_type'] = self.auth_type
+        if self.auth_scope is not None:
+            result['auth_scope'] = self.auth_scope
+        if self.tx_hash_list is not None:
+            result['tx_hash_list'] = self.tx_hash_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('target_tenant') is not None:
+            self.target_tenant = m.get('target_tenant')
+        if m.get('auth_type') is not None:
+            self.auth_type = m.get('auth_type')
+        if m.get('auth_scope') is not None:
+            self.auth_scope = m.get('auth_scope')
+        if m.get('tx_hash_list') is not None:
+            self.tx_hash_list = m.get('tx_hash_list')
+        return self
+
+
+class CancelDataflowAuthorizeResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        order_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 发起授权的请求回执，用于后续做撤销授权的结果查询。
+        self.order_id = order_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        return self
+
+
+class QueryDataflowActionRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        query_type: str = None,
+        order_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 查询类型：
+        # 1. 合约部署：DEPLOY
+        # 2. 授权：AUTH
+        # 3. 撤销授权：CANCEL_AUTH
+        # 4. 密钥上传：PUB_KEY_UPLOAD
+        self.query_type = query_type
+        # 发起操作的请求回执
+        self.order_id = order_id
+
+    def validate(self):
+        self.validate_required(self.query_type, 'query_type')
+        self.validate_required(self.order_id, 'order_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.query_type is not None:
+            result['query_type'] = self.query_type
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('query_type') is not None:
+            self.query_type = m.get('query_type')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        return self
+
+
+class QueryDataflowActionResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        status: int = None,
+        encrypted_pubkey: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 操作状态
+        self.status = status
+        # 信封公钥加密后的存证公钥信息，当查询类型为DEPLOY且status为密钥上传成功时返回。
+        self.encrypted_pubkey = encrypted_pubkey
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.status is not None:
+            result['status'] = self.status
+        if self.encrypted_pubkey is not None:
+            result['encrypted_pubkey'] = self.encrypted_pubkey
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('encrypted_pubkey') is not None:
+            self.encrypted_pubkey = m.get('encrypted_pubkey')
+        return self
+
+
+class UploadDataflowPubkeyRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        pubkey: str = None,
+        from_tenant: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 信封公钥内容
+        self.pubkey = pubkey
+        # 存证方的租户ID
+        self.from_tenant = from_tenant
+
+    def validate(self):
+        self.validate_required(self.pubkey, 'pubkey')
+        self.validate_required(self.from_tenant, 'from_tenant')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.pubkey is not None:
+            result['pubkey'] = self.pubkey
+        if self.from_tenant is not None:
+            result['from_tenant'] = self.from_tenant
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('pubkey') is not None:
+            self.pubkey = m.get('pubkey')
+        if m.get('from_tenant') is not None:
+            self.from_tenant = m.get('from_tenant')
+        return self
+
+
+class UploadDataflowPubkeyResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        order_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 发起密钥上传的请求回执，用于后续做密钥上传结果查询。
+        self.order_id = order_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        return self
+
+
+class CreateDataflowAccountRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_chain_account: str = None,
+        key_algorithm: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 链上账号名称，真实名称会在前加租户ID
+        self.biz_chain_account = biz_chain_account
+        # 账户密钥算法
+        self.key_algorithm = key_algorithm
+
+    def validate(self):
+        self.validate_required(self.biz_chain_account, 'biz_chain_account')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_chain_account is not None:
+            result['biz_chain_account'] = self.biz_chain_account
+        if self.key_algorithm is not None:
+            result['key_algorithm'] = self.key_algorithm
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_chain_account') is not None:
+            self.biz_chain_account = m.get('biz_chain_account')
+        if m.get('key_algorithm') is not None:
+            self.key_algorithm = m.get('key_algorithm')
+        return self
+
+
+class CreateDataflowAccountResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        chain_account: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 实际生成的链上账户ID
+        self.chain_account = chain_account
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.chain_account is not None:
+            result['chain_account'] = self.chain_account
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('chain_account') is not None:
+            self.chain_account = m.get('chain_account')
+        return self
+
+
 class CreateFlowInstanceRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         template_id: str = None,
         flow_name: str = None,
@@ -49085,7 +51808,283 @@
         if m.get('gas_used') is not None:
             self.gas_used = m.get('gas_used')
         if m.get('log_base64') is not None:
             self.log_base_64 = m.get('log_base64')
         return self
 
 
+class CreateTrafficTraceidRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        scene_code: str = None,
+        user_id: str = None,
+        source: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务场景码
+        self.scene_code = scene_code
+        # 用户Id
+        self.user_id = user_id
+        # 渠道说明
+        self.source = source
+
+    def validate(self):
+        self.validate_required(self.scene_code, 'scene_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.source is not None:
+            result['source'] = self.source
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('source') is not None:
+            self.source = m.get('source')
+        return self
+
+
+class CreateTrafficTraceidResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        trace_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 返回traceId，全局唯一
+        self.trace_id = trace_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.trace_id is not None:
+            result['trace_id'] = self.trace_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('trace_id') is not None:
+            self.trace_id = m.get('trace_id')
+        return self
+
+
+class UploadTrafficOperatelogRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        trace_id: str = None,
+        event_time: str = None,
+        page_flag: str = None,
+        action_flag: str = None,
+        cur_url: str = None,
+        position_no: str = None,
+        item_id: str = None,
+        shop_id: str = None,
+        pre_url: str = None,
+        source: str = None,
+        ad_space_level: str = None,
+        group_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 通过trace_id生成接口生成的trace_id
+        self.trace_id = trace_id
+        # 事件时间
+        self.event_time = event_time
+        # 当前页面类型标记
+        self.page_flag = page_flag
+        # 行为标记
+        self.action_flag = action_flag
+        # 当前页面地址
+        self.cur_url = cur_url
+        # 事件对应位置编码
+        self.position_no = position_no
+        # 商品标识
+        self.item_id = item_id
+        # 店铺标识
+        self.shop_id = shop_id
+        # 上一跳页面地址
+        self.pre_url = pre_url
+        # 渠道说明
+        self.source = source
+        # 当前广告位级别
+        self.ad_space_level = ad_space_level
+        # 人群组标签ID
+        self.group_id = group_id
+
+    def validate(self):
+        self.validate_required(self.trace_id, 'trace_id')
+        self.validate_required(self.event_time, 'event_time')
+        self.validate_required(self.page_flag, 'page_flag')
+        self.validate_required(self.action_flag, 'action_flag')
+        self.validate_required(self.cur_url, 'cur_url')
+        self.validate_required(self.position_no, 'position_no')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.trace_id is not None:
+            result['trace_id'] = self.trace_id
+        if self.event_time is not None:
+            result['event_time'] = self.event_time
+        if self.page_flag is not None:
+            result['page_flag'] = self.page_flag
+        if self.action_flag is not None:
+            result['action_flag'] = self.action_flag
+        if self.cur_url is not None:
+            result['cur_url'] = self.cur_url
+        if self.position_no is not None:
+            result['position_no'] = self.position_no
+        if self.item_id is not None:
+            result['item_id'] = self.item_id
+        if self.shop_id is not None:
+            result['shop_id'] = self.shop_id
+        if self.pre_url is not None:
+            result['pre_url'] = self.pre_url
+        if self.source is not None:
+            result['source'] = self.source
+        if self.ad_space_level is not None:
+            result['ad_space_level'] = self.ad_space_level
+        if self.group_id is not None:
+            result['group_id'] = self.group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('trace_id') is not None:
+            self.trace_id = m.get('trace_id')
+        if m.get('event_time') is not None:
+            self.event_time = m.get('event_time')
+        if m.get('page_flag') is not None:
+            self.page_flag = m.get('page_flag')
+        if m.get('action_flag') is not None:
+            self.action_flag = m.get('action_flag')
+        if m.get('cur_url') is not None:
+            self.cur_url = m.get('cur_url')
+        if m.get('position_no') is not None:
+            self.position_no = m.get('position_no')
+        if m.get('item_id') is not None:
+            self.item_id = m.get('item_id')
+        if m.get('shop_id') is not None:
+            self.shop_id = m.get('shop_id')
+        if m.get('pre_url') is not None:
+            self.pre_url = m.get('pre_url')
+        if m.get('source') is not None:
+            self.source = m.get('source')
+        if m.get('ad_space_level') is not None:
+            self.ad_space_level = m.get('ad_space_level')
+        if m.get('group_id') is not None:
+            self.group_id = m.get('group_id')
+        return self
+
+
+class UploadTrafficOperatelogResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        upload_result: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 上传结果
+        self.upload_result = upload_result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.upload_result is not None:
+            result['upload_result'] = self.upload_result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('upload_result') is not None:
+            self.upload_result = m.get('upload_result')
+        return self
+
+
```

### Comparing `antchain_twc-1.8.9/antchain_twc.egg-info/PKG-INFO` & `antchain_twc-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-twc
-Version: 1.8.9
+Name: antchain_twc
+Version: 1.9.0
 Summary: Ant Chain TWC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_twc-1.8.9/setup.py` & `antchain_twc-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_twc.
 
-Created on 25/11/2022
+Created on 24/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_twc"
 NAME = "antchain_twc" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain TWC SDK Library for Python"
```

