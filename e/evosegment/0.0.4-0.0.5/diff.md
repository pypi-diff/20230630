# Comparing `tmp/evosegment-0.0.4.tar.gz` & `tmp/evosegment-0.0.5.tar.gz`

## Comparing `evosegment-0.0.4.tar` & `evosegment-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0   442666 2020-02-02 00:00:00.000000 evosegment-0.0.4/example.ipynb
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_0.tif
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_1-bubble_0-registration.tsv
--rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_1-reg-def.tif
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_1.tif
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_2-bubble_0-registration.tsv
--rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_2-reg-def.tif
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_2.tif
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_3-bubble_0-registration.tsv
--rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_3-reg-def.tif
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.4/data/bubble_3.tif
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 evosegment-0.0.4/evosegment/__init__.py
--rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 evosegment-0.0.4/evosegment/evoSegment.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 evosegment-0.0.4/.gitignore
--rw-r--r--   0        0        0    35076 2020-02-02 00:00:00.000000 evosegment-0.0.4/LICENSE
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 evosegment-0.0.4/README.md
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 evosegment-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    42703 2020-02-02 00:00:00.000000 evosegment-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0   746872 2020-02-02 00:00:00.000000 evosegment-0.0.5/example.ipynb
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_0.tif
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_1-bubble_0-registration.tsv
+-rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_1-reg-def.tif
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_1.tif
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_2-bubble_0-registration.tsv
+-rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_2-reg-def.tif
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_2.tif
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_3-bubble_0-registration.tsv
+-rw-r--r--   0        0        0  2663864 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_3-reg-def.tif
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.5/data/bubble_3.tif
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 evosegment-0.0.5/evosegment/__init__.py
+-rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 evosegment-0.0.5/evosegment/evoSegment.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 evosegment-0.0.5/evosegment/make_release
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 evosegment-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35076 2020-02-02 00:00:00.000000 evosegment-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 evosegment-0.0.5/README.md
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 evosegment-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    42703 2020-02-02 00:00:00.000000 evosegment-0.0.5/PKG-INFO
```

### Comparing `evosegment-0.0.4/data/bubble_0.tif` & `evosegment-0.0.5/data/bubble_0.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.4/data/bubble_1-reg-def.tif` & `evosegment-0.0.5/data/bubble_1-reg-def.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.4/data/bubble_1.tif` & `evosegment-0.0.5/data/bubble_1.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.4/data/bubble_2-reg-def.tif` & `evosegment-0.0.5/data/bubble_2-reg-def.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.4/data/bubble_2.tif` & `evosegment-0.0.5/data/bubble_2.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.4/data/bubble_3-reg-def.tif` & `evosegment-0.0.5/data/bubble_3-reg-def.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.4/data/bubble_3.tif` & `evosegment-0.0.5/data/bubble_3.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.4/LICENSE` & `evosegment-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.4/README.md` & `evosegment-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.4/pyproject.toml` & `evosegment-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "evosegment"
-version = "0.0.4"
+version = "0.0.5"
 description = 'A tool for segmentation of grayscale evolution from 4D tomograhphy data (or other images)'
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file="LICENSE"}
 keywords = []
 authors = [
   { name = "Johan Hektor", email = "johan.hektor@mau.se" },
```

### Comparing `evosegment-0.0.4/PKG-INFO` & `evosegment-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evosegment
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for segmentation of grayscale evolution from 4D tomograhphy data (or other images)
 Project-URL: Documentation, https://gitlab.com/jhektor/evoSegment#readme
 Project-URL: Issues, https://gitlab.com/jhektor/evoSegment/-/issues
 Project-URL: Source, https://gitlab.com/jhektor/evoSegment
 Author-email: Johan Hektor <johan.hektor@mau.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

