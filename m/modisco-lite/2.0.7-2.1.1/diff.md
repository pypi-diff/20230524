# Comparing `tmp/modisco-lite-2.0.7.tar.gz` & `tmp/modisco_lite-2.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modisco-lite-2.0.7.tar", last modified: Tue Mar  7 05:30:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

