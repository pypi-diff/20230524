# Comparing `tmp/mailerlite-0.1.2.tar.gz` & `tmp/mailerlite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailerlite-0.1.2.tar", max compression
+gzip compressed data, was "mailerlite-0.1.3.tar", max compression
```

## Comparing `mailerlite-0.1.2.tar` & `mailerlite-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2023-03-31 08:51:43.704030 mailerlite-0.1.2/LICENSE
--rw-r--r--   0        0        0     1256 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/__init__.py
--rw-r--r--   0        0        0     2264 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/api_client.py
--rw-r--r--   0        0        0      436 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/__init__.py
--rw-r--r--   0        0        0     2246 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/automations.py
--rw-r--r--   0        0        0      982 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/batch.py
--rw-r--r--   0        0        0     6076 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/campaigns.py
--rw-r--r--   0        0        0     3595 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/fields.py
--rw-r--r--   0        0        0     4502 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/forms.py
--rw-r--r--   0        0        0     4993 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/groups.py
--rw-r--r--   0        0        0     4150 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/segments.py
--rw-r--r--   0        0        0     9535 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/subscribers.py
--rw-r--r--   0        0        0      518 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/timezones.py
--rw-r--r--   0        0        0     4150 2023-03-31 08:51:43.704030 mailerlite-0.1.2/mailerlite/sdk/webhooks.py
--rw-r--r--   0        0        0      683 2023-03-31 08:51:43.704030 mailerlite-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 mailerlite-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-24 20:05:39.662003 mailerlite-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1256 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/__init__.py
+-rw-r--r--   0        0        0     2802 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/api_client.py
+-rw-r--r--   0        0        0      436 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/__init__.py
+-rw-r--r--   0        0        0     2246 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/automations.py
+-rw-r--r--   0        0        0      982 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/batch.py
+-rw-r--r--   0        0        0     6076 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/campaigns.py
+-rw-r--r--   0        0        0     3595 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/fields.py
+-rw-r--r--   0        0        0     4502 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/forms.py
+-rw-r--r--   0        0        0     5003 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/groups.py
+-rw-r--r--   0        0        0     4150 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/segments.py
+-rw-r--r--   0        0        0    10498 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/subscribers.py
+-rw-r--r--   0        0        0      518 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/timezones.py
+-rw-r--r--   0        0        0     4150 2023-05-24 20:05:39.666003 mailerlite-0.1.3/mailerlite/sdk/webhooks.py
+-rw-r--r--   0        0        0      683 2023-05-24 20:05:39.666003 mailerlite-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 mailerlite-0.1.3/PKG-INFO
```

### Comparing `mailerlite-0.1.2/LICENSE` & `mailerlite-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/mailerlite/__init__.py` & `mailerlite-0.1.3/mailerlite/__init__.py`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/mailerlite/sdk/automations.py` & `mailerlite-0.1.3/mailerlite/sdk/automations.py`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/mailerlite/sdk/batch.py` & `mailerlite-0.1.3/mailerlite/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/mailerlite/sdk/campaigns.py` & `mailerlite-0.1.3/mailerlite/sdk/campaigns.py`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/mailerlite/sdk/fields.py` & `mailerlite-0.1.3/mailerlite/sdk/fields.py`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/mailerlite/sdk/forms.py` & `mailerlite-0.1.3/mailerlite/sdk/forms.py`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/mailerlite/sdk/groups.py` & `mailerlite-0.1.3/mailerlite/sdk/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
         :param **kwargs: You can pass additional arguments - page, limit, sort or to filter by name
         :raises: :class: `TypeError` : Got an unknown argument
         :return: JSON array
         :rtype: dict
         """
 
-        available_params = ["list", "limit", "page", "sort"]
+        available_params = ["list", "limit", "page", "sort", "filter"]
 
         params = locals()
         query_params = {}
         for key, val in params["kwargs"].items():
             if key not in available_params:
                 raise TypeError("Got an unknown argument '%s'" % key)
             if key == "filter":
```

### Comparing `mailerlite-0.1.2/mailerlite/sdk/segments.py` & `mailerlite-0.1.3/mailerlite/sdk/segments.py`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/mailerlite/sdk/subscribers.py` & `mailerlite-0.1.3/mailerlite/sdk/subscribers.py`

 * *Files 4% similar despite different names*

```diff
@@ -274,7 +274,31 @@
         Ref: https://developers.mailerlite.com/docs/subscribers.html#fetch-total-subscribers-count
 
         :return: JSON array
         :rtype: dict
         """
 
         return self.list(limit=0)
+
+    def forget(self, subscriber_id):
+        """
+        Forget a subscriber
+
+        It will removes the subscriber from your account and all information will be completely deleted in 30 days. This feature is GDPR compliant.If you want to forget a subscriber, send this POST request.
+        Ref: https://developers.mailerlite.com/docs/subscribers.html#forget-a-subscriber
+
+        :param subscriber_id: int Susbscriber ID
+        :raises: :class: `TypeError` : `subscriber_id` type is not valid
+        :return: `true` if action was successful, `false` if subscriber was not found
+        :rtype: bool
+        """
+
+        if not isinstance(subscriber_id, int):
+            raise TypeError(
+                f"`subscriber_id` type is not valid. Expected `int`, got {type(subscriber_id)}."
+            )
+
+        response = self.api_client.request(
+            "POST", f"{self.base_api_url}/{subscriber_id}/forget"
+        )
+
+        return response.status_code
```

### Comparing `mailerlite-0.1.2/mailerlite/sdk/timezones.py` & `mailerlite-0.1.3/mailerlite/sdk/timezones.py`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/mailerlite/sdk/webhooks.py` & `mailerlite-0.1.3/mailerlite/sdk/webhooks.py`

 * *Files identical despite different names*

### Comparing `mailerlite-0.1.2/pyproject.toml` & `mailerlite-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 authors = ["MailerLite <tech@mailerlite.com>"]
 description = "The official MailerLite Python SDK"
 name = "mailerlite"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-python-semantic-release = "^7.32.2"
 requests = "^2.28.1"
 
 [tool.poetry.dev-dependencies]
 black = "^22.10.0"
 coverage = "^6.5.0"
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 python-dotenv = "^0.21.0"
+python-semantic-release = "^7.32.2"
 vcrpy = "^4.2.1"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.semantic_release]
```

### Comparing `mailerlite-0.1.2/PKG-INFO` & `mailerlite-0.1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: mailerlite
-Version: 0.1.2
+Version: 0.1.3
 Summary: The official MailerLite Python SDK
 Author: MailerLite
 Author-email: tech@mailerlite.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: python-semantic-release (>=7.32.2,<8.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

