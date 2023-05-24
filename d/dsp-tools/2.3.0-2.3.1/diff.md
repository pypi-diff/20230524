# Comparing `tmp/dsp_tools-2.3.0.tar.gz` & `tmp/dsp_tools-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-2.3.0.tar", max compression
+gzip compressed data, was "dsp_tools-2.3.1.tar", max compression
```

## Comparing `dsp_tools-2.3.0.tar` & `dsp_tools-2.3.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    35149 2023-05-17 07:10:03.642256 dsp_tools-2.3.0/LICENSE
--rw-r--r--   0        0        0     4373 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/docs/index.md
--rw-r--r--   0        0        0     5142 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0    20021 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/dsp_tools.py
--rw-r--r--   0        0        0    82249 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/excel2xml.py
--rw-r--r--   0        0        0        0 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/__init__.py
--rw-r--r--   0        0        0    29584 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/process_files.py
--rw-r--r--   0        0        0    14430 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/upload_files.py
--rw-r--r--   0        0        0     4157 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/upload_xml.py
--rw-r--r--   0        0        0        0 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      962 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/bitstream.py
--rw-r--r--   0        0        0     9766 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/connection.py
--rw-r--r--   0        0        0     3203 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     9472 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/group.py
--rw-r--r--   0        0        0    16923 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/helpers.py
--rw-r--r--   0        0        0     9810 2023-05-17 07:10:03.658257 dsp_tools-2.3.0/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0    23044 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/listnode.py
--rw-r--r--   0        0        0      506 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/model.py
--rw-r--r--   0        0        0    19744 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/ontology.py
--rw-r--r--   0        0        0     2972 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/permission.py
--rw-r--r--   0        0        0    19120 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/project.py
--rw-r--r--   0        0        0     1930 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0    21101 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/propertyclass.py
--rw-r--r--   0        0        0     1896 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/propertyelement.py
--rw-r--r--   0        0        0    22008 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/resource.py
--rw-r--r--   0        0        0    34520 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/resourceclass.py
--rw-r--r--   0        0        0      419 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/set_encoder.py
--rw-r--r--   0        0        0      890 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/sipi.py
--rw-r--r--   0        0        0    27302 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/user.py
--rw-r--r--   0        0        0    34694 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/value.py
--rw-r--r--   0        0        0     2153 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlallow.py
--rw-r--r--   0        0        0      747 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlbitstream.py
--rw-r--r--   0        0        0      254 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlerror.py
--rw-r--r--   0        0        0     1841 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlpermission.py
--rw-r--r--   0        0        0     2371 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlproperty.py
--rw-r--r--   0        0        0     8874 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlresource.py
--rw-r--r--   0        0        0     2614 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/models/xmlvalue.py
--rw-r--r--   0        0        0     1488 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    23543 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2023-05-17 07:10:03.662257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42584 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32171 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0     2867 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0        0 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0    15112 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_lists.py
--rw-r--r--   0        0        0     4891 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_project.py
--rw-r--r--   0        0        0     7837 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_properties.py
--rw-r--r--   0        0        0    10214 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_resources.py
--rw-r--r--   0        0        0     1170 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/generate_templates.py
--rw-r--r--   0        0        0     3179 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/id_to_iri.py
--rw-r--r--   0        0        0    41148 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/project_create.py
--rw-r--r--   0        0        0     8048 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/project_create_lists.py
--rw-r--r--   0        0        0     4578 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/project_get.py
--rw-r--r--   0        0        0    18834 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/project_validate.py
--rw-r--r--   0        0        0     4265 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/rosetta.py
--rw-r--r--   0        0        0    12854 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0     6838 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/stack_handling.py
--rw-r--r--   0        0        0    50915 2023-05-17 07:10:03.666257 dsp_tools-2.3.0/src/dsp_tools/utils/xml_upload.py
--rw-r--r--   0        0        0     5725 1970-01-01 00:00:00.000000 dsp_tools-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-24 07:58:06.593740 dsp_tools-2.3.1/LICENSE
+-rw-r--r--   0        0        0     4373 2023-05-24 07:58:06.609734 dsp_tools-2.3.1/docs/index.md
+-rw-r--r--   0        0        0     4916 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0    19989 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/dsp_tools.py
+-rw-r--r--   0        0        0    82048 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/excel2xml.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/__init__.py
+-rw-r--r--   0        0        0    29477 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/process_files.py
+-rw-r--r--   0        0        0    14393 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/upload_files.py
+-rw-r--r--   0        0        0     4148 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      962 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/bitstream.py
+-rw-r--r--   0        0        0     9760 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/connection.py
+-rw-r--r--   0        0        0     3197 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     9538 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/group.py
+-rw-r--r--   0        0        0    16915 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/helpers.py
+-rw-r--r--   0        0        0     9810 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0    23066 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/listnode.py
+-rw-r--r--   0        0        0      506 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/model.py
+-rw-r--r--   0        0        0    19744 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/ontology.py
+-rw-r--r--   0        0        0     2972 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/permission.py
+-rw-r--r--   0        0        0    19128 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/project.py
+-rw-r--r--   0        0        0     1930 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0    21129 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/propertyclass.py
+-rw-r--r--   0        0        0     1896 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/propertyelement.py
+-rw-r--r--   0        0        0    22134 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/resource.py
+-rw-r--r--   0        0        0    34527 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/resourceclass.py
+-rw-r--r--   0        0        0      419 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/set_encoder.py
+-rw-r--r--   0        0        0      890 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/sipi.py
+-rw-r--r--   0        0        0    27302 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/user.py
+-rw-r--r--   0        0        0    34725 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/value.py
+-rw-r--r--   0        0        0     2153 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/xmlallow.py
+-rw-r--r--   0        0        0      747 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlbitstream.py
+-rw-r--r--   0        0        0      254 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlerror.py
+-rw-r--r--   0        0        0     1841 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlpermission.py
+-rw-r--r--   0        0        0     2371 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlproperty.py
+-rw-r--r--   0        0        0     8874 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlresource.py
+-rw-r--r--   0        0        0     2614 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlvalue.py
+-rw-r--r--   0        0        0     1488 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    23543 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42584 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32171 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0     2867 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0        0 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0    15096 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_lists.py
+-rw-r--r--   0        0        0     4828 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_project.py
+-rw-r--r--   0        0        0     7818 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_properties.py
+-rw-r--r--   0        0        0    10202 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_resources.py
+-rw-r--r--   0        0        0     1170 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/generate_templates.py
+-rw-r--r--   0        0        0     3174 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/id_to_iri.py
+-rw-r--r--   0        0        0    40875 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/project_create.py
+-rw-r--r--   0        0        0     8032 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/project_create_lists.py
+-rw-r--r--   0        0        0     4617 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/project_get.py
+-rw-r--r--   0        0        0    18724 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/project_validate.py
+-rw-r--r--   0        0        0     4242 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/rosetta.py
+-rw-r--r--   0        0        0    12829 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0     6830 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/stack_handling.py
+-rw-r--r--   0        0        0    51407 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/xml_upload.py
+-rw-r--r--   0        0        0     5677 1970-01-01 00:00:00.000000 dsp_tools-2.3.1/PKG-INFO
```

### Comparing `dsp_tools-2.3.0/LICENSE` & `dsp_tools-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/docs/index.md` & `dsp_tools-2.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/pyproject.toml` & `dsp_tools-2.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # See https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 
 [tool.poetry]
 name = "dsp-tools"
-version = "2.3.0"
+version = "2.3.1"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 documentation = "https://docs.dasch.swiss/latest/DSP-TOOLS/"
 homepage = "https://www.dasch.swiss/"
 repository = "https://github.com/dasch-swiss/dsp-tools"
-include = [
-    "src/dsp_tools/resources/*"
-]
-exclude = [
-    "src/dsp_tools/import_scripts/*"
-]
+include = ["src/dsp_tools/resources/*"]
+exclude = ["src/dsp_tools/import_scripts/*"]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 jsonpath-ng = "^1.5.3"
 argparse = "^1.4.0"
 lxml = "^4.9.2"
@@ -49,36 +45,32 @@
 types-lxml = "^2023.3.28"
 types-jsonschema = "^4.17.0.8"
 types-openpyxl = "^3.1.0.7"
 types-regex = "^2023.5.5.0"
 
 
 [tool.poetry.scripts]
-# definition of the entry point
-dsp-tools = "dsp_tools.dsp_tools:main"
+dsp-tools = "dsp_tools.dsp_tools:main"    # definition of the CLI entry point
 
 
 [tool.poetry-exec-plugin.commands]
-# plugin (https://github.com/keattang/poetry-exec-plugin) to define commands available for the developers
-# e.g. `poetry exec check-links`
+# plugin (https://github.com/keattang/poetry-exec-plugin) to define commands available for the developers, e.g. `poetry exec check-links`
 check-links = "markdown-link-validator ./docs -i \\.\\/assets\\/.+ -i .+github\\.com\\/dasch\\-swiss\\/dsp-tools\\/settings"
 
 
 [build-system]
 # Tells “frontend” build tools (like pip, build, or poetry) what “backend” build tool to use (e.g. setuptools, poetry).
 # The "backend" doesn't need to be installed. It will be installed by the "frontend" in a temporary, isolated
 # environment for use during the build process.
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
+addopts = ["--import-mode=importlib"]
 # see https://docs.pytest.org/en/latest/explanation/goodpractices.html#tests-outside-application-code
 
 
 [tool.autopep8]
 max_line_length = 150
 experimental = true
 
@@ -86,29 +78,24 @@
 [tool.mypy]
 ignore_missing_imports = true              # TODO: deactivate this
 show_column_numbers = true
 strict = true
 exclude = [
     "src/dsp_tools/models",                # TODO: activate this
     "src/dsp_tools/import_scripts",        # TODO: activate this
-    "test/e2e",                            # TODO: activate this
 ]
 
 
 [tool.isort]
 multi_line_output = 3
 known_first_party = ["dsp_tools"]
 
 
 [tool.pylint.MASTER]
-ignore-paths = [
-    "src/dsp_tools/models/.*$",            # TODO: activate this
-    "src/dsp_tools/import_scripts/.*$",    # TODO: activate this
-    "test/e2e/.*$"                         # TODO: activate this
-]
+ignore-paths = ["src/dsp_tools/models/.*$"] # TODO: activate this
 suggestion-mode = true
 
 
 [tool.pylint.format]
 max-line-length = 150
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/dsp_tools.py` & `dsp_tools-2.3.1/src/dsp_tools/dsp_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,25 +55,25 @@
 
     # make a parser
     parser = argparse.ArgumentParser(description=f"DSP-TOOLS (version {version('dsp-tools')}, © {datetime.datetime.now().year} by DaSCH)")
     subparsers = parser.add_subparsers(title="Subcommands", description="Valid subcommands are", help="sub-command help")
 
     # create
     parser_create = subparsers.add_parser(
-        name="create", 
+        name="create",
         help="Create a project defined in a JSON project file on a DSP server. "
              "A project can consist of lists, groups, users, and ontologies (data models)."
     )
     parser_create.set_defaults(action="create")
     parser_create.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
     parser_create.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_create.add_argument("-p", "--password", default=default_pw, help=password_text)
-    parser_create.add_argument("-V", "--validate-only", action="store_true", 
+    parser_create.add_argument("-V", "--validate-only", action="store_true",
                                help="validate the JSON file without creating it on the DSP server")
-    parser_create.add_argument("-l", "--lists-only", action="store_true", 
+    parser_create.add_argument("-l", "--lists-only", action="store_true",
                                help="create only the lists (prerequisite: the project exists on the server)")
     parser_create.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_create.add_argument("-d", "--dump", action="store_true", help="dump test files for DSP-API requests")
     parser_create.add_argument("project_definition", help="path to the JSON project file")
 
     # get
     parser_get = subparsers.add_parser(name="get", help="Retrieve a project with its data model(s) from a DSP server and write it into a JSON file")
@@ -87,18 +87,18 @@
 
     # xmlupload
     parser_upload = subparsers.add_parser(name="xmlupload", help="Upload data defined in an XML file to a DSP server")
     parser_upload.set_defaults(action="xmlupload")
     parser_upload.add_argument("-s", "--server", default=default_dsp_api_url, help="URL of the DSP server where DSP-TOOLS sends the data to")
     parser_upload.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_upload.add_argument("-p", "--password", default=default_pw, help=password_text)
-    parser_upload.add_argument("-S", "--sipi", default=default_sipi, 
+    parser_upload.add_argument("-S", "--sipi", default=default_sipi,
                                help="URL of the SIPI server where DSP-TOOLS sends the multimedia files to")
     parser_upload.add_argument("-i", "--imgdir", default=".", help="folder from where the paths in the <bitstream> tags are evaluated")
-    parser_upload.add_argument("-I", "--incremental", action="store_true", 
+    parser_upload.add_argument("-I", "--incremental", action="store_true",
                                help="The links in the XML file point to IRIs (on the server) instead of IDs (in the same XML file).")
     parser_upload.add_argument("-V", "--validate", action="store_true", help="validate the XML file without uploading it")
     parser_upload.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_upload.add_argument("-m", "--metrics", action="store_true", help="write metrics into a 'metrics' folder")
     parser_upload.add_argument("xmlfile", help="path to the XML file containing the data")
 
     # process-files
@@ -156,43 +156,43 @@
     parser_excel_lists.set_defaults(action="excel2lists")
     parser_excel_lists.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_excel_lists.add_argument("excelfolder", help="path to the folder containing the Excel file(s)")
     parser_excel_lists.add_argument("lists_section", help="path to the output JSON file containing the 'lists' section")
 
     # excel2resources
     parser_excel_resources = subparsers.add_parser(
-        name="excel2resources", 
+        name="excel2resources",
         help="Create the 'resources' section of a JSON project file from one or multiple Excel files"
     )
     parser_excel_resources.set_defaults(action="excel2resources")
     parser_excel_resources.add_argument("excelfile", help="path to the Excel file containing the resources")
     parser_excel_resources.add_argument("resources_section", help="path to the output JSON file containing the 'resources' section")
 
     # excel2properties
     parser_excel_properties = subparsers.add_parser(
-        name="excel2properties", 
+        name="excel2properties",
         help="Create the 'properties' section of a JSON project file from one or multiple Excel files"
     )
     parser_excel_properties.set_defaults(action="excel2properties")
     parser_excel_properties.add_argument("excelfile", help="path to the Excel file containing the properties")
     parser_excel_properties.add_argument("properties_section", help="path to the output JSON file containing the 'properties' section")
 
     # excel2xml
     parser_excel2xml = subparsers.add_parser(
-        name="excel2xml", 
+        name="excel2xml",
         help="Create an XML file from an Excel/CSV file that is already structured according to the DSP specifications"
     )
     parser_excel2xml.set_defaults(action="excel2xml")
     parser_excel2xml.add_argument("data_source", help="path to the CSV or XLS(X) file containing the data")
     parser_excel2xml.add_argument("project_shortcode", help="shortcode of the project that this data belongs to")
     parser_excel2xml.add_argument("ontology_name", help="name of the ontology that this data belongs to")
 
     # id2iri
     parser_id2iri = subparsers.add_parser(
-        name="id2iri", 
+        name="id2iri",
         help="Replace internal IDs in contained in the <resptr> tags of an XML file by IRIs provided in a mapping file"
     )
     parser_id2iri.set_defaults(action="id2iri")
     parser_id2iri.add_argument("--outfile", help="path to the XML output file containing the replaced IDs")
     parser_id2iri.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_id2iri.add_argument("xmlfile", help="path to the XML file containing the data to be replaced")
     parser_id2iri.add_argument("mapping", help="path to the JSON file containing the mapping of IDs to IRIs")
@@ -202,38 +202,38 @@
     parser_stackup.set_defaults(action="start-stack")
     parser_stackup.add_argument("--max_file_size", type=int, help="max. multimedia file size allowed by SIPI, in MB (default: 250, max: 100'000)")
     parser_stackup.add_argument("--prune", action="store_true", help="execute 'docker system prune' without asking")
     parser_stackup.add_argument("--no-prune", action="store_true", help="don't execute 'docker system prune' (and don't ask)")
 
     # shutdown DSP-API
     parser_stackdown = subparsers.add_parser(
-        name="stop-stack", 
+        name="stop-stack",
         help="Shut down the local instance of DSP-API and DSP-APP, and delete all data in it"
     )
     parser_stackdown.set_defaults(action="stop-stack")
 
     # create template repo with minimal JSON and XML files
     parser_template = subparsers.add_parser(
-        name="template", 
+        name="template",
         help="Create a template repository with a minimal JSON and XML file"
     )
     parser_template.set_defaults(action="template")
 
     # clone rosetta
     parser_rosetta = subparsers.add_parser(
-        name="rosetta", 
+        name="rosetta",
         help="Clone the most up to data rosetta repository, create the data model and upload the data"
     )
     parser_rosetta.set_defaults(action="rosetta")
 
     return parser
 
 
 def call_requested_action(
-    user_args: list[str], 
+    user_args: list[str],
     parser: argparse.ArgumentParser,
     logger: logging.Logger
 ) -> bool:
     """
     With the help of the parser, parse the user arguments and call the appropriate method of DSP-TOOLS.
 
     Args:
@@ -241,27 +241,27 @@
         parser: parser to parse the user arguments
         logger: the logger for this module
 
     Raises:
         BaseError from the called methods
         UserError from the called methods
         unexpected errors from the called methods and underlying libraries
-    
+
     Returns:
         success status
     """
     args = parser.parse_args(user_args)
     if not hasattr(args, "action"):
         parser.print_help(sys.stderr)
         sys.exit(1)
-    
+
     logger.info("*****************************************************************************************")
     logger.info(f"***Called DSP-TOOLS action '{args.action}' from command line with these parameters: {args}")
     logger.info("*****************************************************************************************")
-    
+
     if args.action == "create":
         if args.lists_only:
             if args.validate_only:
                 success = validate_lists_section_with_schema(path_to_json_project_file=args.project_definition)
                 print("'Lists' section of the JSON project file is syntactically correct and passed validation.")
             else:
                 _, success = create_lists(
@@ -401,26 +401,26 @@
                 filename=Path.home() / Path(".dsp-tools") / "logging.log",
                 maxBytes=3*1024*1024,
                 backupCount=1
             )
         ]
     )
     logger = logging.getLogger(__name__)
-    
+
     parser = make_parser()
     try:
         success = call_requested_action(
-            user_args=sys.argv[1:], 
-            parser=parser, 
+            user_args=sys.argv[1:],
+            parser=parser,
             logger=logger
         )
     except UserError as err:
         print(err.message)
         sys.exit(1)
     # let BaseError and all unexpected errors escalate, so that a stack trace is printed
 
-    if not success: 
+    if not success:
         sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/excel2xml.py` & `dsp_tools-2.3.1/src/dsp_tools/excel2xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 import pandas as pd
 import regex
 from lxml import etree
 from lxml.builder import E  # pylint: disable=no-name-in-module
 
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import DateTimeStamp
-# explicitly export PropertyElement, so that API users can import it from this module 
+# explicitly export PropertyElement, so that API users can import it from this module
 # (see https://mypy.readthedocs.io/en/stable/command_line.html#cmdoption-mypy-no-implicit-reexport)
-# doing this requires silencing the corresponding pylint warning 
+# doing this requires silencing the corresponding pylint warning
 # (see https://pylint.readthedocs.io/en/latest/user_guide/messages/convention/useless-import-alias.html)
 from dsp_tools.models.propertyelement import \
     PropertyElement as PropertyElement  # pylint: disable=useless-import-alias
 from dsp_tools.models.value import UriValue
-from dsp_tools.utils.shared import (
-    check_notna,
-    simplify_name,
-    validate_xml_against_schema
-)
+from dsp_tools.utils.shared import \
+    check_notna as check_notna  # pylint: disable=useless-import-alias
+from dsp_tools.utils.shared import \
+    simplify_name as simplify_name  # pylint: disable=useless-import-alias
+from dsp_tools.utils.shared import validate_xml_against_schema
 
 xml_namespace_map = {
     None: "https://dasch.swiss/schema",
     "xsi": "http://www.w3.org/2001/XMLSchema-instance"
 }
 
 
@@ -185,28 +185,32 @@
     sep_regex = r"[\./]"
     lookbehind = r"(?<![0-9A-Za-z])"
     lookahead = r"(?![0-9A-Za-z])"
 
     # template: 2021-01-01 | 2015_01_02
     iso_date = re.search(fr"{lookbehind}{year_regex}[_-]([0-1][0-9])[_-]([0-3][0-9]){lookahead}", string)
     # template: 6.-8.3.1948 | 6/2/1947 - 24.03.1948
-    eur_date_range = re.search(fr"{lookbehind}{day_regex}{sep_regex}(?:{month_regex}{sep_regex}{year_regex}?)? ?(?:-|:|to) ?"
-                               fr"{day_regex}{sep_regex}{month_regex}{sep_regex}{year_regex}{lookahead}", string)
+    eur_date_range = re.search(
+        pattern=fr"{lookbehind}{day_regex}{sep_regex}(?:{month_regex}{sep_regex}{year_regex}?)? ?(?:-|:|to) ?"
+                fr"{day_regex}{sep_regex}{month_regex}{sep_regex}{year_regex}{lookahead}",
+        string=string
+    )
     # template: 1.4.2021 | 5/11/2021
     eur_date = re.search(fr"{lookbehind}{day_regex}{sep_regex}{month_regex}{sep_regex}{year_regex}{lookahead}", string)
     # template: March 9, 1908 | March5,1908 | May 11, 1906
     monthname_date = re.search(
-        fr"{lookbehind}(January|Jan|February|Feb|March|Mar|April|Apr|May|June|Jun|July|Jul|August|Aug|September|Sept|"
-        fr"October|Oct|November|Nov|December|Dec) ?{day_regex}, ?{year_regex}{lookahead}", string)
+        pattern=fr"{lookbehind}(January|Jan|February|Feb|March|Mar|April|Apr|May|June|Jun|July|Jul|August|Aug|September|Sept|"
+                fr"October|Oct|November|Nov|December|Dec) ?{day_regex}, ?{year_regex}{lookahead}",
+        string=string
+    )
     # template: 1849/50 | 1849-50 | 1849/1850
-    year_range = re.search(lookbehind + year_regex + r"[/-](\d{2}|\d{4})" +lookahead, string)
+    year_range = re.search(lookbehind + year_regex + r"[/-](\d{2}|\d{4})" + lookahead, string)
     # template: 1907
     year_only = re.search(fr"{lookbehind}{year_regex}{lookahead}", string)
 
-
     if iso_date:
         year = int(iso_date.group(1))
         month = int(iso_date.group(2))
         day = int(iso_date.group(3))
         try:
             startdate = datetime.date(year, month, day)
             enddate = startdate
@@ -306,16 +310,15 @@
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#the-root-element-knora
     """
 
     root = etree.Element(
         "{%s}knora" % (xml_namespace_map[None]),
         attrib={
             str(etree.QName("http://www.w3.org/2001/XMLSchema-instance", "schemaLocation")):
-                "https://dasch.swiss/schema " + \
-                "https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/data.xsd",
+                "https://dasch.swiss/schema https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/data.xsd",
             "shortcode": shortcode,
             "default-ontology": default_ontology
         },
         nsmap=xml_namespace_map
     )
     return root
 
@@ -417,22 +420,21 @@
         "nsmap": xml_namespace_map
     }
     if ark:
         kwargs["ark"] = ark
     if iri:
         kwargs["iri"] = iri
     if ark and iri:
-        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.",
-                      stacklevel=2)
+        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.", stacklevel=2)
     if creation_date:
         try:
             DateTimeStamp(creation_date)
         except BaseError:
-            raise BaseError(f"The resource '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. Did "
-                            f"you perhaps forget the timezone?") from None
+            raise BaseError(f"The resource '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
+                            f"Did you perhaps forget the timezone?") from None
         kwargs["creation_date"] = creation_date
 
     resource_ = etree.Element(
         "{%s}resource" % (xml_namespace_map[None]),
         **kwargs  # type: ignore
     )
     return resource_
@@ -462,19 +464,21 @@
         >>> resource.append(make_bitstream_prop("data/images/tree.jpg"))
         >>> root.append(resource)
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#bitstream
     """
 
     if not os.path.isfile(path):
-        warnings.warn(f"Failed validation in bitstream tag of resource '{calling_resource}': The following path "
-                      f"doesn't point to a file: {path}",
+        warnings.warn(f"Failed validation in bitstream tag of resource '{calling_resource}': The following path doesn't point to a file: {path}",
                       stacklevel=2)
-    prop_ = etree.Element("{%s}bitstream" % (xml_namespace_map[None]), permissions=permissions,
-                          nsmap=xml_namespace_map)
+    prop_ = etree.Element(
+        "{%s}bitstream" % (xml_namespace_map[None]),
+        permissions=permissions,
+        nsmap=xml_namespace_map
+    )
     prop_.text = str(path)
     return prop_
 
 
 def _format_bool(unformatted: Union[bool, str, int], name: str, calling_resource: str) -> str:
     """
     This method takes an unformatted boolean-like value, and transforms it into the string values "true" or "false".
@@ -493,16 +497,15 @@
     if isinstance(unformatted, str):
         unformatted = unformatted.lower()
     if unformatted in (False, "false", "0", 0, "no"):
         return "false"
     elif unformatted in (True, "true", "1", 1, "yes"):
         return "true"
     else:
-        raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                        f"'{unformatted}' is not a valid boolean.")
+        raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': '{unformatted}' is not a valid boolean.")
 
 
 def make_boolean_prop(
     name: str,
     value: Union[PropertyElement, str, int, bool],
     calling_resource: str = ""
 ) -> etree._Element:
@@ -540,16 +543,15 @@
 
     # validate input
     if isinstance(value, PropertyElement):
         value_new = dataclasses.replace(value, value=_format_bool(value.value, name, calling_resource))  # type: ignore
     elif isinstance(value, (str, bool, int)):
         value_new = PropertyElement(_format_bool(value, name, calling_resource))
     else:
-        raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                        f"'{value}' is not a valid boolean.")
+        raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': '{value}' is not a valid boolean.")
 
     # make xml structure of the value
     prop_ = etree.Element(
         "{%s}boolean-prop" % (xml_namespace_map[None]),
         name=name,
         nsmap=xml_namespace_map
     )
@@ -607,16 +609,15 @@
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
     for val in values:
         if not re.search(r"^#[0-9a-f]{6}$", str(val.value).strip(), flags=re.IGNORECASE):
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid color.")
+            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': '{val.value}' is not a valid color.")
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}color-prop" % (xml_namespace_map[None]),
         name=name,
         nsmap=xml_namespace_map
     )
@@ -680,18 +681,19 @@
     """
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
     for val in values:
-        if not re.search(r"^(GREGORIAN:|JULIAN:)?(CE:|BCE:)?(\d{4})(-\d{1,2})?(-\d{1,2})?"
-                         r"((:CE|:BCE)?(:\d{4})(-\d{1,2})?(-\d{1,2})?)?$", str(val.value).strip()):
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid DSP date.")
+        if not re.search(
+            pattern=r"^(GREGORIAN:|JULIAN:)?(CE:|BCE:)?(\d{4})(-\d{1,2})?(-\d{1,2})?((:CE|:BCE)?(:\d{4})(-\d{1,2})?(-\d{1,2})?)?$",
+            string=str(val.value).strip()
+        ):
+            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': '{val.value}' is not a valid DSP date.")
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}date-prop" % (xml_namespace_map[None]),
         name=name,
         nsmap=xml_namespace_map
     )
@@ -1478,22 +1480,21 @@
         "nsmap": xml_namespace_map
     }
     if ark:
         kwargs["ark"] = ark
     if iri:
         kwargs["iri"] = iri
     if ark and iri:
-        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.",
-                      stacklevel=2)
+        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.", stacklevel=2)
     if creation_date:
         try:
             DateTimeStamp(creation_date)
         except BaseError:
-            raise BaseError(f"The region '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. Did "
-                            f"you perhaps forget the timezone?") from None
+            raise BaseError(f"The region '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
+                            f"Did you perhaps forget the timezone?") from None
         kwargs["creation_date"] = creation_date
 
     region_ = etree.Element(
         "{%s}region" % (xml_namespace_map[None]),
         **kwargs  # type: ignore
     )
     return region_
@@ -1537,22 +1538,21 @@
         "nsmap": xml_namespace_map
     }
     if ark:
         kwargs["ark"] = ark
     if iri:
         kwargs["iri"] = iri
     if ark and iri:
-        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.",
-                      stacklevel=2)
+        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.", stacklevel=2)
     if creation_date:
         try:
             DateTimeStamp(creation_date)
         except BaseError:
-            raise BaseError(f"The annotation '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. Did "
-                            f"you perhaps forget the timezone?") from None
+            raise BaseError(f"The annotation '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
+                            f"Did you perhaps forget the timezone?") from None
         kwargs["creation_date"] = creation_date
 
     annotation_ = etree.Element(
         "{%s}annotation" % (xml_namespace_map[None]),
         **kwargs  # type: ignore
     )
     return annotation_
@@ -1596,22 +1596,21 @@
         "nsmap": xml_namespace_map
     }
     if ark:
         kwargs["ark"] = ark
     if iri:
         kwargs["iri"] = iri
     if ark and iri:
-        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.",
-                      stacklevel=2)
+        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.", stacklevel=2)
     if creation_date:
         try:
             DateTimeStamp(creation_date)
         except BaseError:
-            raise BaseError(f"The link '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. Did "
-                            f"you perhaps forget the timezone?") from None
+            raise BaseError(f"The link '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
+                            f"Did you perhaps forget the timezone?") from None
         kwargs["creation_date"] = creation_date
 
     link_ = etree.Element(
         "{%s}link" % (xml_namespace_map[None]),
         **kwargs  # type: ignore
     )
     return link_
@@ -1682,27 +1681,27 @@
             json_subset = elem["nodes"]
     json_values = set(_nested_dict_values_iterator(json_subset))
 
     # build dictionary with the mapping, based on string similarity
     res = dict()
     for excel_value in excel_values_new:
         excel_value_corrected = corrections.get(excel_value, excel_value)
-        excel_value_simpl = simplify_name(excel_value_corrected)  #increase match probability by removing illegal chars
+        excel_value_simpl = simplify_name(excel_value_corrected)  # increase match probability by removing illegal chars
         matches: list[str] = difflib.get_close_matches(
             word=excel_value_simpl,
             possibilities=json_values,
             n=1,
             cutoff=0.6
         )
         if matches:
             res[excel_value] = matches[0]
             res[excel_value.lower()] = matches[0]
         else:
-            warnings.warn(f"Did not find a close match to the excel list entry '{excel_value}' among the values "
-                          f"in the JSON project list '{list_name}'", stacklevel=2)
+            warnings.warn(f"Did not find a close match to the excel list entry '{excel_value}' "
+                          f"among the values in the JSON project list '{list_name}'", stacklevel=2)
 
     return res
 
 
 def _nested_dict_values_iterator(dicts: list[dict[str, Any]]) -> Iterable[str]:
     """
     This function accepts a list of nested dictionaries as argument
@@ -1791,16 +1790,15 @@
     xml_string = xml_string.replace("\'", "'")
     with open(filepath, "w", encoding="utf-8") as f:
         f.write(xml_string)
     try:
         validate_xml_against_schema(input_file=filepath)
         print(f"The XML file was successfully saved to {filepath}")
     except BaseError as err:
-        warnings.warn(f"The XML file was successfully saved to {filepath}, but the following Schema validation "
-                      f"error(s) occurred: {err.message}")
+        warnings.warn(f"The XML file was successfully saved to {filepath}, but the following Schema validation error(s) occurred: {err.message}")
 
 
 def excel2xml(datafile: str, shortcode: str, default_ontology: str) -> bool:
     """
     This is a method that is called from the command line. It isn't intended to be used in a Python script. It takes a
     tabular data source in CSV/XLS(X) format that is formatted according to the specifications, and transforms it to DSP-
     conforming XML file that can be uploaded to a DSP server with the xmlupload command. The output file is saved in the
@@ -1812,15 +1810,15 @@
     Args:
         datafile: path to the data file (CSV or XLS(X))
         shortcode: shortcode of the project that this data belongs to
         default_ontology: name of the ontology that this data belongs to
 
     Raises:
         BaseError if something went wrong
-    
+
     Returns:
         True if everything went well, False otherwise
     """
 
     # general preparation
     # -------------------
     success = True
@@ -1863,16 +1861,16 @@
     # create all resources
     # --------------------
     resource = None
     for index, row in main_df.iterrows():
 
         # there are two cases: either the row is a resource-row or a property-row.
         if not xor(check_notna(row.get("id")), check_notna(row.get("prop name"))):
-            raise BaseError(f"Exactly 1 of the 2 columns 'id' and 'prop name' must have an entry. Excel row no. "
-                            f"{int(str(index)) + 2} has too many/too less entries:\n"
+            raise BaseError(f"Exactly 1 of the 2 columns 'id' and 'prop name' must have an entry. "
+                            f"Excel row no. {int(str(index)) + 2} has too many/too less entries:\n"
                             f"id:        '{row.get('id')}'\n"
                             f"prop name: '{row.get('prop name')}'")
 
         ########### case resource-row ###########
         if check_notna(row.get("id")):
             resource_id = row["id"]
             resource_permissions = row.get("permissions")
@@ -1908,17 +1906,16 @@
                     file_permissions = row.get("file permissions")
                     if not check_notna(file_permissions):
                         if resource_permissions == "res-default":
                             file_permissions = "prop-default"
                         elif resource_permissions == "res-restricted":
                             file_permissions = "prop-restricted"
                         else:
-                            raise BaseError(f"'file permissions' missing for file '{row['file']}' (Excel row "
-                                            f"{int(str(index)) + 2}). An attempt to deduce them from the resource "
-                                            f"permissions failed.")
+                            raise BaseError(f"'file permissions' missing for file '{row['file']}' (Excel row {int(str(index)) + 2}). "
+                                            f"An attempt to deduce them from the resource permissions failed.")
                     resource.append(make_bitstream_prop(
                         path=str(row["file"]),
                         permissions=str(file_permissions),
                         calling_resource=resource_id
                     ))
             elif resource_restype == "Region":
                 resource = make_region(**kwargs_resource)
@@ -1944,34 +1941,31 @@
                 value = row[f"{i}_value"]
                 if pd.notna(value):
                     kwargs_propelem = {
                         "value": value,
                         "permissions": str(row.get(f"{i}_permissions"))
                     }
                     if not check_notna(row.get(f"{i}_permissions")):
-                        raise BaseError(f"Missing permissions for value {value} of property {row['prop name']} "
-                                        f"in resource {resource_id}")
+                        raise BaseError(f"Missing permissions for value {value} of property {row['prop name']} in resource {resource_id}")
                     if check_notna(row.get(f"{i}_comment")):
                         kwargs_propelem["comment"] = str(row[f"{i}_comment"])
                     if check_notna(row.get(f"{i}_encoding")):
                         kwargs_propelem["encoding"] = str(row[f"{i}_encoding"])
-
                     property_elements.append(PropertyElement(**kwargs_propelem))
                 elif check_notna(str(row.get(f"{i}_permissions"))):
-                    raise BaseError(f"Excel row {int(str(index)) + 2} has an entry in column {i}_permissions, but not "
-                                    f"in {i}_value. Please note that cell contents that don't meet the requirements of "
-                                    r"the regex [\p{L}\d_!?\-] are considered inexistent.")
+                    raise BaseError(
+                        f"Excel row {int(str(index)) + 2} has an entry in column {i}_permissions, but not in {i}_value. "
+                        r"Please note that cell contents that don't meet the requirements of the regex [\p{L}\d_!?\-] are considered inexistent."
+                    )
 
             # validate property_elements
             if len(property_elements) == 0:
-                raise BaseError(f"At least one value per property is required, but Excel row {int(str(index)) + 2}"
-                                f"doesn't contain any values.")
+                raise BaseError(f"At least one value per property is required, but Excel row {int(str(index)) + 2} doesn't contain any values.")
             if make_prop_function == make_boolean_prop and len(property_elements) != 1:     # pylint: disable=comparison-with-callable
-                raise BaseError(f"A <boolean-prop> can only have a single value, but Excel row {int(str(index)) + 2} "
-                                f"contains more than one values.")
+                raise BaseError(f"A <boolean-prop> can only have a single value, but Excel row {int(str(index)) + 2} contains more than one value.")
 
             # create the property and append it to resource
             kwargs_propfunc: dict[str, Union[str, PropertyElement, list[PropertyElement]]] = {
                 "name": row["prop name"],
                 "calling_resource": resource_id
             }
             if make_prop_function == make_boolean_prop:                                     # pylint: disable=comparison-with-callable
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/process_files.py` & `dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/process_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Downloads the shell script that is used to extract the preview image from a video.
     """
     user_folder = Path.home() / Path(".dsp-tools/fast-xmlupload")
     user_folder.mkdir(parents=True, exist_ok=True)
     global export_moving_image_frames_script
     export_moving_image_frames_script = user_folder / "export-moving-image-frames.sh"
     script_text = requests.get(
-        "https://github.com/dasch-swiss/dsp-api/raw/main/sipi/scripts/export-moving-image-frames.sh", 
+        "https://github.com/dasch-swiss/dsp-api/raw/main/sipi/scripts/export-moving-image-frames.sh",
         timeout=5
     ).text
     with open(export_moving_image_frames_script, "w", encoding="utf-8") as f:
         f.write(script_text)
 
 
 def _check_if_all_files_were_processed(
@@ -46,38 +46,40 @@
 ) -> bool:
     """
     Go through the result list and print all files that could not be processed.
 
     Args:
         result: list of tuples of Paths. If the second Path is None, the file could not be processed.
         all_paths: list of all paths that should have been processed
-    
+
     Returns:
         success status
     """
-    if len(result) == len(all_paths):
+    processed_paths = [x[1] for x in result if x[1]]
+    if len(processed_paths) == len(all_paths):
         success = True
         print(f"{datetime.now()}: Number of processed files: {len(result)}: Okay")
         logger.info(f"Number of processed files: {len(result)}: Okay")
     else:
         success = False
-        print(f"{datetime.now()}: ERROR: Some files could not be processed: Only {len(result)}/{len(all_paths)} were processed. The failed ones are:")
-        logger.error(f"Some files could not be processed: Only {len(result)}/{len(all_paths)} were processed. The failed ones are:")
-    
+        msg = f"Some files could not be processed: Only {len(processed_paths)}/{len(all_paths)} were processed. The failed ones are:"
+        print(f"{datetime.now()}: ERROR: {msg}")
+        logger.error(msg)
+
     for input_file, output_file in result:
         if not output_file:
-            print(f" - {input_file} could not be processed.")
-            logger.error(f" - {input_file} could not be processed.")
+            print(f" - {input_file}")
+            logger.error(f" - {input_file}")
 
     return success
 
 
 def _process_files_in_parallel(
-    paths: list[Path], 
-    input_dir: Path, 
+    paths: list[Path],
+    input_dir: Path,
     output_dir: Path,
     nthreads: Optional[int]
 ) -> list[tuple[Path, Optional[Path]]]:
     """
     Creates a thread pool and executes the file processing in parallel.
 
     Args:
@@ -124,16 +126,16 @@
     except OSError:
         print(f"{datetime.now()}: An error occurred while writing the result to the pickle file. Content of file: {result}")
         logger.error(f"An error occurred while writing the result to the pickle file. Content of file: {result}", exc_info=True)
         return False
 
 
 def _check_params(
-    input_dir: str, 
-    out_dir: str, 
+    input_dir: str,
+    out_dir: str,
     xml_file: str
 ) -> Optional[tuple[Path, Path, Path]]:
     """
     Checks the input parameters provided by the user and transforms them into the expected types.
 
     Args:
         input_dir: the root directory of the input files
@@ -211,15 +213,15 @@
     try:
         container: Container = docker_client.containers.get(container_name)    # pyright: ignore
     except docker.errors.NotFound:                                             # pyright: ignore
         docker_client.containers.run(image="daschswiss/sipi:3.8.1", name=container_name, volumes=volumes, entrypoint=entrypoint, detach=True)
         print(f"{datetime.now()}: Created and started Sipi container '{container_name}'.")
         logger.info(f"Created and started Sipi container '{container_name}'.")
         return
-    
+
     # Docker container exists
     if not container:
         container_running = False
     elif not container.attrs:
         container_running = False
     elif not container.attrs.get("State", {}).get("Running"):
         container_running = False
@@ -282,15 +284,15 @@
     with open(file, "rb") as f:
         for chunk in iter(lambda: f.read(4096), b""):
             hash_sha256.update(chunk)
     return hash_sha256.hexdigest()
 
 
 def _convert_file_with_sipi(
-    in_file_local_path: Path, 
+    in_file_local_path: Path,
     input_dir: Path,
     out_file_local_path: Path,
     output_dir: Path
 ) -> bool:
     """
     Converts a file by calling a locally running Sipi container.
 
@@ -304,25 +306,25 @@
     in_file_sipi_path = Path("processing-input") / in_file_local_path.relative_to(input_dir)
     out_file_sipi_path = Path("processing-output") / out_file_local_path.relative_to(original_output_dir)
 
     if not sipi_container:
         print(f"{datetime.now()}: ERROR: Cannot convert file {in_file_local_path} with Sipi: Sipi container not found.")
         logger.error(f"Cannot convert file {in_file_local_path} with Sipi: Sipi container not found.")
         return False
-    result = sipi_container.exec_run(f"/sipi/sipi {in_file_sipi_path} {out_file_sipi_path}")
+    result = sipi_container.exec_run(f"/sipi/sipi '{in_file_sipi_path}' {out_file_sipi_path}")
     if result.exit_code != 0:
         print(f"{datetime.now()}: ERROR: Sipi conversion of {in_file_local_path} failed: {result}")
         logger.error(f"Sipi conversion of {in_file_local_path} failed: {result}")
         return False
     return True
 
 
 def _create_orig_file(
-    in_file: Path, 
-    internal_file_name: str, 
+    in_file: Path,
+    internal_file_name: str,
     out_dir: Path
 ) -> bool:
     """
     Creates the .orig file expected by the API.
 
     Args:
         in_file: the input file from which the .orig should be created
@@ -435,15 +437,15 @@
 
     sidecar_file_basename = f"{random_part_of_filename}.info"
     sidecar_file = PurePath(converted_file.parent, sidecar_file_basename)
 
     with open(sidecar_file, "w", encoding="utf-8") as f:
         sidecar_json = json.dumps(sidecar_dict, indent=4)
         f.write(sidecar_json)
-    
+
     logger.info(f"Created sidecar file {sidecar_file}")
     return True
 
 
 def _get_file_category_from_extension(file: Path) -> Optional[str]:
     """
     Gets the file category of a file according to its extension.
@@ -458,19 +460,19 @@
     extensions["image"] = [".jpg", ".jpeg", ".tif", ".tiff", ".jp2", ".png"]
     extensions["video"] = [".mp4"]
     extensions["archive"] = [".7z", ".gz", ".gzip", ".tar", ".tar.gz", ".tgz", ".z", ".zip"]
     extensions["text"] = [".csv", ".txt", ".xml", ".xsd", ".xsl"]
     extensions["document"] = [".doc", ".docx", ".pdf", ".ppt", ".pptx", ".xls", ".xlsx"]
     extensions["audio"] = [".mp3", ".wav"]
 
-    if file.suffix in extensions["video"]:
+    if file.suffix.lower() in extensions["video"]:
         category = "VIDEO"
-    elif file.suffix in extensions["image"]:
+    elif file.suffix.lower() in extensions["image"]:
         category = "IMAGE"
-    elif file.suffix in extensions["archive"] + extensions["text"] + extensions["document"] + extensions["audio"]:
+    elif file.suffix.lower() in extensions["archive"] + extensions["text"] + extensions["document"] + extensions["audio"]:
         category = "OTHER"
     else:
         category = None
         print(f"{datetime.now()}: ERROR: Couldn't get category for {file}")
         logger.error(f"Couldn't get category for {file}")
     return category
 
@@ -481,15 +483,15 @@
 
     Args:
         file: the video file which the preview is extracted from
 
     Returns:
         true if successful, false otherwise
     """
-    
+
     result = subprocess.call(["/bin/bash", f"{export_moving_image_frames_script}", "-i", f"{file}"])
     if result != 0:
         return False
     else:
         return True
 
 
@@ -543,55 +545,55 @@
     # get random UUID for internal file handling, and create directory structure
     internal_filename = str(uuid.uuid4())
     out_dir_full = Path(output_dir, internal_filename[0:2], internal_filename[2:4])
     out_dir_full.mkdir(parents=True, exist_ok=True)
 
     # create .orig file
     if not _create_orig_file(
-        in_file=in_file, 
-        internal_file_name=internal_filename, 
+        in_file=in_file,
+        internal_file_name=internal_filename,
         out_dir=out_dir_full
     ):
         return in_file, None
 
     # convert file (create derivative) and create sidecar file based on category (image, video or other)
     file_category = _get_file_category_from_extension(in_file)
     if not file_category:
         return in_file, None
 
     if file_category == "OTHER":
         result = _process_other_file(
-            in_file=in_file, 
-            internal_filename=internal_filename, 
+            in_file=in_file,
+            internal_filename=internal_filename,
             out_dir=out_dir_full
         )
     elif file_category == "IMAGE":
         result = _process_image_file(
-            in_file=in_file, 
-            internal_filename=internal_filename, 
-            out_dir=out_dir_full, 
+            in_file=in_file,
+            internal_filename=internal_filename,
+            out_dir=out_dir_full,
             input_dir=input_dir
         )
     elif file_category == "VIDEO":
         result = _process_video_file(
-            in_file=in_file, 
-            internal_filename=internal_filename, 
+            in_file=in_file,
+            internal_filename=internal_filename,
             out_dir=out_dir_full
         )
     else:
         print(f"{datetime.now()}: ERROR: Unexpected file category: {file_category}")
         logger.error(f"Unexpected file category: {file_category}")
         return in_file, None
 
     return result
 
 
 def _process_other_file(
-    in_file: Path, 
-    internal_filename: str, 
+    in_file: Path,
+    internal_filename: str,
     out_dir: Path
 ) -> tuple[Path, Optional[Path]]:
     """
     Processes a file of file category OTHER.
     There is no real derivate created, 
     but the original file is copied, 
     and a sidecar file is created.
@@ -609,28 +611,28 @@
     try:
         shutil.copyfile(in_file, converted_file_full_path)
     except Exception:  # pylint: disable=broad-exception-caught
         print(f"{datetime.now()}: ERROR: Couldn't process file of category OTHER: {in_file}")
         logger.error(f"Couldn't process file of category OTHER: {in_file}", exc_info=True)
         return in_file, None
     if not _create_sidecar_file(
-        orig_file=in_file, 
-        converted_file=converted_file_full_path, 
+        orig_file=in_file,
+        converted_file=converted_file_full_path,
         file_category="OTHER"
     ):
         print(f"{datetime.now()}: ERROR: Couldn't create sidecar file for: {in_file}")
         logger.error(f"Couldn't create sidecar file for: {in_file}")
         return in_file, None
     return in_file, converted_file_full_path
 
 
 def _process_image_file(
-    in_file: Path, 
-    internal_filename: str, 
-    out_dir: Path, 
+    in_file: Path,
+    internal_filename: str,
+    out_dir: Path,
     input_dir: Path
 ) -> tuple[Path, Optional[Path]]:
     """
     Processes a file of file category IMAGE
 
     Args:
         in_file: the input file that should be processed
@@ -650,27 +652,27 @@
         output_dir=out_dir
     )
     if not sipi_result:
         print(f"{datetime.now()}: ERROR: Couldn't process file of category IMAGE: {in_file}")
         logger.error(f"Couldn't process file of category IMAGE: {in_file}")
         return in_file, None
     if not _create_sidecar_file(
-        orig_file=in_file, 
-        converted_file=converted_file_full_path, 
+        orig_file=in_file,
+        converted_file=converted_file_full_path,
         file_category="IMAGE"
     ):
         print(f"{datetime.now()}: ERROR: Couldn't create sidecar file for: {in_file}")
         logger.error(f"Couldn't create sidecar file for: {in_file}")
         return in_file, None
     return in_file, converted_file_full_path
 
 
 def _process_video_file(
-    in_file: Path, 
-    internal_filename: str, 
+    in_file: Path,
+    internal_filename: str,
     out_dir: Path
 ) -> tuple[Path, Optional[Path]]:
     """
     Processes a file of file category VIDEO
 
     Args:
         in_file: the input file that should be processed
@@ -685,32 +687,32 @@
     # create derivate file (identical to original file)
     try:
         shutil.copyfile(in_file, converted_file_full_path)
     except Exception:  # pylint: disable=broad-exception-caught
         print(f"{datetime.now()}: ERROR: Couldn't create derivate file for video '{in_file}'")
         logger.error(f"Couldn't create derivate file for video '{in_file}'", exc_info=True)
         return in_file, None
-    
+
     # create preview image
     preview_result = _extract_preview_from_video(converted_file_full_path)
     if not preview_result:
         print(f"{datetime.now()}: ERROR: Couldn't create preview image for video '{in_file}'")
         logger.error(f"Couldn't create preview image for video '{in_file}'")
         return in_file, None
-    
+
     # create sidecar file
     if not _create_sidecar_file(
-        orig_file=in_file, 
-        converted_file=converted_file_full_path, 
+        orig_file=in_file,
+        converted_file=converted_file_full_path,
         file_category="VIDEO"
     ):
         print(f"{datetime.now()}: ERROR: Couldn't create sidecar file for video '{in_file}'")
         logger.error(f"Couldn't create sidecar file for video '{in_file}'")
         return in_file, None
-    
+
     return in_file, converted_file_full_path
 
 
 def process_files(
     input_dir: str,
     output_dir: str,
     xml_file: str,
@@ -725,34 +727,34 @@
     e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2').
 
     Args:
         input_dir: path to the directory where the files should be read from
         output_dir: path to the directory where the transformed / created files should be written to
         xml_file: path to xml file containing the resources
         nthreads: number of threads to use for processing
-    
+
     Returns:
         success status
     """
     logger.info(f"***Call to process_files(input_dir='{input_dir}', out_dir='{output_dir}', xml_file='{xml_file}')***")
     # check the input parameters
     param_check_result = _check_params(
-        input_dir=input_dir, 
-        out_dir=output_dir, 
+        input_dir=input_dir,
+        out_dir=output_dir,
         xml_file=xml_file
     )
     if param_check_result:
         input_dir_path, output_dir_path, xml_file_path = param_check_result
     else:
         raise BaseError("Error reading the input parameters. Please check them.")
 
     # startup the SIPI container
     _start_sipi_container_and_mount_volumes(
-        input_dir=input_dir_path, 
-        output_dir=output_dir_path 
+        input_dir=input_dir_path,
+        output_dir=output_dir_path
     )
     global sipi_container
     sipi_container = _get_sipi_container()
 
     # get the paths of the files referenced in the XML file
     all_paths = _get_file_paths_from_xml(xml_file_path)
     print(f"{datetime.now()}: Found {len(all_paths)} bitstreams in the XML file.")
@@ -763,16 +765,16 @@
         _get_export_moving_image_frames_script()
 
     # process the files in parallel
     start_time = datetime.now()
     print(f"{start_time}: Start local file processing...")
     logger.info("Start local file processing...")
     result = _process_files_in_parallel(
-        paths=all_paths, 
-        input_dir=input_dir_path, 
+        paths=all_paths,
+        input_dir=input_dir_path,
         output_dir=output_dir_path,
         nthreads=nthreads
     )
 
     # check if all files were processed
     end_time = datetime.now()
     print(f"{end_time}: Processing files took: {end_time - start_time}")
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/upload_files.py` & `dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/upload_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.utils.shared import login
 
 logger = logging.getLogger(__name__)
 
+
 def _get_upload_candidates(
-    dir_with_processed_files: Path, 
+    dir_with_processed_files: Path,
     internal_filename_of_processed_file: Path
 ) -> list[Path]:
     """
     Based on the base derivate file, get all files based on the same uuid.
     For example, if the base derivate file is tmp/1f/fb/1ffbbb30-77e8-414c-94ff-7e1c060f9146.jp2,
     the upload candidates are:
     - derivate: tmp/1f/fb/1ffbbb30-77e8-414c-94ff-7e1c060f9146.jp2
@@ -43,15 +44,15 @@
     upload_candidates_paths = [Path(c) for c in upload_candidates]
     upload_candidates_as_str = "\n - " + "\n - ".join([str(c) for c in upload_candidates])
     logger.info(f"Found the following upload candidates for {internal_filename_of_processed_file}: {upload_candidates_as_str}")
     return upload_candidates_paths
 
 
 def _check_upload_candidates(
-    internal_filename_of_processed_file: Path, 
+    internal_filename_of_processed_file: Path,
     upload_candidates: list[Path]
 ) -> bool:
     """
     Make sure that all upload candidates exist, 
     and that there are at least 5 candidates for videos and 3 candidates for all other file types.
 
     Args:
@@ -80,16 +81,16 @@
         return False
 
     logger.info(f"Upload candidates for {internal_filename_of_processed_file} are okay.")
     return True
 
 
 def _upload_without_processing(
-    file: Path, 
-    sipi_url: str, 
+    file: Path,
+    sipi_url: str,
     con: Connection
 ) -> bool:
     """
     Send a single file to the "upload_without_processing" route. 
 
     Args:
         file: file to upload
@@ -111,15 +112,15 @@
                 print(f"{datetime.now()}: ERROR: An exception was raised while calling the /upload_without_processing route for the file {file}")
                 logger.error(f"An exception was raised while calling the /upload_without_processing route for the file {file}", exc_info=True)
                 return False
     except Exception:  # pylint: disable=broad-exception-caught
         print(f"{datetime.now()}: ERROR: Cannot send file to /upload_without_processing route, because the file cannot be opened: {file}")
         logger.error(f"Cannot send file to /upload_without_processing route, because the file cannot be opened: {file}", exc_info=True)
         return False
-    
+
     if response_upload.json().get("message") == "server.fs.mkdir() failed: File exists":
         # This error can be safely ignored, since the file was uploaded correctly.
         logger.info(f"In spite of 'server.fs.mkdir() failed: File exists', successfully uploaded file {file}")
     elif response_upload.status_code != 200:
         print(f"{datetime.now()}: ERROR: An error occurred while uploading the file {file}. The response was {response_upload.json()}")
         logger.error(f"An error occurred while uploading the file {file}. The response was {response_upload.json()}")
         return False
@@ -144,30 +145,30 @@
         sipi_url: URL to the sipi server
         con: connection to the DSP server
 
     Returns:
         tuple with the processed file and a boolean indicating if the upload was successful
     """
     upload_candidates = _get_upload_candidates(
-        dir_with_processed_files=dir_with_processed_files, 
+        dir_with_processed_files=dir_with_processed_files,
         internal_filename_of_processed_file=internal_filename_of_processed_file
     )
 
     check_result = _check_upload_candidates(
-        internal_filename_of_processed_file=internal_filename_of_processed_file, 
+        internal_filename_of_processed_file=internal_filename_of_processed_file,
         upload_candidates=upload_candidates
     )
     if not check_result:
         return internal_filename_of_processed_file, False
 
     results: list[bool] = []
     for candidate in upload_candidates:
         res = _upload_without_processing(
-            file=candidate, 
-            sipi_url=sipi_url, 
+            file=candidate,
+            sipi_url=sipi_url,
             con=con
         )
         results.append(res)
 
     if not all(results):
         logger.error(f"Could not upload all files for {internal_filename_of_processed_file}.")
         return internal_filename_of_processed_file, False
@@ -197,15 +198,15 @@
             print(f"{datetime.now()}: WARNING: There is no processed file for {orig_processed[0]}")
             logger.warning(f"There is no processed file for {orig_processed[0]}")
 
     return processed_paths
 
 
 def _check_params(
-    pkl_file: str, 
+    pkl_file: str,
     dir_with_processed_files: str
 ) -> Optional[tuple[Path, Path]]:
     """
     Checks the input parameters provided by the user and transforms them into the expected types.
 
     Args:
         pkl_file: the XML file the paths are extracted from
@@ -268,34 +269,34 @@
 ) -> bool:
     """
     Print the files which could not be uploaded.
 
     Args:
         result: list of tuples with the path of the file and the success status
         internal_filenames_of_processed_files: list of files that should have been uploaded (uuid filenames)
-    
+
     Returns:
         True if all files were uploaded, False otherwise
     """
     if len(result) == len(internal_filenames_of_processed_files):
         success = True
         print(f"{datetime.now()}: Number of files of which the derivates were uploaded: {len(result)}: Okay")
         logger.info(f"Number of files of which the derivates were uploaded: {len(result)}: Okay")
     else:
         success = False
         msg = f"Some derivates of some files could not be uploaded: Only {len(result)}/{len(internal_filenames_of_processed_files)} were uploaded. " \
-               "The failed ones are:"
+            "The failed ones are:"
         print(f"{datetime.now()}: ERROR: {msg}")
         logger.error(msg)
-    
+
     for path, res in result:
         if not res:
             print(f" - {path} could not be uploaded.")
             logger.error(f"{path} could not be uploaded.")
-    
+
     return success
 
 
 def upload_files(
     pkl_file: str,
     dir_with_processed_files: str,
     nthreads: int,
@@ -313,48 +314,48 @@
                   e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2').
         dir_with_processed_files: path to the directory where the processed files are located
         nthreads: number of threads to use for uploading (optimum depends on the number of CPUs on the server)
         user: the user's e-mail for login into DSP
         password: the user's password for login into DSP
         dsp_url: URL to the DSP server
         sipi_url: URL to the Sipi server
-    
+
     Returns:
         success status
     """
     # check the input parameters
     param_check_result = _check_params(
-        pkl_file=pkl_file, 
+        pkl_file=pkl_file,
         dir_with_processed_files=dir_with_processed_files
     )
     if param_check_result:
         pkl_file_path, dir_with_processed_files_path = param_check_result
     else:
         raise BaseError("Error reading the input parameters. Please check them.")
 
     # read paths from pkl file
     internal_filenames_of_processed_files = _get_paths_from_pkl_file(pkl_file=pkl_file_path)
     print(f"{datetime.now()}: Found {len(internal_filenames_of_processed_files)} files to upload...")
     logger.info(f"Found {len(internal_filenames_of_processed_files)} files to upload...")
 
     # create connection to DSP
     con = login(
-        server=dsp_url, 
-        user=user, 
+        server=dsp_url,
+        user=user,
         password=password
     )
 
     # upload files in parallel
     start_time = datetime.now()
     print(f"{start_time}: Start file uploading...")
     logger.info("Start file uploading...")
     result = _upload_files_in_parallel(
-        dir_with_processed_files=dir_with_processed_files_path, 
-        internal_filenames_of_processed_files=internal_filenames_of_processed_files, 
-        sipi_url=sipi_url, 
+        dir_with_processed_files=dir_with_processed_files_path,
+        internal_filenames_of_processed_files=internal_filenames_of_processed_files,
+        sipi_url=sipi_url,
         con=con,
         nthreads=nthreads
     )
 
     # check if all files were uploaded
     end_time = datetime.now()
     print(f"{datetime.now()}: Uploading files took {end_time - start_time}")
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/fast_xmlupload/upload_xml.py` & `dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/upload_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         if processed_path:
             orig_path_2_uuid_filename[str(orig_path)] = str(processed_path.name)
         else:
             raise BaseError(
                 f"There is no processed file for {orig_path}. The fast xmlupload cannot be started, "
                 "because the resource that uses this file would fail."
             )
-    
+
     return orig_path_2_uuid_filename
 
 
 def replace_bitstream_paths(
-    xml_tree: "etree._ElementTree[etree._Element]", 
+    xml_tree: "etree._ElementTree[etree._Element]",
     orig_path_2_uuid_filename: dict[str, str]
 ) -> "etree._ElementTree[etree._Element]":
     """
     Replace the original filepaths in the <bitstream> Tags by the uuid filenames of the processed files.
 
     Args:
         xml_tree: The parsed original XML tree
@@ -91,15 +91,15 @@
         xml_file: path to XML file containing the resources
         pkl_file: pickle file containing the mapping between the original files and the processed files,
                   e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2')
         user: the user's e-mail for login into DSP
         password: the user's password for login into DSP
         dsp_url: URL to the DSP server
         sipi_url: URL to the Sipi server
-    
+
     Returns:
         success status
     """
     xml_tree_orig = etree.parse(xml_file)
     orig_path_2_uuid_filename = _get_paths_from_pkl_file(pkl_file=Path(pkl_file))
     xml_tree_replaced = replace_bitstream_paths(xml_tree=xml_tree_orig, orig_path_2_uuid_filename=orig_path_2_uuid_filename)
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/bitstream.py` & `dsp_tools-2.3.1/src/dsp_tools/models/bitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/connection.py` & `dsp_tools-2.3.1/src/dsp_tools/models/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 
 def check_for_api_error(response: requests.Response) -> None:
     """
     Check the response of an API request if it contains an error raised by DSP-API.
 
     Args:
         res: The requests.Response object that is returned by the API request
-    
+
     Raises:
         BaseError: If the status code of the response is not 200
     """
     if response.status_code != 200:
         raise BaseError(
             message="KNORA-ERROR: status code=" + str(response.status_code) + "\nMessage:" + response.text,
             status_code=response.status_code,
             json_content_of_api_response=response.text,
             reason_from_api_response=response.reason,
             api_route=response.url
         )
 
+
 class Connection:
     """
     An Connection instance represents a connection to a Knora server.
 
     Attributes
     ----------
 
@@ -107,15 +108,14 @@
             check_for_api_error(response)
             self._token = None
 
     def __del__(self):
         pass
         # self.logout()
 
-
     def post(self, path: str, jsondata: Optional[str] = None):
         """
         Post Json data to a given server using a HTTP POST request
         :param path: Path of RESTful route
         :param jsondata: Valid JSON as string
         :return: Response from server
         """
@@ -155,15 +155,15 @@
                 jsonobj = None
             logobj = {
                 "method": "POST",
                 "headers": headers,
                 "route": path,
                 "body": jsonobj,
                 "return-headers": dict(response.headers),
-                "return": response.json() if response.status_code == 200 else {"status": str(response.status_code), 
+                "return": response.json() if response.status_code == 200 else {"status": str(response.status_code),
                                                                                "message": response.text}
             }
             tmp = path.split('/')
             filename = "POST" + "_".join(tmp) + ".json"
             with open(filename, 'w') as f:
                 json.dump(logobj, f, indent=4)
         check_for_api_error(response)
@@ -212,15 +212,15 @@
                 self._server + path,
                 headers={'Authorization': 'Bearer ' + self._token}
             )
         else:
             response = requests.put(
                 self._server + path,
                 headers={
-                    'Content-Type': content_type + '; charset=UTF-8', 
+                    'Content-Type': content_type + '; charset=UTF-8',
                     'Authorization': 'Bearer ' + self._token
                 },
                 data=jsondata)
         check_for_api_error(response)
         result = response.json()
         return result
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/exceptions.py` & `dsp_tools-2.3.1/src/dsp_tools/models/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     status_code: Optional[int]
     json_content_of_api_response: Optional[str]
     original_error_msg_from_api: Optional[str] = None
     reason_from_api_response: Optional[str]
     api_route: Optional[str]
 
     def __init__(
-        self, 
-        message: str, 
+        self,
+        message: str,
         status_code: Optional[int] = None,
         json_content_of_api_response: Optional[str] = None,
         reason_from_api_response: Optional[str] = None,
         api_route: Optional[str] = None
     ) -> None:
         """
         A basic error class for DSP-TOOLS.
@@ -51,15 +51,15 @@
                     knora_api_error = parsed_json["knora-api:error"]
                     knora_api_error = re.sub(r"^dsp\.errors\.[A-Za-z]+?: ?", "", knora_api_error)
                     self.original_error_msg_from_api = knora_api_error
             except json.JSONDecodeError:
                 pass
         self.reason_from_api_response = reason_from_api_response
         self.api_route = api_route
-    
+
     def __str__(self) -> str:
         return self.message
 
 
 class InternalError(BaseError):
     """
     Class for errors that will be handled by a higher level function
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/group.py` & `dsp_tools-2.3.1/src/dsp_tools/models/group.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     _selfjoin: bool
     _status: bool
 
     def __init__(self,
                  con: Connection,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
-                 descriptions: LangString = None,
+                 descriptions: Optional[LangString] = None,
                  project: Optional[Union[str, Project]] = None,
                  selfjoin: Optional[bool] = None,
                  status: Optional[bool] = None):
         super().__init__(con)
         self._id = str(id) if id is not None else None
         self._name = str(name) if name is not None else None
         self._descriptions = LangString(descriptions)
@@ -112,15 +112,15 @@
 
     @name.setter
     def name(self, value: str):
         self._name = value
         self._changed.add('name')
 
     @property
-    def descriptions(self) -> Optional[LangString]:
+    def descriptions(self) -> LangString:
         return self._descriptions
 
     @descriptions.setter
     def descriptions(self, value: Optional[LangString]) -> None:
         self._descriptions = LangString(value)
         self._changed.add('descriptions')
 
@@ -213,31 +213,32 @@
 
     def create(self) -> Group:
         jsonobj = self.toJsonObj(Actions.Create)
         jsondata = json.dumps(jsonobj)
         result = self._con.post(Group.ROUTE, jsondata)
         return Group.fromJsonObj(self._con, result['group'])
 
-    def read(self):
+    def read(self) -> Group:
         result = self._con.get(Group.ROUTE_SLASH + quote_plus(self._id))
         return Group.fromJsonObj(self._con, result['group'])
 
-    def update(self):
+    def update(self) -> Optional[Group]:
+        updated_group = None
         jsonobj = self.toJsonObj(Actions.Update)
         if jsonobj:
             jsondata = json.dumps(jsonobj)
             result = self._con.put(Group.ROUTE_SLASH + quote_plus(self._id), jsondata)
             updated_group = Group.fromJsonObj(self._con, result['group'])
         if self._status is not None and 'status' in self._changed:
             jsondata = json.dumps({'status': self._status})
             result = self._con.put(Group.ROUTE_SLASH + quote_plus(self._id) + '/status', jsondata)
             updated_group = Group.fromJsonObj(self._con, result['group'])
         return updated_group
 
-    def delete(self):
+    def delete(self) -> Group:
         result = self._con.delete(Group.ROUTE_SLASH + quote_plus(self._id))
         return Group.fromJsonObj(self._con, result['group'])
 
     @staticmethod
     def getAllGroups(con: Connection) -> list[Group]:
         result = con.get(Group.ROUTE)
         return [Group.fromJsonObj(con, group_item) for group_item in result["groups"]]
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/helpers.py` & `dsp_tools-2.3.1/src/dsp_tools/models/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
                 else:
                     raise BaseError("Iri cannot be resolved to a well-known prefix!")
         return result
 
     def get_qualified_iri(self, val: Optional[str]) -> Optional[str]:
         """
         Given an IRI, its fully qualified name is returned.
-        
+
         Args:
             val: The input IRI
 
         Returns:
             the fully qualified IRI
         """
         if not val:
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/langstring.py` & `dsp_tools-2.3.1/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/listnode.py` & `dsp_tools-2.3.1/src/dsp_tools/models/listnode.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     _children: Optional[list['ListNode']]
     _rootNodeIri: Optional[str]
 
     def __init__(self,
                  con: Connection,
                  id: Optional[str] = None,
                  project: Optional[Union[Project, str]] = None,
-                 label: LangString = None,
+                 label: Optional[LangString] = None,
                  comments: Optional[LangString] = None,
                  name: Optional[str] = None,
                  parent: Optional[Union['ListNode', str]] = None,
                  isRootNode: bool = False,
                  children: Optional[list['ListNode']] = None,
                  rootNodeIri: Optional[str] = None):
         """
@@ -215,16 +215,16 @@
     def project(self, value: str) -> None:
         if self._project:
             raise BaseError('Project id cannot be modified!')
         else:
             self._project = value
 
     @property
-    def label(self) -> Optional[LangString]:
-        return self._label
+    def label(self) -> LangString:
+        return self._label or LangString({})
 
     @label.setter
     def label(self, value: Optional[Union[LangString, str]]) -> None:
         self._label = LangString(value)
         self._changed.add('label')
 
     def addLabel(self, lang: Union[Languages, str], value: str) -> None:
@@ -246,16 +246,16 @@
         :param lang: The language the label to be removed is in, either a string "EN", "DE", "FR", "IT" or a Language instance
         :return: None
         """
         del self._label[lang]
         self._changed.add('label')
 
     @property
-    def comments(self) -> Optional[LangString]:
-        return self._comments
+    def comments(self) -> LangString:
+        return self._comments or LangString({})
 
     @comments.setter
     def comments(self, value: Optional[Union[LangString, str]]) -> None:
         self._comments = LangString(value)
         self._changed.add('comments')
 
     def addComment(self, lang: Union[Languages, str], value: str) -> None:
@@ -305,16 +305,16 @@
         return self._isRootNode
 
     @isRootNode.setter
     def isRootNode(self, value: bool) -> None:
         raise BaseError('Property isRootNode cannot be set!')
 
     @property
-    def children(self) -> Optional[list['ListNode']]:
-        return self._children
+    def children(self) -> list['ListNode']:
+        return self._children or []
 
     @children.setter
     def children(self, value: list['ListNode']) -> None:
         self._children = value
 
     @staticmethod
     def __getChildren(con: Connection,
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/ontology.py` & `dsp_tools-2.3.1/src/dsp_tools/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/permission.py` & `dsp_tools-2.3.1/src/dsp_tools/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/project.py` & `dsp_tools-2.3.1/src/dsp_tools/models/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,16 +194,16 @@
     @longname.setter
     def longname(self, value: str) -> None:
         if self._longname != str(value):
             self._longname = str(value)
             self._changed.add('longname')
 
     @property
-    def description(self) -> Optional[LangString]:
-        return self._description
+    def description(self) -> LangString:
+        return self._description or LangString({})
 
     @description.setter
     def description(self, value: Optional[LangString]) -> None:
         self._description = LangString(value)
         self._changed.add('description')
 
     def addDescription(self, lang: Union[Languages, str], value: str) -> None:
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/projectContext.py` & `dsp_tools-2.3.1/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/propertyclass.py` & `dsp_tools-2.3.1/src/dsp_tools/models/propertyclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,27 +66,27 @@
             if isinstance(label, str):
                 self._label = LangString(label)
             elif isinstance(label, LangString):
                 self._label = label
             else:
                 raise BaseError('Invalid LangString for label!')
         else:
-            self._label = None
+            self._label = LangString({})
         #
         # process comment
         #
         if comment is not None:
             if isinstance(comment, str):
                 self._comment = LangString(comment)
             elif isinstance(comment, LangString):
                 self._comment = comment
             else:
                 raise BaseError('Invalid LangString for comment!')
         else:
-            self._comment = None
+            self._comment = LangString({})
 
         self._editable = editable
         self._linkvalue = linkvalue
 
     #
     # Here follows a list of getters/setters
     #
@@ -162,15 +162,15 @@
 
     def rmGuiAttribute(self, key: str) -> None:
         if self._gui_attributes.get(key) is not None:
             del self._gui_attributes[key]
             self._changed.append('gui_attributes')
 
     @property
-    def label(self) -> Optional[LangString]:
+    def label(self) -> LangString:
         return self._label
 
     @label.setter
     def label(self, value: Optional[Union[LangString, str]]) -> None:
         if value is None:
             self._label.empty()  # clear all labels
         else:
@@ -187,15 +187,15 @@
         self._changed.add('label')
 
     def rmLabel(self, lang: Union[Languages, str]) -> None:
         del self._label[lang]
         self._changed.add('label')
 
     @property
-    def comment(self) -> Optional[LangString]:
+    def comment(self) -> LangString:
         return self._comment
 
     @comment.setter
     def comment(self, value: Optional[LangString]) -> None:
         if value is None:
             self._comment.empty()  # clear all comments!
         else:
@@ -432,17 +432,17 @@
             for sc in self.superproperties:
                 superprops.append(context.reduce_iri(sc, shortname))
             property["super"] = superprops
         if self.subject:
             property["subject"] = context.reduce_iri(self.subject, shortname)
         if self.object:
             property["object"] = context.reduce_iri(self.object, shortname)
-        if self.label:
+        if not self.label.isEmpty():
             property["labels"] = self.label.createDefinitionFileObj()
-        if self.comment:
+        if not self.comment.isEmpty():
             property["comments"] = self.comment.createDefinitionFileObj()
         if self.gui_element:
             property["gui_element"] = context.reduce_iri(self.gui_element, shortname)
         if self.gui_attributes:
             gui_elements = {}
             for (attname, attvalue) in self.gui_attributes.items():
                 if attname == "size":
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/propertyelement.py` & `dsp_tools-2.3.1/src/dsp_tools/models/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/resource.py` & `dsp_tools-2.3.1/src/dsp_tools/models/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,17 @@
                 if value:
                     # property has multiple values
                     if type(value) is list:
                         self._values[property_name] = []
                         for val in value:
                             # check if cardinality allows multiple values for a property
                             if cardinality == Cardinality.C_0_1 or cardinality == Cardinality.C_1:
-                                raise BaseError(f"ERROR in resource with label '{self._label}': Ontology does not allow multiple values for '{property_name}'")
+                                raise BaseError(
+                                    f"ERROR in resource with label '{self._label}': Ontology does not allow multiple values for '{property_name}'"
+                                )
 
                             if type(val) is Value:
                                 self._values[property_name].append(val)
 
                             elif type(val) is dict:
                                 if value_type is ListValue:
                                     val['lists'] = self.lists
@@ -172,15 +174,17 @@
                             if value_type is ListValue:
                                 value = {'value': value, 'lists': self.lists}
                                 self._values[property_name] = value_type(**value)
                             else:
                                 self._values[property_name] = value_type(value)
                 else:
                     if cardinality == Cardinality.C_1 or cardinality == Cardinality.C_1_n:
-                        raise BaseError(f"ERROR in resource with label '{self._label}': The ontology requires at least one value for '{property_name}'")
+                        raise BaseError(
+                            f"ERROR in resource with label '{self._label}': The ontology requires at least one value for '{property_name}'"
+                        )
 
             for property_name in values:
                 if property_name not in self.knora_properties and not self.properties.get(property_name):
                     raise BaseError(f"ERROR in resource with label '{self._label}': Property '{property_name}' is not part of ontology")
 
     def value(self, item) -> Optional[list[Value]]:
         if self._values.get(item):
@@ -381,15 +385,15 @@
 
         self._lists = [x.getAllNodes() for x in ListNode.getAllLists(con=con, project_iri=self._project.id)]
 
         tmp_ontologies = Ontology.getProjectOntologies(con=con, project_id=self._project.id)
         shared_project = Project(con=con, shortcode="0000").read()
         shared_ontologies = Ontology.getProjectOntologies(con=con, project_id=shared_project.id)
         tmp_ontologies.extend(shared_ontologies)
-        knora_api_onto = [x for x in Ontology.getAllOntologies(con=con) if x.name=="knora-api"][0]
+        knora_api_onto = [x for x in Ontology.getAllOntologies(con=con) if x.name == "knora-api"][0]
         tmp_ontologies.append(knora_api_onto)
         self._ontoname2iri = {x.name: x.id for x in tmp_ontologies}
 
         ontology_ids = [x.id for x in tmp_ontologies]
         self._ontologies = {}
         self._properties = {}
         self._context = {}
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/resourceclass.py` & `dsp_tools-2.3.1/src/dsp_tools/models/resourceclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,17 +274,17 @@
     def delete(self, last_modification_date: DateTimeStamp) -> DateTimeStamp:
         raise BaseError("Cannot remove a single property from a class!")
         # ToDo: Check with Ben if we could add this feature...
 
     def createDefinitionFileObj(self, context: Context, shortname: str):
         cardinality = {}
         if self._ptype == HasProperty.Ptype.other or self.property_id in [
-            "knora-api:isSequenceOf", 
-            "knora-api:hasSequenceBounds", 
-            "knora-api:isPartOf", 
+            "knora-api:isSequenceOf",
+            "knora-api:hasSequenceBounds",
+            "knora-api:isPartOf",
             "knora-api:seqnum"
         ]:
             cardinality["propname"] = context.reduce_iri(self._property_id, shortname)
             cardinality["cardinality"] = self._cardinality.value
             if self._gui_order is not None:
                 cardinality["gui_order"] = self._gui_order
         return cardinality
@@ -443,27 +443,27 @@
             if isinstance(label, str):
                 self._label = LangString(label)
             elif isinstance(label, LangString):
                 self._label = label
             else:
                 raise BaseError('Invalid LangString for label!')
         else:
-            self._label = None
+            self._label = LangString({})
         #
         # process comment
         #
         if comment is not None:
             if isinstance(comment, str):
                 self._comment = LangString(comment)
             elif isinstance(comment, LangString):
                 self._comment = comment
             else:
                 raise BaseError('Invalid LangString for comment!')
         else:
-            self._comment = None
+            self._comment = LangString({})
         self._permissions = permissions
         self._has_properties = has_properties
         self._changed = set()
 
     #
     # Here follows a list of getters/setters
     #
@@ -496,15 +496,15 @@
         return self._superclasses
 
     @superclasses.setter
     def superclasses(self, value: list[str]) -> None:
         raise BaseError('"superclasses" cannot be modified!')
 
     @property
-    def label(self) -> Optional[LangString]:
+    def label(self) -> LangString:
         return self._label
 
     @label.setter
     def label(self, value: Optional[Union[LangString, str]]) -> None:
         if value is None:
             self._label.empty()  # clear all labels
         else:
@@ -521,15 +521,15 @@
         self._changed.add('label')
 
     def rmLabel(self, lang: Union[Languages, str]) -> None:
         del self._label[lang]
         self._changed.add('label')
 
     @property
-    def comment(self) -> Optional[LangString]:
+    def comment(self) -> LangString:
         return self._comment
 
     @comment.setter
     def comment(self, value: Optional[LangString]) -> None:
         if value is None:
             self._comment.empty()  # clear all comments!
         else:
@@ -785,32 +785,31 @@
                 superclasses = []
                 for sc in self._superclasses:
                     superclasses.append(context.reduce_iri(sc, shortname))
             else:
                 superclasses = context.reduce_iri(self._superclasses[0], shortname)
             resource["super"] = superclasses
         resource["labels"] = self._label.createDefinitionFileObj()
-        if self._comment:
+        if not self._comment.isEmpty():
             resource["comments"] = self._comment.createDefinitionFileObj()
         if self._has_properties:
             cardinalities = []
             for pid, hp in self._has_properties.items():
                 if hp.property_id in skiplist:
                     continue
                 if hp.ptype == HasProperty.Ptype.other or hp.property_id in [
-                    "knora-api:isSequenceOf", 
-                    "knora-api:hasSequenceBounds", 
-                    "knora-api:isPartOf", 
+                    "knora-api:isSequenceOf",
+                    "knora-api:hasSequenceBounds",
+                    "knora-api:isPartOf",
                     "knora-api:seqnum"
                 ]:
                     cardinalities.append(hp.createDefinitionFileObj(context, shortname))
             if cardinalities:
                 resource["cardinalities"] = cardinalities
 
-
         return resource
 
     def print(self, offset: int = 0):
         blank = ' '
         print(f'{blank:>{offset}}Resource Class Info')
         print(f'{blank:>{offset + 2}}Name:            {self._name}')
         print(f'{blank:>{offset + 2}}Ontology prefix: {self._ontology_id}')
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/sipi.py` & `dsp_tools-2.3.1/src/dsp_tools/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/user.py` & `dsp_tools-2.3.1/src/dsp_tools/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/value.py` & `dsp_tools-2.3.1/src/dsp_tools/models/value.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                  iri: Optional[str] = None,
                  comment: Optional[LangString] = None,
                  permissions: Optional[Permissions] = None,
                  upermission: Optional[PermissionValue] = None,
                  ark_url: Optional[str] = None,
                  vark_url: Optional[str] = None):
         self._iri = iri
-        self._comment = comment
+        self._comment = str(comment) if comment else None
         self._permissions = permissions
         self._upermission = upermission
         self._ark_url = ark_url
         self._vark_url = vark_url
 
     def __str__(self):
         if self._iri:
@@ -95,15 +95,15 @@
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = {}
         if action == Actions.Create:
             if self._permissions:
                 tmp["knora-api:hasPermissions"] = self.permissions.toJsonLdObj()
             if self._comment:
-                tmp["knora-api:valueHasComment"] = str(self._comment)
+                tmp["knora-api:valueHasComment"] = self._comment
         return tmp
 
     @staticmethod
     def get_typed_value(key: str, jsonld_obj: Any) -> Union[str, float]:
         try:
             tmp = jsonld_obj[key]
             if tmp.get("@type") == "xsd:decimal":
@@ -118,18 +118,18 @@
                 result = str(tmp["@value"])
             elif tmp.get("@id"):
                 result = tmp["@id"]
             else:
                 raise BaseError("Invalid data type in JSON-LD: \"{}\"!".format(tmp["@type"]))
             return result
         except KeyError as kerr:
-            raise BaseError("Error in JSON-LD returned!")
+            raise BaseError("Error in JSON-LD returned!") from kerr
 
     @staticmethod
-    def getFromJsonLd(jsonld_obj) -> dict[str, Union[str, float]]:
+    def getFromJsonLd(jsonld_obj) -> dict[str, Any]:
 
         return {
             'iri': jsonld_obj.get("@id"),
             'comment': jsonld_obj.get("knora-api:valueHasComment"),
             'ark_url': Value.get_typed_value("knora-api:arkUrl", jsonld_obj),
             'vark_url': Value.get_typed_value("knora-api:versionArkUrl", jsonld_obj),
             'permissions': Permissions.fromString(jsonld_obj.get("knora-api:hasPermissions")),
@@ -949,17 +949,19 @@
         'knora-api:IntervalValue': IntervalValue,
         'knora-api:ListValue': ListValue,
         'knora-api:LinkValue': LinkValue,
     }
     return switcher[jsonld_obj.get('@type')].fromJsonLdObj(jsonld_obj)
 
 
-def make_value(value: Value,
-               comment: Optional[str] = None,
-               permissions: Optional[Permissions] = None):
+def make_value(
+    value: Union[Value, str],
+    comment: Optional[str] = None,
+    permissions: Optional[Permissions] = None
+) -> dict[str, Any]:
     res = {}
     res['value'] = value
     if comment:
         res['comment'] = comment
     if permissions:
         res['permissions'] = permissions
     return res
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/xmlallow.py` & `dsp_tools-2.3.1/src/dsp_tools/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/xmlbitstream.py` & `dsp_tools-2.3.1/src/dsp_tools/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/xmlpermission.py` & `dsp_tools-2.3.1/src/dsp_tools/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/xmlproperty.py` & `dsp_tools-2.3.1/src/dsp_tools/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/xmlresource.py` & `dsp_tools-2.3.1/src/dsp_tools/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/models/xmlvalue.py` & `dsp_tools-2.3.1/src/dsp_tools/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-2.3.1/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-2.3.1/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-2.3.1/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-2.3.1/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/resources/schema/project.json` & `dsp_tools-2.3.1/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-2.3.1/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-2.3.1/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-2.3.1/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_lists.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_lists.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     JSON, and returns the expanded "lists" section. If there are no references to Excel files, the "lists" section is
     returned as is.
     Returns a tuple consisting of the expanded "lists" section and a boolean value: True if everything went smoothly,
     False if one of the lists couldn't be expanded correctly.
 
     Args:
         lists_section: the "lists" section of a parsed JSON project file. If this is an empty list, an empty list will be returned.
-    
+
     Raises:
         BaseError: if a problem occurred while trying to expand the Excel files
 
     Returns:
         the same "lists" section, but without references to Excel files
     """
     new_lists = []
@@ -56,17 +56,19 @@
                 # section needs to replace the Excel folder reference. But the rest of the user-defined list element
                 # needs to stay intact, e.g. the labels and comments.
                 _list["nodes"] = returned_lists_section[0]["nodes"]
                 new_lists.append(_list)
                 print(f"\tThe list '{_list['name']}' contains a reference to the folder '{foldername}'. The Excel "
                       f"files therein have been temporarily expanded into the 'lists' section of your project.")
             except BaseError as err:
-                raise BaseError(f"\tWARNING: The list '{_list['name']}' contains a reference to the folder '{foldername}', but a "
-                      f"problem occurred while trying to expand the Excel files therein into the 'lists' section of "
-                      f"your project: {err.message}") from None
+                raise BaseError(
+                    f"\tWARNING: The list '{_list['name']}' contains a reference to the folder '{foldername}', but a "
+                    f"problem occurred while trying to expand the Excel files therein into the 'lists' section of "
+                    f"your project: {err.message}"
+                ) from None
 
     return new_lists
 
 
 def _get_values_from_excel(
     excelfiles: dict[str, Worksheet],
     base_file: dict[str, Worksheet],
@@ -99,30 +101,32 @@
     nodes: list[dict[str, Any]] = []
     currentnode: dict[str, Any] = dict()
     base_file_ws: Worksheet = list(base_file.values())[0]
     cell: Cell = base_file_ws.cell(column=col, row=row)
 
     for excelfile in excelfiles.values():
         if any((not excelfile["A1"].value, excelfile["B1"].value)):
-            raise BaseError(f"ERROR: Inconsistency in Excel list: The first row must consist of exactly one value, in "
-                            f"cell A1. All other cells of row 1 must be empty.\nInstead, found the following:\n"
-                            f"Cell A1: '{excelfile['A1'].value}'\n"
-                            f"Cell B1: '{excelfile['B1'].value}'")
+            raise BaseError(
+                f"ERROR: Inconsistency in Excel list: The first row must consist of exactly one value, in cell A1. "
+                f"All other cells of row 1 must be empty.\nInstead, found the following:\n"
+                f" - Cell A1: '{excelfile['A1'].value}'\n"
+                f" - Cell B1: '{excelfile['B1'].value}'"
+            )
 
     if col > 1:
         # append the cell value of the parent node (which is one value to the left of the current cell) to the list of
         # previous values
         preval.append(str(base_file_ws.cell(column=col-1, row=row).value).strip())
 
     while cell.value and regex.search(r"\p{L}", str(cell.value), flags=re.UNICODE):
         # check if all predecessors in row (values to the left) are consistent with the values in preval list
         for idx, val in enumerate(preval[:-1]):
             if val != str(base_file_ws.cell(column=idx+1, row=row).value).strip():
-                raise BaseError(f"ERROR: Inconsistency in Excel list: {val} not equal to "
-                                f"{str(base_file_ws.cell(column=idx+1, row=row).value).strip()}")
+                raise BaseError("ERROR: Inconsistency in Excel list: "
+                                f"{val} not equal to {str(base_file_ws.cell(column=idx+1, row=row).value).strip()}")
 
         # loop through the row until the last (furthest right) value is found
         next_value = base_file_ws.cell(column=col+1, row=row).value
         if next_value and regex.search(r"\p{L}", str(next_value), flags=re.UNICODE):
             row, _ = _get_values_from_excel(
                 excelfiles=excelfiles,
                 base_file=base_file,
@@ -137,32 +141,32 @@
         else:
             # check if there are duplicate nodes (i.e. identical rows), raise a BaseError if so
             new_check_list = preval.copy()
             new_check_list.append(str(cell.value).strip())
             list_of_lists_of_previous_cell_values.append(new_check_list)
 
             if any(list_of_lists_of_previous_cell_values.count(x) > 1 for x in list_of_lists_of_previous_cell_values):
-                raise BaseError(f"ERROR: There is at least one duplicate node in the list. Found duplicate in column "
-                                f"{cell.column}, row {cell.row}:\n'{str(cell.value).strip()}'")
+                raise BaseError(f"ERROR: There is at least one duplicate node in the list. "
+                                f"Found duplicate in column {cell.column}, row {cell.row}:\n'{str(cell.value).strip()}'")
 
             # create a simplified version of the cell value and use it as name of the node
             nodename = simplify_name(str(cell.value).strip())
             list_of_previous_node_names.append(nodename)
 
             # append a number (p.ex. node-name-2) if there are list nodes with identical names
             n = list_of_previous_node_names.count(nodename)
             if n > 1:
                 nodename = nodename + "-" + str(n)
 
             # read label values from the other Excel files (other languages)
             labels_dict: dict[str, str] = {}
             for other_lang, ws_other_lang in excelfiles.items():
                 cell_value = ws_other_lang.cell(column=col, row=row).value
-                if not(isinstance(cell_value, str) and len(cell_value) > 0):
-                    raise BaseError(f"ERROR: Malformed Excel file: The Excel file with the language code "
+                if not (isinstance(cell_value, str) and len(cell_value) > 0):
+                    raise BaseError("ERROR: Malformed Excel file: The Excel file with the language code "
                                     f"'{other_lang}' should have a value in row {row}, column {col}")
                 else:
                     labels_dict[other_lang] = cell_value.strip()
 
             # create current node from extracted cell values and append it to the nodes list
             currentnode = {"name": nodename, "labels": labels_dict}
             nodes.append(currentnode)
@@ -259,32 +263,33 @@
         BaseError with a detailed error report if the validation fails
 
     Returns:
         True if the "lists" section passed validation
     """
     if bool(path_to_json_project_file) == bool(lists_section):
         raise BaseError("Validation of the 'lists' section works only if exactly one of the two arguments is given.")
-    
+
     with importlib.resources.files("dsp_tools").joinpath("resources/schema/lists-only.json").open(encoding="utf-8") as schema_file:
         lists_schema = json.load(schema_file)
 
     if path_to_json_project_file:
         with open(path_to_json_project_file, encoding="utf-8") as f:
             project = json.load(f)
             lists_section = project["project"].get("lists")
             if not lists_section:
-                raise BaseError(f"Cannot validate \"lists\" section of {path_to_json_project_file}, because there is "
-                                f"no \"lists\" section in this file.")
+                raise BaseError(f"Cannot validate \"lists\" section of {path_to_json_project_file}, "
+                                "because there is no \"lists\" section in this file.")
 
     try:
         jsonschema.validate(instance={"lists": lists_section}, schema=lists_schema)
     except jsonschema.ValidationError as err:
-        raise BaseError(f'"lists" section did not pass validation. The error message is: {err.message}\n'
-                        f'The error occurred at {err.json_path}') from None
-    
+        raise BaseError(
+            f'"lists" section did not pass validation. The error message is: {err.message}\nThe error occurred at {err.json_path}'
+        ) from None
+
     return True
 
 
 def _extract_excel_file_paths(excelfolder: str) -> list[str]:
     """
     This method extracts the names of the Excel files that are in the folder, and asserts that they are named according
     to the requirements.
@@ -297,17 +302,18 @@
 
     Returns:
         list of the Excel file paths to process
     """
     if not os.path.isdir(excelfolder):
         raise BaseError(f"ERROR: {excelfolder} is not a directory.")
 
-    excel_file_paths = [filename for filename in glob.iglob(f"{excelfolder}/*.xlsx")
-                        if not os.path.basename(filename).startswith("~$")
-                        and os.path.isfile(filename)]
+    excel_file_paths = [
+        filename for filename in glob.iglob(f"{excelfolder}/*.xlsx")
+        if not os.path.basename(filename).startswith("~$") and os.path.isfile(filename)
+    ]
 
     for filepath in excel_file_paths:
         if not re.search(r'^(de|en|fr|it|rm)\.xlsx$', os.path.basename(filepath)):
             raise BaseError(f"Invalid file name '{filepath}'. Expected format: 'languagecode.xlsx'")
 
     return excel_file_paths
 
@@ -332,15 +338,15 @@
         a tuple consisting of the "lists" section as Python list, and the success status (True if everything went well)
     """
     # read the data
     excel_file_paths = _extract_excel_file_paths(excelfolder)
     if verbose:
         print("The following Excel files will be processed:")
         print(*(f" - {filename}" for filename in excel_file_paths), sep="\n")
-    
+
     # construct the "lists" section
     finished_lists = _make_json_lists_from_excel(excel_file_paths, verbose=verbose)
     validate_lists_section_with_schema(lists_section=finished_lists)
 
     # write final "lists" section
     if path_to_output_file:
         with open(path_to_output_file, "w", encoding="utf-8") as fp:
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_project.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,39 +46,36 @@
     if not os.path.isdir(data_model_files):
         raise BaseError(f"ERROR: {data_model_files} is not a directory.")
     folder = [x for x in os.scandir(data_model_files) if not re.search(r"^(\.|~\$).+", x.name)]
 
     processed_files = []
     onto_folders = [x for x in folder if os.path.isdir(x) and re.search(r"([\w.-]+) (\([\w.\- ]+\))", x.name)]
     if len(onto_folders) == 0:
-        raise BaseError(f"'{data_model_files}' must contain at least one subfolder named after the pattern "
-                        f"'onto_name (onto_label)'")
+        raise BaseError(f"'{data_model_files}' must contain at least one subfolder named after the pattern 'onto_name (onto_label)'")
     for onto_folder in onto_folders:
         contents = sorted([x.name for x in os.scandir(onto_folder) if not re.search(r"^(\.|~\$).+", x.name)])
         if contents != ["properties.xlsx", "resources.xlsx"]:
             raise BaseError(f"ERROR: '{data_model_files}/{onto_folder.name}' must contain one file 'properties.xlsx' "
-                            f"and one file 'resources.xlsx', but nothing else.")
+                            "and one file 'resources.xlsx', but nothing else.")
         processed_files.extend([f"{data_model_files}/{onto_folder.name}/{file}" for file in contents])
 
     listfolder = [x for x in folder if os.path.isdir(x) and x.name == "lists"]
     if listfolder:
         listfolder_contents = [x for x in os.scandir(listfolder[0]) if not re.search(r"^(\.|~\$).+", x.name)]
         if not all(re.search(r"(de|en|fr|it|rm).xlsx", file.name) for file in listfolder_contents):
-            raise BaseError(f"The only files allowed in '{data_model_files}/lists' are en.xlsx, de.xlsx, fr.xlsx, "
-                            f"it.xlsx, rm.xlsx")
+            raise BaseError(f"The only files allowed in '{data_model_files}/lists' are en.xlsx, de.xlsx, fr.xlsx, it.xlsx, rm.xlsx")
         processed_files = [f"{data_model_files}/lists/{file.name}" for file in listfolder_contents] + processed_files
 
     if len(onto_folders) + len(listfolder) != len(folder):
-        raise BaseError(f"The only allowed subfolders in '{data_model_files}' are 'lists' and folders that match the "
-                        f"pattern 'onto_name (onto_label)'")
+        raise BaseError(f"The only allowed subfolders in '{data_model_files}' are 'lists' "
+                        "and folders that match the pattern 'onto_name (onto_label)'")
 
     print("The following files will be processed:")
     print(*(f" - {file}" for file in processed_files), sep="\n")
 
-
     # create output
     # -------------
     lists, success = excel2lists(excelfolder=f"{data_model_files}/lists") if listfolder else (None, True)
     if not success:
         overall_success = False
 
     ontologies = []
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_properties.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
     This function checks if the "properties" section of a JSON project file is valid according to the JSON schema,
     and if the property names are unique.
 
     Args:
         properties_list: the "properties" section of a JSON project as a list of dicts
         excelfile: path to the Excel file containing the properties
-    
+
     Raises:
         BaseError with a detailed error report if the validation fails
 
     Returns:
         True if the "properties" section passed validation
     """
     with importlib.resources.files("dsp_tools").joinpath("resources/schema/properties-only.json").open(encoding="utf-8") as schema_file:
@@ -42,27 +42,27 @@
             err_msg += f"The problematic property is '{wrong_property_name}' in Excel row {excel_row}. "
             affected_field = re.search(r"name|labels|comments|super|subject|object|gui_element|gui_attributes", err.json_path)
             if affected_field:
                 err_msg += f"The problem is that the column '{affected_field.group(0)}' has an invalid value: {err.message}"
         else:
             err_msg += f"The error message is: {err.message}\nThe error occurred at {err.json_path}"
         raise BaseError(err_msg) from None
-    
+
     # check if property names are unique
     all_names = [p["name"] for p in properties_list]
     duplicates: dict[int, str] = dict()
     for index, propdef in enumerate(properties_list):
         if all_names.count(propdef["name"]) > 1:
             duplicates[index+2] = propdef["name"]
     if duplicates:
         err_msg = f"Property names must be unique inside every ontology, but your Excel file '{excelfile}' contains duplicates:\n"
         for row_no, propname in duplicates.items():
             err_msg += f" - Row {row_no}: {propname}\n"
         raise BaseError(err_msg)
-    
+
     return True
 
 
 def _row2prop(row: pd.Series, row_count: int, excelfile: str) -> dict[str, Any]:
     """
     Takes a row from a pandas DataFrame, reads its content, and returns a dict object of the property
 
@@ -90,16 +90,16 @@
     gui_attributes = dict()
     if row.get("hlist"):
         gui_attributes["hlist"] = row["hlist"]
     if row.get("gui_attributes"):
         pairs = row["gui_attributes"].split(",")
         for pair in pairs:
             if pair.count(":") != 1:
-                raise BaseError(f"Row {row_count} of Excel file {excelfile} contains invalid data in column "
-                                 f"'gui_attributes'. The expected format is 'attribute: value[, attribute: value]'.")
+                raise BaseError(f"Row {row_count} of Excel file {excelfile} contains invalid data in column 'gui_attributes'. "
+                                "The expected format is 'attribute: value[, attribute: value]'.")
             attr, val = [x.strip() for x in pair.split(":")]
             if re.search(r"^\d+\.\d+$", val):
                 val = float(val)
             elif re.search(r"^\d+$", val):
                 val = int(val)
             gui_attributes[attr] = val
 
@@ -130,15 +130,15 @@
 
     Raises:
         BaseError if something went wrong
 
     Returns:
         a tuple consisting of the "properties" section as Python list, and the success status (True if everything went well)
     """
-    
+
     # load file
     try:
         df: pd.DataFrame = pd.read_excel(excelfile)
     except ValueError:
         # Pandas relies on openpyxl to parse XLSX files.
         # A strange behaviour of openpyxl prevents pandas from opening files with some formatting properties
         # (unclear which formatting properties exactly).
@@ -177,9 +177,8 @@
     # write final JSON file
     _validate_properties(properties_list=props, excelfile=excelfile)
     if path_to_output_file:
         with open(file=path_to_output_file, mode="w", encoding="utf-8") as file:
             json.dump(props, file, indent=4, ensure_ascii=False)
             print('"properties" section was created successfully and written to file:', path_to_output_file)
 
-
     return props, True
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/excel_to_json_resources.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,40 +50,40 @@
                                f"in row {excel_row}, column 'Cardinality': {err.message}"
                 elif err.json_path.endswith("propname"):
                     err_msg += f"The problem is that the Excel sheet '{wrong_resource_name}' contains an invalid value " \
                                f"in row {excel_row}, column 'Property': {err.message}"
         else:
             err_msg += f"The error message is: {err.message}\nThe error occurred at {err.json_path}"
         raise BaseError(err_msg) from None
-    
+
     # check if resource names are unique
     all_names = [r["name"] for r in resources_list]
     duplicates: dict[int, str] = dict()
     for index, resdef in enumerate(resources_list):
         if all_names.count(resdef["name"]) > 1:
             duplicates[index+2] = resdef["name"]
     if duplicates:
         err_msg = f"Resource names must be unique inside every ontology, but your Excel file '{excelfile}' contains duplicates:\n"
         for row_no, resname in duplicates.items():
             err_msg += f" - Row {row_no}: {resname}\n"
         raise BaseError(err_msg)
-    
+
     return True
 
 
 def _row2resource(row: pd.Series, excelfile: str) -> dict[str, Any]:
     """
     Method that reads one row from the "classes" DataFrame, 
     opens the corresponding details DataFrame, 
     and builds a dict object of the resource.
 
     Args:
         row: row from the "classes" DataFrame
         excelfile: Excel file where the data comes from
-    
+
     Raises:
         BaseError if the row or the details sheet contains invalid data
 
     Returns:
         dict object of the resource
     """
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/generate_templates.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/generate_templates.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/id_to_iri.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/id_to_iri.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,27 @@
 
 from lxml import etree
 
 from dsp_tools.models.exceptions import BaseError
 
 
 def id_to_iri(xml_file: str, json_file: str, out_file: Optional[str], verbose: bool) -> bool:
-
     """
     This function replaces all occurrences of internal IDs with their respective IRIs inside an XML file. It gets the
     mapping from the JSON file provided as parameter for this function.
 
     Args:
         xml_file: the XML file with the data to be replaced
         json_file: the JSON file with the mapping (dict) of internal IDs to IRIs
         out_file: path to the output XML file with replaced IDs (optional), default "id2iri_replaced_" + timestamp + ".xml"
         verbose: verbose feedback if set to True
 
     Raises:
         BaseError if one of the two input files is not a valid file
-    
+
     Returns:
         True if everything went well, False otherwise
     """
     success = True
 
     # check that provided files exist
     if not os.path.isfile(xml_file):
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/project_create.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/project_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,20 +47,20 @@
         # the normal, expected case is that this try block fails
         project_local = Project(con=con, shortcode=project_definition["project"]["shortcode"])
         project_remote: Project = try_network_action(project_local.read)
         print(f"\tWARNING: Project '{project_remote.shortname}' ({project_remote.shortcode}) already exists on the DSP server. Updating it...")
         logger.warning(f"Project '{project_remote.shortname}' ({project_remote.shortcode}) already exists on the DSP server. Updating it...")
         # try to update the basic info
         project_remote, _ = _update_basic_info_of_project(project=project_remote, project_definition=project_definition, verbose=verbose)
-        # It doesn't matter if the update is successful or not: continue anyway, because success is anyways false. 
+        # It doesn't matter if the update is successful or not: continue anyway, because success is anyways false.
         # There are other things from this file that can be created on the server, e.g. the groups and users, so the process must continue.
         return project_remote, False
     except BaseError:
         pass
-    
+
     success = True
     project_local = Project(
         con=con,
         shortcode=project_definition["project"]["shortcode"],
         shortname=project_definition["project"]["shortname"],
         longname=project_definition["project"]["longname"],
         description=LangString(project_definition["project"].get("descriptions")),
@@ -145,15 +145,15 @@
     except BaseError:
         err_msg = "Unable to check if group names are already existing on DSP server, because it is " \
                   "not possible to retrieve the remote groups from the DSP server."
         print(f"WARNING: {err_msg}")
         logger.warning(err_msg, exc_info=True)
         remote_groups = []
         overall_success = False
-        
+
     for group in groups:
         group_name = group["name"]
 
         # if the group already exists, add it to "current_project_groups" (for later usage), then skip it
         remotely_existing_group = [g for g in remote_groups if g.name == group_name]
         if remotely_existing_group:
             current_project_groups[group_name] = remotely_existing_group[0]
@@ -163,15 +163,15 @@
 
         # create the group
         group_local = Group(
             con=con,
             name=group_name,
             descriptions=LangString(group["descriptions"]),
             project=project,
-            status=bool(group.get("status", True)),  
+            status=bool(group.get("status", True)),
             selfjoin=bool(group.get("selfjoin", False))
         )
         try:
             group_remote: Group = try_network_action(group_local.create)
         except BaseError:
             print(f"\tWARNING: Unable to create group '{group_name}'.")
             logger.warning(f"Unable to create group '{group_name}'.", exc_info=True)
@@ -181,18 +181,18 @@
         current_project_groups[group_remote.name] = group_remote  # type: ignore
         print(f"\tCreated group '{group_name}'.")
 
     return current_project_groups, overall_success
 
 
 def _get_group_iris_for_user(
-    json_user_definition: dict[str, str], 
-    current_project: Project, 
-    current_project_groups: dict[str, Group], 
-    con: Connection, 
+    json_user_definition: dict[str, str],
+    current_project: Project,
+    current_project_groups: dict[str, Group],
+    con: Connection,
     verbose: bool
 ) -> tuple[set[str], bool, bool]:
     """
     Retrieve the IRIs of the groups that the user belongs to.
 
     Args:
         json_user_definition: the section of the JSON file that defines a user
@@ -210,32 +210,30 @@
     username = json_user_definition["username"]
     group_iris: set[str] = set()
     sysadmin = False
     remote_groups: list[Group] = []
     for full_group_name in json_user_definition.get("groups", []):
         # full_group_name has the form '[project_shortname]:group_name' or 'SystemAdmin'
         if ":" not in full_group_name and full_group_name != "SystemAdmin":
-            print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because such a "
-                    f"group doesn't exist.")
+            print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because such a group doesn't exist.")
             success = False
             continue
 
         if full_group_name == "SystemAdmin":
             sysadmin = True
             if verbose:
                 print(f"\tAdded user '{username}' to group 'SystemAdmin'.")
             continue
 
         # all other cases (":" in full_group_name)
         project_shortname, group_name = full_group_name.split(":")
         if not project_shortname:
             # full_group_name refers to a group inside the same project
             if group_name not in current_project_groups:
-                print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because "
-                        f"such a group doesn't exist.")
+                print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because such a group doesn't exist.")
                 success = False
                 continue
             group = current_project_groups[group_name]
         else:
             # full_group_name refers to an already existing group on DSP
             try:
                 # "remote_groups" might be available from a previous loop cycle
@@ -245,31 +243,30 @@
                           f"exists on the DSP server, but no groups could be retrieved from the DSP server."
                 print(f"\tWARNING: {err_msg}")
                 logger.warning(err_msg, exc_info=True)
                 success = False
                 continue
             existing_group = [g for g in remote_groups if g.project == current_project.id and g.name == group_name]
             if not existing_group:
-                print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because "
-                        f"such a group doesn't exist.")
+                print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because such a group doesn't exist.")
                 success = False
                 continue
             group = existing_group[0]
 
         group_iris.add(group.id)  # type: ignore
         if verbose:
             print(f"\tAdded user '{username}' to group '{full_group_name}'.")
 
     return group_iris, sysadmin, success
 
 
 def _get_projects_where_user_is_admin(
-    json_user_definition: dict[str, str], 
-    current_project: Project, 
-    con: Connection, 
+    json_user_definition: dict[str, str],
+    current_project: Project,
+    con: Connection,
     verbose: bool
 ) -> tuple[dict[str, bool], bool]:
     """
     Create a dict that tells for every project if the user is administrator in that project or not.
 
     Args:
         json_user_definition: the section of the JSON file that defines a user
@@ -283,16 +280,15 @@
     success = True
     username = json_user_definition["username"]
     project_info: dict[str, bool] = {}
     remote_projects: list[Project] = []
     for full_project_name in json_user_definition.get("projects", []):
         # full_project_name has the form '[project_name]:member' or '[project_name]:admin'
         if ":" not in full_project_name:
-            print(f"\tWARNING: Provided project '{full_project_name}' for user '{username}' is not valid. "
-                    f"Skipping...")
+            print(f"\tWARNING: Provided project '{full_project_name}' for user '{username}' is not valid. Skipping...")
             success = False
             continue
 
         project_name, project_role = full_project_name.split(":")
         if not project_name:
             # full_project_name refers to the current project
             in_project = current_project
@@ -306,24 +302,23 @@
                           f"because the projects cannot be retrieved from the DSP server."
                 print(f"\tWARNING: {err_msg}")
                 logger.warning(err_msg, exc_info=True)
                 success = False
                 continue
             in_project_list = [p for p in remote_projects if p.shortname == project_name]
             if not in_project_list:
-                print(f"\tWARNING: Provided project '{full_project_name}' for user '{username}' is not valid. "
-                        f"Skipping...")
+                print(f"\tWARNING: Provided project '{full_project_name}' for user '{username}' is not valid. Skipping...")
                 success = False
                 continue
             in_project = in_project_list[0]
 
         project_info[in_project.id] = bool(project_role == "admin")  # type: ignore
         if verbose:
             print(f"\tAdded user '{username}' as {project_role} to project '{in_project.shortname}'.")
-        
+
     return project_info, success
 
 
 def _create_users(
     con: Connection,
     users_section: list[dict[str, str]],
     current_project_groups: dict[str, Group],
@@ -413,15 +408,15 @@
     Args:
         unsorted_resources: list of resources from a parsed JSON project file
         onto_name: name of the onto
 
     Returns:
         sorted list of resource classes
     """
-    
+
     # do not modify the original unsorted_resources, which points to the original JSON project file
     resources_to_sort = unsorted_resources.copy()
     sorted_resources: list[dict[str, Any]] = list()
     ok_resource_names: list[str] = list()
     while len(resources_to_sort) > 0:
         # inside the for loop, resources_to_sort is modified, so a copy must be made to iterate over
         for res in resources_to_sort.copy():
@@ -765,19 +760,18 @@
     print("\tAdd cardinalities to resource classes...")
     switcher = {
         "1": Cardinality.C_1,
         "0-1": Cardinality.C_0_1,
         "0-n": Cardinality.C_0_n,
         "1-n": Cardinality.C_1_n
     }
-    for res_class in ontology_definition.get("resources", []): 
+    for res_class in ontology_definition.get("resources", []):
         res_class_remote = remote_res_classes.get(ontology_remote.id + "#" + res_class["name"])
         if not res_class_remote:
-            print(f"WARNING: Unable to add cardinalities to resource class '{res_class['name']}': This class "
-                  f"doesn't exist on the DSP server.")
+            print(f"WARNING: Unable to add cardinalities to resource class '{res_class['name']}': This class doesn't exist on the DSP server.")
             overall_success = False
             continue
         for card_info in res_class.get("cardinalities", []):
             if ":" in card_info["propname"]:
                 prefix, prop = card_info["propname"].split(":")
                 qualified_propname = card_info["propname"] if prefix else f"{ontology_remote.name}:{prop}"
             else:
@@ -840,25 +834,27 @@
         True if everything went smoothly, False if a warning or error occurred
     """
 
     knora_api_prefix = "knora-api:"
     overall_success = True
 
     project_definition = parse_json_input(project_file_as_path_or_parsed=project_file_as_path_or_parsed)
+    proj_shortname = project_definition['project']['shortname']
+    proj_shortcode = project_definition['project']['shortcode']
     context = Context(project_definition.get("prefixes", {}))
 
     # expand the Excel files referenced in the "lists" section of the project (if any), and add them to the project
     new_lists = expand_lists_from_excel(project_definition.get("project", {}).get("lists", []))
     if new_lists:
         project_definition["project"]["lists"] = new_lists
 
     # validate against JSON schema
     validate_project(project_definition, expand_lists=False)
     print('\tJSON project file is syntactically correct and passed validation.')
-    print(f"Create project '{project_definition['project']['shortname']}' ({project_definition['project']['shortcode']})...")
+    print(f"Create project '{proj_shortname}' ({proj_shortcode})...")
 
     # establish connection to DSP server
     con = login(server=server, user=user_mail, password=password)
     if dump:
         con.start_logging()
 
     # create project on DSP server
@@ -871,41 +867,41 @@
         overall_success = False
 
     # create the lists
     list_root_nodes: dict[str, Any] = {}
     if project_definition["project"].get("lists"):
         print("Create lists...")
         list_root_nodes, success = create_lists_on_server(
-            lists_to_create=project_definition["project"]["lists"], 
-            con=con, 
+            lists_to_create=project_definition["project"]["lists"],
+            con=con,
             project_remote=project_remote
         )
         if not success:
             overall_success = False
 
     # create the groups
     current_project_groups: dict[str, Group] = {}
     if project_definition["project"].get("groups"):
         print("Create groups...")
         current_project_groups, success = _create_groups(
-            con=con, 
-            groups=project_definition["project"]["groups"], 
+            con=con,
+            groups=project_definition["project"]["groups"],
             project=project_remote
         )
         if not success:
             overall_success = False
 
     # create or update the users
     if project_definition["project"].get("users"):
         print("Create users...")
         success = _create_users(
-            con=con, 
-            users_section=project_definition["project"]["users"], 
-            current_project_groups=current_project_groups, 
-            current_project=project_remote, 
+            con=con,
+            users_section=project_definition["project"]["users"],
+            current_project_groups=current_project_groups,
+            current_project=project_remote,
             verbose=verbose
         )
         if not success:
             overall_success = False
 
     # create the ontologies
     success = _create_ontologies(
@@ -919,17 +915,15 @@
     )
     if not success:
         overall_success = False
 
     # final steps
     if overall_success:
         print("========================================================\n",
-              f"Successfully created project '{project_definition['project']['shortname']}' "
-              f"({project_definition['project']['shortcode']}) with all its ontologies. There were no problems during "
-              f"the creation process.")
+              f"Successfully created project '{proj_shortname}' ({proj_shortcode}) with all its ontologies. "
+              f"There were no problems during the creation process.")
     else:
         print("========================================================\n",
-              f"WARNING: The project '{project_definition['project']['shortname']}' ({project_definition['project']['shortcode']}) "
-              f"with its ontologies could be created, but during the creation process, some problems occurred. "
-              f"Please carefully check the console output.")
+              f"WARNING: The project '{proj_shortname}' ({proj_shortcode}) with its ontologies could be created, but during the creation process, "
+              f"some problems occurred. Please carefully check the console output.")
 
     return overall_success
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/project_create_lists.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/project_create_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,28 +79,28 @@
         lists_to_create: "lists" section of a JSON project definition
         con: connection to the DSP server
         project_remote: representation of the project on the DSP server
 
     Returns:
         tuple consisting of the IRIs of the list nodes and the success status (True if everything went well)
     """
-    
+
     overall_success = True
-    
+
     # retrieve existing lists
     try:
         existing_lists: list[ListNode] = try_network_action(
             lambda: ListNode.getAllLists(con=con, project_iri=project_remote.id)
         )
     except BaseError:
         print("WARNING: Unable to retrieve existing lists on DSP server. Cannot check if your lists are already existing.")
         logger.warning("Unable to retrieve existing lists on DSP server. Cannot check if your lists are already existing.", exc_info=True)
         existing_lists = []
         overall_success = False
-    
+
     current_project_lists: dict[str, Any] = {}
     for new_list in lists_to_create:
         # if list exists already, add it to "current_project_lists" (for later usage), then skip it
         existing_list = [x for x in existing_lists if x.project == project_remote.id and x.name == new_list["name"]]
         if existing_list:
             current_project_lists[existing_list[0].name] = {"id": existing_list[0].id, "nodes": new_list["nodes"]}  # type: ignore
             print(f"\tWARNING: List '{new_list['name']}' already exists on the DSP server. Skipping...")
@@ -108,15 +108,15 @@
             continue
 
         created_list, success = _create_list_node(con=con, project=project_remote, node=new_list)
         current_project_lists.update(created_list)
         if not success:
             overall_success = False
         print(f"\tCreated list '{new_list['name']}'.")
-    
+
     return current_project_lists, overall_success
 
 
 def create_lists(
     project_file_as_path_or_parsed: Union[str, dict[str, Any]],
     server: str,
     user: str,
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/project_get.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/project_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         server : the DSP server where the data should be read from
         user : the user (e-mail) who sends the request
         password : the password of the user who sends the request
         verbose : verbose option for the command, if used more output is given to the user
 
     Raises:
         BaseError if something went wrong
-    
+
     Returns:
         True if the process finishes without errors
     """
     con = Connection(server)
     if user and password:
         con.login(user, password)
 
@@ -40,15 +40,14 @@
         project = Project(con=con, shortname=project_identifier.lower())
     elif re.match("^(http)s?://([\\w\\.\\-~]+:?\\d{,4})(/[\\w\\-~]+)+$", project_identifier):  # iri
         project = Project(con=con, shortname=project_identifier)
     else:
         raise BaseError(f"ERROR Invalid project identifier '{project_identifier}'. Use the project's shortcode, shortname or IRI.")
 
     project = project.read()
-
     project_obj = project.createDefinitionFileObj()
 
     # get groups
     if verbose:
         print("Getting groups...")
     groups_obj: list[dict[str, Any]] = []
     groups = Group.getAllGroupsForProject(con=con, proj_iri=str(project.id))
@@ -62,19 +61,21 @@
     # get users
     if verbose:
         print("Getting users...")
     users_obj: list[dict[str, Any]] = []
     users = User.getAllUsersForProject(con=con, proj_shortcode=str(project.shortcode))
     if users:
         for usr in users:
-            users_obj.append(usr.createDefinitionFileObj(
-                con=con, 
-                proj_shortname=str(project.shortname), 
-                proj_iri=str(project.id)
-            ))
+            users_obj.append(
+                usr.createDefinitionFileObj(
+                    con=con,
+                    proj_shortname=str(project.shortname),
+                    proj_iri=str(project.id)
+                )
+            )
             if verbose:
                 print(f"\tGot user '{usr.username}'")
         project_obj["users"] = users_obj
 
     # get the lists
     if verbose:
         print("Getting lists...")
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/project_validate.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/project_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,40 +30,39 @@
     propnames_duplicates: dict[str, set[str]] = dict()
     for onto in project_definition["project"]["ontologies"]:
         resnames = [r["name"] for r in onto["resources"]]
         if len(set(resnames)) != len(resnames):
             for elem in resnames:
                 if resnames.count(elem) > 1:
                     if not resnames_duplicates.get(onto["name"]):
-                        resnames_duplicates[onto["name"]] = {elem,}
+                        resnames_duplicates[onto["name"]] = {elem, }
                     else:
                         resnames_duplicates[onto["name"]].add(elem)
-        
+
         propnames = [p["name"] for p in onto["properties"]]
         if len(set(propnames)) != len(propnames):
             for elem in propnames:
                 if propnames.count(elem) > 1:
                     if not propnames_duplicates.get(onto["name"]):
-                        propnames_duplicates[onto["name"]] = {elem,}
+                        propnames_duplicates[onto["name"]] = {elem, }
                     else:
                         propnames_duplicates[onto["name"]].add(elem)
-        
+
     if not resnames_duplicates and not propnames_duplicates:
         return True
-    
+
     err_msg = "Resource names and property names must be unique inside every ontology.\n"
     for ontoname, res_duplicates in resnames_duplicates.items():
         for res_duplicate in sorted(res_duplicates):
-            err_msg += f"Resource '{res_duplicate}' appears multiple times in the ontology '{ontoname}'.\n" 
+            err_msg += f"Resource '{res_duplicate}' appears multiple times in the ontology '{ontoname}'.\n"
     for ontoname, prop_duplicates in propnames_duplicates.items():
         for prop_duplicate in sorted(prop_duplicates):
-            err_msg += f"Property '{prop_duplicate}' appears multiple times in the ontology '{ontoname}'.\n" 
-        
+            err_msg += f"Property '{prop_duplicate}' appears multiple times in the ontology '{ontoname}'.\n"
+
     raise BaseError(err_msg)
-    
 
 
 def _check_for_undefined_super_resource(project_definition: dict[str, Any]) -> bool:
     """
     Check the superresources that claim to point to a resource defined in the same JSON project.
     Check if the resource they point to actually exists.
     (DSP base resources and resources from other ontologies are not considered.)
@@ -84,28 +83,28 @@
         for res in onto["resources"]:
             supers = res["super"] if isinstance(res["super"], list) else [res["super"],]
             # form of supers:
             #  - Resource      # DSP base resource
             #  - other:res     # other onto
             #  - same:res      # same onto
             #  - :res          # same onto (short form)
-            
+
             # filter out DSP base resources
             supers = [s for s in supers if ":" in s]
             # extend short form
             supers = [regex.sub(r"^:", f"{ontoname}:", s) for s in supers]
             # filter out other ontos
             supers = [s for s in supers if regex.search(f"^{ontoname}:", s)]
             # convert to short form
             supers = [regex.sub(f"^{ontoname}", "", s) for s in supers]
 
             invalid_references = [s for s in supers if regex.sub(":", "", s) not in resnames]
             if invalid_references:
                 errors[f"Ontology '{ontoname}', resource '{res['name']}'"] = invalid_references
-    
+
     if errors:
         err_msg = "Your data model contains resources that are derived from an invalid super-resource:\n"
         err_msg += "\n".join(f" - {loc}: {invalids}" for loc, invalids in errors.items())
         raise BaseError(err_msg)
     return True
 
 
@@ -131,28 +130,28 @@
         for prop in onto["properties"]:
             supers = prop["super"]
             # form of supers:
             #  - isSequenceOf  # DSP base property
             #  - other:prop    # other onto
             #  - same:prop     # same onto
             #  - :prop         # same onto (short form)
-            
+
             # filter out DSP base properties
             supers = [s for s in supers if ":" in s]
             # extend short form
             supers = [regex.sub(r"^:", f"{ontoname}:", s) for s in supers]
             # filter out other ontos
             supers = [s for s in supers if regex.search(f"^{ontoname}:", s)]
             # convert to short form
             supers = [regex.sub(f"^{ontoname}", "", s) for s in supers]
 
             invalid_references = [s for s in supers if regex.sub(":", "", s) not in propnames]
             if invalid_references:
                 errors[f"Ontology '{ontoname}', property '{prop['name']}'"] = invalid_references
-    
+
     if errors:
         err_msg = "Your data model contains properties that are derived from an invalid super-property:\n"
         err_msg += "\n".join(f" - {loc}: {invalids}" for loc, invalids in errors.items())
         raise BaseError(err_msg)
     return True
 
 
@@ -177,28 +176,28 @@
         for res in onto["resources"]:
             cardnames = [card["propname"] for card in res.get("cardinalities", [])]
             # form of the cardnames:
             #  - isSequenceOf  # DSP base property
             #  - other:prop    # other onto
             #  - same:prop     # same onto
             #  - :prop         # same onto (short form)
-            
+
             # filter out DSP base properties
             cardnames = [card for card in cardnames if ":" in card]
             # extend short form
             cardnames = [regex.sub(r"^:", f"{ontoname}:", card) for card in cardnames]
             # filter out other ontos
             cardnames = [card for card in cardnames if regex.search(f"^{ontoname}:", card)]
             # convert to short form
             cardnames = [regex.sub(ontoname, "", card) for card in cardnames]
-            
+
             invalid_cardnames = [card for card in cardnames if regex.sub(":", "", card) not in propnames]
             if invalid_cardnames:
                 errors[f"Ontology '{ontoname}', resource '{res['name']}'"] = invalid_cardnames
-    
+
     if errors:
         err_msg = "Your data model contains cardinalities with invalid propnames:\n"
         err_msg += "\n".join(f" - {loc}: {invalids}" for loc, invalids in errors.items())
         raise BaseError(err_msg)
     return True
 
 
@@ -211,15 +210,15 @@
 
     First, the Excel file references in the "lists" section are expanded
     (unless this behaviour is disabled). 
 
     Then, the project is validated against the JSON schema. 
 
     Next, some checks are performed that are too complex for JSON schema.
-    
+
     At last, a check is performed
     if this project's ontologies contain properties derived from hasLinkTo 
     that form a circular reference.
     If so, these properties must have the cardinality 0-1 or 0-n, 
     because during the xmlupload process, 
     these values are temporarily removed.
 
@@ -273,15 +272,15 @@
     """
     Check a JSON project file if it contains properties derived from hasLinkTo that form a circular reference. If so,
     these properties must have the cardinality 0-1 or 0-n, because during the xmlupload process, these values
     are temporarily removed.
 
     Args:
         project_definition: dictionary with a DSP project (as defined in a JSON project file)
-    
+
     Raises:
         BaseError: if there is a circle with at least one element that has a cardinality of "1" or "1-n"
 
     Returns:
         True if no circle was detected, or if all elements of all circles are of cardinality "0-1" or "0-n".
     """
 
@@ -302,18 +301,18 @@
             error_message = f"{error_message}\n\t- Resource {error[0]}, property {error[1]}"
         raise BaseError(error_message)
 
 
 def _collect_link_properties(project_definition: dict[Any, Any]) -> dict[str, list[str]]:
     """
     Maps the properties derived from hasLinkTo to the resource classes they point to.
-    
+
     Args:
         project_definition: parsed JSON file
-    
+
     Returns:
         A (possibly empty) dictionary in the form {"rosetta:hasImage2D": ["rosetta:Image2D"], ...}
     """
     ontos = project_definition["project"]["ontologies"]
     hasLinkTo_props = {"hasLinkTo", "isPartOf", "isRegionOf", "isAnnotationOf"}
     link_properties: dict[str, list[str]] = dict()
     for index, onto in enumerate(ontos):
@@ -346,15 +345,15 @@
         if "Resource" in targ:
             link_properties[prop] = all_res_names
 
     return link_properties
 
 
 def _identify_problematic_cardinalities(
-    project_definition: dict[Any, Any], 
+    project_definition: dict[Any, Any],
     link_properties: dict[str, list[str]]
 ) -> list[tuple[str, str]]:
     """
     Make an error list with all cardinalities that are part of a circle but have a cardinality of "1" or "1-n".
 
     Args:
         project_definition: parsed JSON file
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/rosetta.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/rosetta.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,40 +23,40 @@
         completed_process = subprocess.run("git pull", shell=True, cwd=rosetta_folder, check=False)
         if not completed_process or completed_process.returncode != 0:
             print(f"'git pull' failed. Remove '{rosetta_folder}'...")
             shutil.rmtree(rosetta_folder, ignore_errors=True)
             is_rosetta_up_to_date = False
     else:
         is_rosetta_up_to_date = False
-    
+
     return is_rosetta_up_to_date
-    
+
 
 def _clone_repo(rosetta_folder: Path, enclosing_folder: Path) -> None:
     """
     Clones the rosetta repo into the enclosing folder.
 
     Args:
         rosetta_folder: path to the (not yet existing) clone 
         enclosing_folder: path to the (existing) destination where rosetta should be cloned into
 
     Raises:
         UserError: If rosetta cannot be cloned
     """
     print(f"Clone into {rosetta_folder}...")
     completed_process = subprocess.run(
-        "git clone https://github.com/dasch-swiss/082E-rosetta-scripts.git", 
-        shell=True, 
-        cwd=enclosing_folder, 
+        "git clone https://github.com/dasch-swiss/082E-rosetta-scripts.git",
+        shell=True,
+        cwd=enclosing_folder,
         check=False
     )
     if not completed_process or completed_process.returncode != 0:
         raise UserError("There was a problem while cloning the rosetta test project")
 
-    
+
 def _create_json(rosetta_folder: Path) -> bool:
     """
     Creates the rosetta project on the locally running DSP stack.
 
     Args:
         rosetta_folder: path to the clone
 
@@ -118,12 +118,12 @@
     enclosing_folder = Path.home() / Path(".dsp-tools/rosetta")
     enclosing_folder.mkdir(parents=True, exist_ok=True)
     rosetta_folder = enclosing_folder / "082E-rosetta-scripts"
 
     is_rosetta_up_to_date = _update_possibly_existing_repo(rosetta_folder=rosetta_folder)
     if not is_rosetta_up_to_date:
         _clone_repo(rosetta_folder=rosetta_folder, enclosing_folder=enclosing_folder)
-    
+
     success1 = _create_json(rosetta_folder=rosetta_folder)
     success2 = _upload_xml(rosetta_folder=rosetta_folder)
-    
+
     return success1 and success2
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/shared.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     Validates an XML file against the DSP XSD schema.
 
     Args:
         input_file: path to the XML file to be validated, or parsed ElementTree
 
     Raises:
         UserError with a detailed error log if the XML file is invalid
-    
+
     Returns:
         True if the XML file is valid
     """
     with importlib.resources.files("dsp_tools").joinpath("resources/schema/data.xsd").open(encoding="utf-8") as schema_file:
         xmlschema = etree.XMLSchema(etree.parse(schema_file))
     if isinstance(input_file, (str, Path)):
         try:
@@ -131,17 +131,17 @@
     if not xmlschema.validate(doc):
         error_msg = "The XML file cannot be uploaded due to the following validation error(s):"
         for error in xmlschema.error_log:
             error_msg = error_msg + f"\n  Line {error.line}: {error.message}"
         error_msg = error_msg.replace("{https://dasch.swiss/schema}", "")
         logger.error(error_msg)
         raise UserError(error_msg)
-    
+
     # make sure there are no XML tags in simple texts
-    _validate_xml_tags_in_text_properties(doc)    
+    _validate_xml_tags_in_text_properties(doc)
 
     logger.info("The XML file is syntactically correct and passed validation.")
     print("The XML file is syntactically correct and passed validation.")
     return True
 
 
 def _validate_xml_tags_in_text_properties(doc: Union[etree._ElementTree[etree._Element], etree._Element]) -> bool:
@@ -168,30 +168,30 @@
     """
     # first: remove namespaces
     doc_without_namespace = copy.deepcopy(doc)
     for elem in doc_without_namespace.iter():
         # pylint: disable-next=protected-access
         if not isinstance(elem, (etree._Comment, etree._ProcessingInstruction)):
             elem.tag = etree.QName(elem).localname
-    
+
     # then: make the test
     resources_with_illegal_xml_tags = list()
     for text in doc_without_namespace.findall(path="resource/text-prop/text"):
         if text.attrib["encoding"] == "utf8":
             if regex.search(r'<([a-zA-Z/"]+|[^\s0-9].*[^\s0-9])>', str(text.text)) or len(list(text.iterchildren())) > 0:
                 sourceline = f" line {text.sourceline}: " if text.sourceline else " "
                 propname = text.getparent().attrib["name"]           # type: ignore
                 resname = text.getparent().getparent().attrib["id"]  # type: ignore
                 resources_with_illegal_xml_tags.append(f" -{sourceline}resource '{resname}', property '{propname}'")
     if resources_with_illegal_xml_tags:
-        err_msg = "XML-tags are not allowed in text properties with encoding=utf8. The following resources of your XML file violate this rule:\n" 
+        err_msg = "XML-tags are not allowed in text properties with encoding=utf8. The following resources of your XML file violate this rule:\n"
         err_msg += "\n".join(resources_with_illegal_xml_tags)
         logger.error(err_msg, exc_info=True)
         raise UserError(err_msg)
-    
+
     return True
 
 
 def prepare_dataframe(df: pd.DataFrame, required_columns: list[str], location_of_sheet: str) -> pd.DataFrame:
     """
     Takes a pandas DataFrame, 
     strips the column headers from whitespaces and transforms them to lowercase,
@@ -201,15 +201,15 @@
     Args:
         df: pandas DataFrame
         required_columns: headers of the columns where a value is required
         location_of_sheet: for better error messages, provide this information of the caller
 
     Raises:
         BaseError if one of the required columns doesn't exist, or if the resulting DataFrame would be empty
-    
+
     Returns:
         prepared DataFrame
     """
     # strip column headers and transform to lowercase, so that the script doesn't break when the headers vary a bit
     new_df = df.rename(columns=lambda x: x.strip().lower())
     required_columns = [x.strip().lower() for x in required_columns]
     # strip every cell, and insert "" if there is no valid word in it
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/stack_handling.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/stack_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Start the Docker containers of DSP-API and DSP-APP, and load some basic data models and data. After startup, ask
     user if Docker should be pruned or not.
 
     Args:
         max_file_size: max. multimedia file size allowed by SIPI, in MB (max: 100'000)
         enforce_docker_system_prune: if True, prune Docker without asking the user
         suppress_docker_system_prune: if True, don't prune Docker (and don't ask)
-    
+
     Raises:
         BaseError if the stack cannot be started with the parameters passed by the user
 
     Returns:
         True if everything went well, False otherwise
     """
     # validate input
@@ -126,15 +126,15 @@
     else:
         prune_docker = None
         while prune_docker not in ["y", "n"]:
             prune_docker = input("Allow dsp-tools to execute 'docker system prune'? This is necessary to keep your "
                                  "Docker clean. If you are unsure what that means, just type y and press Enter. [y/n]")
     if prune_docker == "y":
         subprocess.run("docker system prune -f", shell=True, cwd=docker_path_of_user, check=False)
-    
+
     return True
 
 
 def stop_stack() -> bool:
     """
     Shut down the Docker containers of your local DSP stack and delete all data that is in it.
```

### Comparing `dsp_tools-2.3.0/src/dsp_tools/utils/xml_upload.py` & `dsp_tools-2.3.1/src/dsp_tools/utils/xml_upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     save_location = Path.home() / Path(".dsp-tools") / "xmluploads" / server_as_foldername / proj_shortcode / onto_name
     save_location.mkdir(parents=True, exist_ok=True)
     return save_location, server_as_foldername, timestamp_str
 
 
 def _write_id2iri_mapping_and_metrics(
     id2iri_mapping: dict[str, str],
-    metrics: Optional[list[MetricRecord]], 
+    metrics: Optional[list[MetricRecord]],
     failed_uploads: list[str],
     input_file: Union[str, Path, etree._ElementTree[Any]],
     timestamp_str: str,
     server_as_foldername: str
 ) -> bool:
     """
     Writes the id2iri mapping and the metrics into the current working directory,
@@ -121,15 +121,15 @@
     # determine names of files
     if isinstance(input_file, (str, Path)):
         id2iri_filename = f"{Path(input_file).stem}_id2iri_mapping_{timestamp_str}.json"
         metrics_filename = f"{timestamp_str}_metrics_{server_as_foldername}_{Path(input_file).stem}.csv"
     else:
         id2iri_filename = f"{timestamp_str}_id2iri_mapping.json"
         metrics_filename = f"{timestamp_str}_metrics_{server_as_foldername}.csv"
-    
+
     # write files and print info
     success = True
     with open(id2iri_filename, "x", encoding="utf-8") as f:
         json.dump(id2iri_mapping, f, ensure_ascii=False, indent=4)
         print(f"The mapping of internal IDs to IRIs was written to {id2iri_filename}")
         logger.info(f"The mapping of internal IDs to IRIs was written to {id2iri_filename}")
     if failed_uploads:
@@ -141,19 +141,22 @@
         df = pd.DataFrame(metrics)
         df.to_csv(f"metrics/{metrics_filename}")
         print(f"Total time of xmlupload: {sum(int(record.duration_ms) for record in metrics) / 1000:.1f} seconds")
 
     return success
 
 
-def _remove_circular_references(resources: list[XMLResource], verbose: bool) -> \
-        tuple[list[XMLResource],
-              dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
-              dict[XMLResource, dict[XMLProperty, list[str]]]
-              ]:
+def _remove_circular_references(
+    resources: list[XMLResource],
+    verbose: bool
+) -> tuple[
+    list[XMLResource],
+    dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
+    dict[XMLResource, dict[XMLProperty, list[str]]]
+]:
     """
     Temporarily removes problematic resource-references from a list of resources. A reference is problematic if
     it creates a circle (circular references).
 
     Args:
         resources: list of resources that possibly contain circular references
         verbose: verbose output if True
@@ -343,15 +346,15 @@
         tree = etree.parse(source=input_file, parser=parser)
     else:
         tree = copy.deepcopy(input_file)
         for c in tree.xpath('//comment()'):
             c.getparent().remove(c)
         for c in tree.xpath('//processing-instruction()'):
             c.getparent().remove(c)
-    
+
     # remove namespace URI from the elements' names and transform the special tags to their technically correct form
     for elem in tree.iter():
         elem.tag = etree.QName(elem).localname   # remove namespace URI in the element's name
         if elem.tag == "annotation":
             elem.attrib["restype"] = "Annotation"
             elem.tag = "resource"
         elif elem.tag == "link":
@@ -401,54 +404,54 @@
     knora_properties = resclass_name_2_type[resources[0].restype].knora_properties  # type: ignore
 
     for resource in resources:
 
         # check that the resource type is consistent with the ontology
         if resource.restype not in resclass_name_2_type:
             err_msg = f"=========================\n" \
-                      f"ERROR: Resource '{resource.label}' (ID: {resource.id}) has an invalid resource type " \
-                      f"'{resource.restype}'. Is your syntax correct? Remember the rules:\n" \
+                      f"ERROR: Resource '{resource.label}' (ID: {resource.id}) has an invalid resource type '{resource.restype}'. " \
+                      f"Is your syntax correct? Remember the rules:\n" \
                       f" - DSP-API internals: <resource restype=\"restype\">         " \
-                              f"(will be interpreted as 'knora-api:restype')\n" \
+                            f"(will be interpreted as 'knora-api:restype')\n" \
                       f" - current ontology:  <resource restype=\":restype\">        " \
-                              f"('restype' must be defined in the 'resources' section of your ontology)\n" \
+                            f"('restype' must be defined in the 'resources' section of your ontology)\n" \
                       f" - other ontology:    <resource restype=\"other:restype\">   " \
-                              f"(not yet implemented: 'other' must be defined in the same JSON project file than your ontology)" 
+                            f"(not yet implemented: 'other' must be defined in the same JSON project file as your ontology)"
             logger.error(err_msg)
             raise UserError(err_msg)
 
         # check that the property types are consistent with the ontology
         resource_properties = resclass_name_2_type[resource.restype].properties.keys()  # type: ignore
         for propname in [prop.name for prop in resource.properties]:
             if propname not in knora_properties and propname not in resource_properties:
                 err_msg = f"=========================\n" \
                           f"ERROR: Resource '{resource.label}' (ID: {resource.id}) has an invalid property '{propname}'. " \
                           f"Is your syntax correct? Remember the rules:\n" \
                           f" - DSP-API internals: <text-prop name=\"propname\">         " \
-                                  f"(will be interpreted as 'knora-api:propname')\n" \
+                                f"(will be interpreted as 'knora-api:propname')\n" \
                           f" - current ontology:  <text-prop name=\":propname\">        " \
-                                  f"('propname' must be defined in the 'properties' section of your ontology)\n" \
+                                f"('propname' must be defined in the 'properties' section of your ontology)\n" \
                           f" - other ontology:    <text-prop name=\"other:propname\">   " \
-                                  f"(not yet implemented: 'other' must be defined in the same JSON project file than your ontology)" 
+                                f"(not yet implemented: 'other' must be defined in the same JSON project file than your ontology)"
                 logger.error(err_msg)
                 raise UserError(err_msg)
 
     print("Resource types and properties are consistent with the ontology.")
     logger.info("Resource types and properties are consistent with the ontology.")
 
 
 def xml_upload(
-    input_file: Union[str, Path, etree._ElementTree[Any]],  
-    server: str, 
-    user: str, 
-    password: str, 
-    imgdir: str, 
-    sipi: str, 
+    input_file: Union[str, Path, etree._ElementTree[Any]],
+    server: str,
+    user: str,
+    password: str,
+    imgdir: str,
+    sipi: str,
     verbose: bool,
-    incremental: bool, 
+    incremental: bool,
     save_metrics: bool,
     preprocessing_done: bool
 ) -> bool:
     """
     This function reads an XML file and imports the data described in it onto the DSP server.
 
     Args:
@@ -462,22 +465,22 @@
         incremental: if set, IRIs instead of internal IDs are expected as resource pointers
         save_metrics: if true, saves time measurements into a "metrics" folder in the current working directory
         preprocessing_done: if set, all multimedia files referenced in the XML file must already be on the server
 
     Raises:
         BaseError or UserError in case of permanent network or software failure
         UserError if the XML file is invalid
-    
+
     Returns:
         True if all resources could be uploaded without errors; False if one of the resources could not be
         uploaded because there is an error in it
     """
 
-    logger.info(f"Method call xml_upload(input_file='{input_file}', server='{server}', user='{user}', imgdir='{imgdir}', "
-                f"sipi='{sipi}', verbose={verbose}, incremental={incremental}, save_metrics={save_metrics})")
+    logger.info(f"Method call xml_upload(input_file='{input_file}', server='{server}', user='{user}', imgdir='{imgdir}', sipi='{sipi}', "
+                f"verbose={verbose}, incremental={incremental}, save_metrics={save_metrics}, preprocessing_done={preprocessing_done})")
 
     # parse the XML file
     validate_xml_against_schema(input_file=input_file)
     root = _parse_xml_file(input_file=input_file)
     shortcode = root.attrib['shortcode']
     default_ontology = root.attrib['default-ontology']
     logger.info(f"Validated and parsed the XML file. Shortcode='{shortcode}' and default_ontology='{default_ontology}'")
@@ -485,15 +488,15 @@
     # determine save location that will be used for diagnostic info if the xmlupload is interrupted
     save_location, server_as_foldername, timestamp_str = _determine_save_location_of_diagnostic_info(
         server=server,
         proj_shortcode=shortcode,
         onto_name=default_ontology
     )
     logger.info(f"save_location='{save_location}'")
-    
+
     # start metrics
     metrics: list[MetricRecord] = []
     preparation_start = datetime.now()
 
     # Connect to the DaSCH Service Platform API and get the project context
     con = login(server=server, user=user, password=password)
     try:
@@ -545,21 +548,39 @@
     # upload all resources, then update the resources with the stashed XML texts and resptrs
     id2iri_mapping: dict[str, str] = {}
     failed_uploads: list[str] = []
     nonapplied_resptr_props = {}
     nonapplied_xml_texts = {}
     try:
         id2iri_mapping, failed_uploads, metrics = _upload_resources(
-            resources, imgdir, sipi_server, permissions_lookup, resclass_name_2_type, id2iri_mapping, con,
-            failed_uploads, metrics, preprocessing_done
+            resources=resources,
+            imgdir=imgdir,
+            sipi_server=sipi_server,
+            permissions_lookup=permissions_lookup,
+            resclass_name_2_type=resclass_name_2_type,
+            id2iri_mapping=id2iri_mapping,
+            con=con,
+            failed_uploads=failed_uploads,
+            metrics=metrics,
+            preprocessing_done=preprocessing_done
         )
         if stashed_xml_texts:
-            nonapplied_xml_texts = _upload_stashed_xml_texts(verbose, id2iri_mapping, con, stashed_xml_texts) 
+            nonapplied_xml_texts = _upload_stashed_xml_texts(
+                verbose=verbose,
+                id2iri_mapping=id2iri_mapping,
+                con=con,
+                stashed_xml_texts=stashed_xml_texts
+            )
         if stashed_resptr_props:
-            nonapplied_resptr_props = _upload_stashed_resptr_props(verbose, id2iri_mapping, con, stashed_resptr_props)
+            nonapplied_resptr_props = _upload_stashed_resptr_props(
+                verbose=verbose,
+                id2iri_mapping=id2iri_mapping,
+                con=con,
+                stashed_resptr_props=stashed_resptr_props
+            )
         if nonapplied_resptr_props or nonapplied_xml_texts:
             logger.error("Some stashed resptrs or XML texts could not be reapplied to their resources on the DSP server.")
             raise BaseError("Some stashed resptrs or XML texts could not be reapplied to their resources on the DSP server.")
     except BaseException as err:      # pylint: disable=broad-except
         # The forseeable errors are already handled by the variables failed_uploads, nonapplied_xml_texts, and nonapplied_resptr_props.
         # Here we catch the unforseeable exceptions, hence BaseException (=the base class of all exceptions)
         _handle_upload_error(
@@ -567,15 +588,15 @@
             id2iri_mapping=id2iri_mapping,
             failed_uploads=failed_uploads,
             stashed_xml_texts=nonapplied_xml_texts or stashed_xml_texts,
             stashed_resptr_props=nonapplied_resptr_props or stashed_resptr_props,
             save_location=save_location,
             timestamp_str=timestamp_str
         )
-    
+
     # write id2iri mapping, metrics, and print some final info
     success = _write_id2iri_mapping_and_metrics(
         id2iri_mapping=id2iri_mapping,
         failed_uploads=failed_uploads,
         metrics=metrics if save_metrics else None,
         input_file=input_file,
         timestamp_str=timestamp_str,
@@ -731,15 +752,15 @@
             # resource could not be uploaded to DSP, so the stash cannot be uploaded either
             # no action necessary: this resource will remain in nonapplied_xml_texts, which will be handled by the caller
             continue
         res_iri = id2iri_mapping[resource.id]
         try:
             existing_resource = try_network_action(con.get, path=f'/v2/resources/{quote_plus(res_iri)}')
         except BaseError as err:
-            # print the message to keep track of the cause for the failure. Apart from that, no action is necessary: 
+            # print the message to keep track of the cause for the failure. Apart from that, no action is necessary:
             # this resource will remain in nonapplied_xml_texts, which will be handled by the caller
             orig_err_msg = err.original_error_msg_from_api or err.message
             err_msg = f"Unable to upload XML texts of resource '{resource.id}', because the resource cannot be retrieved from the DSP server."
             print(f"  WARNING: {err_msg} Original error message: {orig_err_msg}")
             logger.warning(err_msg, exc_info=True)
             continue
         print(f'  Upload XML text(s) of resource "{resource.id}"...')
@@ -784,28 +805,31 @@
                 }
                 jsondata = json.dumps(jsonobj, indent=4, separators=(',', ': '), cls=KnoraStandoffXmlEncoder)
 
                 # execute API call
                 try:
                     try_network_action(con.put, path='/v2/values', jsondata=jsondata)
                 except BaseError as err:
-                    # print the message to keep track of the cause for the failure. Apart from that, no action is necessary: 
+                    # print the message to keep track of the cause for the failure. Apart from that, no action is necessary:
                     # this resource will remain in nonapplied_xml_texts, which will be handled by the caller
                     orig_err_msg = err.original_error_msg_from_api or err.message
                     err_msg = f"Unable to upload the xml text of '{link_prop.name}' of resource '{resource.id}'."
                     print(f"    WARNING: {err_msg} Original error message: {orig_err_msg}")
                     logger.warning(err_msg, exc_info=True)
                     continue
                 nonapplied_xml_texts[resource][link_prop].pop(pure_text)
                 if verbose:
                     print(f'  Successfully uploaded xml text of "{link_prop.name}"\n')
                     logger.info(f'  Successfully uploaded xml text of "{link_prop.name}"\n')
 
     # make a purged version of nonapplied_xml_texts, without empty entries
-    nonapplied_xml_texts = _purge_stashed_xml_texts(stashed_xml_texts=nonapplied_xml_texts, id2iri_mapping=id2iri_mapping)
+    nonapplied_xml_texts = _purge_stashed_xml_texts(
+        stashed_xml_texts=nonapplied_xml_texts,
+        id2iri_mapping=id2iri_mapping
+    )
     return nonapplied_xml_texts
 
 
 def _purge_stashed_xml_texts(
     stashed_xml_texts: dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
     id2iri_mapping: dict[str, str]
 ) -> dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]]:
@@ -862,15 +886,15 @@
             # resource could not be uploaded to DSP, so the stash cannot be uploaded either
             # no action necessary: this resource will remain in nonapplied_resptr_props, which will be handled by the caller
             continue
         res_iri = id2iri_mapping[resource.id]
         try:
             existing_resource = try_network_action(con.get, path=f'/v2/resources/{quote_plus(res_iri)}')
         except BaseError as err:
-            # print the message to keep track of the cause for the failure. Apart from that, no action is necessary: 
+            # print the message to keep track of the cause for the failure. Apart from that, no action is necessary:
             # this resource will remain in nonapplied_resptr_props, which will be handled by the caller
             orig_err_msg = err.original_error_msg_from_api or err.message
             err_msg = f"Unable to upload resptrs of resource '{resource.id}', because the resource cannot be retrieved from the DSP server."
             print(f"  WARNING: {err_msg} Original error message: {orig_err_msg}")
             logger.warning(err_msg, exc_info=True)
             continue
         print(f'  Upload resptrs of resource "{resource.id}"...')
@@ -890,28 +914,31 @@
                     },
                     '@context': existing_resource['@context']
                 }
                 jsondata = json.dumps(jsonobj, indent=4, separators=(',', ': '))
                 try:
                     try_network_action(con.post, path='/v2/values', jsondata=jsondata)
                 except BaseError as err:
-                    # print the message to keep track of the cause for the failure. Apart from that, no action is necessary: 
+                    # print the message to keep track of the cause for the failure. Apart from that, no action is necessary:
                     # this resource will remain in nonapplied_resptr_props, which will be handled by the caller
                     orig_err_msg = err.original_error_msg_from_api or err.message
                     err_msg = f"Unable to upload the resptr prop of '{link_prop.name}' of resource '{resource.id}'."
                     print(f"    WARNING: {err_msg} Original error message: {orig_err_msg}")
                     logger.warning(err_msg, exc_info=True)
                     continue
                 nonapplied_resptr_props[resource][link_prop].remove(resptr)
                 if verbose:
                     print(f'  Successfully uploaded resptr-prop of "{link_prop.name}". Value: {resptr}')
                     logger.info(f'Successfully uploaded resptr-prop of "{link_prop.name}". Value: {resptr}')
 
     # make a purged version of nonapplied_resptr_props, without empty entries
-    nonapplied_resptr_props = _purge_stashed_resptr_props(stashed_resptr_props=nonapplied_resptr_props, id2iri_mapping=id2iri_mapping)
+    nonapplied_resptr_props = _purge_stashed_resptr_props(
+        stashed_resptr_props=nonapplied_resptr_props,
+        id2iri_mapping=id2iri_mapping
+    )
     return nonapplied_resptr_props
 
 
 def _purge_stashed_resptr_props(
     stashed_resptr_props: dict[XMLResource, dict[XMLProperty, list[str]]],
     id2iri_mapping: dict[str, str]
 ) -> dict[XMLResource, dict[XMLProperty, list[str]]]:
@@ -974,43 +1001,60 @@
     """
 
     print("\n=========================================="
           "\nxmlupload must be aborted because of an error")
     logger.info("xmlupload must be aborted because of an error")
 
     # only stashed properties of resources that already exist in DSP are of interest
-    stashed_xml_texts = _purge_stashed_xml_texts(stashed_xml_texts, id2iri_mapping)
-    stashed_resptr_props = _purge_stashed_resptr_props(stashed_resptr_props, id2iri_mapping)
+    stashed_xml_texts = _purge_stashed_xml_texts(
+        stashed_xml_texts=stashed_xml_texts,
+        id2iri_mapping=id2iri_mapping
+    )
+    stashed_resptr_props = _purge_stashed_resptr_props(
+        stashed_resptr_props=stashed_resptr_props,
+        id2iri_mapping=id2iri_mapping
+    )
 
     if id2iri_mapping:
         id2iri_mapping_file = f"{save_location}/{timestamp_str}_id2iri_mapping.json"
         with open(id2iri_mapping_file, "x", encoding="utf-8") as f:
             json.dump(id2iri_mapping, f, ensure_ascii=False, indent=4)
         print(f"The mapping of internal IDs to IRIs was written to {id2iri_mapping_file}")
         logger.info(f"The mapping of internal IDs to IRIs was written to {id2iri_mapping_file}")
 
     if stashed_xml_texts:
         stashed_xml_texts_serializable = {r.id: {p.name: xml for p, xml in rdict.items()} for r, rdict in stashed_xml_texts.items()}
         xml_filename = f"{save_location}/{timestamp_str}_stashed_text_properties.json"
         with open(xml_filename, "x", encoding="utf-8") as f:
-            json.dump(stashed_xml_texts_serializable, f, ensure_ascii=False, indent=4, cls=KnoraStandoffXmlEncoder)
-        print(f"There are stashed text properties that could not be reapplied to the resources they were stripped "
-              f"from. They were saved to {xml_filename}.")
-        logger.info(f"There are stashed text properties that could not be reapplied to the resources they were stripped "
-                    f"from. They were saved to {xml_filename}.")
+            json.dump(
+                obj=stashed_xml_texts_serializable,
+                fp=f,
+                ensure_ascii=False,
+                indent=4,
+                cls=KnoraStandoffXmlEncoder
+            )
+        msg = f"There are stashed text properties that could not be reapplied to the resources they were stripped from. " \
+              f"They were saved to {xml_filename}."
+        print(msg)
+        logger.info(msg)
 
     if stashed_resptr_props:
         stashed_resptr_props_serializable = {r.id: {p.name: plist for p, plist in rdict.items()} for r, rdict in stashed_resptr_props.items()}
         resptr_filename = f"{save_location}/{timestamp_str}_stashed_resptr_properties.json"
         with open(resptr_filename, "x", encoding="utf-8") as f:
-            json.dump(stashed_resptr_props_serializable, f, ensure_ascii=False, indent=4)
-        print(f"There are stashed resptr properties that could not be reapplied to the resources they were stripped "
-              f"from. They were saved to {resptr_filename}")
-        logger.info(f"There are stashed resptr properties that could not be reapplied to the resources they were stripped "
-                    f"from. They were saved to {resptr_filename}")
+            json.dump(
+                obj=stashed_resptr_props_serializable,
+                fp=f,
+                ensure_ascii=False,
+                indent=4
+            )
+        msg = f"There are stashed resptr properties that could not be reapplied to the resources they were stripped from. " \
+              f"They were saved to {resptr_filename}"
+        print(msg)
+        logger.info(msg)
 
     # print the resources that threw an error when they were tried to be uploaded
     if failed_uploads:
         print(f"Independently of this error, there were some resources that could not be uploaded: {failed_uploads}")
         logger.info(f"Independently of this error, there were some resources that could not be uploaded: {failed_uploads}")
 
     if isinstance(err, KeyboardInterrupt):
```

### Comparing `dsp_tools-2.3.0/PKG-INFO` & `dsp_tools-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 2.3.0
+Version: 2.3.1
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: docker (>=6.1.2,<7.0.0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: networkx (>=3.1.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
```

