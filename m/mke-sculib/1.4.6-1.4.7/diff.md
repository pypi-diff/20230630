# Comparing `tmp/mke_sculib-1.4.6.tar.gz` & `tmp/mke_sculib-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-1.4.6.tar", last modified: Thu Oct 20 13:32:36 2022, max compression
+gzip compressed data, was "mke_sculib-1.4.7.tar", last modified: Fri Jun 30 19:35:04 2023, max compression
```

## Comparing `mke_sculib-1.4.6.tar` & `mke_sculib-1.4.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-10-20 13:32:36.543582 mke_sculib-1.4.6/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:44.000000 mke_sculib-1.4.6/LICENSE
--rw-rw-rw-   0        0        0     4039 2022-10-20 13:32:36.543582 mke_sculib-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     3224 2022-07-08 13:02:46.000000 mke_sculib-1.4.6/README.rst
--rw-rw-rw-   0        0        0      945 2022-10-20 13:32:36.544579 mke_sculib-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:09.000000 mke_sculib-1.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-20 13:32:36.528622 mke_sculib-1.4.6/src/
-drwxrwxrwx   0        0        0        0 2022-10-20 13:32:36.535603 mke_sculib-1.4.6/src/mke_sculib/
--rw-rw-rw-   0        0        0       21 2022-10-20 13:31:44.000000 mke_sculib-1.4.6/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:15.000000 mke_sculib-1.4.6/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24319 2022-07-27 12:10:57.000000 mke_sculib-1.4.6/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0    19332 2022-10-20 13:28:07.000000 mke_sculib-1.4.6/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    59092 2022-10-20 12:57:41.000000 mke_sculib-1.4.6/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    18060 2022-10-20 12:34:55.000000 mke_sculib-1.4.6/src/mke_sculib/sim.py
-drwxrwxrwx   0        0        0        0 2022-10-20 13:32:36.543582 mke_sculib-1.4.6/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4039 2022-10-20 13:32:36.000000 mke_sculib-1.4.6/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2022-10-20 13:32:36.000000 mke_sculib-1.4.6/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-20 13:32:36.000000 mke_sculib-1.4.6/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-10-20 13:32:36.000000 mke_sculib-1.4.6/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:04.893643 mke_sculib-1.4.7/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:44.000000 mke_sculib-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0     4039 2023-06-30 19:35:04.893643 mke_sculib-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3224 2022-07-08 13:02:46.000000 mke_sculib-1.4.7/README.rst
+-rw-rw-rw-   0        0        0      945 2023-06-30 19:35:04.894639 mke_sculib-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:09.000000 mke_sculib-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:04.880678 mke_sculib-1.4.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:04.890650 mke_sculib-1.4.7/src/mke_sculib/
+-rw-rw-rw-   0        0        0       21 2023-06-30 19:34:05.000000 mke_sculib-1.4.7/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:15.000000 mke_sculib-1.4.7/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:38.000000 mke_sculib-1.4.7/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0    19332 2022-10-20 13:28:07.000000 mke_sculib-1.4.7/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0    59398 2023-06-30 19:31:54.000000 mke_sculib-1.4.7/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    18060 2022-10-20 12:34:55.000000 mke_sculib-1.4.7/src/mke_sculib/sim.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:35:04.893643 mke_sculib-1.4.7/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4039 2023-06-30 19:35:04.000000 mke_sculib-1.4.7/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-06-30 19:35:04.000000 mke_sculib-1.4.7/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 19:35:04.000000 mke_sculib-1.4.7/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 19:35:04.000000 mke_sculib-1.4.7/src/mke_sculib.egg-info/top_level.txt
```

### Comparing `mke_sculib-1.4.6/LICENSE` & `mke_sculib-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.6/PKG-INFO` & `mke_sculib-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 1.4.6
+Version: 1.4.7
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Platform: UNKNOWN
```

### Comparing `mke_sculib-1.4.6/README.rst` & `mke_sculib-1.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.6/setup.cfg` & `mke_sculib-1.4.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.6/src/mke_sculib/cam_sensors.py` & `mke_sculib-1.4.7/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.6/src/mke_sculib/chan_list_acu.py` & `mke_sculib-1.4.7/src/mke_sculib/chan_list_acu.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
  'acu.command_arbiter.act_authority',
     
  'acu.safety_controller.state',
  'acu.safety_controller.safety_status_bs.abs_init',
  'acu.safety_controller.safety_status_bs.safety_system_error',
  'acu.safety_controller.safety_status_bs.safety_system_run',
  'acu.safety_controller.safety_status_bs.door_switch_status_ped',
- 'acu.safety_controller.safety_status_bs.door_switch_status_psc',
+#  'acu.safety_controller.safety_status_bs.door_switch_status_psc',
  'acu.safety_controller.safety_status_bs.lockout_azimuth',
  'acu.safety_controller.safety_status_bs.lockout_elevation',
  'acu.safety_controller.safety_status_bs.lockout_feedindexer',
  'acu.safety_controller.safety_status_bs.e_stop_hhd_lockout_box',
  'acu.safety_controller.safety_status_bs.e_stop_feed_indexer',
  'acu.safety_controller.safety_status_bs.sto_az',
  'acu.safety_controller.safety_status_bs.sto_el',
@@ -600,7 +600,10 @@
 'acu.pointing.incl_signal_y_filtered',
 'acu.pointing.incl_signal_y_corrected',
 'acu.pointing.incl_temp',
 'acu.pointing.incl_corr_val_az',
 'acu.pointing.incl_corr_val_el'
 ]
 
+if __name__ == "__main__":
+    for l in channels_detailed:
+        print(l)
```

### Comparing `mke_sculib-1.4.6/src/mke_sculib/mock_telescope.py` & `mke_sculib-1.4.7/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.6/src/mke_sculib/scu.py` & `mke_sculib-1.4.7/src/mke_sculib/scu.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,18 +536,22 @@
         if not isinstance(path, str):
             fun = lambda p: self.scu_get("/devices/statusValue", {"path": p}).json()['value']
             return [fun(p) for p in path]
         else:
             return self.scu_get("/devices/statusValue", {"path": path}).json()['value']
         
     #commands to ACU
-    def stow(self):
+    def stow(self, pre_move=True):
         """stow the antenna on pos 1 (both axes) and wait for stowing to be completed
         """
         log('Stowing...')
+        if pre_move:
+            self.abs_azel(+90, 88)
+            self.wait_settle()
+
         self.scu_put("/devices/command", {"path": "acu.dish_management_controller.stow", "params": {"action": "1"}})
 
         self.wait_duration(3, no_stout=True)
         self.wait_state("acu.stow_pin_controller.azimuth_status", "LOCKED")
         self.wait_state("acu.stow_pin_controller.elevation_status", "LOCKED")
 
         
@@ -1255,19 +1259,26 @@
         """
         spem_keys= ["p1_encoder_offset_azimuth", "p2_collimation",
                 "p3_non_orthog_nasmyth", "p4_e_w_azimuth_tilt",
                 "p5_n_s_azimuth_tilt", "p6_declination_error",
                 "p7_encoder_offset_elevation", "p8_cos_terx_gray_nasmyth",
                 "p9_sin_term_gray_nasmyth"]
 
+        if band == 'all':
+            for b in bands_dc.values():
+                self.point_spem_set(params, b, activate)
+            return 
+        
         d = {k:v for k, v in zip(spem_keys, params)}
 
         if isinstance(band, str):
             assert band in bands_dc_inv, 'ERROR: Band not in allowed bands: ' + str(bands_dc_inv)
             bandi = bands_dc_inv[band]
+        else:
+            bandi = band
 
         assert bandi in bands_dc, 'ERROR: Band not in allowed bands: ' + str(bands_dc_inv)
 
         d['band_information'] = bandi
 
         path = 'acu.pointing_controller.set_static_pointing_model_parameters'
         self.scu_put('/devices/command', json={'path': path, "params": d})
@@ -1312,15 +1323,15 @@
         Returns:
             list: list of values corresponding to the keys given in pathes
         """
         return [self.get_device_status_value(p) for p in pathes]
 
             
 
-    def start(self, az_start=None, el_start=None, band_start=None, az_speed=None, el_speed=None, send_default_configs=True):
+    def start(self, az_start=None, el_start=None, band_start=None, az_speed=None, el_speed=None, send_default_configs=False):
         """getting command authority, unstow, activate and start the antenna for usage
 
         Args:
             az_start (-270 <= az_start <= 270, optional): start position for AZ axis in degree. Defaults to None.
             el_start (15 <= el_start <= 90, optional): start position for EL axis in degree. Defaults to None.
             band_start (str or int, optional): start position ('Band 1'... 'Band 5c' or 1...7) for the Feed Indexer Axis to move to. Defaults to None.
             az_speed (0 < az_speed <= 3.0, optional): azimuth speed to use for movement to inital position. None means as fast as possible. Defaults to None.
```

### Comparing `mke_sculib-1.4.6/src/mke_sculib/sim.py` & `mke_sculib-1.4.7/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-1.4.6/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-1.4.7/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 1.4.6
+Version: 1.4.7
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Platform: UNKNOWN
```

