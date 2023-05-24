# Comparing `tmp/ya_django_toolkit_jp-0.0.0.post0.tar.gz` & `tmp/ya_django_toolkit_jp-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ya_django_toolkit_jp-0.0.0.post0.tar", max compression
+gzip compressed data, was "ya_django_toolkit_jp-0.0.1.tar", max compression
```

## Comparing `ya_django_toolkit_jp-0.0.0.post0.tar` & `ya_django_toolkit_jp-0.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       12 2023-05-24 01:44:59.637636 ya_django_toolkit_jp-0.0.0.post0/CHANGELOG.md
--rw-r--r--   0        0        0      292 2023-05-24 01:44:59.637636 ya_django_toolkit_jp-0.0.0.post0/README.md
--rw-r--r--   0        0        0     1270 2023-05-24 01:44:59.637636 ya_django_toolkit_jp-0.0.0.post0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 01:44:59.637636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/__init__.py
--rw-r--r--   0        0        0      169 2023-05-24 01:44:59.637636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/apps.py
--rw-r--r--   0        0        0        0 2023-05-24 01:44:59.637636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/base/__init__.py
--rw-r--r--   0        0        0      186 2023-05-24 01:44:59.637636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/base/models/__init__.py
--rw-r--r--   0        0        0      139 2023-05-24 01:44:59.637636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/base/models/base.py
--rw-r--r--   0        0        0      183 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/base/models/base_ulid.py
--rw-r--r--   0        0        0      175 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/base/models/base_uuid.py
--rw-r--r--   0        0        0      212 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/base/models/ulid.py
--rw-r--r--   0        0        0     1292 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/base_app_settings.py
--rw-r--r--   0        0        0      109 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/fields/__init__.py
--rw-r--r--   0        0        0      366 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/fields/normalize_char_field.py
--rw-r--r--   0        0        0      743 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/fields/ulid.py
--rw-r--r--   0        0        0        0 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/ja/__init__.py
--rw-r--r--   0        0        0      118 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/ja/fields/__init__.py
--rw-r--r--   0        0        0      399 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/ja/fields/hiragana_char.py
--rw-r--r--   0        0        0      399 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/ja/fields/katakana_char.py
--rw-r--r--   0        0        0     1955 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/ja/utils.py
--rw-r--r--   0        0        0      130 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/ja/validators/__init__.py
--rw-r--r--   0        0        0      200 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/ja/validators/hiragana_only.py
--rw-r--r--   0        0        0      200 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/ja/validators/katakana_only.py
--rw-r--r--   0        0        0        0 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/utils/__init__.py
--rw-r--r--   0        0        0      624 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/utils/file.py
--rw-r--r--   0        0        0     2031 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/utils/ip.py
--rw-r--r--   0        0        0      711 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/utils/ipv6.py
--rw-r--r--   0        0        0      206 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/utils/mimetypes.py
--rw-r--r--   0        0        0      508 2023-05-24 01:44:59.641636 ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/utils/view.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 ya_django_toolkit_jp-0.0.0.post0/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      292 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/README.md
+-rw-r--r--   0        0        0     1133 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/apps.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/base/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/base/models/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/base/models/base.py
+-rw-r--r--   0        0        0      183 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/base/models/base_ulid.py
+-rw-r--r--   0        0        0      175 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/base/models/base_uuid.py
+-rw-r--r--   0        0        0      212 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/base/models/ulid.py
+-rw-r--r--   0        0        0     1292 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/base_app_settings.py
+-rw-r--r--   0        0        0      109 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/fields/__init__.py
+-rw-r--r--   0        0        0      366 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/fields/normalize_char_field.py
+-rw-r--r--   0        0        0      743 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/fields/ulid.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/ja/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/ja/fields/__init__.py
+-rw-r--r--   0        0        0      399 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/ja/fields/hiragana_char.py
+-rw-r--r--   0        0        0      399 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/ja/fields/katakana_char.py
+-rw-r--r--   0        0        0     1940 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/ja/utils.py
+-rw-r--r--   0        0        0      131 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/ja/validators/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/ja/validators/hirakgana_only.py
+-rw-r--r--   0        0        0      200 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/ja/validators/katakana_only.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/utils/__init__.py
+-rw-r--r--   0        0        0      624 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/utils/file.py
+-rw-r--r--   0        0        0     2031 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/utils/ip.py
+-rw-r--r--   0        0        0      711 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/utils/ipv6.py
+-rw-r--r--   0        0        0      206 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/utils/mimetypes.py
+-rw-r--r--   0        0        0      508 2023-05-23 18:17:53.620657 ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/utils/view.py
+-rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 ya_django_toolkit_jp-0.0.1/PKG-INFO
```

### Comparing `ya_django_toolkit_jp-0.0.0.post0/pyproject.toml` & `ya_django_toolkit_jp-0.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -9,36 +9,31 @@
 readme = "README.md"
 packages = [{include = "ya_django_toolkit_jp"}]
 license = "MIT"
 include = ["CHANGELOG.md"]
 
 [tool.poetry-git-version-plugin]
 make_alpha_version = true
-alpha_version_format = '{version}.post{distance}'
+alpha_version_format = '{version}a{distance}+{commit_hash}'
 
 [tool.poetry.dependencies]
 python = "^3.11"
 django = "^4.2"
 
-[tool.taskipy.tasks]
-test = "coverage run --source ./ya_django_toolkit_jp/ -m unittest discover ./tests/"
-
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 flake8-isort = "^6.0.0"
 autopep8 = "^2.0.2"
 pre-commit = "^3.3.2"
 types-backports = "^0.1.3"
 django-types = "^0.17.0"
 mypy = "^1.3.0"
 safety = "^2.3.5"
-taskipy = "^1.11.0"
-coverage = "^7.2.5"
 
 
 [tool.poetry.group.all.dependencies]
 ulid-py = "^1.1.0"
 django-boost = "^2.1"
 
 [build-system]
```

### Comparing `ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/base_app_settings.py` & `ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/base_app_settings.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/fields/ulid.py` & `ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/fields/ulid.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/ja/utils.py` & `ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/ja/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,19 @@
 
     Returns:
         str: 正規化した文字列
     """
     return unicode_normalize(remove_control_characters(s))
 
 
-def replace_hyphen(text: str, replace_hyphen: str = '-') -> str:
+def replace_hyphen(text: str, replace_hyphen: str) -> str:
     """全ての横棒を半角ハイフンに置換する
     Args:
         text (str): 入力するテキスト
-        replace_hyphen (str): ハイフンの置換先文字列
+        replace_hyphen (str): 置換したい文字列
     Returns:
         (str): 置換後のテキスト
     """
     # https://qiita.com/non-caffeine/items/77360dda05c8ce510084
     hyphens = '-˗ᅳ᭸‐‑‒–—―⁃⁻−▬─━➖ーㅡ﹘﹣－ｰ𐄐𐆑 '
     hyphens = '|'.join(hyphens)
     return re.sub(hyphens, replace_hyphen, text)
```

### Comparing `ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/utils/file.py` & `ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/utils/file.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/utils/ip.py` & `ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/utils/ip.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.0.post0/ya_django_toolkit_jp/utils/ipv6.py` & `ya_django_toolkit_jp-0.0.1/ya_django_toolkit_jp/utils/ipv6.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.0.post0/PKG-INFO` & `ya_django_toolkit_jp-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya-django-toolkit-jp
-Version: 0.0.0.post0
+Version: 0.0.1
 Summary: 日本語（マルチバイト文字）の考慮も入れた Django プロジェクトのためのユーティリティです。
 Home-page: https://github.com/yk-lab
 License: MIT
 Author: yk-lab a.k.a YetAnother_yk
 Author-email: yk-lab@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

