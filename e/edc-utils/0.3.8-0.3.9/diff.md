# Comparing `tmp/edc-utils-0.3.8.tar.gz` & `tmp/edc-utils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-utils-0.3.8.tar", last modified: Tue May 10 13:35:33 2022, max compression
+gzip compressed data, was "edc-utils-0.3.9.tar", last modified: Wed May 25 18:36:47 2022, max compression
```

## Comparing `edc-utils-0.3.8.tar` & `edc-utils-0.3.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-10 13:35:33.098824 edc-utils-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2020-03-10 19:59:42.000000 edc-utils-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-06 00:13:47.000000 edc-utils-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-10 13:35:33.091502 edc-utils-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-10 13:35:33.095040 edc-utils-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1745 2021-08-01 23:09:08.000000 edc-utils-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1255 2022-05-01 21:53:04.000000 edc-utils-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-01 21:53:04.000000 edc-utils-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-01 21:53:04.000000 edc-utils-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-10 19:59:42.000000 edc-utils-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       88 2022-05-01 21:53:04.000000 edc-utils-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1548 2022-05-10 13:35:33.098966 edc-utils-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2021-02-06 00:13:47.000000 edc-utils-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-05-10 13:35:23.000000 edc-utils-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-06 00:13:47.000000 edc-utils-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-10 13:35:33.097578 edc-utils-0.3.8/edc_utils/
--rw-r--r--   0 erikvw     (501) staff       (20)     1321 2022-05-10 13:35:23.000000 edc-utils-0.3.8/edc_utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2515 2022-05-01 21:53:04.000000 edc-utils-0.3.8/edc_utils/age.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1210 2022-05-01 21:53:04.000000 edc-utils-0.3.8/edc_utils/date.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-05-01 21:53:04.000000 edc-utils-0.3.8/edc_utils/disable_signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1690 2022-05-01 21:53:04.000000 edc-utils-0.3.8/edc_utils/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      843 2022-05-01 21:53:04.000000 edc-utils-0.3.8/edc_utils/get_static_file.py
--rw-r--r--   0 erikvw     (501) staff       (20)      440 2021-07-30 12:56:29.000000 edc-utils-0.3.8/edc_utils/paths_for_urlpatterns.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2934 2022-05-01 21:53:04.000000 edc-utils-0.3.8/edc_utils/show_urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      235 2020-03-10 19:59:42.000000 edc-utils-0.3.8/edc_utils/sqlite.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-10 13:35:33.098697 edc-utils-0.3.8/edc_utils/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-10 19:59:42.000000 edc-utils-0.3.8/edc_utils/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5045 2022-05-01 21:57:06.000000 edc-utils-0.3.8/edc_utils/tests/test_utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-05-01 21:53:04.000000 edc-utils-0.3.8/edc_utils/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2689 2022-05-01 21:53:04.000000 edc-utils-0.3.8/edc_utils/text.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-10 13:35:33.098267 edc-utils-0.3.8/edc_utils.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1548 2022-05-10 13:35:32.000000 edc-utils-0.3.8/edc_utils.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      661 2022-05-10 13:35:33.000000 edc-utils-0.3.8/edc_utils.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-10 13:35:32.000000 edc-utils-0.3.8/edc_utils.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-10 20:00:44.000000 edc-utils-0.3.8/edc_utils.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       10 2022-05-10 13:35:33.000000 edc-utils-0.3.8/edc_utils.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1579 2022-05-01 21:53:04.000000 edc-utils-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-03-01 04:11:26.000000 edc-utils-0.3.8/requirements.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1133 2021-02-06 00:13:47.000000 edc-utils-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1178 2022-05-10 13:35:33.099340 edc-utils-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:36:47.654591 edc-utils-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2020-03-10 19:59:42.000000 edc-utils-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-06 00:13:47.000000 edc-utils-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:36:47.648502 edc-utils-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:36:47.651355 edc-utils-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-utils-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1255 2022-05-01 21:53:04.000000 edc-utils-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-01 21:53:04.000000 edc-utils-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-01 21:53:04.000000 edc-utils-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-10 19:59:42.000000 edc-utils-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       88 2022-05-01 21:53:04.000000 edc-utils-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1528 2022-05-25 18:36:47.654727 edc-utils-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2021-02-06 00:13:47.000000 edc-utils-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-05-25 18:36:39.000000 edc-utils-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-06 00:13:47.000000 edc-utils-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:36:47.653274 edc-utils-0.3.9/edc_utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1321 2022-05-10 13:35:23.000000 edc-utils-0.3.9/edc_utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2528 2022-05-25 18:36:39.000000 edc-utils-0.3.9/edc_utils/age.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1108 2022-05-25 18:36:39.000000 edc-utils-0.3.9/edc_utils/date.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-05-01 21:53:04.000000 edc-utils-0.3.9/edc_utils/disable_signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1690 2022-05-01 21:53:04.000000 edc-utils-0.3.9/edc_utils/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      843 2022-05-01 21:53:04.000000 edc-utils-0.3.9/edc_utils/get_static_file.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      440 2021-07-30 12:56:29.000000 edc-utils-0.3.9/edc_utils/paths_for_urlpatterns.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2934 2022-05-01 21:53:04.000000 edc-utils-0.3.9/edc_utils/show_urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      235 2020-03-10 19:59:42.000000 edc-utils-0.3.9/edc_utils/sqlite.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:36:47.654408 edc-utils-0.3.9/edc_utils/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-10 19:59:42.000000 edc-utils-0.3.9/edc_utils/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5045 2022-05-01 21:57:06.000000 edc-utils-0.3.9/edc_utils/tests/test_utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-05-01 21:53:04.000000 edc-utils-0.3.9/edc_utils/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2702 2022-05-25 18:36:39.000000 edc-utils-0.3.9/edc_utils/text.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-25 18:36:47.653881 edc-utils-0.3.9/edc_utils.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1528 2022-05-25 18:36:47.000000 edc-utils-0.3.9/edc_utils.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      661 2022-05-25 18:36:47.000000 edc-utils-0.3.9/edc_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-25 18:36:47.000000 edc-utils-0.3.9/edc_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-10 20:00:44.000000 edc-utils-0.3.9/edc_utils.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       10 2022-05-25 18:36:47.000000 edc-utils-0.3.9/edc_utils.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1579 2022-05-01 21:53:04.000000 edc-utils-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-03-01 04:11:26.000000 edc-utils-0.3.9/requirements.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1133 2021-02-06 00:13:47.000000 edc-utils-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1228 2022-05-25 18:36:47.655061 edc-utils-0.3.9/setup.cfg
```

### Comparing `edc-utils-0.3.8/.github/workflows/build.yml` & `edc-utils-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/.gitignore` & `edc-utils-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/LICENSE` & `edc-utils-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/PKG-INFO` & `edc-utils-0.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edc-utils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple utilities for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-utils
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc visit schedule,data collection schedule,clinicedc,clinical trials
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
@@ -36,9 +35,7 @@
   :target: https://github.com/clinicedc/edc-utils/actions?query=workflow:build
 
 .. |codecov| image:: https://codecov.io/gh/clinicedc/edc-utils/branch/develop/graph/badge.svg
   :target: https://codecov.io/gh/clinicedc/edc-utils
 
 .. |downloads| image:: https://pepy.tech/badge/edc-utils
    :target: https://pepy.tech/project/edc-utils
-
-
```

### Comparing `edc-utils-0.3.8/README.rst` & `edc-utils-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/edc_utils/__init__.py` & `edc-utils-0.3.9/edc_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/edc_utils/age.py` & `edc-utils-0.3.9/edc_utils/age.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import date, datetime
 from typing import Optional, Union
+from zoneinfo import ZoneInfo
 
 import arrow
-import pytz
 from dateutil.relativedelta import relativedelta
 from django.conf import settings
 
 from .date import get_utcnow, to_arrow_utc
 
 
 class AgeValueError(Exception):
@@ -56,15 +56,15 @@
     born: Union[date, datetime, None],
     reference_dt: Union[date, datetime],
     timezone: Optional[str] = None,
 ) -> str:
     age_as_str = "?"
     if born:
         timezone = timezone or getattr(settings, "TIME_ZONE", "UTC")
-        born = arrow.Arrow.fromdate(born, tzinfo=pytz.timezone(timezone)).datetime
+        born = arrow.Arrow.fromdate(born, tzinfo=ZoneInfo(timezone)).datetime
         reference_dt = reference_dt or get_utcnow()
         age_delta = age(born, reference_dt or get_utcnow())
         if age_delta.years == 0 and age_delta.months <= 0:
             age_as_str = f"{age_delta.days}d"
         elif age_delta.years == 0 and 0 < age_delta.months <= 2:
             age_as_str = f"{age_delta.months}m{age_delta.days}d"
         elif age_delta.years == 0 and age_delta.months > 2:
```

### Comparing `edc-utils-0.3.8/edc_utils/date.py` & `edc-utils-0.3.9/edc_utils/date.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from datetime import date, datetime
 from typing import Optional
+from zoneinfo import ZoneInfo
 
 import arrow
-import pytz
 from arrow.arrow import Arrow
-from django.conf import settings
 
 
 class EdcDatetimeError(Exception):
     pass
 
 
 def get_utcnow() -> datetime:
@@ -23,16 +22,15 @@
     """Returns an arrow instance in UTC after converting date or datetime from
     the given timezone string to \'UTC\'.
     """
     try:
         dt.date()
     except AttributeError:
         # handle born as date. Use 0hr as time before converting to UTC
-        timezone = timezone or getattr(settings, "TIME_ZONE", "UTC")
-        r_utc = arrow.Arrow.fromdate(dt, tzinfo=pytz.timezone(timezone)).to("utc")
+        r_utc = arrow.Arrow.fromdate(dt, tzinfo=ZoneInfo("UTC"))
     else:
         if timezone:
             raise EdcDatetimeError("Timezone param not expected if dt is a datetime.")
         # handle born as datetime
         r_utc = arrow.Arrow.fromdatetime(dt, tzinfo=dt.tzinfo).to("utc")
     return r_utc
```

### Comparing `edc-utils-0.3.8/edc_utils/disable_signals.py` & `edc-utils-0.3.9/edc_utils/disable_signals.py`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/edc_utils/forms.py` & `edc-utils-0.3.9/edc_utils/forms.py`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/edc_utils/get_static_file.py` & `edc-utils-0.3.9/edc_utils/get_static_file.py`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/edc_utils/show_urls.py` & `edc-utils-0.3.9/edc_utils/show_urls.py`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/edc_utils/tests/test_utils.py` & `edc-utils-0.3.9/edc_utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/edc_utils/text.py` & `edc-utils-0.3.9/edc_utils/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import re
+from zoneinfo import ZoneInfo
 
-import pytz
 from arrow.arrow import Arrow
 from django.conf import settings
 
 safe_allowed_chars = "ABCDEFGHKMNPRTUVWXYZ2346789"
 
 
 def get_safe_random_string(length=12, safe=None, allowed_chars=None):
@@ -64,15 +64,15 @@
 
 def formatted_datetime(aware_datetime, php_dateformat=None, tz=None, format_as_date=None):
     """Returns a formatted datetime string, localized by default.
 
     format_as_date: does not affect the calculation, just the formatted output.
     """
     if aware_datetime:
-        tz = tz or pytz.timezone(settings.TIME_ZONE)
+        tz = tz or ZoneInfo(settings.TIME_ZONE)
         utc = Arrow.fromdatetime(aware_datetime)
         local = utc.to(tz)
         if format_as_date:
             php_dateformat = php_dateformat or settings.SHORT_DATE_FORMAT
             return local.datetime.date().strftime(convert_php_dateformat(php_dateformat))
         else:
             php_dateformat = php_dateformat or settings.SHORT_DATETIME_FORMAT
```

### Comparing `edc-utils-0.3.8/edc_utils.egg-info/PKG-INFO` & `edc-utils-0.3.9/edc_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edc-utils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple utilities for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-utils
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc visit schedule,data collection schedule,clinicedc,clinical trials
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
@@ -36,9 +35,7 @@
   :target: https://github.com/clinicedc/edc-utils/actions?query=workflow:build
 
 .. |codecov| image:: https://codecov.io/gh/clinicedc/edc-utils/branch/develop/graph/badge.svg
   :target: https://codecov.io/gh/clinicedc/edc-utils
 
 .. |downloads| image:: https://pepy.tech/badge/edc-utils
    :target: https://pepy.tech/project/edc-utils
-
-
```

### Comparing `edc-utils-0.3.8/edc_utils.egg-info/SOURCES.txt` & `edc-utils-0.3.9/edc_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/pyproject.toml` & `edc-utils-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/runtests.py` & `edc-utils-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-utils-0.3.8/setup.cfg` & `edc-utils-0.3.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 author_email = ew2789@gmail.com
 url = https://github.com/clinicedc/edc-utils
 license = GPL license, see LICENSE
 description = Simple utilities for clinicedc/edc projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django edc visit schedule, data collection schedule, clinicedc, clinical trials
+install_requires = 
+	arrow
+	tqdm
+	python-dateutil
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
```

