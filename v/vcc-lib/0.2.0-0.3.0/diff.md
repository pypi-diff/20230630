# Comparing `tmp/vcc_lib-0.2.0.tar.gz` & `tmp/vcc_lib-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcc_lib-0.2.0.tar", last modified: Wed Apr  5 11:14:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

