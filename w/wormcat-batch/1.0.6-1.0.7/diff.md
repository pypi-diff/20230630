# Comparing `tmp/wormcat_batch-1.0.6.tar.gz` & `tmp/wormcat_batch-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormcat_batch-1.0.6.tar", last modified: Fri Jun 30 14:14:54 2023, max compression
+gzip compressed data, was "wormcat_batch-1.0.7.tar", last modified: Fri Jun 30 16:21:59 2023, max compression
```

## Comparing `wormcat_batch-1.0.6.tar` & `wormcat_batch-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-30 14:14:54.341600 wormcat_batch-1.0.6/
--rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.0.6/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-30 14:14:54.341507 wormcat_batch-1.0.6/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2346 2023-06-28 11:53:36.000000 wormcat_batch-1.0.6/README.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-06-30 14:14:54.341636 wormcat_batch-1.0.6/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      670 2023-06-30 13:00:05.000000 wormcat_batch-1.0.6/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-30 14:14:54.340532 wormcat_batch-1.0.6/wormcat_batch/
--rw-r--r--   0 dan        (501) staff       (20)     2024 2022-08-16 12:41:26.000000 wormcat_batch-1.0.6/wormcat_batch/create_wormcat_xlsx.py
--rw-r--r--   0 dan        (501) staff       (20)     2486 2023-06-27 18:05:20.000000 wormcat_batch-1.0.6/wormcat_batch/execute_r.py
--rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.0.6/wormcat_batch/is_wormcat_installed.R
--rwxr-xr-x   0 dan        (501) staff       (20)     8383 2023-06-30 14:09:43.000000 wormcat_batch-1.0.6/wormcat_batch/run_wormcat_batch.py
--rwxr-xr-x   0 dan        (501) staff       (20)     1446 2022-08-16 12:41:26.000000 wormcat_batch-1.0.6/wormcat_batch/worm_cat.R
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-30 14:14:54.341348 wormcat_batch-1.0.6/wormcat_batch.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-30 14:14:54.000000 wormcat_batch-1.0.6/wormcat_batch.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      451 2023-06-30 14:14:54.000000 wormcat_batch-1.0.6/wormcat_batch.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-30 14:14:54.000000 wormcat_batch-1.0.6/wormcat_batch.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       69 2023-06-30 14:14:54.000000 wormcat_batch-1.0.6/wormcat_batch.egg-info/entry_points.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-30 14:14:54.000000 wormcat_batch-1.0.6/wormcat_batch.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)       27 2023-06-30 14:14:54.000000 wormcat_batch-1.0.6/wormcat_batch.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       14 2023-06-30 14:14:54.000000 wormcat_batch-1.0.6/wormcat_batch.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-30 16:21:59.393750 wormcat_batch-1.0.7/
+-rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.0.7/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-30 16:21:59.393612 wormcat_batch-1.0.7/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2346 2023-06-28 11:53:36.000000 wormcat_batch-1.0.7/README.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-06-30 16:21:59.393792 wormcat_batch-1.0.7/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      676 2023-06-30 16:12:34.000000 wormcat_batch-1.0.7/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-30 16:21:59.392517 wormcat_batch-1.0.7/wormcat_batch/
+-rw-r--r--   0 dan        (501) staff       (20)     2024 2022-08-16 12:41:26.000000 wormcat_batch-1.0.7/wormcat_batch/create_wormcat_xlsx.py
+-rw-r--r--   0 dan        (501) staff       (20)     2486 2023-06-27 18:05:20.000000 wormcat_batch-1.0.7/wormcat_batch/execute_r.py
+-rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.0.7/wormcat_batch/is_wormcat_installed.R
+-rwxr-xr-x   0 dan        (501) staff       (20)     8734 2023-06-30 16:19:02.000000 wormcat_batch-1.0.7/wormcat_batch/run_wormcat_batch.py
+-rwxr-xr-x   0 dan        (501) staff       (20)     1446 2022-08-16 12:41:26.000000 wormcat_batch-1.0.7/wormcat_batch/worm_cat.R
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-30 16:21:59.393444 wormcat_batch-1.0.7/wormcat_batch.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-30 16:21:59.000000 wormcat_batch-1.0.7/wormcat_batch.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      451 2023-06-30 16:21:59.000000 wormcat_batch-1.0.7/wormcat_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-30 16:21:59.000000 wormcat_batch-1.0.7/wormcat_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-06-30 16:21:59.000000 wormcat_batch-1.0.7/wormcat_batch.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-30 14:14:54.000000 wormcat_batch-1.0.7/wormcat_batch.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       23 2023-06-30 16:21:59.000000 wormcat_batch-1.0.7/wormcat_batch.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       14 2023-06-30 16:21:59.000000 wormcat_batch-1.0.7/wormcat_batch.egg-info/top_level.txt
```

### Comparing `wormcat_batch-1.0.6/README.md` & `wormcat_batch-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.6/wormcat_batch/create_wormcat_xlsx.py` & `wormcat_batch-1.0.7/wormcat_batch/create_wormcat_xlsx.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.6/wormcat_batch/execute_r.py` & `wormcat_batch-1.0.7/wormcat_batch/execute_r.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.6/wormcat_batch/run_wormcat_batch.py` & `wormcat_batch-1.0.7/wormcat_batch/run_wormcat_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,28 +150,38 @@
         for root, dirs, files in os.walk(zip_path):
             for file in files:
                 file_path = os.path.join(root, file)
                 rel_path = os.path.relpath(file_path, zip_path)  # Get relative path
                 zipf.write(file_path, arcname=rel_path)
     return output_path
 
+def find_version(file_path):
+    with open(file_path, 'r') as file:
+        for line in file:
+            if "version=" in line:
+                # Extract the version number from the line
+                version_number = line.split("version='")[1].split("'")[0]
+                return version_number
+
+    # If the version is not found, return None or an appropriate value
+    return "NA"
+
 ##########################################################
 
 def main():
     print("Wormcat Batch")
     parser = argparse.ArgumentParser()
     help_statement="wormcat_cli --input-excel <full_path_to_excel> --output-path <full_path_to_out_dir> --backup-output-path True --annotation-file-nm 'whole_genome_v2_nov-11-2021.csv' "
     parser.add_argument('-i', '--input-excel', help='Inputfile in Excel format')
     parser.add_argument('-o', '--output-path', help='Output path')
     parser.add_argument('-b', '--backup-output-path', default=True, help='Backup or create outpath path if it does not exists')
     parser.add_argument('-a', '--annotation-file-nm', default='whole_genome_v2_nov-11-2021.csv', help='Annotation file name')
 
-    with open('setup.json', 'r') as file:
-            data = json.load(file)
-    parser.add_argument('-v', '--version', action='version', version=f'%(prog)s v{data["version"]}')
+    version_num = find_version('setup.py')
+    parser.add_argument('-v', '--version', action='version', version=f'%(prog)s v{version_num}')
     args = parser.parse_args()
 
     if not args.input_excel:
         print(help_statement)
         print("Inputfile in Excel format is missing.")
         return
```

### Comparing `wormcat_batch-1.0.6/wormcat_batch/worm_cat.R` & `wormcat_batch-1.0.7/wormcat_batch/worm_cat.R`

 * *Files identical despite different names*

