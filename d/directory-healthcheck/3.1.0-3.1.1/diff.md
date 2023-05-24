# Comparing `tmp/directory_healthcheck-3.1.0-py3-none-any.whl.zip` & `tmp/directory_healthcheck-3.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5609 bytes, number of entries: 10
--rw-r--r--  2.0 unx       68 b- defN 23-May-17 10:36 directory_healthcheck/__init__.py
--rw-r--r--  2.0 unx      324 b- defN 23-May-17 10:36 directory_healthcheck/apps.py
--rw-r--r--  2.0 unx     2244 b- defN 23-May-17 10:36 directory_healthcheck/backends.py
--rw-r--r--  2.0 unx     1087 b- defN 23-May-17 10:36 directory_healthcheck/views.py
--rw-r--r--  2.0 unx      339 b- defN 23-May-17 10:36 directory_healthcheck/templates/directory_healthcheck/healthcheck.html
--rw-r--r--  2.0 unx     1091 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4074 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      932 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/RECORD
-10 files, 10273 bytes uncompressed, 3979 bytes compressed:  61.3%
+Zip file size: 5620 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       68 b- defN 23-May-24 14:05 directory_healthcheck/__init__.py
+-rw-r--r--  2.0 unx      324 b- defN 23-May-24 14:05 directory_healthcheck/apps.py
+-rw-r--r--  2.0 unx     2244 b- defN 23-May-24 14:05 directory_healthcheck/backends.py
+-rw-r--r--  2.0 unx     1176 b- defN 23-May-24 14:05 directory_healthcheck/views.py
+-rw-r--r--  2.0 unx      339 b- defN 23-May-24 14:05 directory_healthcheck/templates/directory_healthcheck/healthcheck.html
+-rw-r--r--  2.0 unx     1091 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4074 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      932 b- defN 23-May-24 14:06 directory_healthcheck-3.1.1.dist-info/RECORD
+10 files, 10362 bytes uncompressed, 3990 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: directory_healthcheck/views.py
 Comment: 
 
 Filename: directory_healthcheck/templates/directory_healthcheck/healthcheck.html
 Comment: 
 
-Filename: directory_healthcheck-3.1.0.dist-info/LICENSE
+Filename: directory_healthcheck-3.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: directory_healthcheck-3.1.0.dist-info/METADATA
+Filename: directory_healthcheck-3.1.1.dist-info/METADATA
 Comment: 
 
-Filename: directory_healthcheck-3.1.0.dist-info/WHEEL
+Filename: directory_healthcheck-3.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: directory_healthcheck-3.1.0.dist-info/top_level.txt
+Filename: directory_healthcheck-3.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_healthcheck-3.1.0.dist-info/RECORD
+Filename: directory_healthcheck-3.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## directory_healthcheck/views.py

```diff
@@ -1,35 +1,36 @@
 from django.conf import settings
 from django.http import HttpResponse, HttpResponseForbidden
 from django.utils.crypto import constant_time_compare
 from django.views import View
+from django.utils.decorators import method_decorator
 from django.views.decorators.cache import never_cache
 
 import health_check.views
 
 
 class HealthcheckView(health_check.views.MainView):
     template_name = 'directory_healthcheck/healthcheck.html'
 
     def has_permission(self):
         return constant_time_compare(
             self.request.GET.get('token'),
             settings.DIRECTORY_HEALTHCHECK_TOKEN
         )
 
-    @never_cache
+    @method_decorator(never_cache)
     def get(self, *args, **kwargs):
         if not self.has_permission():
             return HttpResponseForbidden()
         return super().get(*args, **kwargs)
 
     def render_to_response(self, context, status):
         context['errored_plugins'] = [
             plugin for plugin in context['plugins'] if plugin.errors
         ]
         return super().render_to_response(context=context, status=status)
 
 
 class PingView(View):
-    @never_cache
+    @method_decorator(never_cache)
     def get(self, request, *args, **kwargs):
         return HttpResponse('OK')
```

## Comparing `directory_healthcheck-3.1.0.dist-info/LICENSE` & `directory_healthcheck-3.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_healthcheck-3.1.0.dist-info/METADATA` & `directory_healthcheck-3.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory-healthcheck
-Version: 3.1.0
+Version: 3.1.1
 Summary: Library to streamline healthchecks for Directory apps.
 Home-page: https://github.com/uktrade/directory-healthcheck
 Author: Department for International Trade
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

## Comparing `directory_healthcheck-3.1.0.dist-info/RECORD` & `directory_healthcheck-3.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 directory_healthcheck/__init__.py,sha256=MzxjIY-3JI1bs39tYXgNHjZdG8srfCVhLqfzp4nHh_U,68
 directory_healthcheck/apps.py,sha256=0YlRHNWpSolt1BeQ7kWG1IFauQ54GH-694hg26sQ4Bw,324
 directory_healthcheck/backends.py,sha256=-UOn5GJsRcuBAuqEWfPRnKpKIygqoDiEg68FvzIY0-Q,2244
-directory_healthcheck/views.py,sha256=GM69IDljqvY8S4IZntiXxL1u38NUjkmS72e-SGKlaHQ,1087
+directory_healthcheck/views.py,sha256=Lz2XsOm2698urVIJuCi7rCwRCc67FtZszgRGQY47-C0,1176
 directory_healthcheck/templates/directory_healthcheck/healthcheck.html,sha256=Na6eXAmCvfSUOG1IEEIUn4UbhkkUJpbKLlamkZQrRBg,339
-directory_healthcheck-3.1.0.dist-info/LICENSE,sha256=4QTWtORsQRx8DlWoAAEQHCse85Eas0SqCllvkojIO_M,1091
-directory_healthcheck-3.1.0.dist-info/METADATA,sha256=PntYBJEQO-nm-ko79gHNxDNqk0LifGsDV1wjxKDWyxI,4074
-directory_healthcheck-3.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-directory_healthcheck-3.1.0.dist-info/top_level.txt,sha256=ulfdOAfZlBGuRGJ3NNjj_a-FxUHXi2-B3sJrTu_U9Y0,22
-directory_healthcheck-3.1.0.dist-info/RECORD,,
+directory_healthcheck-3.1.1.dist-info/LICENSE,sha256=4QTWtORsQRx8DlWoAAEQHCse85Eas0SqCllvkojIO_M,1091
+directory_healthcheck-3.1.1.dist-info/METADATA,sha256=zhIf16meltt43XaiPhSs3xGH2Sr23LehvfUbXrsnvkI,4074
+directory_healthcheck-3.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+directory_healthcheck-3.1.1.dist-info/top_level.txt,sha256=ulfdOAfZlBGuRGJ3NNjj_a-FxUHXi2-B3sJrTu_U9Y0,22
+directory_healthcheck-3.1.1.dist-info/RECORD,,
```

