# Comparing `tmp/django-pictures-1.0rc5.tar.gz` & `tmp/django_pictures-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pictures-1.0rc5.tar", last modified: Thu Oct 27 08:43:18 2022, max compression
+gzip compressed data, was "django_pictures-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django-pictures-1.0rc5.tar` & `django_pictures-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1324 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/LICENSE
--rw-r--r--   0        0        0     8619 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/README.md
--rw-r--r--   0        0        0      171 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/__init__.py
--rw-r--r--   0        0        0      174 2022-10-27 08:43:17.999077 django-pictures-1.0rc5/pictures/_version.py
--rw-r--r--   0        0        0      155 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/apps.py
--rw-r--r--   0        0        0     1012 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/checks.py
--rw-r--r--   0        0        0      624 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/conf.py
--rw-r--r--   0        0        0        0 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/contrib/__init__.py
--rw-r--r--   0        0        0     2050 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/contrib/rest_framework.py
--rw-r--r--   0        0        0      857 2022-10-27 08:43:02.170796 django-pictures-1.0rc5/pictures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1179 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3195 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/migrations.py
--rw-r--r--   0        0        0     8040 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/models.py
--rw-r--r--   0        0        0     3726 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/tasks.py
--rw-r--r--   0        0        0      165 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/templates/pictures/attrs.html
--rw-r--r--   0        0        0      537 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/templates/pictures/picture.html
--rw-r--r--   0        0        0        0 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/templatetags/__init__.py
--rw-r--r--   0        0        0     2001 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/templatetags/pictures.py
--rw-r--r--   0        0        0      214 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/urls.py
--rw-r--r--   0        0        0     3695 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/utils.py
--rw-r--r--   0        0        0     1907 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/validators.py
--rw-r--r--   0        0        0      725 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pictures/views.py
--rw-r--r--   0        0        0     2278 2022-10-27 08:42:14.361959 django-pictures-1.0rc5/pyproject.toml
--rw-r--r--   0        0        0    10667 1970-01-01 00:00:00.000000 django-pictures-1.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1324 2023-05-24 17:01:29.714398 django_pictures-1.1.0/LICENSE
+-rw-r--r--   0        0        0     9256 2023-05-24 17:01:29.714398 django_pictures-1.1.0/README.md
+-rw-r--r--   0        0        0      171 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-24 17:01:49.962679 django_pictures-1.1.0/pictures/_version.py
+-rw-r--r--   0        0        0      155 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/apps.py
+-rw-r--r--   0        0        0     1012 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/checks.py
+-rw-r--r--   0        0        0      683 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/conf.py
+-rw-r--r--   0        0        0        0 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/contrib/__init__.py
+-rw-r--r--   0        0        0     2343 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/contrib/rest_framework.py
+-rw-r--r--   0        0        0      857 2023-05-24 17:01:42.970592 django_pictures-1.1.0/pictures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1179 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3195 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/migrations.py
+-rw-r--r--   0        0        0     8495 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/models.py
+-rw-r--r--   0        0        0     3726 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/tasks.py
+-rw-r--r--   0        0        0      165 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/templates/pictures/attrs.html
+-rw-r--r--   0        0        0      618 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/templates/pictures/picture.html
+-rw-r--r--   0        0        0        0 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/templatetags/__init__.py
+-rw-r--r--   0        0        0     2281 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/templatetags/pictures.py
+-rw-r--r--   0        0        0      214 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/urls.py
+-rw-r--r--   0        0        0     4023 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/utils.py
+-rw-r--r--   0        0        0     1907 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/validators.py
+-rw-r--r--   0        0        0      725 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/views.py
+-rw-r--r--   0        0        0     2349 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11381 1970-01-01 00:00:00.000000 django_pictures-1.1.0/PKG-INFO
```

### Comparing `django-pictures-1.0rc5/LICENSE` & `django_pictures-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc5/README.md` & `django_pictures-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,41 +20,45 @@
 
 Before you start, it can be a good idea to understand the fundamentals of
 [responsive images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images).
 
 Once you get a feeling how complicated things can get with all device types, you'll probably find
 a new appreciation for this package and are ready to adopt in you project :)
 
-
 ```python
 # models.py
 from django.db import models
 from pictures.models import PictureField
 
 class Profile(models.Model):
     title = models.CharField(max_length=255)
     picture = PictureField(upload_to="avatars")
 ```
 
 ```html
 <!-- template.html -->
 {% load pictures %}
-{% picture profile.picture alt="Spiderman" loading="lazy" m=6 l=4 %}
+{% picture profile.picture img_alt="Spiderman" img_loading="lazy" picture_class="my-picture" m=6 l=4 %}
 ```
 
 The template above will render into:
 ```html
-<picture>
+<picture class="my-picture">
   <source type="image/webp"
           srcset="/media/testapp/profile/image/800w.webp 800w, /media/testapp/profile/image/100w.webp 100w, /media/testapp/profile/image/200w.webp 200w, /media/testapp/profile/image/300w.webp 300w, /media/testapp/profile/image/400w.webp 400w, /media/testapp/profile/image/500w.webp 500w, /media/testapp/profile/image/600w.webp 600w, /media/testapp/profile/image/700w.webp 700w"
           sizes="(min-width: 0px) and (max-width: 991px) 100vw, (min-width: 992px) and (max-width: 1199px) 33vw, 600px">
   <img src="/media/testapp/profile/image.jpg" alt="Spiderman" width="800" height="800" loading="lazy">
 </picture>
 ```
 
+Note that arbitrary attributes can be passed
+to either the `<picture>` or `<img>` element
+by prefixing parameters to the `{% picture %}` tag
+with `picture_` or `img_` respectively.
+
 ## Setup
 
 ### Installation
 
 ```shell
 python3 -m pip install django-pictures
 ```
@@ -77,14 +81,18 @@
         "l": 1200,
         "xl": 1400,
     },
     "GRID_COLUMNS": 12,
     "CONTAINER_WIDTH": 1200,
     "FILE_TYPES": ["WEBP"],
     "PIXEL_DENSITIES": [1, 2],
+    "USE_PLACEHOLDERS": True,
+    "QUEUE_NAME": "pictures",
+    "PROCESSOR": "pictures.tasks.process_picture",
+
 }
 ```
 
 If you have either Dramatiq or Celery installed, we will default to async
 image processing. You will need workers to listen to the `pictures` queue.
 
 ### Placeholders
@@ -148,15 +156,15 @@
       aspect_ratios=[None, "1/1", "3/2", "16/9"],
     )
 ```
 
 ```html
 # template.html
 {% load pictures %}
-{% picture profile.picture alt="Spiderman" ratio="16/9" m=6 l=4 %}
+{% picture profile.picture img_alt="Spiderman" ratio="16/9" m=6 l=4 %}
 ```
 
 If you don't specify an aspect ratio or None in your template, the image will be
 served with the original aspect ratio of the file.
 
 You may only use aspect ratios in templates, that have been defined on the model.
 The model `aspect_ratios` will default to `[None]`, if other value is provided.
@@ -192,32 +200,35 @@
 
 ### Pixel densities
 
 Unless you really care that your images hold of if you hold your UHD phone very
 close to your eyeballs, you should be fine, serving at the default `1x` and `2x`
 densities.
 
-
 ### Async image processing
 
 If you have either Dramatiq or Celery installed, we will default to async
 image processing. You will need workers to listen to the `pictures` queue.
 You can override the queue name, via the `PICTURES["QUEUE_NAME"]` setting.
 
+You can also override the processor, via the `PICTURES["PROCESSOR"]` setting.
+The default processor is `pictures.tasks.process_picture`. It takes a single
+argument, the `PictureFileFile` instance. You can use this to override the
+processor, should you need to do some custom processing.
+
 ## Migrations
 
 Django doesn't support file field migrations, but we do.
 You can simply auto create the migration and replace Django's
 `AlterField` operation with `AlterPictureField`. That's it.
 
 You can follow [the example][migration] in our test app, to see how it works.
 
 [migration]: tests/testapp/migrations/0002_alter_profile_picture.py
 
-
 ## Contrib
 
 ### Django Rest Framework ([DRF])
 
 We do ship with a read-only `PictureField` that can be used to include all
 available picture sizes in a DRF serializer.
```

### Comparing `django-pictures-1.0rc5/pictures/checks.py` & `django_pictures-1.1.0/pictures/checks.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc5/pictures/conf.py` & `django_pictures-1.1.0/pictures/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,10 +17,11 @@
             },
             "GRID_COLUMNS": 12,
             "CONTAINER_WIDTH": 1200,
             "FILE_TYPES": ["WEBP"],
             "PIXEL_DENSITIES": [1, 2],
             "USE_PLACEHOLDERS": settings.DEBUG,
             "QUEUE_NAME": "pictures",
+            "PROCESSOR": "pictures.tasks.process_picture",
             **getattr(settings, "PICTURES", {}),
         },
     )
```

### Comparing `django-pictures-1.0rc5/pictures/contrib/rest_framework.py` & `django_pictures-1.1.0/pictures/contrib/rest_framework.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 
+from django.http import QueryDict
 from rest_framework import serializers
 
 __all__ = ["PictureField"]
 
 from pictures import utils
 from pictures.conf import get_settings
 from pictures.models import PictureFieldFile, SimplePicture
@@ -30,20 +31,26 @@
                         for file_type, sizes in sources.items()
                     },
                 }
                 for ratio, sources in obj.aspect_ratios.items()
             },
         }
         try:
-            query_params = self.context["request"].GET
+            query_params: QueryDict = self.context["request"].GET
         except KeyError:
             pass
         else:
             ratio = query_params.get(f"{self.source}_ratio")
             container = query_params.get(f"{self.source}_container")
+            try:
+                container = int(container)
+            except TypeError:
+                container = None
+            except ValueError as e:
+                raise ValueError(f"Container width is not a number: {container}") from e
             breakpoints = {
                 bp: int(query_params.get(f"{self.source}_{bp}"))
                 for bp in get_settings().BREAKPOINTS
                 if f"{self.source}_{bp}" in query_params
             }
             if ratio is not None:
                 try:
```

### Comparing `django-pictures-1.0rc5/pictures/locale/de/LC_MESSAGES/django.mo` & `django_pictures-1.1.0/pictures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc5/pictures/locale/de/LC_MESSAGES/django.po` & `django_pictures-1.1.0/pictures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc5/pictures/migrations.py` & `django_pictures-1.1.0/pictures/migrations.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc5/pictures/models.py` & `django_pictures-1.1.0/pictures/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,20 @@
 from django.db.models import ImageField
 from django.db.models.fields.files import ImageFieldFile
 from django.urls import reverse
 from PIL import Image, ImageOps
 
 __all__ = ["PictureField", "PictureFieldFile"]
 
+from django.utils.module_loading import import_string
 
 from pictures import conf, utils
 
+RGB_FORMATS = ["JPEG"]
+
 
 @dataclasses.dataclass
 class SimplePicture:
     """A simple picture class similar to Django's image class."""
 
     parent_name: str
     file_type: str
@@ -46,15 +49,15 @@
                     else None,
                     "file_type": self.file_type,
                 },
             )
         return self.storage.url(self.name)
 
     @property
-    def height(self) -> int or None:
+    def height(self) -> int | None:
         if self.aspect_ratio:
             return math.floor(self.width / self.aspect_ratio)
 
     @property
     def name(self) -> str:
         path = Path(self.parent_name).with_suffix("")
         if self.aspect_ratio:
@@ -62,27 +65,29 @@
         return str(path / f"{self.width}w.{self.file_type.lower()}")
 
     @property
     def path(self) -> Path:
         return Path(self.storage.path(self.name))
 
     def process(self, image) -> Image:
+        image = ImageOps.exif_transpose(image)  # crates a copy
         height = self.height or self.width / Fraction(*image.size)
         size = math.floor(self.width), math.floor(height)
 
         if self.aspect_ratio:
             image = ImageOps.fit(image, size)
         else:
-            image = image.copy()
             image.thumbnail(size)
         return image
 
     def save(self, image):
         with io.BytesIO() as file_buffer:
             img = self.process(image)
+            if (self.file_type in RGB_FORMATS) and (img.mode != "RGB"):
+                img = img.convert("RGB")
             img.save(file_buffer, format=self.file_type)
             self.storage.delete(self.name)  # avoid any filename collisions
             self.storage.save(self.name, ContentFile(file_buffer.getvalue()))
 
     def delete(self):
         self.storage.delete(self.name)
 
@@ -90,17 +95,15 @@
 class PictureFieldFile(ImageFieldFile):
     def save(self, name, content, save=True):
         super().save(name, content, save)
         self.save_all()
 
     def save_all(self):
         if self:
-            from . import tasks
-
-            tasks.process_picture(self)
+            import_string(conf.get_settings().PROCESSOR)(self)
 
     def delete(self, save=True):
         self.delete_all()
         super().delete(save=save)
 
     def delete_all(self, aspect_ratios=None):
         aspect_ratios = aspect_ratios or self.aspect_ratios
@@ -230,15 +233,15 @@
     def _check_width_height_field(self):
         if None in self.aspect_ratios and not (self.width_field and self.height_field):
             return [
                 checks.Warning(
                     "width_field and height_field attributes are missing",
                     obj=self,
                     id="fields.E101",
-                    hint="Set both the width_field and height_field attribute to avoid storage IO",
+                    hint=f"Please add two positive integer fields to '{self.model._meta.app_label}.{self.model.__name__}' and add their field names as the 'width_field' and 'height_field' attribute for your picture field. Otherwise Django will not be able to cache the image aspect size causing disk IO and potential response time increases.",
                 )
             ]
         return []
 
     def deconstruct(self):
         name, path, args, kwargs = super().deconstruct()
         return (
```

### Comparing `django-pictures-1.0rc5/pictures/tasks.py` & `django_pictures-1.1.0/pictures/tasks.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc5/pictures/templates/pictures/picture.html` & `django_pictures-1.1.0/pictures/templates/pictures/picture.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-<picture>{% for type, srcset in sources.items %}
+<picture{% include 'pictures/attrs.html' with attrs=picture_attrs %}>{% for type, srcset in sources.items %}
   <source type="image/{{ type|lower }}"
           srcset="{% for width, pic in srcset.items %}{% if use_placeholders %}{% url 'pictures:placeholder' alt|urlencode:'' ratio width type %}{% else %}{{ pic.url }}{% endif %} {{ width }}w{% if not forloop.last %}, {% endif %}{% endfor %}"
           sizes="{{ media }}">{% endfor %}
-  <img src="{{ field_file.url }}" alt="{{ alt }}" width="{{ field_file.width }}" height="{{ field_file.height }}"{% include 'pictures/attrs.html' %}>
+  <img src="{{ field_file.url }}" alt="{{ alt }}" width="{{ field_file.width }}" height="{{ field_file.height }}"{% include 'pictures/attrs.html' with attrs=img_attrs %}>
 </picture>
```

### Comparing `django-pictures-1.0rc5/pictures/templatetags/pictures.py` & `django_pictures-1.1.0/pictures/templatetags/pictures.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,39 +4,45 @@
 from .. import utils
 from ..conf import get_settings
 
 register = template.Library()
 
 
 @register.simple_tag()
-def picture(field_file, alt=None, ratio=None, container=None, **kwargs):
+def picture(field_file, img_alt=None, ratio=None, container=None, **kwargs):
     settings = get_settings()
     container = container or settings.CONTAINER_WIDTH
     tmpl = loader.get_template("pictures/picture.html")
     breakpoints = {}
-    attrs = {}
+    picture_attrs = {}
+    img_attrs = {}
     try:
         sources = field_file.aspect_ratios[ratio]
     except KeyError as e:
         raise ValueError(
             f"Invalid ratio: {ratio}. Choices are: {', '.join(filter(None, field_file.aspect_ratios.keys()))}"
         ) from e
     for key, value in kwargs.items():
         if key in settings.BREAKPOINTS:
             breakpoints[key] = value
+        elif key.startswith("picture_"):
+            picture_attrs[key[8:]] = value
+        elif key.startswith("img_"):
+            img_attrs[key[4:]] = value
         else:
-            attrs[key] = value
+            raise TypeError(f"Invalid keyword argument: {key}")
     return tmpl.render(
         {
             "field_file": field_file,
-            "alt": alt,
+            "alt": img_alt,
             "ratio": (ratio or "3/2").replace("/", "x"),
             "sources": sources,
             "media": utils.sizes(container_width=container, **breakpoints),
-            "attrs": attrs,
+            "picture_attrs": picture_attrs,
+            "img_attrs": img_attrs,
             "use_placeholders": settings.USE_PLACEHOLDERS,
         }
     )
 
 
 @register.simple_tag()
 def img_url(field_file, file_type, width, ratio=None) -> str:
```

### Comparing `django-pictures-1.0rc5/pictures/utils.py` & `django_pictures-1.1.0/pictures/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import math
 import random
 import sys
+import warnings
 from fractions import Fraction
 from functools import lru_cache
 from urllib.parse import unquote
 
 from PIL import Image, ImageDraw, ImageFont
 
 from . import conf
@@ -35,15 +36,21 @@
         if container_width and width >= container_width:
             yield f"(min-width: {prev_width}px) and (max-width: {container_width - 1}px) {math.floor(ratio * 100)}vw"
             break
         if prev_ratio and prev_ratio != ratio:
             yield f"(min-width: {prev_width}px) and (max-width: {width - 1}px) {math.floor(prev_ratio * 100)}vw"
             prev_width = width
         prev_ratio = ratio
-    yield f"{math.floor(prev_ratio * container_width)}px" if container_width else f"{math.floor(prev_ratio * 100)}vw"
+    if prev_ratio:
+        yield f"{math.floor(prev_ratio * container_width)}px" if container_width else f"{math.floor(prev_ratio * 100)}vw"
+    else:
+        warnings.warn(
+            "Your container is smaller than all your breakpoints.", UserWarning
+        )
+        yield f"{container_width}px" if container_width else "100vw"
 
 
 def sizes(*, cols=12, container_width: int = None, **breakpoints: {str: int}) -> str:
     breakpoints = dict(_grid(_columns=cols, **breakpoints))
     return ", ".join(_media_query(container_width=container_width, **breakpoints))
 
 
@@ -79,17 +86,19 @@
     fontsize = 32
     if sys.platform == "win32":
         font_name = r"C:\WINDOWS\Fonts\CALIBRI.TTF"
     elif sys.platform in ["linux", "linux2"]:
         font_name = "DejaVuSans-Bold"
     elif sys.platform == "darwin":
         font_name = "Helvetica"
+    else:  # pragma: no cover
+        raise RuntimeError(f"Unsupported platform: {sys.platform}")
     font = ImageFont.truetype(font_name, fontsize)
     text = unquote(f"{alt}\n<{width}x{height}>")
-    while font.getsize(text)[0] < width / 2:
+    while font.getlength(text) < width / 2:
         # iterate until the text size is just larger than the criteria
         fontsize += 1
         font = ImageFont.truetype(font_name, fontsize)
 
     draw.text(
         (width / 2, height / 2),
         text,
```

### Comparing `django-pictures-1.0rc5/pictures/validators.py` & `django_pictures-1.1.0/pictures/validators.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc5/pictures/views.py` & `django_pictures-1.1.0/pictures/views.py`

 * *Files identical despite different names*

### Comparing `django-pictures-1.0rc5/pyproject.toml` & `django_pictures-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -8,35 +8,36 @@
   { name = "Johannes Maron", email = "johannes@maron.family" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["pillow", "Django", "image", "pictures", "WebP", "AVIF"]
 dynamic = ["version", "description"]
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Environment :: Web Environment",
   "Topic :: Multimedia :: Graphics :: Graphics Conversion",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Topic :: Software Development",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
-  "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
 ]
 requires-python = ">=3.8"
-dependencies = ["django", "pillow"]
+dependencies = ["django>=3.2.0", "pillow>=9.0.0"]
 
 [project.optional-dependencies]
 test = [
   "pytest",
   "pytest-cov",
   "pytest-django",
   "redis",
```

### Comparing `django-pictures-1.0rc5/PKG-INFO` & `django_pictures-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: django-pictures
-Version: 1.0rc5
+Version: 1.1.0
 Summary: Responsive cross-browser image library using modern codes like AVIF & WebP.
 Keywords: pillow,Django,image,pictures,WebP,AVIF
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
-Requires-Dist: django
-Requires-Dist: pillow
+Classifier: Framework :: Django :: 4.2
+Requires-Dist: django>=3.2.0
+Requires-Dist: pillow>=9.0.0
 Requires-Dist: celery ; extra == "celery"
 Requires-Dist: django-cleanup ; extra == "cleanup"
 Requires-Dist: django-dramatiq ; extra == "dramatiq"
 Requires-Dist: djangorestframework ; extra == "drf"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-django ; extra == "test"
@@ -67,41 +68,45 @@
 
 Before you start, it can be a good idea to understand the fundamentals of
 [responsive images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images).
 
 Once you get a feeling how complicated things can get with all device types, you'll probably find
 a new appreciation for this package and are ready to adopt in you project :)
 
-
 ```python
 # models.py
 from django.db import models
 from pictures.models import PictureField
 
 class Profile(models.Model):
     title = models.CharField(max_length=255)
     picture = PictureField(upload_to="avatars")
 ```
 
 ```html
 <!-- template.html -->
 {% load pictures %}
-{% picture profile.picture alt="Spiderman" loading="lazy" m=6 l=4 %}
+{% picture profile.picture img_alt="Spiderman" img_loading="lazy" picture_class="my-picture" m=6 l=4 %}
 ```
 
 The template above will render into:
 ```html
-<picture>
+<picture class="my-picture">
   <source type="image/webp"
           srcset="/media/testapp/profile/image/800w.webp 800w, /media/testapp/profile/image/100w.webp 100w, /media/testapp/profile/image/200w.webp 200w, /media/testapp/profile/image/300w.webp 300w, /media/testapp/profile/image/400w.webp 400w, /media/testapp/profile/image/500w.webp 500w, /media/testapp/profile/image/600w.webp 600w, /media/testapp/profile/image/700w.webp 700w"
           sizes="(min-width: 0px) and (max-width: 991px) 100vw, (min-width: 992px) and (max-width: 1199px) 33vw, 600px">
   <img src="/media/testapp/profile/image.jpg" alt="Spiderman" width="800" height="800" loading="lazy">
 </picture>
 ```
 
+Note that arbitrary attributes can be passed
+to either the `<picture>` or `<img>` element
+by prefixing parameters to the `{% picture %}` tag
+with `picture_` or `img_` respectively.
+
 ## Setup
 
 ### Installation
 
 ```shell
 python3 -m pip install django-pictures
 ```
@@ -124,14 +129,18 @@
         "l": 1200,
         "xl": 1400,
     },
     "GRID_COLUMNS": 12,
     "CONTAINER_WIDTH": 1200,
     "FILE_TYPES": ["WEBP"],
     "PIXEL_DENSITIES": [1, 2],
+    "USE_PLACEHOLDERS": True,
+    "QUEUE_NAME": "pictures",
+    "PROCESSOR": "pictures.tasks.process_picture",
+
 }
 ```
 
 If you have either Dramatiq or Celery installed, we will default to async
 image processing. You will need workers to listen to the `pictures` queue.
 
 ### Placeholders
@@ -195,15 +204,15 @@
       aspect_ratios=[None, "1/1", "3/2", "16/9"],
     )
 ```
 
 ```html
 # template.html
 {% load pictures %}
-{% picture profile.picture alt="Spiderman" ratio="16/9" m=6 l=4 %}
+{% picture profile.picture img_alt="Spiderman" ratio="16/9" m=6 l=4 %}
 ```
 
 If you don't specify an aspect ratio or None in your template, the image will be
 served with the original aspect ratio of the file.
 
 You may only use aspect ratios in templates, that have been defined on the model.
 The model `aspect_ratios` will default to `[None]`, if other value is provided.
@@ -239,32 +248,35 @@
 
 ### Pixel densities
 
 Unless you really care that your images hold of if you hold your UHD phone very
 close to your eyeballs, you should be fine, serving at the default `1x` and `2x`
 densities.
 
-
 ### Async image processing
 
 If you have either Dramatiq or Celery installed, we will default to async
 image processing. You will need workers to listen to the `pictures` queue.
 You can override the queue name, via the `PICTURES["QUEUE_NAME"]` setting.
 
+You can also override the processor, via the `PICTURES["PROCESSOR"]` setting.
+The default processor is `pictures.tasks.process_picture`. It takes a single
+argument, the `PictureFileFile` instance. You can use this to override the
+processor, should you need to do some custom processing.
+
 ## Migrations
 
 Django doesn't support file field migrations, but we do.
 You can simply auto create the migration and replace Django's
 `AlterField` operation with `AlterPictureField`. That's it.
 
 You can follow [the example][migration] in our test app, to see how it works.
 
 [migration]: tests/testapp/migrations/0002_alter_profile_picture.py
 
-
 ## Contrib
 
 ### Django Rest Framework ([DRF])
 
 We do ship with a read-only `PictureField` that can be used to include all
 available picture sizes in a DRF serializer.
```

