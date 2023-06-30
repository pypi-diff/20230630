# Comparing `tmp/mke_sculib-1.4.7.tar.gz` & `tmp/mke_sculib-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-1.4.7.tar", last modified: Fri Jun 30 19:35:04 2023, max compression
+gzip compressed data, was "mke_sculib-1.4.8.tar", last modified: Fri Jun 30 19:54:07 2023, max compression
```

## Comparing `mke_sculib-1.4.7.tar` & `mke_sculib-1.4.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:04.893643 mke_sculib-1.4.7/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:44.000000 mke_sculib-1.4.7/LICENSE
--rw-rw-rw-   0        0        0     4039 2023-06-30 19:35:04.893643 mke_sculib-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     3224 2022-07-08 13:02:46.000000 mke_sculib-1.4.7/README.rst
--rw-rw-rw-   0        0        0      945 2023-06-30 19:35:04.894639 mke_sculib-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:09.000000 mke_sculib-1.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:04.880678 mke_sculib-1.4.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:04.890650 mke_sculib-1.4.7/src/mke_sculib/
--rw-rw-rw-   0        0        0       21 2023-06-30 19:34:05.000000 mke_sculib-1.4.7/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:15.000000 mke_sculib-1.4.7/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:38.000000 mke_sculib-1.4.7/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0    19332 2022-10-20 13:28:07.000000 mke_sculib-1.4.7/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    59398 2023-06-30 19:31:54.000000 mke_sculib-1.4.7/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    18060 2022-10-20 12:34:55.000000 mke_sculib-1.4.7/src/mke_sculib/sim.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:04.893643 mke_sculib-1.4.7/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4039 2023-06-30 19:35:04.000000 mke_sculib-1.4.7/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-06-30 19:35:04.000000 mke_sculib-1.4.7/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 19:35:04.000000 mke_sculib-1.4.7/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-30 19:35:04.000000 mke_sculib-1.4.7/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 19:54:07.708707 mke_sculib-1.4.8/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:44.000000 mke_sculib-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0     4039 2023-06-30 19:54:07.708707 mke_sculib-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3224 2022-07-08 13:02:46.000000 mke_sculib-1.4.8/README.rst
+-rw-rw-rw-   0        0        0      945 2023-06-30 19:54:07.709697 mke_sculib-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:09.000000 mke_sculib-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:54:07.692710 mke_sculib-1.4.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 19:54:07.700688 mke_sculib-1.4.8/src/mke_sculib/
+-rw-rw-rw-   0        0        0       21 2023-06-30 19:53:40.000000 mke_sculib-1.4.8/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:15.000000 mke_sculib-1.4.8/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:38.000000 mke_sculib-1.4.8/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0    19332 2022-10-20 13:28:07.000000 mke_sculib-1.4.8/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0    59427 2023-06-30 19:53:19.000000 mke_sculib-1.4.8/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    18060 2022-10-20 12:34:55.000000 mke_sculib-1.4.8/src/mke_sculib/sim.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:54:07.707678 mke_sculib-1.4.8/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4039 2023-06-30 19:54:07.000000 mke_sculib-1.4.8/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-06-30 19:54:07.000000 mke_sculib-1.4.8/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 19:54:07.000000 mke_sculib-1.4.8/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 19:54:07.000000 mke_sculib-1.4.8/src/mke_sculib.egg-info/top_level.txt
```

### Comparing `mke_sculib-1.4.7/LICENSE` & `mke_sculib-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.7/PKG-INFO` & `mke_sculib-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 1.4.7
+Version: 1.4.8
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Platform: UNKNOWN
```

### Comparing `mke_sculib-1.4.7/README.rst` & `mke_sculib-1.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.7/setup.cfg` & `mke_sculib-1.4.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.7/src/mke_sculib/cam_sensors.py` & `mke_sculib-1.4.8/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.7/src/mke_sculib/chan_list_acu.py` & `mke_sculib-1.4.8/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.7/src/mke_sculib/mock_telescope.py` & `mke_sculib-1.4.8/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.7/src/mke_sculib/scu.py` & `mke_sculib-1.4.8/src/mke_sculib/scu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1245,20 +1245,20 @@
     def point_spem_ON(self):
         self.__point_toggle(1, '20')
     
     def point_spem_OFF(self):
         self.__point_toggle(0, '20')
     
 
-    def point_spem_set(self, params:list, band = 0, activate = True):
+    def point_spem_set(self, params:list, band = 1, activate = True):
         """set new pointing model parameters to a specific band in ArcSec
 
         Args:
             params (list): list of parameters (must be of length 9 only contain numbers and in ArcSeconds)
-            band (int, optional): the band to set these values to (1...7). Defaults to 0.
+            band (int, optional): the band to set these values to (1...7). Defaults to 1.
             activate (bool, optional): whether or not ton directly activate after setting (there seems to be an error currently). Defaults to False.
         """
         spem_keys= ["p1_encoder_offset_azimuth", "p2_collimation",
                 "p3_non_orthog_nasmyth", "p4_e_w_azimuth_tilt",
                 "p5_n_s_azimuth_tilt", "p6_declination_error",
                 "p7_encoder_offset_elevation", "p8_cos_terx_gray_nasmyth",
                 "p9_sin_term_gray_nasmyth"]
@@ -1267,20 +1267,21 @@
             for b in bands_dc.values():
                 self.point_spem_set(params, b, activate)
             return 
         
         d = {k:v for k, v in zip(spem_keys, params)}
 
         if isinstance(band, str):
-            assert band in bands_dc_inv, 'ERROR: Band not in allowed bands: ' + str(bands_dc_inv)
+            assert band in bands_dc_inv, f'ERROR: Band "{band}" not in allowed bands: ' + str(bands_dc_inv)
             bandi = bands_dc_inv[band]
         else:
+            assert band in bands_dc, f'ERROR: Band "{band}" not in allowed bands: ' + str(bands_dc)
             bandi = band
 
-        assert bandi in bands_dc, 'ERROR: Band not in allowed bands: ' + str(bands_dc_inv)
+        
 
         d['band_information'] = bandi
 
         path = 'acu.pointing_controller.set_static_pointing_model_parameters'
         self.scu_put('/devices/command', json={'path': path, "params": d})
         
         if activate:
```

### Comparing `mke_sculib-1.4.7/src/mke_sculib/sim.py` & `mke_sculib-1.4.8/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.7/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-1.4.8/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 1.4.7
+Version: 1.4.8
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Platform: UNKNOWN
```

