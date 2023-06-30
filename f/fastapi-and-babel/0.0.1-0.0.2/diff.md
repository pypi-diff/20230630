# Comparing `tmp/fastapi-and-babel-0.0.1.tar.gz` & `tmp/fastapi_and_babel-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-and-babel-0.0.1.tar", last modified: Fri Jun 30 18:29:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

