# Comparing `tmp/kr8s-0.3.0.tar.gz` & `tmp/kr8s-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.3.0.tar", max compression
+gzip compressed data, was "kr8s-0.4.0.tar", max compression
```

## Comparing `kr8s-0.3.0.tar` & `kr8s-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1549 2023-03-23 14:43:10.894081 kr8s-0.3.0/LICENSE
--rw-r--r--   0        0        0     2113 2023-04-24 13:00:16.267776 kr8s-0.3.0/README.md
--rw-r--r--   0        0        0      488 2023-05-05 14:21:46.010648 kr8s-0.3.0/kr8s/__init__.py
--rw-r--r--   0        0        0    10163 2023-05-05 12:16:31.343064 kr8s-0.3.0/kr8s/_api.py
--rw-r--r--   0        0        0     4650 2023-05-05 14:21:31.262579 kr8s-0.3.0/kr8s/_asyncio.py
--rw-r--r--   0        0        0     5260 2023-04-27 16:24:20.588740 kr8s-0.3.0/kr8s/_auth.py
--rw-r--r--   0        0        0      361 2023-04-04 19:30:47.872877 kr8s-0.3.0/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-04-27 12:49:41.923098 kr8s-0.3.0/kr8s/_exceptions.py
--rw-r--r--   0        0        0    23828 2023-05-05 12:16:31.343064 kr8s-0.3.0/kr8s/_objects.py
--rw-r--r--   0        0        0     7500 2023-04-30 18:57:48.474523 kr8s-0.3.0/kr8s/_portforward.py
--rw-r--r--   0        0        0      672 2023-04-03 16:55:51.155586 kr8s-0.3.0/kr8s/_testutils.py
--rw-r--r--   0        0        0      886 2023-04-30 18:57:48.474523 kr8s-0.3.0/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0      658 2023-05-05 12:16:31.343064 kr8s-0.3.0/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0       50 2023-04-30 18:57:48.474523 kr8s-0.3.0/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5575 2023-04-30 18:57:48.474523 kr8s-0.3.0/kr8s/conftest.py
--rw-r--r--   0        0        0     5739 2023-05-05 12:16:31.343064 kr8s-0.3.0/kr8s/objects.py
--rw-r--r--   0        0        0      157 2023-04-30 18:57:48.478523 kr8s-0.3.0/kr8s/portforward.py
--rw-r--r--   0        0        0       61 2023-03-31 20:28:17.436142 kr8s-0.3.0/kr8s/tests/resources/serviceaccount.yaml
--rwxr-xr-x   0        0        0      614 2023-04-03 16:55:51.155586 kr8s-0.3.0/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     3963 2023-05-05 14:21:31.262579 kr8s-0.3.0/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3130 2023-04-30 18:57:48.478523 kr8s-0.3.0/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      300 2023-04-04 19:30:47.872877 kr8s-0.3.0/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0    11641 2023-04-30 18:57:48.478523 kr8s-0.3.0/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-04-03 16:55:51.155586 kr8s-0.3.0/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2504 2023-05-05 14:21:46.010648 kr8s-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 kr8s-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-03-23 14:43:10.894081 kr8s-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2113 2023-04-24 13:00:16.267776 kr8s-0.4.0/README.md
+-rw-r--r--   0        0        0      551 2023-05-10 14:32:13.762405 kr8s-0.4.0/kr8s/__init__.py
+-rw-r--r--   0        0        0    10418 2023-05-10 09:14:38.833344 kr8s-0.4.0/kr8s/_api.py
+-rw-r--r--   0        0        0     5208 2023-05-10 09:14:38.833344 kr8s-0.4.0/kr8s/_asyncio.py
+-rw-r--r--   0        0        0     5830 2023-05-10 09:14:38.833344 kr8s-0.4.0/kr8s/_auth.py
+-rw-r--r--   0        0        0      361 2023-04-04 19:30:47.872877 kr8s-0.4.0/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-04-27 12:49:41.923098 kr8s-0.4.0/kr8s/_exceptions.py
+-rw-r--r--   0        0        0    24124 2023-05-10 09:14:38.833344 kr8s-0.4.0/kr8s/_objects.py
+-rw-r--r--   0        0        0     7500 2023-04-30 18:57:48.474523 kr8s-0.4.0/kr8s/_portforward.py
+-rw-r--r--   0        0        0      672 2023-04-03 16:55:51.155586 kr8s-0.4.0/kr8s/_testutils.py
+-rw-r--r--   0        0        0       30 2023-05-10 09:14:38.833344 kr8s-0.4.0/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0      916 2023-05-10 09:14:38.833344 kr8s-0.4.0/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0      658 2023-05-05 12:16:31.343064 kr8s-0.4.0/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0       50 2023-04-30 18:57:48.474523 kr8s-0.4.0/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5575 2023-04-30 18:57:48.474523 kr8s-0.4.0/kr8s/conftest.py
+-rw-r--r--   0        0        0     5739 2023-05-05 12:16:31.343064 kr8s-0.4.0/kr8s/objects.py
+-rw-r--r--   0        0        0      157 2023-04-30 18:57:48.478523 kr8s-0.4.0/kr8s/portforward.py
+-rw-r--r--   0        0        0       61 2023-03-31 20:28:17.436142 kr8s-0.4.0/kr8s/tests/resources/serviceaccount.yaml
+-rwxr-xr-x   0        0        0      614 2023-04-03 16:55:51.155586 kr8s-0.4.0/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     4133 2023-05-10 09:14:38.833344 kr8s-0.4.0/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3144 2023-05-10 09:14:38.833344 kr8s-0.4.0/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      300 2023-04-04 19:30:47.872877 kr8s-0.4.0/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0    11749 2023-05-10 09:14:38.833344 kr8s-0.4.0/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-04-03 16:55:51.155586 kr8s-0.4.0/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2525 2023-05-10 14:32:13.762405 kr8s-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 kr8s-0.4.0/PKG-INFO
```

### Comparing `kr8s-0.3.0/LICENSE` & `kr8s-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.3.0/README.md` & `kr8s-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.3.0/kr8s/_api.py` & `kr8s-0.4.0/kr8s/_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,21 @@
             url=self._url,
             kubeconfig=self._kubeconfig,
             serviceaccount=self._serviceaccount,
             namespace=kwargs.get("namespace"),
         )
         Api._instances[frozenset(kwargs.items())] = self
 
+    def __await__(self):
+        async def f():
+            await self.auth
+            return self
+
+        return f().__await__()
+
     async def _create_session(self):
         headers = {"User-Agent": self.__version__, "content-type": "application/json"}
         self._sslcontext = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
         if self.auth.client_key_file:
             self._sslcontext.load_cert_chain(
                 certfile=self.auth.client_cert_file,
                 keyfile=self.auth.client_key_file,
@@ -121,20 +128,24 @@
         while True:
             try:
                 async with call_method(**kwargs) as response:
                     yield response
             except aiohttp.ClientResponseError as e:
                 if e.status in (401, 403) and auth_attempts < 3:
                     auth_attempts += 1
-                    self.auth.reauthenticate()
+                    await self.auth.reauthenticate()
                     continue
                 else:
                     raise
             break
 
+    async def reauthenticate(self):
+        """Reauthenticate the API."""
+        await self.auth.reauthenticate()
+
     @contextlib.asynccontextmanager
     async def _get_kind(
         self,
         kind: str,
         namespace: str = None,
         label_selector: str = None,
         field_selector: str = None,
```

### Comparing `kr8s-0.3.0/kr8s/_asyncio.py` & `kr8s-0.4.0/kr8s/_asyncio.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Jupyter Development Team., MrNaif2018, Dask Developers, NVIDIA
 # SPDX-License-Identifier: MIT License, BSD 3-Clause License
 #
-# This file is a fork of universalasync (commit d397911) and jupyter-core (commit 98b9a1a).
+# This file contains a fork of universalasync (commit d397911) and jupyter-core (commit 98b9a1a).
 # Both projects attempt to solve the same problem: how to run nested asyncio tasks.
 # Neither solution quite fit in here, so we forked them and combined them.
 #
 # universalasync License: https://github.com/bitcartcc/universalasync/blob/d397911/LICENSE
 # jupyter-core License: https://github.com/jupyter/jupyter_core/blob/98b9a1a/COPYING.md
 #
 # This implementation uses the _TaskRunner from jupyter-core, but with a modified version of the wraps
 # decorator from universalasync.
 
 import asyncio
 import atexit
 import inspect
 import threading
+from functools import wraps
 from typing import (
     Any,
     AsyncGenerator,
     Awaitable,
     Callable,
     Generator,
     Optional,
@@ -77,14 +78,15 @@
 
     Returns
     -------
     result :
         Whatever the coroutine-function returns.
     """
 
+    @wraps(coro)
     def wrapped(*args, **kwargs):
         name = threading.current_thread().name
         inner = coro(*args, **kwargs)
         try:
             # If a loop is currently running use a task runner to
             # run in a new loop in a separate thread.
             asyncio.get_running_loop()
@@ -146,7 +148,24 @@
         elif name == "__aenter__" and not hasattr(source, "__enter__"):
             setattr(source, "__enter__", run_sync(method))
 
         elif name == "__aexit__" and not hasattr(source, "__exit__"):
             setattr(source, "__exit__", run_sync(method))
 
     return source
+
+
+async def check_output(*args, **kwargs):
+    """Run a command and return its output."""
+    p = await asyncio.create_subprocess_exec(
+        *args,
+        stdout=asyncio.subprocess.PIPE,
+        stderr=asyncio.subprocess.PIPE,
+        **kwargs,
+    )
+    stdout_data, stderr_data = await p.communicate()
+    if p.returncode == 0:
+        return stdout_data.decode()
+    else:
+        raise RuntimeError(
+            f"Process exited with non-zero code {p.returncode}:\n{stderr_data.decode()}"
+        )
```

### Comparing `kr8s-0.3.0/kr8s/_objects.py` & `kr8s-0.4.0/kr8s/_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,25 @@
     scalable_spec = "replicas"
     _asyncio = True
 
     def __init__(self, resource: dict, api: Api = None) -> None:
         """Initialize an APIObject."""
         # TODO support passing pykube or kubernetes objects in addition to dicts
         self._raw = resource
-        self.api = api or (kr8s.asyncio.api() if self._asyncio else kr8s.api())
+        self.api = api
+        if self.api is None and not self._asyncio:
+            self.api = kr8s.api()
+
+    def __await__(self):
+        async def f():
+            if self.api is None:
+                self.api = await kr8s.asyncio.api()
+            return self
+
+        return f().__await__()
 
     def __repr__(self):
         """Return a string representation of the Kubernetes resource."""
         return f"<{self.kind} {self.name}>"
 
     def __str__(self):
         """Return a string representation of the Kubernetes resource."""
@@ -101,15 +111,20 @@
 
     @classmethod
     async def get(
         cls, name: str, namespace: str = None, api: Api = None, **kwargs
     ) -> "APIObject":
         """Get a Kubernetes resource by name."""
 
-        api = api or (kr8s.asyncio.api() if cls._asyncio else kr8s.api())
+        if api is None:
+            if cls._asyncio:
+                api = await kr8s.asyncio.api()
+            else:
+                api = kr8s.api()
+
         try:
             resources = await api._get(
                 cls.endpoint, name, namespace=namespace, **kwargs
             )
             [resource] = resources
         except ValueError:
             raise ValueError(
```

### Comparing `kr8s-0.3.0/kr8s/_portforward.py` & `kr8s-0.4.0/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.3.0/kr8s/_testutils.py` & `kr8s-0.4.0/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.3.0/kr8s/asyncio/objects.py` & `kr8s-0.4.0/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.3.0/kr8s/conftest.py` & `kr8s-0.4.0/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.3.0/kr8s/objects.py` & `kr8s-0.4.0/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.3.0/kr8s/tests/scripts/envexec.py` & `kr8s-0.4.0/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.3.0/kr8s/tests/test_api.py` & `kr8s-0.4.0/kr8s/tests/test_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,43 +14,43 @@
         _ = kr8s.Api()
     assert not kr8s.Api._instances
     _ = kr8s.api()
     assert kr8s.Api._instances
 
 
 async def test_api_factory(serviceaccount):
-    k1 = kr8s.api()
-    k2 = kr8s.api()
+    k1 = await kr8s.asyncio.api()
+    k2 = await kr8s.asyncio.api()
     assert k1 is k2
 
-    k3 = kr8s.api(serviceaccount=serviceaccount)
-    k4 = kr8s.api(serviceaccount=serviceaccount)
+    k3 = await kr8s.asyncio.api(serviceaccount=serviceaccount)
+    k4 = await kr8s.asyncio.api(serviceaccount=serviceaccount)
     assert k1 is not k3
     assert k3 is k4
 
-    p = Pod({})
+    p = await Pod({})
     assert p.api is k1
     assert p.api is not k3
 
 
 async def test_api_factory_with_kubeconfig(k8s_cluster, serviceaccount):
-    k1 = kr8s.api(kubeconfig=k8s_cluster.kubeconfig_path)
-    k2 = kr8s.api(serviceaccount=serviceaccount)
-    k3 = kr8s.api()
+    k1 = await kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
+    k2 = await kr8s.asyncio.api(serviceaccount=serviceaccount)
+    k3 = await kr8s.asyncio.api()
     assert k1 is not k2
     assert k3 is k1
     assert k3 is not k2
 
-    p = Pod({})
+    p = await Pod({})
     assert p.api is k1
 
-    p2 = Pod({}, api=k2)
+    p2 = await Pod({}, api=k2)
     assert p2.api is k2
 
-    p3 = Pod({}, api=k3)
+    p3 = await Pod({}, api=k3)
     assert p3.api is k3
     assert p3.api is not k2
 
 
 def test_version_sync():
     kubernetes = kr8s.api()
     version = kubernetes.version()
@@ -60,45 +60,45 @@
 async def test_version_sync_in_async():
     kubernetes = kr8s.api()
     version = kubernetes.version()
     assert "major" in version
 
 
 async def test_version():
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     version = await kubernetes.version()
     assert "major" in version
 
 
 async def test_bad_api_version():
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     with pytest.raises(ValueError):
         async with kubernetes.call_api("GET", version="foo"):
             pass  # pragma: no cover
 
 
 @pytest.mark.parametrize("namespace", [kr8s.ALL, "kube-system"])
 async def test_get_pods(namespace):
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     pods = await kubernetes.get("pods", namespace=namespace)
     assert isinstance(pods, list)
     assert len(pods) > 0
     assert isinstance(pods[0], Pod)
 
 
 async def test_get_pods_as_table():
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     pods = await kubernetes.get("pods", namespace="kube-system", as_object=Table)
     assert isinstance(pods, Table)
     assert len(pods.rows) > 0
 
 
 async def test_watch_pods(example_pod_spec):
-    kubernetes = kr8s.asyncio.api()
-    pod = Pod(example_pod_spec)
+    kubernetes = await kr8s.asyncio.api()
+    pod = await Pod(example_pod_spec)
     await pod.create()
     while not await pod.ready():
         await asyncio.sleep(0.1)
     async for event, obj in kubernetes.watch("pods"):
         assert event in ["ADDED", "MODIFIED", "DELETED"]
         assert isinstance(obj, Pod)
         if obj.name == pod.name:
@@ -109,21 +109,21 @@
                 while await obj.exists():
                     await asyncio.sleep(0.1)
             elif event == "DELETED":
                 break
 
 
 async def test_get_deployments():
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     deployments = await kubernetes.get("deployments")
     assert isinstance(deployments, list)
 
 
 async def test_api_resources():
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     resources = await kubernetes.api_resources()
 
     names = [r["name"] for r in resources]
     assert "nodes" in names
     assert "pods" in names
     assert "services" in names
     assert "namespaces" in names
```

### Comparing `kr8s-0.3.0/kr8s/tests/test_auth.py` & `kr8s-0.4.0/kr8s/tests/test_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,65 +35,65 @@
         with tempfile.NamedTemporaryFile() as f:
             f.write(yaml.safe_dump(kubeconfig).encode())
             f.flush()
             yield f.name
 
 
 async def test_kubeconfig(k8s_cluster):
-    kubernetes = kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
+    kubernetes = await kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
     version = await kubernetes.version()
     assert "major" in version
 
 
 async def test_reauthenticate(k8s_cluster):
-    kubernetes = kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
-    kubernetes.auth.reauthenticate()
+    kubernetes = await kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
+    await kubernetes.reauthenticate()
     version = await kubernetes.version()
     assert "major" in version
 
 
 def test_reauthenticate_sync(k8s_cluster):
-    kubernetes = kr8s.api(kubeconfig=k8s_cluster.kubeconfig_path)
-    kubernetes.auth.reauthenticate()
-    version = kubernetes.version()
+    client = kr8s.api(kubeconfig=k8s_cluster.kubeconfig_path)
+    client.reauthenticate()
+    version = client.version()
     assert "major" in version
 
 
 async def test_bad_auth(serviceaccount):
     (Path(serviceaccount) / "token").write_text("abc123")
-    kubernetes = kr8s.asyncio.api(
+    kubernetes = await kr8s.asyncio.api(
         serviceaccount=serviceaccount, kubeconfig="/no/file/here"
     )
     serviceaccount = Path(serviceaccount)
     with pytest.raises(aiohttp.ClientResponseError):
         await kubernetes.version()
 
 
 async def test_url(kubectl_proxy):
-    kubernetes = kr8s.asyncio.api(url=kubectl_proxy)
+    kubernetes = await kr8s.asyncio.api(url=kubectl_proxy)
     version = await kubernetes.version()
     assert "major" in version
 
 
-async def test_no_config():
+def test_no_config():
     with pytest.raises(ValueError):
         kr8s.api(kubeconfig="/no/file/here")
 
 
 async def test_service_account(serviceaccount):
-    kubernetes = kr8s.asyncio.api(
+    kubernetes = await kr8s.asyncio.api(
         serviceaccount=serviceaccount, kubeconfig="/no/file/here"
     )
     await kubernetes.version()
 
     serviceaccount = Path(serviceaccount)
     assert kubernetes.auth.server
     assert kubernetes.auth.token == (serviceaccount / "token").read_text()
     assert str(serviceaccount) in kubernetes.auth.server_ca_file
     assert "BEGIN CERTIFICATE" in Path(kubernetes.auth.server_ca_file).read_text()
     assert kubernetes.auth.namespace == (serviceaccount / "namespace").read_text()
 
 
 async def test_exec(kubeconfig_with_exec):
-    kubernetes = kr8s.asyncio.api(kubeconfig=kubeconfig_with_exec)
+    kubernetes = await kr8s.asyncio.api(kubeconfig=kubeconfig_with_exec)
     version = await kubernetes.version()
     assert "major" in version
```

### Comparing `kr8s-0.3.0/kr8s/tests/test_objects.py` & `kr8s-0.4.0/kr8s/tests/test_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "httpGet": {"path": "/", "port": 80},
         "initialDelaySeconds": 0,
         "periodSeconds": 1,
         "timeoutSeconds": 1,
         "successThreshold": 2,
     }
     example_pod_spec["metadata"]["labels"]["app"] = example_pod_spec["metadata"]["name"]
-    pod = Pod(example_pod_spec)
+    pod = await Pod(example_pod_spec)
     await pod.create()
     while not await pod.ready():
         await asyncio.sleep(0.1)
     # TODO replace with pod.exec() once implemented
     k8s_cluster.kubectl(
         "exec",
         example_pod_spec["metadata"]["name"],
@@ -55,24 +55,24 @@
     await pod.delete()
 
 
 @pytest.fixture
 async def nginx_service(example_service_spec, nginx_pod):
     example_service_spec["metadata"]["name"] = nginx_pod.name
     example_service_spec["spec"]["selector"] = nginx_pod.labels
-    service = Service(example_service_spec)
+    service = await Service(example_service_spec)
     await service.create()
     while not await service.ready():
         await asyncio.sleep(0.1)  # pragma: no cover
     yield service
     await service.delete()
 
 
 async def test_pod_create_and_delete(example_pod_spec):
-    pod = Pod(example_pod_spec)
+    pod = await Pod(example_pod_spec)
     await pod.create()
     with pytest.raises(NotImplementedError):
         pod.replicas
     assert await pod.exists()
     while not await pod.ready():
         await asyncio.sleep(0.1)
     await pod.delete()
@@ -92,24 +92,24 @@
     pod.delete()
     while pod.exists():
         time.sleep(0.1)
     assert not pod.exists()
 
 
 async def test_list_and_ensure():
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     pods = await kubernetes.get("pods", namespace=kr8s.ALL)
     assert len(pods) > 0
     for pod in pods:
         await pod.refresh()
         assert await pod.exists(ensure=True)
 
 
 async def test_nonexistant():
-    pod = Pod(
+    pod = await Pod(
         {
             "apiVersion": "v1",
             "kind": "Pod",
             "metadata": {
                 "name": "nonexistant",
                 "namespace": "nonexistant",
             },
@@ -117,55 +117,55 @@
     )
     assert not await pod.exists()
     with pytest.raises(kr8s.NotFoundError):
         await pod.exists(ensure=True)
 
 
 async def test_pod_metadata(example_pod_spec):
-    pod = Pod(example_pod_spec)
+    pod = await Pod(example_pod_spec)
     await pod.create()
     assert "name" in pod.metadata
     assert "hello" in pod.labels
     assert "foo" in pod.annotations
     assert "default" == pod.namespace
     assert "example-" in pod.name
     assert "containers" in pod.spec
     assert "phase" in pod.status
     await pod.delete()
 
 
 async def test_pod_missing_labels_annotations(example_pod_spec):
     del example_pod_spec["metadata"]["labels"]
     del example_pod_spec["metadata"]["annotations"]
-    pod = Pod(example_pod_spec)
+    pod = await Pod(example_pod_spec)
     await pod.create()
     assert not pod.labels
     assert not pod.annotations
     await pod.delete()
 
 
 async def test_pod_get(example_pod_spec):
-    pod = Pod(example_pod_spec)
+    pod = await Pod(example_pod_spec)
     await pod.create()
     pod2 = await Pod.get(pod.name, namespace=pod.namespace)
     assert pod2.name == pod.name
     assert pod2.namespace == pod.namespace
     await pod.delete()
     while await pod.exists():
         await asyncio.sleep(0.1)
     with pytest.raises(kr8s.NotFoundError):
         await pod2.delete()
 
 
 async def test_selectors(example_pod_spec):
     example_pod_spec["metadata"]["labels"]["abc"] = "123def"
-    pod = Pod(example_pod_spec)
+    pod = await Pod(example_pod_spec)
     await pod.create()
 
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     pods = await kubernetes.get("pods", namespace=kr8s.ALL, label_selector="abc=123def")
     assert len(pods) == 1
 
     pods = await kubernetes.get(
         "pods", namespace=kr8s.ALL, field_selector="metadata.name=" + pod.name
     )
     assert len(pods) == 1
@@ -175,15 +175,15 @@
     )
     assert len(pods) == 0
 
     await pod.delete()
 
 
 async def test_pod_watch(example_pod_spec):
-    pod = Pod(example_pod_spec)
+    pod = await Pod(example_pod_spec)
     await pod.create()
     async for event, obj in pod.watch():
         assert event in ("ADDED", "MODIFIED", "DELETED")
         assert obj.name == pod.name
         break
     await pod.delete()
 
@@ -195,24 +195,24 @@
         assert event in ("ADDED", "MODIFIED", "DELETED")
         assert obj.name == pod.name
         break
     pod.delete()
 
 
 async def test_patch_pod(example_pod_spec):
-    pod = Pod(example_pod_spec)
+    pod = await Pod(example_pod_spec)
     await pod.create()
     assert "patched" not in pod.labels
     await pod.patch({"metadata": {"labels": {"patched": "true"}}})
     assert "patched" in pod.labels
     await pod.delete()
 
 
 async def test_all_v1_objects_represented():
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     objects = await kubernetes.api_resources()
     supported_apis = (
         "v1",
         "apps/v1",
         "autoscaling/v2",
         "batch/v1",
         "networking.k8s.io/v1",
@@ -251,47 +251,47 @@
         singular = "myresource"
         namespaced = True
 
     get_class("MyResource", "foo.kr8s.org/v1alpha1")
 
 
 async def test_deployment_scale(example_deployment_spec):
-    deployment = Deployment(example_deployment_spec)
+    deployment = await Deployment(example_deployment_spec)
     await deployment.create()
     assert deployment.replicas == 1
     await deployment.scale(2)
     assert deployment.replicas == 2
     while not await deployment.ready():
         await asyncio.sleep(0.1)
     await deployment.scale(1)
     assert deployment.replicas == 1
     await deployment.delete()
 
 
 async def test_node():
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     nodes = await kubernetes.get("nodes")
     assert len(nodes) > 0
     for node in nodes:
         assert node.unschedulable is False
         await node.cordon()
         assert node.unschedulable is True
         await node.uncordon()
 
 
 async def test_service_proxy():
-    kubernetes = kr8s.asyncio.api()
+    kubernetes = await kr8s.asyncio.api()
     [service] = await kubernetes.get("services", "kubernetes")
     assert service.name == "kubernetes"
     data = await service.proxy_http_get("/version", raise_for_status=False)
     assert isinstance(data, aiohttp.ClientResponse)
 
 
 async def test_pod_logs(example_pod_spec):
-    pod = Pod(example_pod_spec)
+    pod = await Pod(example_pod_spec)
     await pod.create()
     while not await pod.ready():
         await asyncio.sleep(0.1)
     log = await pod.logs(container="pause")
     assert isinstance(log, str)
     await pod.delete()
 
@@ -358,12 +358,12 @@
         async with session.get(f"http://localhost:{port}/foo") as resp:
             assert resp.status == 404
     await pf.stop()
     assert pf._bg_task is None
 
 
 async def test_unsupported_port_forward():
-    pv = PersistentVolume({})
+    pv = await PersistentVolume({})
     with pytest.raises(AttributeError):
         await pv.portforward(80)
     with pytest.raises(ValueError):
         await PortForward(pv, 80).start()
```

### Comparing `kr8s-0.3.0/kr8s/tests/test_testutils.py` & `kr8s-0.4.0/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.3.0/pyproject.toml` & `kr8s-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.3.0"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.4.0"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = false
@@ -33,14 +33,15 @@
 files = ["kr8s/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.8.4"
 pyyaml = "^6.0"
 asyncio-atexit = "^1.0.1"
+aiofiles = "^23.1.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
 pytest-kind = {git = "https://codeberg.org/hjacobs/pytest-kind.git"}
 pytest-timeout = "^2.1.0"
```

### Comparing `kr8s-0.3.0/PKG-INFO` & `kr8s-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asyncio-atexit (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 <div style="text-align: center; width: 100%;"><img src="branding/logo-wide.png" style="max-height: 200px;" /></div>
```

