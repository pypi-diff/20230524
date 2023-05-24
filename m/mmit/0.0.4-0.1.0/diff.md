# Comparing `tmp/mmit-0.0.4.tar.gz` & `tmp/mmit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmit-0.0.4.tar", last modified: Tue May 16 22:04:17 2023, max compression
+gzip compressed data, was "mmit-0.1.0.tar", last modified: Wed May 24 21:08:00 2023, max compression
```

## Comparing `mmit-0.0.4.tar` & `mmit-0.1.0.tar`

### file list

```diff
@@ -1,54 +1,107 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.528817 mmit-0.0.4/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2758 2023-05-13 11:08:20.000000 mmit-0.0.4/.gitignore
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      413 2023-05-13 11:21:05.000000 mmit-0.0.4/.pre-commit-config.yaml
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1086 2023-05-16 17:34:06.000000 mmit-0.0.4/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2104 2023-05-16 22:04:17.528817 mmit-0.0.4/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1674 2023-05-16 17:52:36.000000 mmit-0.0.4/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.524817 mmit-0.0.4/docker/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-13 09:59:03.000000 mmit-0.0.4/docker/Dockerfile
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-13 09:58:52.000000 mmit-0.0.4/docker/requirement.txt
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.524817 mmit-0.0.4/docs/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      634 2023-05-13 11:56:02.000000 mmit-0.0.4/docs/Makefile
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1473 2023-05-13 12:41:57.000000 mmit-0.0.4/docs/conf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      473 2023-05-13 11:56:02.000000 mmit-0.0.4/docs/index.rst
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      800 2023-05-13 11:56:02.000000 mmit-0.0.4/docs/make.bat
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.524817 mmit-0.0.4/mmit/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       62 2023-05-16 19:29:08.000000 mmit-0.0.4/mmit/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.528817 mmit-0.0.4/mmit/base/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-13 13:41:15.000000 mmit-0.0.4/mmit/base/activations.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-13 13:35:04.000000 mmit-0.0.4/mmit/base/extra.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-13 13:41:28.000000 mmit-0.0.4/mmit/base/normlayers.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      475 2023-05-15 23:17:11.000000 mmit-0.0.4/mmit/base/upsamplers.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.528817 mmit-0.0.4/mmit/decoders/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       60 2023-05-16 19:29:08.000000 mmit-0.0.4/mmit/decoders/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1210 2023-05-14 20:36:31.000000 mmit-0.0.4/mmit/decoders/basedecoder.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.528817 mmit-0.0.4/mmit/decoders/unet/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-13 15:45:38.000000 mmit-0.0.4/mmit/decoders/unet/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3171 2023-05-16 19:29:08.000000 mmit-0.0.4/mmit/decoders/unet/model.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1967 2023-05-15 23:20:22.000000 mmit-0.0.4/mmit/decoders/unet/parts.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.528817 mmit-0.0.4/mmit/decoders/unetplusplus/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-14 15:38:16.000000 mmit-0.0.4/mmit/decoders/unetplusplus/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4965 2023-05-16 19:29:55.000000 mmit-0.0.4/mmit/decoders/unetplusplus/model.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.528817 mmit-0.0.4/mmit/encoders/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       26 2023-05-16 19:29:08.000000 mmit-0.0.4/mmit/encoders/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      757 2023-05-16 19:01:07.000000 mmit-0.0.4/mmit/encoders/basencoder.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.528817 mmit-0.0.4/mmit/encoders/timm/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-16 19:03:36.000000 mmit-0.0.4/mmit/encoders/timm/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1555 2023-05-16 22:02:44.000000 mmit-0.0.4/mmit/encoders/timm/model.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.528817 mmit-0.0.4/mmit/factory/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       47 2023-05-16 19:26:29.000000 mmit-0.0.4/mmit/factory/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      999 2023-05-16 19:45:14.000000 mmit-0.0.4/mmit/factory/factory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2560 2023-05-16 19:42:10.000000 mmit-0.0.4/mmit/factory/registry.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.524817 mmit-0.0.4/mmit.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2104 2023-05-16 22:04:17.000000 mmit-0.0.4/mmit.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      912 2023-05-16 22:04:17.000000 mmit-0.0.4/mmit.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-16 22:04:17.000000 mmit-0.0.4/mmit.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      208 2023-05-16 22:04:17.000000 mmit-0.0.4/mmit.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        5 2023-05-16 22:04:17.000000 mmit-0.0.4/mmit.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1099 2023-05-16 21:59:23.000000 mmit-0.0.4/pyproject.toml
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2023-05-16 22:04:17.528817 mmit-0.0.4/setup.cfg
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 22:04:17.528817 mmit-0.0.4/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      125 2023-05-16 19:29:08.000000 mmit-0.0.4/tests/conftest.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-13 16:25:37.000000 mmit-0.0.4/tests/test_decoders.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-13 16:25:32.000000 mmit-0.0.4/tests/test_encoders.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1792 2023-05-16 22:03:34.000000 mmit-0.0.4/tests/test_encoders_decoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.801251 mmit-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.785251 mmit-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-24 21:07:45.000000 mmit-0.1.0/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 21:07:45.000000 mmit-0.1.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.785251 mmit-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-24 21:07:45.000000 mmit-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-24 21:07:45.000000 mmit-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-24 21:07:45.000000 mmit-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-24 21:07:45.000000 mmit-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-24 21:08:00.801251 mmit-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-24 21:07:45.000000 mmit-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.785251 mmit-0.1.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/docker/requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.781251 mmit-0.1.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/_static/css/baseline.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/_static/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/_static/logo/logo_title.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/api/create_decoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/api/create_encoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/api/create_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/guide/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/guide/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/guide/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.785251 mmit-0.1.0/docs/source/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/modules/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/modules/decoders/fpn.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/modules/decoders/unet++.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/modules/decoders/unet.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/docs/source/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 21:07:45.000000 mmit-0.1.0/docs/source/modules/encoders/timm.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.789251 mmit-0.1.0/mmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/base/upsamplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/basedecoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/decoders/fpn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/fpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/fpn/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/fpn/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/decoders/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit/decoders/unetplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unetplusplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/unetplusplus/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/decoders/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/utils/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/decoders/utils/resizing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/encoders/basencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/encoders/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/encoders/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/encoders/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/factory/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/factory/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/factory/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/heads/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/heads/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.797251 mmit-0.1.0/mmit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-24 21:07:45.000000 mmit-0.1.0/mmit/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.793251 mmit-0.1.0/mmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 21:08:00.000000 mmit-0.1.0/mmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-24 21:07:45.000000 mmit-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 21:08:00.801251 mmit-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.801251 mmit-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:08:00.801251 mmit-0.1.0/tests/demo_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/demo_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/demo_blocks/classic_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/demo_blocks/classic_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/demo_blocks/cursed_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/test_base_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/test_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-24 21:07:45.000000 mmit-0.1.0/tests/test_end2end.py
```

### Comparing `mmit-0.0.4/.gitignore` & `mmit-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mmit-0.0.4/docs/Makefile` & `mmit-0.1.0/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
+SOURCEDIR     = source
+BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `mmit-0.0.4/docs/make.bat` & `mmit-0.1.0/docs/make.bat`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
-set SOURCEDIR=.
-set BUILDDIR=_build
+set SOURCEDIR=source
+set BUILDDIR=build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
```

### Comparing `mmit-0.0.4/mmit/decoders/unet/model.py` & `mmit-0.1.0/mmit/decoders/unet/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,71 @@
 from functools import partial
 from typing import List, Optional, Type
 
 import torch
 from torch import nn
 
+from mmit.base import mismatch as mm
 from mmit.base import upsamplers as up
 from mmit.factory import register
 
-from ..basedecoder import BaseDecoder, size_control
-from .parts import UpBlock
+from ..basedecoder import BaseDecoder
+from ..utils.resize import size_control
+from .parts import UBlock
 
 __all__ = ["UNet"]
 
-DEFAULT_CHANNELS = (256, 128, 64, 32, 16)
+DEFAULT_CHANNELS = (256, 128, 64, 32, 16, 8)
 
 
 @register
 class UNet(BaseDecoder):
+    """
+    Implementation of the U-Net decoder. Paper: https://arxiv.org/abs/1505.04597
+
+    Args:
+        input_channels: The channels of the input features.
+        input_reductions: The reduction factor of the input features.
+        decoder_channels: The channels on each layer of the decoder.
+        upsample_layer: Layer to use for the upsampling.
+        norm_layer: Normalization layer to use.
+        activation_layer: Activation function to use.
+        extra_layer: Addional layer to use.
+        mismatch_layer: Strategy to deal with odd resolutions.
+
+    """
+
     def __init__(
         self,
         input_channels: List[int],
         input_reductions: List[int],
         decoder_channels: Optional[List[int]] = None,
         upsample_layer: Type[nn.Module] = up.ConvTranspose2d,
         norm_layer: Type[nn.Module] = nn.BatchNorm2d,
-        activation: Type[nn.Module] = nn.ReLU,
+        activation_layer: Type[nn.Module] = nn.ReLU,
         extra_layer: Type[nn.Module] = nn.Identity,
+        mismatch_layer: Type[nn.Module] = mm.Pad,
     ):
-        super().__init__()
+        super().__init__(input_channels, input_reductions)
 
         if decoder_channels is None:
             decoder_channels = DEFAULT_CHANNELS[: len(input_channels) - 1]
 
         in_ch, skip_ch, out_ch = self._format_channels(input_channels, decoder_channels)
         up_lays = self._format_upsample_layers(input_reductions, upsample_layer)
 
-        specs = norm_layer, activation, extra_layer
+        specs = norm_layer, activation_layer, extra_layer, mismatch_layer
         blocks = []
 
         for ic, sc, oc, up_lay in zip(in_ch, skip_ch, out_ch, up_lays):
-            upblock = UpBlock(ic, sc, oc, up_lay, *specs)
-            blocks.append(upblock)
+            ublock = UBlock(ic, sc, oc, up_lay, *specs)
+            blocks.append(ublock)
 
         self.blocks = nn.ModuleList(blocks)
+        self._output_classes = out_ch[-1]
 
     @size_control
     def forward(self, *features: torch.Tensor) -> torch.Tensor:
         # Dropping the first channel since we don't use the input image
         features = features[1:]
 
         # Reversing the input channels since we're going from the bottom up
@@ -57,14 +76,18 @@
 
         for i, decoder_block in enumerate(self.blocks):
             skip = skips[i] if i < len(skips) else None
             x = decoder_block(x, skip)
 
         return x
 
+    @property
+    def out_classes(self) -> int:
+        return self._output_classes
+
     def _format_channels(self, input_channels, decoder_channels):
         # We drop the first channel since we don't use the input image
         input_channels = input_channels[1:]
 
         # We reverse the input channels since we're going from the bottom up
         input_channels = input_channels[::-1]
```

### Comparing `mmit-0.0.4/mmit/decoders/unet/parts.py` & `mmit-0.1.0/mmit/decoders/unet/parts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 from typing import Type
 
 import torch
-import torch.nn.functional as F
 from torch import nn
 
+from mmit.base import mismatch as mm
+from mmit.base import upsamplers as up
 
-class UpBlock(nn.Module):
+
+class UBlock(nn.Module):
     def __init__(
         self,
         in_channels: int,
         skip_channels: int,
         out_channels: int,
-        upsample_layer: Type[nn.Module] = nn.ConvTranspose2d,
+        upsample_layer: Type[nn.Module] = up.ConvTranspose2d,
         norm_layer: Type[nn.Module] = nn.BatchNorm2d,
         activation: Type[nn.Module] = nn.ReLU,
         extra_layer: Type[nn.Module] = nn.Identity,
+        mismatch_layer: Type[nn.Module] = mm.Pad,
     ):
         super().__init__()
 
         self.up = upsample_layer(in_channels)
 
         conv_channels = in_channels + skip_channels
         self.conv = DoubleConvBlock(conv_channels, out_channels, norm_layer, activation)
 
         self.extra_layer = extra_layer()
+        self.fix_mismatch = mismatch_layer()
 
     def forward(self, x, skip=None):
         x = self.up(x)
 
         if skip is not None:
-            x = self.concatenate(x, skip)
+            x, skip = self.fix_mismatch(x, skip)
+            x = torch.cat([x, skip], dim=1)
 
         x = self.extra_layer(x)
         x = self.conv(x)
         return x
 
-    def concatenate(self, x, skip):
-        x_size, skip_size = x.shape[2:], skip.shape[2:]
-
-        if x_size != skip_size:
-            x = F.interpolate(x, size=skip_size, mode="bilinear")
-
-        return torch.cat([x, skip], dim=1)
-
 
 class DoubleConvBlock(nn.Module):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         norm_layer: Type[nn.Module] = nn.BatchNorm2d,
```

### Comparing `mmit-0.0.4/mmit/decoders/unetplusplus/model.py` & `mmit-0.1.0/mmit/decoders/unetplusplus/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,79 @@
 from functools import partial
-from typing import Type
+from typing import List, Type
 
 import torch
 import torch.nn as nn
 
+from mmit.base import mismatch as mm
 from mmit.base import upsamplers as up
 from mmit.factory import register
 
-from ..basedecoder import BaseDecoder, size_control
-from ..unet.parts import UpBlock
+from ..basedecoder import BaseDecoder
+from ..unet.parts import UBlock
+from ..utils.resize import size_control
 
 __all__ = ["UNetPlusPlus"]
 
-DEFAULT_CHANNELS = (256, 128, 64, 32, 16)
+DEFAULT_CHANNELS = (256, 128, 64, 32, 16, 8)
 
 
 @register
 class UNetPlusPlus(BaseDecoder):
-    """UNet++ decoder implementation from https://arxiv.org/abs/1807.10165.
+    """
+    Implementation of the U-Net++ decoder. Paper: https://arxiv.org/abs/1807.10165.
 
     In this implementation, we follow the following naming convention referring to Figure 1.a in the paper:
         - `lidx` is the layer index, i.e. the index that spans horizontally.
         - `didx` is the depth index, i.e. the index that spans vertically.
         - `i_j` will be the key of the block that is at depth `i` and layer `j`.
         - `i_j` will also be the key of the resulting tensor after the block that is at depth `i` and layer `j`.
 
     Since we implement only the decoder, there will be no `i_0` blocks, and the `i_0` tensors will be the input tensors.
+
+    Args:
+        input_channels: The channels of the input features.
+        input_reductions: The reduction factor of the input features.
+        decoder_channels: The channels on each layer of the decoder.
+        upsample_layer: Layer to use for the upsampling.
+        norm_layer: Normalization layer to use.
+        activation_layer: Activation function to use.
+        extra_layer: Addional layer to use.
+        mismatch_layer: Strategy to deal with odd resolutions.
     """
 
     def __init__(
         self,
-        input_channels: list[int],
-        input_reductions: list[int],
-        decoder_channels: list[int] = None,
+        input_channels: List[int],
+        input_reductions: List[int],
+        decoder_channels: List[int] = None,
         upsample_layer: Type[nn.Module] = up.ConvTranspose2d,
         norm_layer: Type[nn.Module] = nn.BatchNorm2d,
-        activation: Type[nn.Module] = nn.ReLU,
+        activation_layer: Type[nn.Module] = nn.ReLU,
         extra_layer: Type[nn.Module] = nn.Identity,
+        mismatch_layer: Type[nn.Module] = mm.Pad,
     ):
-        super().__init__()
+        super().__init__(input_channels, input_reductions)
+
         self.depth = len(input_channels)
         if decoder_channels is None:
             decoder_channels = DEFAULT_CHANNELS[: self.depth - 1]
-            print(f"Using default decoder channels: {decoder_channels}")
 
         channels = self._format_channels(input_channels, decoder_channels)
         up_lays = self._format_upsample_layers(input_reductions, upsample_layer)
-        specs = norm_layer, activation, extra_layer
+        specs = norm_layer, activation_layer, extra_layer, mismatch_layer
 
         blocks = {}
         for key, (in_ch, skip_ch, out_ch) in channels.items():
             didx = int(key.split("_")[0])
             up_lay = up_lays[didx]
-            blocks[key] = UpBlock(in_ch, skip_ch, out_ch, up_lay, *specs)
+            blocks[key] = UBlock(in_ch, skip_ch, out_ch, up_lay, *specs)
 
         self.blocks = nn.ModuleDict(blocks)
+        self._out_classes = out_ch
 
     @size_control
     def forward(self, *features):
         features = self._preprocess_features(features)
         for lidx in range(1, self.depth):
             for didx in range(self.depth - lidx):
                 # Get the corresponding block
@@ -75,14 +90,18 @@
                 features[f"{didx}_{lidx}"] = output
 
         # The final output is the output of the last block
         final_output = features[f"0_{self.depth-1}"]
 
         return final_output
 
+    @property
+    def out_classes(self):
+        return self._out_classes
+
     def _preprocess_features(self, features):
         """Preprocess features by removing the first feature and reversing the order."""
         features = {f"{i}_0": f for i, f in enumerate(features)}
         return features
 
     def _format_channels(self, input_channels, decoder_channels):
         decoder_channels = decoder_channels[::-1]
```

### Comparing `mmit-0.0.4/mmit/encoders/basencoder.py` & `mmit-0.1.0/mmit/encoders/basencoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from __future__ import annotations
 
 import torch.nn as nn
 from torch import Tensor
 
 
 class BaseEncoder(nn.Module):
+    def __init__(
+        self,
+        pretrained: bool = True,
+        in_chans: int = 3,
+        out_indices: tuple = (0, 1, 2, 3, 4),
+        output_stride: int = 32,
+    ):
+        super().__init__()
+
     def forward(self, x: Tensor) -> list[Tensor]:
         """Forward pass of the encoder
 
         Args:
             x: Input tensor of shape (B, C, H, W)
 
         Returns:
-            A list of tensors of shape (B, C, H, W) with the features.
-            The first element is the input tensor.
+            A list of tensors of shape (B, C, H // fi, W // fi) with the features.
+            The first element is the input tensor, fi is the reduction factor of the i-th feature.
         """
         raise NotImplementedError
 
     @property
     def out_channels(self) -> tuple[int, ...]:
         """Number of channels of the output tensors"""
         raise NotImplementedError
```

### Comparing `mmit-0.0.4/mmit/encoders/timm/model.py` & `mmit-0.1.0/mmit/encoders/timm/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,30 +7,36 @@
 from ..basencoder import BaseEncoder
 
 __all__ = ["TimmEncoder"]
 
 
 @register
 class TimmEncoder(BaseEncoder):
-    """Wrapper for timm encoders. Inspired by segmentation_models_pytorch."""
+    """
+    Wrapper for timm encoders.
+
+    Args:
+        name: The name of the timm encoder.
+        pretrained: If True, returns a model pre-trained on ImageNet.
+        in_chans: The number of input channels.
+        out_indices: The indices of the layers to return.
+        output_stride: The output stride of the encoder.
+    """
 
     def __init__(
         self,
         name: str,
         pretrained: bool = True,
         in_chans: int = 3,
-        out_indices: int | tuple = 5,
+        out_indices: tuple = (0, 1, 2, 3, 4),
         output_stride: int = 32,
         **kwargs,
     ):
         super().__init__()
 
-        if isinstance(out_indices, (int, float)):
-            out_indices = tuple(range(out_indices))
-
         model_kwargs = {
             "pretrained": pretrained,
             "in_chans": in_chans,
             "features_only": True,
             "out_indices": out_indices,
         }
         model_kwargs.update(kwargs)
```

### Comparing `mmit-0.0.4/mmit/factory/registry.py` & `mmit-0.1.0/mmit/factory/registry.py`

 * *Files identical despite different names*

### Comparing `mmit-0.0.4/pyproject.toml` & `mmit-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 [project]
 name = "mmit"
 description = "A Python package for computer vision experiments and research."
 readme = "README.md"
 authors = [{ name = "Andrea Boscolo Camiletto", email = "abcamiletto@gmail.com" }]
 dependencies = [
     "timm>=0.9.0",
-    "torch>=1.9"
+    "torch>=1.10"
 ]
-requires-python = ">=3.9"
-version = "0.0.4"
+requires-python = ">=3.8"
+version = "0.1.0"
 
 [project.urls]
 Homepage = "https://github.com/abcamiletto/mmit"
 Repository = "https://github.com/abcamiletto/mmit"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pytest", "pytest-cov", "pytest-lazy-fixture", "pre-commit"]
-docs = ["sphinx",
+docs = ["sphinx==6.2.1",
         "sphinx-autobuild",
         "sphinx-rtd-theme",
         "sphinxcontrib.spelling",
         "sphinx-autodoc-typehints",
-        "sphinx_copybutton"
+        "sphinx_copybutton",
+        "sphinx-autoapi",
+        "myst-parser"
 ]
 
 [tool.setuptools.packages.find]
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
 [tool.ruff]
 line-length = 120
```

### Comparing `mmit-0.0.4/tests/test_encoders_decoders.py` & `mmit-0.1.0/tests/test_decoders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 import pytest
 import torch
-from conftest import DECODERS, TIMM_ENCODERS
+from conftest import DECODERS, TEST_ENCODERS
 
 import mmit
 
 
-@pytest.mark.parametrize("encoder_name", TIMM_ENCODERS)
+@pytest.mark.parametrize("encoder_name", TEST_ENCODERS)
 @pytest.mark.parametrize("decoder_name", DECODERS)
 def test_timm_encoder_decoder(encoder_name, decoder_name):
     """Test that the timm encoder and decoder work together."""
     encoder = mmit.create_encoder(encoder_name, pretrained=False)
     decoder = mmit.create_decoder(decoder_name)
 
     x = torch.randn(2, 3, 256, 256)
     with torch.no_grad():
         features = encoder(x)
         out = decoder(*features)
 
     assert out.shape[-2:] == x.shape[-2:]
+    assert out.shape[1] == decoder.out_classes
 
 
-@pytest.mark.parametrize("encoder_name", TIMM_ENCODERS)
+@pytest.mark.parametrize("encoder_name", TEST_ENCODERS)
 @pytest.mark.parametrize("decoder_name", DECODERS)
 @pytest.mark.parametrize("input_shape", [(151, 210), (87, 141)])
 def test_timm_encoder_decoder_awful_shape(encoder_name, decoder_name, input_shape):
     """Test that the timm encoder and decoder work together."""
     encoder = mmit.create_encoder(encoder_name, pretrained=False)
     decoder = mmit.create_decoder(decoder_name)
 
     x = torch.randn(2, 3, *input_shape)
     with torch.no_grad():
         features = encoder(x)
         out = decoder(*features)
 
     assert out.shape[-2:] == x.shape[-2:]
+    assert out.shape[1] == decoder.out_classes
 
 
-@pytest.mark.parametrize("encoder_name", TIMM_ENCODERS)
+@pytest.mark.parametrize("encoder_name", TEST_ENCODERS)
 @pytest.mark.parametrize("decoder_name", DECODERS)
 def test_timm_encoder_layers_stride_decoder(encoder_name, decoder_name):
     """Test that the timm encoder and decoder work together."""
     encoder = mmit.create_encoder(
         encoder_name, pretrained=False, out_indices=(0, 3, 4), output_stride=8
     )
     decoder = mmit.create_decoder(decoder_name)
 
     x = torch.randn(2, 3, 256, 256)
     with torch.no_grad():
         features = encoder(x)
         out = decoder(*features)
 
     assert out.shape[-2:] == x.shape[-2:]
+    assert out.shape[1] == decoder.out_classes
```

