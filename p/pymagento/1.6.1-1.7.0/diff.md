# Comparing `tmp/pymagento-1.6.1.tar.gz` & `tmp/pymagento-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymagento-1.6.1.tar", max compression
+gzip compressed data, was "pymagento-1.7.0.tar", max compression
```

## Comparing `pymagento-1.6.1.tar` & `pymagento-1.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-04-14 13:46:01.789723 pymagento-1.6.1/LICENSE
--rw-r--r--   0        0        0      908 2023-04-14 13:46:01.789723 pymagento-1.6.1/README.md
--rw-r--r--   0        0        0     1189 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/__init__.py
--rw-r--r--   0        0        0     4773 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/attributes.py
--rw-r--r--   0        0        0     3849 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/batches.py
--rw-r--r--   0        0        0    35623 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/client.py
--rw-r--r--   0        0        0     1768 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/exceptions.py
--rw-r--r--   0        0        0      963 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/order_helpers.py
--rw-r--r--   0        0        0        0 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/py.typed
--rw-r--r--   0        0        0     3374 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/queries.py
--rw-r--r--   0        0        0      357 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/types.py
--rw-r--r--   0        0        0       22 2023-04-14 13:46:01.793723 pymagento-1.6.1/magento/version.py
--rw-r--r--   0        0        0     1219 2023-04-14 13:46:01.793723 pymagento-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 pymagento-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-24 14:40:28.566347 pymagento-1.7.0/LICENSE
+-rw-r--r--   0        0        0      908 2023-05-24 14:40:28.566347 pymagento-1.7.0/README.md
+-rw-r--r--   0        0        0     1189 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/__init__.py
+-rw-r--r--   0        0        0     4773 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/attributes.py
+-rw-r--r--   0        0        0     3849 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/batches.py
+-rw-r--r--   0        0        0    35332 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/client.py
+-rw-r--r--   0        0        0     1768 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/exceptions.py
+-rw-r--r--   0        0        0      963 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/order_helpers.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/py.typed
+-rw-r--r--   0        0        0     3374 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/queries.py
+-rw-r--r--   0        0        0      357 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/types.py
+-rw-r--r--   0        0        0       22 2023-05-24 14:40:28.566347 pymagento-1.7.0/magento/version.py
+-rw-r--r--   0        0        0     1219 2023-05-24 14:40:28.566347 pymagento-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pymagento-1.7.0/PKG-INFO
```

### Comparing `pymagento-1.6.1/LICENSE` & `pymagento-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.1/README.md` & `pymagento-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.1/magento/__init__.py` & `pymagento-1.7.0/magento/__init__.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.1/magento/attributes.py` & `pymagento-1.7.0/magento/attributes.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.1/magento/batches.py` & `pymagento-1.7.0/magento/batches.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.1/magento/client.py` & `pymagento-1.7.0/magento/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,43 +92,41 @@
     def __init__(self,
                  token: Optional[str] = None,
                  base_url: Optional[str] = None,
                  scope: Optional[str] = None,
                  logger: Optional[Logger] = None,
                  read_only=False,
                  user_agent=None,
-                 verbose=False):
+                 **kwargs):
         """
         Create a Magento client instance. All arguments are optional and fall back on environment variables named
         ``PYMAGENTO_ + argument.upper()`` (``PYMAGENTO_TOKEN``, ``PYMAGENTO_BASE_URL``, etc).
         The ``token`` and ``base_url`` **must** be given either as arguments or environment variables.
 
         :param token: API integration token
         :param base_url: base URL of the Magento instance
         :param scope: API scope
         :param logger: optional logger.
-        :param verbose: if True, log the progress of get_paginated. This has no effect if logger is not set.
         :param read_only: if True,
         :param user_agent: User-Agent
         """
         token = token or environ.get("PYMAGENTO_TOKEN")
         base_url = base_url or environ.get("PYMAGENTO_BASE_URL")
         scope = scope or environ.get("PYMAGENTO_SCOPE") or DEFAULT_SCOPE
         user_agent = user_agent or environ.get("PYMAGENTO_USER_AGENT") or USER_AGENT
 
         if token is None:
             raise RuntimeError("Missing API token")
         if base_url is None:
             raise RuntimeError("Missing API base URL")
 
-        super().__init__(base_url=base_url, user_agent=user_agent, read_only=read_only)
+        super().__init__(base_url=base_url, user_agent=user_agent, read_only=read_only, **kwargs)
 
         self.scope = scope
         self.logger = logger
-        self.verbose = verbose if logger else False
         self.headers['Authorization'] = f"Bearer {token}"
 
     # Attributes
     # ==========
 
     def save_attribute(self, attribute: MagentoEntity, *, with_defaults=True, throw=True, **kwargs) -> MagentoEntity:
         if with_defaults:
@@ -557,31 +555,30 @@
 
     def save_product_media(self, sku: Sku, media_entry: MediaEntry):
         return self.post_api(f'/V1/products/{sku}/media', json={"entry": media_entry}, throw=True).json()
 
     def delete_product_media(self, sku: Sku, media_id: PathId, throw=False):
         return self.delete_api(f'/V1/products/{sku}/media/{media_id}', throw=throw)
 
-    def save_product(self, product, *, log_response=False, save_options: Optional[bool] = None) -> Product:
+    def save_product(self, product, *, save_options: Optional[bool] = None) -> Product:
         """
         Save a product.
 
         :param product: (partial) product to save.
-        :param log_response: if True and ``self.logger`` is set, log the response.
         :param save_options: set the `saveOptions` attribute.
         :return:
         """
         payload: JSONDict = {"product": product}
         if save_options is not None:
             payload["saveOptions"] = save_options
 
         # throw=False so the log is printed before we raise
         resp = self.post_api('/V1/products', json=payload, throw=False)
-        if log_response and self.logger:
-            self.logger.info("Save product response: %s", resp.text)
+        if self.logger:
+            self.logger.debug("Save product response: %s", resp.text)
         raise_for_response(resp)
         return cast(Product, resp.json())
 
     def update_product(self, sku: Sku, product: Product, *, save_options: Optional[bool] = None) -> Product:
         """
         Update a product.
 
@@ -938,16 +935,16 @@
             items = res.get('items', [])
             if not items:
                 break
 
             total_count = res["total_count"]
 
             for item in items:
-                if self.verbose and self.logger and count and count % 1000 == 0:
-                    self.logger.info(f'loaded {count} items')
+                if self.logger and count and count % 1000 == 0:
+                    self.logger.debug(f'loaded {count} items')
                 yield item
                 count += 1
                 if count >= total_count:
                     return
 
                 if is_limited and count >= limit:
                     return
```

### Comparing `pymagento-1.6.1/magento/exceptions.py` & `pymagento-1.7.0/magento/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.1/magento/order_helpers.py` & `pymagento-1.7.0/magento/order_helpers.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.1/magento/queries.py` & `pymagento-1.7.0/magento/queries.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.6.1/pyproject.toml` & `pymagento-1.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymagento"
-version = "1.6.1"
+version = "1.7.0"
 description = "Python client for the Magento 2 API"
 authors = ["Bixoto <tech@bixoto.com>"]
 license = "MIT"
 homepage = "https://github.com/Bixoto/PyMagento"
 include = ["magento/py.typed"]
 readme = "README.md"
 packages = [
```

### Comparing `pymagento-1.6.1/PKG-INFO` & `pymagento-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pymagento
-Version: 1.6.1
+Version: 1.7.0
 Summary: Python client for the Magento 2 API
 Home-page: https://github.com/Bixoto/PyMagento
 License: MIT
 Author: Bixoto
 Author-email: tech@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=4.4.0,<5.0.0) ; extra == "docs"
 Requires-Dist: api-session (>=1.3.2,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
 Description-Content-Type: text/markdown
 
 # PyMagento
```

