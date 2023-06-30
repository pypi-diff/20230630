# Comparing `tmp/rtc-tools-hydraulic-structures-2.0.0a8.tar.gz` & `tmp/rtc-tools-hydraulic-structures-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rtc-tools-hydraulic-structures-2.0.0a8.tar", last modified: Thu Oct 17 20:47:17 2019, max compression
+gzip compressed data, was "dist/rtc-tools-hydraulic-structures-2.0.0a9.tar", last modified: Fri Jan 24 16:09:09 2020, max compression
```

## Comparing `rtc-tools-hydraulic-structures-2.0.0a8.tar` & `rtc-tools-hydraulic-structures-2.0.0a9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/
--rw-r--r--   0 root         (0) root         (0)     1006 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1741 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     7652 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)      402 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      211 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtc_tools_hydraulic_structures.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtc_tools_hydraulic_structures.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtc_tools_hydraulic_structures.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1367 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtc_tools_hydraulic_structures.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       87 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtc_tools_hydraulic_structures.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtc_tools_hydraulic_structures.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtc_tools_hydraulic_structures.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/
--rw-rw-rw-   0 root         (0) root         (0)    72975 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/pumping_station_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8794 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/polygon_enclosure.py
--rw-rw-rw-   0 root         (0) root         (0)       92 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/Weir/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/Weir/Weir.mo
--rw-rw-rw-   0 root         (0) root         (0)       61 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/Weir/package.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/
--rw-rw-rw-   0 root         (0) root         (0)      543 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/Resistance.mo
--rw-rw-rw-   0 root         (0) root         (0)      971 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/PumpingStation.mo
--rw-rw-rw-   0 root         (0) root         (0)       81 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/package.mo
--rw-rw-rw-   0 root         (0) root         (0)     2138 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/Pump.mo
--rw-rw-rw-   0 root         (0) root         (0)       71 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/package.mo
--rw-r--r--   0 root         (0) root         (0)      499 2019-10-17 20:47:17.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8189 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/weir_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/util.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/versioneer.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2019-10-17 20:47:08.000000 rtc-tools-hydraulic-structures-2.0.0a8/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/COPYING.LESSER
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/
+-rw-r--r--   0 root         (0) root         (0)      499 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/Weir/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/Weir/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/Weir/Weir.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/
+-rw-rw-rw-   0 root         (0) root         (0)      543 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/Resistance.mo
+-rw-rw-rw-   0 root         (0) root         (0)      971 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/PumpingStation.mo
+-rw-rw-rw-   0 root         (0) root         (0)       81 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2138 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/Pump.mo
+-rw-rw-rw-   0 root         (0) root         (0)       71 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/package.mo
+-rw-rw-rw-   0 root         (0) root         (0)       92 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     8794 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/polygon_enclosure.py
+-rw-rw-rw-   0 root         (0) root         (0)     8189 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/weir_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    72979 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/pumping_station_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtc_tools_hydraulic_structures.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1006 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtc_tools_hydraulic_structures.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1367 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtc_tools_hydraulic_structures.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtc_tools_hydraulic_structures.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtc_tools_hydraulic_structures.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtc_tools_hydraulic_structures.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/src/rtc_tools_hydraulic_structures.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      139 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/versioneer.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2020-01-24 16:09:09.000000 rtc-tools-hydraulic-structures-2.0.0a9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2020-01-24 16:09:00.000000 rtc-tools-hydraulic-structures-2.0.0a9/README
```

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/PKG-INFO` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtc_tools_hydraulic_structures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rtc-tools-hydraulic-structures
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: Hydraulic structures models for RTC-Tools 2.
 Home-page: http://www.deltares.nl/en/software/rtc-tools/
 Author: Deltares
 Maintainer: Jack Vreeken
 License: LGPLv3
 Description: UNKNOWN
 Keywords: rtctools optimization weir pump
```

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/setup.py` & `rtc-tools-hydraulic-structures-2.0.0a9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,19 +40,19 @@
     maintainer='Jack Vreeken',
     license='LGPLv3',
     keywords='rtctools optimization weir pump',
     platforms=['Windows', 'Linux', 'Mac OS-X', 'Unix'],
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
-        'rtc-tools >= 2.3.0',
-        'rtc-tools-channel-flow',
-        'numpy',
-        'casadi'
+        'rtc-tools >= 2.4.0a6',
+        'rtc-tools-channel-flow >= 1.1',
+        'casadi == 3.5.*'
     ],
+    tests_require=['pytest', 'pytest-runner'],
     include_package_data=True,
     python_requires='>=3.5',
     cmdclass=versioneer.get_cmdclass(),
     entry_points={
         'rtctools.libraries.modelica': [
             'library_folder = rtctools_hydraulic_structures:modelica',
         ]
```

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/COPYING.LESSER` & `rtc-tools-hydraulic-structures-2.0.0a9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtc_tools_hydraulic_structures.egg-info/PKG-INFO` & `rtc-tools-hydraulic-structures-2.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rtc-tools-hydraulic-structures
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: Hydraulic structures models for RTC-Tools 2.
 Home-page: http://www.deltares.nl/en/software/rtc-tools/
 Author: Deltares
 Maintainer: Jack Vreeken
 License: LGPLv3
 Description: UNKNOWN
 Keywords: rtctools optimization weir pump
```

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtc_tools_hydraulic_structures.egg-info/SOURCES.txt` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtc_tools_hydraulic_structures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/pumping_station_mixin.py` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/pumping_station_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -929,15 +929,15 @@
                     status_range_inds = [np.arange(i + 1, min((e + 1), len(times))).tolist()
                                          for i, e in enumerate(status_end_inds)]
                     assert isinstance(status_range_inds[0][0], int), \
                         "Indexing CasADi symbols only fast with list of _Python_ ints"
 
                     for i in range(1, num_tsteps):
                         cur_status_inds = status_range_inds[i - 1]
-                        sum_ = ca.sum1(self.state_vector(status_sym)[cur_status_inds])
+                        sum_ = ca.sum1(1 - self.state_vector(status_sym)[cur_status_inds])
                         constraints.append(
                             (sum_ - len(cur_status_inds) * self.state_vector(sw_off_sym)[i], 0, inf))
 
         return constraints
 
     def _solve_hq_subproblem(self, H, Q, f, constraints=None, bounds=None):
         # Caching of the results of this function. SWIG object cannot be
```

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/polygon_enclosure.py` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/polygon_enclosure.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/Weir/Weir.mo` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/Weir/Weir.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/Resistance.mo` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/Resistance.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/PumpingStation.mo` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/PumpingStation.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/Pump.mo` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/modelica/Deltares/HydraulicStructures/PumpingStation/Pump.mo`

 * *Files identical despite different names*

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/weir_mixin.py` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/weir_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/src/rtctools_hydraulic_structures/util.py` & `rtc-tools-hydraulic-structures-2.0.0a9/src/rtctools_hydraulic_structures/util.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-hydraulic-structures-2.0.0a8/versioneer.py` & `rtc-tools-hydraulic-structures-2.0.0a9/versioneer.py`

 * *Files identical despite different names*

