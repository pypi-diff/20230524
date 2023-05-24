# Comparing `tmp/mapel-2.0.3.dev1.tar.gz` & `tmp/mapel-2.0.3.dev6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-2.0.3.dev1.tar", last modified: Mon Feb 27 20:15:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

