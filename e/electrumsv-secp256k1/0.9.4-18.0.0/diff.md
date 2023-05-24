# Comparing `tmp/electrumsv-secp256k1-0.9.4.tar.gz` & `tmp/electrumsv_secp256k1-18.0.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrumsv-secp256k1-0.9.4.tar", last modified: Wed Oct 27 05:55:09 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

