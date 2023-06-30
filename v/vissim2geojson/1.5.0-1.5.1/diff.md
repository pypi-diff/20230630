# Comparing `tmp/vissim2geojson-1.5.0.tar.gz` & `tmp/vissim2geojson-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vissim2geojson-1.5.0.tar", last modified: Thu Jun  1 22:11:56 2023, max compression
+gzip compressed data, was "vissim2geojson-1.5.1.tar", last modified: Fri Jun 30 00:34:16 2023, max compression
```

## Comparing `vissim2geojson-1.5.0.tar` & `vissim2geojson-1.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 22:11:56.701382 vissim2geojson-1.5.0/
--rw-rw-rw-   0        0        0     1083 2022-06-14 17:24:15.000000 vissim2geojson-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     3420 2023-06-01 22:11:56.701382 vissim2geojson-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2856 2023-06-01 22:11:23.000000 vissim2geojson-1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 22:11:56.701382 vissim2geojson-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-06-01 21:59:22.000000 vissim2geojson-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:11:56.667174 vissim2geojson-1.5.0/vissim2geojson/
--rw-rw-rw-   0        0        0      326 2023-06-01 22:04:23.000000 vissim2geojson-1.5.0/vissim2geojson/__init__.py
--rw-rw-rw-   0        0        0      320 2022-06-15 00:12:24.000000 vissim2geojson-1.5.0/vissim2geojson/_model.py
--rw-rw-rw-   0        0        0    13617 2023-06-01 22:10:12.000000 vissim2geojson-1.5.0/vissim2geojson/vissim2geojson.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:11:56.701382 vissim2geojson-1.5.0/vissim2geojson.egg-info/
--rw-rw-rw-   0        0        0     3420 2023-06-01 22:11:56.000000 vissim2geojson-1.5.0/vissim2geojson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-06-01 22:11:56.000000 vissim2geojson-1.5.0/vissim2geojson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 22:11:56.000000 vissim2geojson-1.5.0/vissim2geojson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-01 22:11:56.000000 vissim2geojson-1.5.0/vissim2geojson.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 00:34:16.318982 vissim2geojson-1.5.1/
+-rw-rw-rw-   0        0        0     1083 2022-06-14 17:24:15.000000 vissim2geojson-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     3351 2023-06-30 00:34:16.318476 vissim2geojson-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2856 2023-06-01 22:11:23.000000 vissim2geojson-1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 00:34:16.318982 vissim2geojson-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1745 2023-06-30 00:32:56.000000 vissim2geojson-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:34:16.285754 vissim2geojson-1.5.1/vissim2geojson/
+-rw-rw-rw-   0        0        0      326 2023-06-30 00:33:19.000000 vissim2geojson-1.5.1/vissim2geojson/__init__.py
+-rw-rw-rw-   0        0        0      320 2022-06-15 00:12:24.000000 vissim2geojson-1.5.1/vissim2geojson/_model.py
+-rw-rw-rw-   0        0        0    13617 2023-06-01 22:10:12.000000 vissim2geojson-1.5.1/vissim2geojson/vissim2geojson.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:34:16.315477 vissim2geojson-1.5.1/vissim2geojson.egg-info/
+-rw-rw-rw-   0        0        0     3351 2023-06-30 00:34:15.000000 vissim2geojson-1.5.1/vissim2geojson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-06-30 00:34:16.000000 vissim2geojson-1.5.1/vissim2geojson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 00:34:15.000000 vissim2geojson-1.5.1/vissim2geojson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-30 00:34:15.000000 vissim2geojson-1.5.1/vissim2geojson.egg-info/top_level.txt
```

### Comparing `vissim2geojson-1.5.0/LICENSE` & `vissim2geojson-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vissim2geojson-1.5.0/PKG-INFO` & `vissim2geojson-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: vissim2geojson
-Version: 1.5.0
-Summary: Convert vissim files(.inpx and .fzp to geojson, .fhz to csv). This tool help user to convert vissim files to wgs1984 and csv files.
+Version: 1.5.1
+Summary: Convert VISSIM files: .inpx to .geojson, .fzp and .fhz to csv.
 Home-page: https://github.com/Xiangyongluo/vissim2wgs1984
 Author: Xiangyong Luo
 Author-email: luoxiangyong01@gamil.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vissim2wgs1984
 
 Convert vissim files (.inpx and .fzp to geojson, .fhz to csv).
```

### Comparing `vissim2geojson-1.5.0/README.md` & `vissim2geojson-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `vissim2geojson-1.5.0/setup.py` & `vissim2geojson-1.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,31 +15,33 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in fh.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="vissim2geojson",  # Replace with your own username
-    version="1.5.0",
+    version="1.5.1",
     author="Xiangyong Luo",
     author_email="luoxiangyong01@gamil.com",
-    description="Convert vissim files(.inpx and .fzp to geojson, .fhz to csv). This tool help user to convert vissim files to wgs1984 and csv files.",
+    description="Convert VISSIM files: .inpx to .geojson, .fzp and .fhz to csv.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xiangyongluo/vissim2wgs1984",
 
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 
     install_requires=modules_needed,
     packages=setuptools.find_packages(),
     include_package_data=True,
 
-    package_data={'': ['*.txt', '*.xls', '*.xlsx', '*.csv', '*.png', "*.inpx", "*.fhz", "*.fzp"],
+    package_data={'': ['*.txt', '*.xls', '*.xlsx', '*.csv', '*.png',
+                       "*.inpx", "*.fhz", "*.fzp", "*.db", "*.geojson",
+                       "*.err", "*.knr", "*.lsa", "*.mer", "*.ovw", "*.rsr", "*.inp0", "*.layx", "*.sig"],
                   "test_data": ['*.txt', '*.png', "*.inpx", "*.fhz", "*.fzp"]},
-    data_files=[("vissim_data", ["vissim_data/*"])]
+    # data_files=[("vissim_data", ["vissim_data/*"])]
 )
```

### Comparing `vissim2geojson-1.5.0/vissim2geojson/vissim2geojson.py` & `vissim2geojson-1.5.1/vissim2geojson/vissim2geojson.py`

 * *Files identical despite different names*

### Comparing `vissim2geojson-1.5.0/vissim2geojson.egg-info/PKG-INFO` & `vissim2geojson-1.5.1/vissim2geojson.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: vissim2geojson
-Version: 1.5.0
-Summary: Convert vissim files(.inpx and .fzp to geojson, .fhz to csv). This tool help user to convert vissim files to wgs1984 and csv files.
+Version: 1.5.1
+Summary: Convert VISSIM files: .inpx to .geojson, .fzp and .fhz to csv.
 Home-page: https://github.com/Xiangyongluo/vissim2wgs1984
 Author: Xiangyong Luo
 Author-email: luoxiangyong01@gamil.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vissim2wgs1984
 
 Convert vissim files (.inpx and .fzp to geojson, .fhz to csv).
```

