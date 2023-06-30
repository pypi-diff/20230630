# Comparing `tmp/h5parm-1.0.6.tar.gz` & `tmp/h5parm-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5parm-1.0.6.tar", last modified: Fri Jun 30 15:27:55 2023, max compression
+gzip compressed data, was "h5parm-1.0.7.tar", last modified: Fri Jun 30 15:44:49 2023, max compression
```

## Comparing `h5parm-1.0.6.tar` & `h5parm-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:27:55.384185 h5parm-1.0.6/
--rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-1.0.6/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-06-30 15:27:55.384185 h5parm-1.0.6/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-1.0.6/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:27:55.384185 h5parm-1.0.6/h5parm/
--rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-1.0.6/h5parm/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:27:55.384185 h5parm-1.0.6/h5parm/arrays/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-1.0.6/h5parm/arrays/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-1.0.6/h5parm/arrays/dsa2000.W.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-1.0.6/h5parm/arrays/gmrtPos.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-1.0.6/h5parm/arrays/lofar.antenna.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-1.0.6/h5parm/arrays/lofar.hba.antenna.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)    33533 2023-05-18 12:41:43.000000 h5parm-1.0.6/h5parm/datapack.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-1.0.6/h5parm/maintenance.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16449 2023-06-30 15:27:31.000000 h5parm-1.0.6/h5parm/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:27:55.384185 h5parm-1.0.6/h5parm.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-06-30 15:27:55.000000 h5parm-1.0.6/h5parm.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      419 2023-06-30 15:27:55.000000 h5parm-1.0.6/h5parm.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-30 15:27:55.000000 h5parm-1.0.6/h5parm.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        7 2023-06-30 15:27:55.000000 h5parm-1.0.6/h5parm.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-30 15:27:55.384185 h5parm-1.0.6/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     1135 2023-06-30 15:27:31.000000 h5parm-1.0.6/setup.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:27:55.384185 h5parm-1.0.6/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)     4660 2023-06-22 17:45:55.000000 h5parm-1.0.6/tests/test_datapack.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:44:49.528761 h5parm-1.0.7/
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-1.0.7/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-06-30 15:44:49.528761 h5parm-1.0.7/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-1.0.7/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:44:49.524761 h5parm-1.0.7/h5parm/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-1.0.7/h5parm/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:44:49.528761 h5parm-1.0.7/h5parm/arrays/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-1.0.7/h5parm/arrays/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-1.0.7/h5parm/arrays/dsa2000.W.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-1.0.7/h5parm/arrays/gmrtPos.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-1.0.7/h5parm/arrays/lofar.antenna.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-1.0.7/h5parm/arrays/lofar.hba.antenna.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)    33533 2023-05-18 12:41:43.000000 h5parm-1.0.7/h5parm/datapack.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-1.0.7/h5parm/maintenance.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16463 2023-06-30 15:43:51.000000 h5parm-1.0.7/h5parm/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:44:49.528761 h5parm-1.0.7/h5parm.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-06-30 15:44:49.000000 h5parm-1.0.7/h5parm.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      419 2023-06-30 15:44:49.000000 h5parm-1.0.7/h5parm.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-30 15:44:49.000000 h5parm-1.0.7/h5parm.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        7 2023-06-30 15:44:49.000000 h5parm-1.0.7/h5parm.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-30 15:44:49.528761 h5parm-1.0.7/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     1135 2023-06-30 15:44:31.000000 h5parm-1.0.7/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-30 15:44:49.528761 h5parm-1.0.7/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4969 2023-06-30 15:43:31.000000 h5parm-1.0.7/tests/test_datapack.py
```

### Comparing `h5parm-1.0.6/LICENSE` & `h5parm-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.6/PKG-INFO` & `h5parm-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 1.0.6
+Version: 1.0.7
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `h5parm-1.0.6/README.md` & `h5parm-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.6/h5parm/arrays/dsa2000.W.cfg` & `h5parm-1.0.7/h5parm/arrays/dsa2000.W.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.6/h5parm/arrays/gmrtPos.cfg` & `h5parm-1.0.7/h5parm/arrays/gmrtPos.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.6/h5parm/arrays/lofar.antenna.cfg` & `h5parm-1.0.7/h5parm/arrays/lofar.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.6/h5parm/arrays/lofar.hba.antenna.cfg` & `h5parm-1.0.7/h5parm/arrays/lofar.hba.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.6/h5parm/datapack.py` & `h5parm-1.0.7/h5parm/datapack.py`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.6/h5parm/maintenance.py` & `h5parm-1.0.7/h5parm/maintenance.py`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.6/h5parm/utils.py` & `h5parm-1.0.7/h5parm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,9 +399,9 @@
     dec_idx = format.index('Dec')
     if len(data) == 0:
         raise ValueError(f'No data in skymodel.')
     directions = list(map(lambda d: parse_coordinates_bbs(d[ra_idx], d[dec_idx]), data))
     if len(directions) > 1:
         directions = ac.concatenate(directions)
     else:
-        directions = directions[0]
+        directions = directions[0].reshape((1,))
     return directions.transform_to(ac.ICRS())
```

### Comparing `h5parm-1.0.6/h5parm.egg-info/PKG-INFO` & `h5parm-1.0.7/h5parm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 1.0.6
+Version: 1.0.7
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `h5parm-1.0.6/setup.py` & `h5parm-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                   'tables>=' + __minimum_tables_version__,
                   'astropy>=' + __minimum_astropy_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='h5parm',
-      version='1.0.6',
+      version='1.0.7',
       description='H5Parm data pack interface',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/h5parm",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

### Comparing `h5parm-1.0.6/tests/test_datapack.py` & `h5parm-1.0.7/tests/test_datapack.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,22 @@
         _, pols = dp.get_pols(axes['pol'])
         assert len(directions) == 2
         assert len(times) == 1
         assert len(freqs) == 2
         assert len(pols) == 1
 
     sky_model_bbs = "# (Name, Type, Ra, Dec, I) = format\n" \
+                    "A, POINT, 00:00:00.123456, +37.07.47.12345, 1.0"
+    with open('test_sky_model.bbs', 'w') as f:
+        f.write(sky_model_bbs)
+
+    directions = directions_from_sky_model('test_sky_model.bbs')
+    assert len(directions) == 1
+
+    sky_model_bbs = "# (Name, Type, Ra, Dec, I) = format\n" \
                     "A, POINT, 00:00:00.123456, +37.07.47.12345, 1.0\n" \
                     "B, POINT, 00:00:00.123456, +37.37.47.12345, 1.0"
     with open('test_sky_model.bbs', 'w') as f:
         f.write(sky_model_bbs)
 
     directions = directions_from_sky_model('test_sky_model.bbs')
     assert len(directions) == 2
```

