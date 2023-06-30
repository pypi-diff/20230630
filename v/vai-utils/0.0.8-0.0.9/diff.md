# Comparing `tmp/vai_utils-0.0.8.tar.gz` & `tmp/vai_utils-0.0.9.tar.gz`

## Comparing `vai_utils-0.0.8.tar` & `vai_utils-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vai_utils-0.0.8/requirements.txt
--rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.06565430985926124.png
--rw-r--r--   0        0        0    47189 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.07147342294341652.png
--rw-r--r--   0        0        0    33753 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.10837279097800767.png
--rw-r--r--   0        0        0    15973 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.14226826635823298.png
--rw-r--r--   0        0        0    14047 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.2966477897710217.png
--rw-r--r--   0        0        0    18545 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.5082194061656471.png
--rw-r--r--   0        0        0    42225 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.5284006170869843.png
--rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.6682099640762634.png
--rw-r--r--   0        0        0    43577 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.6929515496940593.png
--rw-r--r--   0        0        0    42433 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.701794926485459.png
--rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.9143838183319077.png
--rw-r--r--   0        0        0    47189 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/0.9859292536666209.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/__init__.py
--rw-r--r--   0        0        0    32793 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/plot.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 vai_utils-0.0.8/src/vai_utils/vai.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 vai_utils-0.0.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 vai_utils-0.0.8/LICENSE
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 vai_utils-0.0.8/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 vai_utils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 vai_utils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vai_utils-0.0.9/requirements.txt
+-rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.06565430985926124.png
+-rw-r--r--   0        0        0    47189 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.07147342294341652.png
+-rw-r--r--   0        0        0    33753 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.10837279097800767.png
+-rw-r--r--   0        0        0    15973 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.14226826635823298.png
+-rw-r--r--   0        0        0    14047 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.2966477897710217.png
+-rw-r--r--   0        0        0    18545 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.5082194061656471.png
+-rw-r--r--   0        0        0    42225 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.5284006170869843.png
+-rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.6682099640762634.png
+-rw-r--r--   0        0        0    43577 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.6929515496940593.png
+-rw-r--r--   0        0        0    42433 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.701794926485459.png
+-rw-r--r--   0        0        0    22000 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.7966868954273035.png
+-rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.9143838183319077.png
+-rw-r--r--   0        0        0    47189 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/0.9859292536666209.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/__init__.py
+-rw-r--r--   0        0        0    79172 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/heatmap.png
+-rw-r--r--   0        0        0   118489 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/line_chart.png
+-rw-r--r--   0        0        0    61896 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/plot.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 vai_utils-0.0.9/src/vai_utils/vai.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 vai_utils-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 vai_utils-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 vai_utils-0.0.9/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 vai_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 vai_utils-0.0.9/PKG-INFO
```

### Comparing `vai_utils-0.0.8/src/vai_utils/0.06565430985926124.png` & `vai_utils-0.0.9/src/vai_utils/0.06565430985926124.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.07147342294341652.png` & `vai_utils-0.0.9/src/vai_utils/0.07147342294341652.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.10837279097800767.png` & `vai_utils-0.0.9/src/vai_utils/0.10837279097800767.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.14226826635823298.png` & `vai_utils-0.0.9/src/vai_utils/0.14226826635823298.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.2966477897710217.png` & `vai_utils-0.0.9/src/vai_utils/0.2966477897710217.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.5082194061656471.png` & `vai_utils-0.0.9/src/vai_utils/0.5082194061656471.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.5284006170869843.png` & `vai_utils-0.0.9/src/vai_utils/0.5284006170869843.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.6682099640762634.png` & `vai_utils-0.0.9/src/vai_utils/0.6682099640762634.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.6929515496940593.png` & `vai_utils-0.0.9/src/vai_utils/0.6929515496940593.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.701794926485459.png` & `vai_utils-0.0.9/src/vai_utils/0.701794926485459.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.9143838183319077.png` & `vai_utils-0.0.9/src/vai_utils/0.9143838183319077.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/0.9859292536666209.png` & `vai_utils-0.0.9/src/vai_utils/0.9859292536666209.png`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/src/vai_utils/vai.py` & `vai_utils-0.0.9/src/vai_utils/vai.py`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/.gitignore` & `vai_utils-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/LICENSE` & `vai_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/README.md` & `vai_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vai_utils-0.0.8/pyproject.toml` & `vai_utils-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vai_utils"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="VirtuousAI", email="info@virtuousai.com" },
 ]
 dynamic = ["dependencies"]
 description = "VAI utils"
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `vai_utils-0.0.8/PKG-INFO` & `vai_utils-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vai_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: VAI utils
 Author-email: VirtuousAI <info@virtuousai.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

