# Comparing `tmp/anonupload-1.1.1.tar.gz` & `tmp/anonupload-1.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonupload-1.1.1.tar", last modified: Sat Feb 25 06:20:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

