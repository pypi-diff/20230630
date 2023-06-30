# Comparing `tmp/leafy-0.1.4.tar.gz` & `tmp/leafy-0.1.5a0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leafy-0.1.4.tar", last modified: Mon Dec 26 11:04:27 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

