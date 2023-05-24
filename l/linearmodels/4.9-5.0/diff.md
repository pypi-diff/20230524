# Comparing `tmp/linearmodels-4.9.tar.gz` & `tmp/linearmodels-5.0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linearmodels-4.9.tar", last modified: Wed Aug 29 15:12:30 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

