# Comparing `tmp/byquant-1.6.28.tar.gz` & `tmp/byquant-1.6.29-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-1.6.28.tar", last modified: Fri Jun 30 01:06:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

