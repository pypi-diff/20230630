# Comparing `tmp/echr_extractor-1.0.8.tar.gz` & `tmp/echr_extractor-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echr_extractor-1.0.8.tar", last modified: Wed Jan  4 14:25:56 2023, max compression
+gzip compressed data, was "echr_extractor-1.0.9.tar", last modified: Wed Jan 18 16:40:41 2023, max compression
```

## Comparing `echr_extractor-1.0.8.tar` & `echr_extractor-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 14:25:56.836684 echr_extractor-1.0.8/
--rw-rw-rw-   0        0        0     9474 2023-01-04 14:25:56.835684 echr_extractor-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8896 2022-12-11 19:26:32.000000 echr_extractor-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-04 14:25:56.824684 echr_extractor-1.0.8/echr_extractor/
--rw-rw-rw-   0        0        0     2643 2022-12-05 19:35:28.000000 echr_extractor-1.0.8/echr_extractor/ECHR_html_downloader.py
--rw-rw-rw-   0        0        0     7658 2022-12-25 15:50:48.000000 echr_extractor-1.0.8/echr_extractor/ECHR_metadata_harvester.py
--rw-rw-rw-   0        0        0       59 2022-12-05 19:10:22.000000 echr_extractor-1.0.8/echr_extractor/__init__.py
--rw-rw-rw-   0        0        0     4037 2022-12-25 15:50:35.000000 echr_extractor-1.0.8/echr_extractor/echr.py
--rw-rw-rw-   0        0        0     1598 2022-12-21 16:55:27.000000 echr_extractor-1.0.8/echr_extractor/testing_file.py
-drwxrwxrwx   0        0        0        0 2023-01-04 14:25:56.833684 echr_extractor-1.0.8/echr_extractor.egg-info/
--rw-rw-rw-   0        0        0     9474 2023-01-04 14:25:56.000000 echr_extractor-1.0.8/echr_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-01-04 14:25:56.000000 echr_extractor-1.0.8/echr_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 14:25:56.000000 echr_extractor-1.0.8/echr_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-01-04 14:25:56.000000 echr_extractor-1.0.8/echr_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-01-04 14:25:56.000000 echr_extractor-1.0.8/echr_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-04 14:25:56.836684 echr_extractor-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1000 2023-01-04 14:16:50.000000 echr_extractor-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-18 16:40:41.160078 echr_extractor-1.0.9/
+-rw-rw-rw-   0        0        0     9474 2023-01-18 16:40:41.158078 echr_extractor-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8896 2022-12-11 19:26:32.000000 echr_extractor-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-18 16:40:41.146077 echr_extractor-1.0.9/echr_extractor/
+-rw-rw-rw-   0        0        0     2643 2022-12-05 19:35:28.000000 echr_extractor-1.0.9/echr_extractor/ECHR_html_downloader.py
+-rw-rw-rw-   0        0        0     7658 2022-12-25 15:50:48.000000 echr_extractor-1.0.9/echr_extractor/ECHR_metadata_harvester.py
+-rw-rw-rw-   0        0        0       59 2022-12-05 19:10:22.000000 echr_extractor-1.0.9/echr_extractor/__init__.py
+-rw-rw-rw-   0        0        0     4038 2023-01-18 16:21:46.000000 echr_extractor-1.0.9/echr_extractor/echr.py
+-rw-rw-rw-   0        0        0     1598 2022-12-21 16:55:27.000000 echr_extractor-1.0.9/echr_extractor/testing_file.py
+drwxrwxrwx   0        0        0        0 2023-01-18 16:40:41.156078 echr_extractor-1.0.9/echr_extractor.egg-info/
+-rw-rw-rw-   0        0        0     9474 2023-01-18 16:40:41.000000 echr_extractor-1.0.9/echr_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-01-18 16:40:41.000000 echr_extractor-1.0.9/echr_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-18 16:40:41.000000 echr_extractor-1.0.9/echr_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-01-18 16:40:41.000000 echr_extractor-1.0.9/echr_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-01-18 16:40:41.000000 echr_extractor-1.0.9/echr_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-18 16:40:41.160078 echr_extractor-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2023-01-18 16:40:17.000000 echr_extractor-1.0.9/setup.py
```

### Comparing `echr_extractor-1.0.8/PKG-INFO` & `echr_extractor-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echr_extractor
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for extracting ECHR data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: a.gade@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: echr_extractor Version: 1.0.8 Summary: Library for
+Metadata-Version: 2.1 Name: echr_extractor Version: 1.0.9 Summary: Library for
 extracting ECHR data Home-page: UNKNOWN Author: LawTech Lab Author-email:
 a.gade@student.maastrichtuniversity.nl License: MIT Project-URL: Bug Tracker,
 https://github.com/maastrichtlawtech/extraction_libraries Project-URL: Build
 Source, https://github.com/maastrichtlawtech/extraction_libraries Keywords:
 echr,extractor,european,convention,human,rights,european convention,human
 rights,european convention on human rights Platform: UNKNOWN Description-
 Content-Type: text/markdown ## echr extractor This library contains functions
```

### Comparing `echr_extractor-1.0.8/README.md` & `echr_extractor-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `echr_extractor-1.0.8/echr_extractor/ECHR_html_downloader.py` & `echr_extractor-1.0.9/echr_extractor/ECHR_html_downloader.py`

 * *Files identical despite different names*

### Comparing `echr_extractor-1.0.8/echr_extractor/ECHR_metadata_harvester.py` & `echr_extractor-1.0.9/echr_extractor/ECHR_metadata_harvester.py`

 * *Files identical despite different names*

### Comparing `echr_extractor-1.0.8/echr_extractor/echr.py` & `echr_extractor-1.0.9/echr_extractor/echr.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_echr(start_id=0, end_id=None, start_date=None, count=None, end_date=None, verbose=False,
              skip_missing_dates=True, save_file='y', fields=None):
     if count:
         end_id = int(start_id) + count
     print("--- STARTING ECHR DOWNLOAD ---")
-    fields = None
+    #fields = None
     df, resultcount = read_echr_metadata(start_id=start_id, end_id=end_id, start_date=start_date, end_date=end_date,
                                          verbose=verbose, skip_missing_dates=skip_missing_dates, fields=fields)
     if df is False and resultcount is False:
         return False
     if save_file == "y":
         filename = determine_filename(start_id, end_id, start_date, end_date)
         Path('data').mkdir(parents=True, exist_ok=True)
```

### Comparing `echr_extractor-1.0.8/echr_extractor/testing_file.py` & `echr_extractor-1.0.9/echr_extractor/testing_file.py`

 * *Files identical despite different names*

### Comparing `echr_extractor-1.0.8/echr_extractor.egg-info/PKG-INFO` & `echr_extractor-1.0.9/echr_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echr-extractor
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for extracting ECHR data
 Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: a.gade@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: echr-extractor Version: 1.0.8 Summary: Library for
+Metadata-Version: 2.1 Name: echr-extractor Version: 1.0.9 Summary: Library for
 extracting ECHR data Home-page: UNKNOWN Author: LawTech Lab Author-email:
 a.gade@student.maastrichtuniversity.nl License: MIT Project-URL: Bug Tracker,
 https://github.com/maastrichtlawtech/extraction_libraries Project-URL: Build
 Source, https://github.com/maastrichtlawtech/extraction_libraries Keywords:
 echr,extractor,european,convention,human,rights,european convention,human
 rights,european convention on human rights Platform: UNKNOWN Description-
 Content-Type: text/markdown ## echr extractor This library contains functions
```

### Comparing `echr_extractor-1.0.8/setup.py` & `echr_extractor-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='echr_extractor',
     packages=find_packages(include=['echr_extractor']),
-    version='1.0.8',
+    version='1.0.9',
     description='Library for extracting ECHR data',
     author='LawTech Lab',
     license='MIT',
     install_requires=["requests~=2.26.0","pandas~=1.2.5","beautifulsoup4~=4.9.3"],
     author_email='a.gade@student.maastrichtuniversity.nl',
     keywords=['echr', 'extractor', 'european', 'convention', 'human', 'rights', 'european convention', 'human rights',
               'european convention on human rights'],
```

