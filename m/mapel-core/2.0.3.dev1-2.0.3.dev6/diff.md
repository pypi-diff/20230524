# Comparing `tmp/mapel-core-2.0.3.dev1.tar.gz` & `tmp/mapel_core-2.0.3.dev6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-core-2.0.3.dev1.tar", last modified: Mon Feb 27 20:15:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

