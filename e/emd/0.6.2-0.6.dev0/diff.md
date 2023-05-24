# Comparing `tmp/emd-0.6.2.tar.gz` & `tmp/emd-0.6.dev0-py3.7.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/emd-0.6.2.tar", last modified: Wed May 24 21:01:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

