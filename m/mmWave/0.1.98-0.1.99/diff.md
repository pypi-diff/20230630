# Comparing `tmp/mmWave-0.1.98.tar.gz` & `tmp/mmWave-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmWave-0.1.98.tar", last modified: Thu May 25 08:10:59 2023, max compression
+gzip compressed data, was "dist/mmWave-0.1.99.tar", last modified: Fri Jun 30 09:33:39 2023, max compression
```

## Comparing `mmWave-0.1.98.tar` & `mmWave-0.1.99.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-25 08:10:59.588364 mmWave-0.1.98/
--rw-r--r--   0 zach       (501) staff       (20)     6395 2023-05-25 08:10:59.588575 mmWave-0.1.98/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)     5894 2023-05-25 08:07:13.000000 mmWave-0.1.98/README.md
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-25 08:10:59.585758 mmWave-0.1.98/mmWave/
--rw-r--r--   0 zach       (501) staff       (20)        2 2019-01-18 15:34:28.000000 mmWave-0.1.98/mmWave/__init__.py
--rwxrwxrwx   0 zach       (501) staff       (20)    15857 2020-05-13 09:15:42.000000 mmWave-0.1.98/mmWave/droneRN.py
--rwxrwxrwx   0 zach       (501) staff       (20)     8286 2019-07-03 01:50:56.000000 mmWave-0.1.98/mmWave/highAccuracy.py
--rw-r--r--   0 zach       (501) staff       (20)    18084 2021-05-26 05:59:29.000000 mmWave-0.1.98/mmWave/lpdFDS.py
--rwxrwxrwx   0 zach       (501) staff       (20)    12507 2023-02-04 06:54:20.000000 mmWave-0.1.98/mmWave/lpdISK.py
--rwxrwxrwx   0 zach       (501) staff       (20)     4465 2019-12-05 19:36:36.000000 mmWave-0.1.98/mmWave/lpdISK_kv.py
--rwxrwxrwx   0 zach       (501) staff       (20)    11171 2022-11-03 03:52:22.000000 mmWave-0.1.98/mmWave/lpdISK_v2.py
--rwxrwxrwx   0 zach       (501) staff       (20)    17158 2023-03-24 07:25:35.000000 mmWave-0.1.98/mmWave/mrRadar.py
--rwxrwxrwx   0 zach       (501) staff       (20)    18021 2021-12-30 16:06:25.000000 mmWave-0.1.98/mmWave/pc3.py
--rw-rw-r--   0 zach       (501) staff       (20)    19716 2022-10-06 04:29:24.000000 mmWave-0.1.98/mmWave/pc3OVH.py
--rw-r--r--   0 zach       (501) staff       (20)    19045 2022-09-02 15:04:31.000000 mmWave-0.1.98/mmWave/pc3_360.py
--rwxrwxrwx   0 zach       (501) staff       (20)    21401 2023-05-25 08:05:08.000000 mmWave-0.1.98/mmWave/pc3_oob.py
--rw-r--r--   0 zach       (501) staff       (20)    16407 2023-04-07 03:18:25.000000 mmWave-0.1.98/mmWave/pc3_v1884R.py
--rwxrwxrwx   0 zach       (501) staff       (20)    19380 2022-06-13 08:50:32.000000 mmWave-0.1.98/mmWave/pc3_v2.py
--rwxrwxrwx   0 zach       (501) staff       (20)    22899 2022-09-02 02:15:42.000000 mmWave-0.1.98/mmWave/pc3_vsd.py
--rwxrwxrwx   0 zach       (501) staff       (20)    11294 2022-09-15 06:03:06.000000 mmWave-0.1.98/mmWave/pc3_vsd_v2.py
--rwxrwxrwx   0 zach       (501) staff       (20)    10563 2019-12-01 23:33:06.000000 mmWave-0.1.98/mmWave/pc3d.py
--rwxrwxrwx   0 zach       (501) staff       (20)     4209 2019-12-01 23:33:32.000000 mmWave-0.1.98/mmWave/pc3d_kv.py
--rw-r--r--   0 zach       (501) staff       (20)    18872 2023-02-09 15:38:21.000000 mmWave-0.1.98/mmWave/pct.py
--rwxrwxrwx   0 zach       (501) staff       (20)     4052 2019-11-26 11:17:46.000000 mmWave-0.1.98/mmWave/people3D.py
--rwxrwxrwx   0 zach       (501) staff       (20)     8311 2020-04-21 03:50:24.000000 mmWave-0.1.98/mmWave/peopleMB.py
--rw-r--r--   0 zach       (501) staff       (20)     5914 2022-10-13 04:02:11.000000 mmWave-0.1.98/mmWave/roadwayTMD_kv.py
--rwxrwxrwx   0 zach       (501) staff       (20)     9165 2021-12-30 05:31:56.000000 mmWave-0.1.98/mmWave/srradar.py
--rwxrwxrwx   0 zach       (501) staff       (20)    15643 2020-04-17 03:47:43.000000 mmWave-0.1.98/mmWave/surfaceVD.py
--rwxrwxrwx   0 zach       (501) staff       (20)    18348 2023-03-24 07:23:52.000000 mmWave-0.1.98/mmWave/trafficMD.py
--rw-r--r--   0 zach       (501) staff       (20)    19893 2023-03-24 07:30:55.000000 mmWave-0.1.98/mmWave/trafficMD_I480.py
--rw-r--r--   0 zach       (501) staff       (20)     4612 2020-04-30 09:13:56.000000 mmWave-0.1.98/mmWave/trafficMD_kv.py
--rwxrwxrwx   0 zach       (501) staff       (20)    10456 2020-04-21 03:35:54.000000 mmWave-0.1.98/mmWave/vehicleOD.py
--rw-r--r--   0 zach       (501) staff       (20)    10075 2020-07-21 15:14:04.000000 mmWave-0.1.98/mmWave/vehicleODHeatMap.py
--rwxrwxrwx   0 zach       (501) staff       (20)    14108 2021-01-07 04:09:32.000000 mmWave-0.1.98/mmWave/vehicleODR.py
--rw-r--r--   0 zach       (501) staff       (20)     7125 2020-02-04 15:39:27.000000 mmWave-0.1.98/mmWave/vitalsign.py
--rw-r--r--   0 zach       (501) staff       (20)     2498 2020-10-21 06:27:00.000000 mmWave-0.1.98/mmWave/vitalsign_kv.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-25 08:10:59.587911 mmWave-0.1.98/mmWave.egg-info/
--rw-r--r--   0 zach       (501) staff       (20)     6395 2023-05-25 08:10:58.000000 mmWave-0.1.98/mmWave.egg-info/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)      770 2023-05-25 08:10:59.000000 mmWave-0.1.98/mmWave.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (501) staff       (20)        1 2023-05-25 08:10:58.000000 mmWave-0.1.98/mmWave.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (501) staff       (20)        7 2023-05-25 08:10:59.000000 mmWave-0.1.98/mmWave.egg-info/top_level.txt
--rw-r--r--   0 zach       (501) staff       (20)       38 2023-05-25 08:10:59.589233 mmWave-0.1.98/setup.cfg
--rw-r--r--   0 zach       (501) staff       (20)     6568 2023-05-25 08:09:01.000000 mmWave-0.1.98/setup.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-06-30 09:33:39.643620 mmWave-0.1.99/
+-rw-r--r--   0 zach       (501) staff       (20)     6443 2023-06-30 09:33:39.643839 mmWave-0.1.99/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     5942 2023-06-30 09:31:02.000000 mmWave-0.1.99/README.md
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-06-30 09:33:39.640931 mmWave-0.1.99/mmWave/
+-rw-r--r--   0 zach       (501) staff       (20)        2 2019-01-18 15:34:28.000000 mmWave-0.1.99/mmWave/__init__.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    15857 2020-05-13 09:15:42.000000 mmWave-0.1.99/mmWave/droneRN.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     8286 2019-07-03 01:50:56.000000 mmWave-0.1.99/mmWave/highAccuracy.py
+-rw-r--r--   0 zach       (501) staff       (20)    18084 2021-05-26 05:59:29.000000 mmWave-0.1.99/mmWave/lpdFDS.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    12507 2023-02-04 06:54:20.000000 mmWave-0.1.99/mmWave/lpdISK.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     4465 2019-12-05 19:36:36.000000 mmWave-0.1.99/mmWave/lpdISK_kv.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    11171 2022-11-03 03:52:22.000000 mmWave-0.1.99/mmWave/lpdISK_v2.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    17158 2023-03-24 07:25:35.000000 mmWave-0.1.99/mmWave/mrRadar.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    18021 2021-12-30 16:06:25.000000 mmWave-0.1.99/mmWave/pc3.py
+-rw-rw-r--   0 zach       (501) staff       (20)    19716 2022-10-06 04:29:24.000000 mmWave-0.1.99/mmWave/pc3OVH.py
+-rw-r--r--   0 zach       (501) staff       (20)    19045 2022-09-02 15:04:31.000000 mmWave-0.1.99/mmWave/pc3_360.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    21401 2023-05-25 08:05:08.000000 mmWave-0.1.99/mmWave/pc3_oob.py
+-rw-r--r--   0 zach       (501) staff       (20)    16407 2023-04-07 03:18:25.000000 mmWave-0.1.99/mmWave/pc3_v1884R.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    22256 2023-06-30 09:24:56.000000 mmWave-0.1.99/mmWave/pc3_v2.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    22899 2022-09-02 02:15:42.000000 mmWave-0.1.99/mmWave/pc3_vsd.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    11294 2022-09-15 06:03:06.000000 mmWave-0.1.99/mmWave/pc3_vsd_v2.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    10563 2019-12-01 23:33:06.000000 mmWave-0.1.99/mmWave/pc3d.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     4209 2019-12-01 23:33:32.000000 mmWave-0.1.99/mmWave/pc3d_kv.py
+-rw-r--r--   0 zach       (501) staff       (20)    18872 2023-02-09 15:38:21.000000 mmWave-0.1.99/mmWave/pct.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     4052 2019-11-26 11:17:46.000000 mmWave-0.1.99/mmWave/people3D.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     8311 2020-04-21 03:50:24.000000 mmWave-0.1.99/mmWave/peopleMB.py
+-rw-r--r--   0 zach       (501) staff       (20)     5914 2022-10-13 04:02:11.000000 mmWave-0.1.99/mmWave/roadwayTMD_kv.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     9165 2021-12-30 05:31:56.000000 mmWave-0.1.99/mmWave/srradar.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    15643 2020-04-17 03:47:43.000000 mmWave-0.1.99/mmWave/surfaceVD.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    18348 2023-03-24 07:23:52.000000 mmWave-0.1.99/mmWave/trafficMD.py
+-rw-r--r--   0 zach       (501) staff       (20)    19893 2023-03-24 07:30:55.000000 mmWave-0.1.99/mmWave/trafficMD_I480.py
+-rw-r--r--   0 zach       (501) staff       (20)     4612 2020-04-30 09:13:56.000000 mmWave-0.1.99/mmWave/trafficMD_kv.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    10456 2020-04-21 03:35:54.000000 mmWave-0.1.99/mmWave/vehicleOD.py
+-rw-r--r--   0 zach       (501) staff       (20)    10075 2020-07-21 15:14:04.000000 mmWave-0.1.99/mmWave/vehicleODHeatMap.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    14108 2021-01-07 04:09:32.000000 mmWave-0.1.99/mmWave/vehicleODR.py
+-rw-r--r--   0 zach       (501) staff       (20)     7125 2020-02-04 15:39:27.000000 mmWave-0.1.99/mmWave/vitalsign.py
+-rw-r--r--   0 zach       (501) staff       (20)     2498 2020-10-21 06:27:00.000000 mmWave-0.1.99/mmWave/vitalsign_kv.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-06-30 09:33:39.643176 mmWave-0.1.99/mmWave.egg-info/
+-rw-r--r--   0 zach       (501) staff       (20)     6443 2023-06-30 09:33:38.000000 mmWave-0.1.99/mmWave.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)      770 2023-06-30 09:33:39.000000 mmWave-0.1.99/mmWave.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (501) staff       (20)        1 2023-06-30 09:33:38.000000 mmWave-0.1.99/mmWave.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (501) staff       (20)        7 2023-06-30 09:33:38.000000 mmWave-0.1.99/mmWave.egg-info/top_level.txt
+-rw-r--r--   0 zach       (501) staff       (20)       38 2023-06-30 09:33:39.644526 mmWave-0.1.99/setup.cfg
+-rw-r--r--   0 zach       (501) staff       (20)     6633 2023-06-30 09:28:55.000000 mmWave-0.1.99/setup.py
```

### Comparing `mmWave-0.1.98/PKG-INFO` & `mmWave-0.1.99/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmWave
-Version: 0.1.98
+Version: 0.1.99
 Summary: Joybien mmWave (Batman-101/201/301/501/601) library
 Home-page: http://www.joybien.com
 Download-URL: https://pypi.org/project/mmWave
 Author: Bighead Chen
 Author-email: zach_chen@joybien.com
 Project-URL: API Source Code, https://github.com/bigheadG/mmWave
 Classifier: Programming Language :: Python :: 3
@@ -118,14 +118,15 @@
 14. mmWave-1.0.77      
     2022/06/09 mrRadar added headerShowAll()
 15. mmWave-1.0.78
     2022/06/10 pc3_v2 v2.0.1, (v6 data update) add sx,sy,sz
     2022/06/13 pc3_v2 v2.0.2, added azimuth offset 
 16. mmWave-1.0.79
     2022/06/13 pc3_v2 v2.0.2, added azimuth offset 
+    2023/06/30 pc3_v2 v2.0.3, playback function
 17. mmWave-1.0.80
     2022/07/18 pc3OVH v1.0.0, added tilt,install height and (sx,sy,sz) in raw data mode     
 18. mmWave-1.0.81 
     2022/07/19 pc3OVH v1.0.1, added v6 fetch time
 19. mmWave-1.0.83 (fix 82)
     2022/07/20 v1.0.2 raw data: (elv,azi,ran,dop,snr,sx,sy,sz)..
 20. mmWave-1.0.84
```

### Comparing `mmWave-0.1.98/README.md` & `mmWave-0.1.99/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 14. mmWave-1.0.77      
     2022/06/09 mrRadar added headerShowAll()
 15. mmWave-1.0.78
     2022/06/10 pc3_v2 v2.0.1, (v6 data update) add sx,sy,sz
     2022/06/13 pc3_v2 v2.0.2, added azimuth offset 
 16. mmWave-1.0.79
     2022/06/13 pc3_v2 v2.0.2, added azimuth offset 
+    2023/06/30 pc3_v2 v2.0.3, playback function
 17. mmWave-1.0.80
     2022/07/18 pc3OVH v1.0.0, added tilt,install height and (sx,sy,sz) in raw data mode     
 18. mmWave-1.0.81 
     2022/07/19 pc3OVH v1.0.1, added v6 fetch time
 19. mmWave-1.0.83 (fix 82)
     2022/07/20 v1.0.2 raw data: (elv,azi,ran,dop,snr,sx,sy,sz)..
 20. mmWave-1.0.84
```

### Comparing `mmWave-0.1.98/mmWave/droneRN.py` & `mmWave-0.1.99/mmWave/droneRN.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/highAccuracy.py` & `mmWave-0.1.99/mmWave/highAccuracy.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/lpdFDS.py` & `mmWave-0.1.99/mmWave/lpdFDS.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/lpdISK.py` & `mmWave-0.1.99/mmWave/lpdISK.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/lpdISK_kv.py` & `mmWave-0.1.99/mmWave/lpdISK_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/lpdISK_v2.py` & `mmWave-0.1.99/mmWave/lpdISK_v2.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/mrRadar.py` & `mmWave-0.1.99/mmWave/mrRadar.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pc3.py` & `mmWave-0.1.99/mmWave/pc3.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pc3OVH.py` & `mmWave-0.1.99/mmWave/pc3OVH.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pc3_360.py` & `mmWave-0.1.99/mmWave/pc3_360.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pc3_oob.py` & `mmWave-0.1.99/mmWave/pc3_oob.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pc3_v1884R.py` & `mmWave-0.1.99/mmWave/pc3_v1884R.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pc3_v2.py` & `mmWave-0.1.99/mmWave/trafficMD.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,229 +1,235 @@
-# Overhead People Counting 3D - ISK & AOP Raw Data (OHPC)
-# ver:2.0
-# 2022/04/19
-# 
-# parsing People Counting 3D data use AOP-ISK
-# hardware:(Batman-201)ISK IWR6843 ES2.0 & BM-501 AOP
-#    Fireware version: I470
-# Fit : wall mount
+# Traffic Monitor Detector Raw Data (TMD)
+# modify from LPD
+# ver:0.0.2
+# 2021/04/24
+# parsing Traffic Monitor Detector
+# hardware:(Batman-201): ISK IWR6843 ES2.0
 # company: Joybien Technologies: www.joybien.com
 # author: Zach Chen
 #===========================================
-# output: V6,V7,V8 Raw data
-# v0.0.1 : 2020/06/19 release
-#          (1)Output list data
-# v0.1.0 : 2021/04/01 
-#          (1)Output DataFrame
-# v0.1.1 : 2021/08/12
-#           (doppler and range swap in V6 output)
-# v0.1.2 : 2021/09/17
-#           v7 dataframe:'tid' move to front of 'ec0'
-# v2.0 : 2022/04/19
-#          pc3_v2: add ec[16],g,confidenceLevel
-#          this version lib same as pc3OVH 
+# output: V6,V7,V8,v9 Raw data
+# v0.0.1 : 2020/04/30 release
+# v0.1.0 : 2021/04/24 release
+#    added DataFrame 
+# v0.1.1 : 2023/03/24 release
+#          header enable/disable in inital
 #
-# v2.0.1: 2022/06/10 v6 add sx,sy,sz
-#
-# v2.0.2: 2022/06/13 added azimuth offset
-#                    azi_offset
-#
-
 import serial
 import time
 import struct
 import pandas as pd
 import numpy as np
 
 class header:
 	version = 0
 	totalPackLen = 0
 	platform = 0
+	timeStamp = 0
+	totalPacketLen = 0
 	frameNumber = 0
-	subframeNumber = 0
+	subFrameNumber = 0
 	chirpMargin = 0
 	frameMargin = 0 
 	trackProcessTime = 0
 	uartSendTime = 0
 	numTLVs = 0
 	checksum = 0
 
-class unitS:
-	elevationUnit:float = 0.0
-	azimuthUnit : float = 0.0
-	dopplerUnit :float = 0.0
-	rangeUnit :float = 0.0
-	snrUnit :float = 0.0
 
-class Pc3_v2:
+class TrafficMD:
 	
 	magicWord =  [b'\x02',b'\x01',b'\x04',b'\x03',b'\x06',b'\x05',b'\x08',b'\x07',b'\0x99']
 	port = ""
 	hdr = header
-	u = unitS
-	frameNumber = 0
-	azi_offset = 0.0
-	
+
 	# provide csv file dataframe
 	# real-time 
-	v6_col_names_rt = ['fN','type','elv','azimuth','range','doppler','snr','sx', 'sy', 'sz'] 
-	v7_col_names_rt = ['fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8','ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi','tid']
+	v6_col_names_rt = ['fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz'] #ok
+	v7_col_names_rt = ['fN','type','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']
 	v8_col_names_rt = ['fN','type','targetID']
+	v9_col_names_rt = ['fN','type','snr','noise']
 	
 	# read from file for trace point clouds
 	fileName = ''
-	v6_col_names = ['time','fN','type','elv','azimuth','range','doppler','snr','sx', 'sy', 'sz']
-	#v7_col_names = ['time','fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8','ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi','tid']
-	v7_col_names = ['time','fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','tid','ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8','ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi'] #v0.1.2
+	v6_col_names = ['time','fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz']
+	v7_col_names = ['time','fN','type','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']
 	v8_col_names = ['time','fN','type','targetID']
+	v9_col_names = ['fN','type','snr','noise']
 	sim_startFN = 0
 	sim_stopFN  = 0 
 	
+	v6simo = []
+	v7simo = []
+	v8simo = []
+	v9simo = []
+	
 	# add for interal use
 	tlvLength = 0
 	numOfPoints = 0
 	# for debug use 
 	dbg = False #Packet unpacket Check: True show message 
-	sm  = False #Observed StateMachine: True Show message
+	sm = False #Observed StateMachine: True Show message
 	plen = 16 
 	
-	def __init__(self,port, degree = None):
+	def __init__(self,port,show = True):
 		self.port = port
-		self.azi_offset = 0.0 if degree == None else degree * 3.14159/180.0
-		
-		print("(jb)People Counting 3D v2.0 (Wall Mount) initial")
-		print("(jb)vsersion:v2.0")
-		print("(jb)For Hardware:Batman-201(ISK) & BM-501 (AOP)")
-		print("(jb)Hardware: IWR-6843 & AOP")
-		print("(jb)Firmware: PC3-I470")
-		print("(jb)UART Baud Rate:921600")
-		print("Output: V6,V7,V8 data:(RAW)")
+		if show:
+			print("(jb)Traffic Monitor Detector(TMD) raw Data lib initial")
+			print("(jb)For Hardware:Batman-201(ISK)")
+			print("(jb)Version: v0.1.0")
+			print("(jb)Hardware: IWR-6843 ES2.0")
+			print("(jb)Firmware: TMD")
+			print("(jb)UART Baud Rate:921600")
+			print("==============Info=================")
+			print("Output: V6,V7,V8,V9 data:(RAW)")
+			print("V6: Point Cloud Spherical")
+			print("v6 structure: [(range,azimuth,elevation,doppler),......]")
+			print("V7: Target Object List")
+			print("V7 structure: [(tid,posX,posY,velX,velY,accX,accY,posZ,velZ,accZ),....]")
+			print("V8: Target Index")
+			print("V8 structure: [id1,id2....]")
+			print("V9: Point Cloud Side Info")
+			print("V9 [(snr,noise),....]")
+			print("===================================")
+	 
 		
 	def useDebug(self,ft):
 		self.dbg = ft
 		
 	def stateMachine(self,ft):
 		self.sm = ft
 		
 	def getHeader(self):
 		return self.hdr
 		
 	def headerShow(self):
-		print("******* Header ********") 
+		print("***Header***********") 
 		print("Version:     \t%x "%(self.hdr.version))
 		print("Platform:    \t%X "%(self.hdr.platform))
+		#print("TimeStamp:   \t%s "%(self.hdr.timeStamp))
 		print("TotalPackLen:\t%d "%(self.hdr.totalPackLen))
 		print("PID(frame#): \t%d "%(self.hdr.frameNumber))
-		print("subframe#  : \t%d "%(self.hdr.subframeNumber))
+		print("subframe#  : \t%d "%(self.hdr.subFrameNumber))
 		print("Inter-frame Processing Time:\t{:d} us".format(self.hdr.trackProcessTime))
 		print("UART Send Time:\t{:d} us".format(self.hdr.uartSendTime))
 		print("Inter-chirp Processing Margin:\t{:d} us".format(self.hdr.chirpMargin))
 		print("Inter-frame Processing Margin:\t{:d} us".format(self.hdr.frameMargin))
 		print("numTLVs:     \t%d "%(self.hdr.numTLVs))
 		print("Check Sum   :\t{:x}".format(self.hdr.checksum))
 		print("***End Of Header***") 
 			
 	#for class internal use
 	def tlvTypeInfo(self,dtype,count,dShow):
-		
 		sbyte = 8  #tlvHeader Struct = 8 bytes
 		unitByte = 20 
 		dataByte = 0
 		pString = ""
 		nString = "numOfPoints :"
-		stateString = "V6-unit"
+		stateString = "V6"
 		if dtype == 6:
-			unitByte = 20  #pointUnit= 20bytes (elvUnit(4),aziUnit(4),dopplerUnit(4),rangeUnit(4),snrUnit(4))
-			sbyte = 8      #tlvHeader Struct = 8 bytes (type(4)/lenth(4))
-			dataByte= 8    #pointStruct 8bytes:(elevation(1),azimuth(1),doppler(2),range(2),snr(2))
-			pString = "Point Cloud TLV and pointUnit"
+			unitByte = 0   #pointUnit= 20bytes
+			sbyte = 8      #tlvHeader Struct = 8 bytes
+			dataByte= 16    #pointStruct 8bytes:(range,azimuth,elevation,doppler)
+			pString = "DPIF Point Cloud Spherical TLV"
 			nString = ""
+			stateString = "V6"
 		elif dtype == 7:
 			unitByte = 0   #pointUnit= 0bytes 
-			sbyte = 8 	   #tlvHeader Struct = 8 bytes (type(4)/lenth(4))
-			dataByte = 112  #target struct 112 bytes:(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,confi)  
-			pString = "Target Object TLV"
+			sbyte = 8 	   #tlvHeader Struct = 8 bytes
+			dataByte = 40  #target struct 40 bytes:(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ)  
+			pString = "Target Object List TLV"
 			nString = "numOfObjects:"
 			stateString = "V7"
 		elif dtype == 8:
 			unitByte = 0 #pointUnit= 0bytes 
 			sbyte = 8    #tlvHeader Struct = 8 bytes
 			dataByte = 1 #targetID = 1 byte
 			pString = "Target Index TLV"
 			nString = "numOfIDs"
 			stateString = "V8"
+		elif dtype == 9:
+			unitByte = 0 #pointUnit= 0bytes 
+			sbyte = 8    #tlvHeader Struct = 8 bytes
+			dataByte = 4 #(snr,noise") =  4 byte
+			pString = "DPIF Point Cloud Side Info"
+			nString = "numOfIDs"
+			stateString = "V9"
 		else:
 			unitByte = 0
 			sbyte = 1
 			pString = "*** Type Error ***"
 			stateString = 'idle'
 		 
-		retCnt = count - unitByte -sbyte
-		nPoint = retCnt / sbyte
-		#dShow = True
+		#retCnt = count - unitByte - sbyte
+		nPoint = count / dataByte
 		if dShow == True:
-			print("-----[{:}] ----".format(pString))
-			print("tlv Type({:2d}B):  \t{:d}".format(sbyte,dtype))
+			print("-----[{:}] ----:{:}".format(pString,stateString))
+			print("tlv Type({:2d}Bytes):  \t{:d}".format(sbyte,dtype))
 			print("tlv length:      \t{:d}".format(count)) 
-			print("{:}      \t{:d}".format(nString,int(nPoint)))
-			print("value length:    \t{:d}".format(retCnt))  
+			print("num of point:    \t{:d}".format(int(nPoint)))
+			print("value length:    \t{:d}".format(count))  
 		
-		return unitByte,stateString, sbyte, dataByte,retCnt, int(nPoint)
+		return unitByte,stateString, sbyte, dataByte,count, int(nPoint)
+		
+	def list2df(self,dck,l6,l7,l8,l9):
+		#print("---------------list2df: v6----------------")
+		#print(l6)
 		
-	def list2df(self,dck,l6,l7,l8):
 		ll6 = pd.DataFrame(l6,columns=self.v6_col_names_rt)
 		ll7 = pd.DataFrame(l7,columns=self.v7_col_names_rt)
-		ll8 = l8 #pd.DataFrame(l8,columns=self.v8_col_names_rt)
-		return (dck,ll6,ll7,ll8)
+		ll8 = pd.DataFrame(l8,columns=self.v8_col_names_rt)
+		ll9 = pd.DataFrame(l9,columns=self.v9_col_names_rt)
+		#print("------ll6---------list2df: v6----------------")
+		#print(ll6)
+		return (dck,ll6,ll7,ll8,ll9)
 
 #
 # TLV: Type-Length-Value
 # read TLV data
 # input:
 #     disp: True:print message
 #			False: hide printing message
-#     df: 
 # output:(return parameter)
-# (pass_fail, v6, v7, v8)
+# (pass_fail, v6, v7, v8, v9)
 #  pass_fail: True: Data available    False: Data not available
-#  v6: point cloud infomation
-#  v7: Target Object information
+#
+#  v6: DPIF point cloud Spherical infomation
+#  v7: Target Object List information
 #  v8: Target Index information
-#  
-# 
+#  v9: DPIF Point Cloud Side Infomation
 #
 	def tlvRead(self,disp,df = None):
-		
 		#print("---tlvRead---")
 		#ds = dos
-		typeList = [6,7,8]
+		typeList = [6,7,8,9]
 		idx = 0
 		lstate = 'idle'
 		sbuf = b""
 		lenCount = 0
 		unitByteCount = 0
 		dataBytes = 0
 		numOfPoints = 0
 		tlvCount = 0
 		pbyte = 16
 		v6 = ([])
 		v7 = ([])
 		v8 = ([])
+		v9 = ([])
 		v6df = ([])
 		v7df = ([])
 		v8df = ([])
-		
+		v9df = ([])
+	
 		while True:
 			try:
 				ch = self.port.read()
 			except:
-				#return (False,v6,v7,v8)
-				#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6,v7,v8)
-				return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
-				
+				#return (False,v6,v7,v8,v9)
+				return self.list2df(False,v6,v7,v8,v9) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 			#print(str(ch))
 			if lstate == 'idle':
 				#print(self.magicWord)
 				if ch == self.magicWord[idx]:
 					#print("*** magicWord:"+ "{:02x}".format(ord(ch)) + ":" + str(idx))
 					idx += 1
 					if idx == 8:
@@ -231,316 +237,321 @@
 						lstate = 'header'
 						rangeProfile = b""
 						sbuf = b""
 				else:
 					#print("not: magicWord state:")
 					idx = 0
 					rangeProfile = b""
-					#return (False,v6,v7,v8)
-					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+					#return (False,v6,v7,v8,v9)
+					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 		
 			elif lstate == 'header':
 				sbuf += ch
 				idx += 1
-				if idx == 40: 
+				if idx == 44: 
 					#print("------header-----")
 					#print(":".join("{:02x}".format(c) for c in sbuf)) 	 
 					#print("len:{:d}".format(len(sbuf))) 
 					# [header - Magicword]
 					try: 
-						(self.hdr.version,self.hdr.totalPackLen,self.hdr.platform,
-						self.hdr.frameNumber,self.hdr.subframeNumber,
+						(self.hdr.version,self.hdr.platform,self.hdr.timeStamp,self.hdr.totalPackLen,
+						self.hdr.frameNumber,self.hdr.subFrameNumber,
 						self.hdr.chirpMargin,self.hdr.frameMargin,self.hdr.trackProcessTime,self.hdr.uartSendTime,
-						self.hdr.numTLVs,self.hdr.checksum) = struct.unpack('9I2H', sbuf)
-						self.frameNumber = self.hdr.frameNumber
+						self.hdr.numTLVs,self.hdr.checksum) = struct.unpack('10I2H', sbuf)
+						
 					except:
 						if self.dbg == True:
 							print("(Header)Improper TLV structure found: ")
-						#return (False,v6,v7,v8)
-						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+						#return (False,v6,v7,v8,v9)
+						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 					
 					if disp == True:  
 						self.headerShow()
 					
 					tlvCount = self.hdr.numTLVs
-					#print("tlvCount:{:}".format(tlvCount))
 					if self.hdr.numTLVs == 0:
-						#return (True,v6,v7,v8)
-						#return (True,v6,v7,v8) if (df == None) else self.list2df(True,v6df,v7df,v8df)
-						return self.list2df(True,v6df,v7df,v8df) if (df == 'DataFrame') else (True,v6,v7,v8)
+						#return (False,v6,v7,v8,v9)
+						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 						
 					if self.sm == True:
 						print("(Header)")
 						
 					sbuf = b""
 					idx = 0
 					lstate = 'TL'
 					  
-				elif idx > 44:
+				elif idx > 48:
 					idx = 0
 					lstate = 'idle'
-					#return (False,v6,v7,v8)
-					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+					#return (False,v6,v7,v8,v9)
+					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 					
 			elif lstate == 'TL': #TLV Header type/length
 				sbuf += ch
 				idx += 1
 				if idx == 8:
 					#print(":".join("{:02x}".format(c) for c in sbuf))
-					try:
+					try: 
 						ttype,self.tlvLength = struct.unpack('2I', sbuf)
-						#print("--tlvNum:{:d}: tlvCount({:d})-------ttype:tlvLength:{:d}:{:d}".format(self.hdr.numTLVs,tlvCount,ttype,self.tlvLength))
+						#print("(TL)numTLVs({:d}): tlvCount({:d})-------ttype:tlvLength:{:d}:{:d}".format(self.hdr.numTLVs,tlvCount,ttype,self.tlvLength))
+						
 						if ttype not in typeList or self.tlvLength > 10000:
 							if self.dbg == True:
 								print("(TL)Improper TL Length(hex):(T){:d} (L){:x} numTLVs:{:d}".format(ttype,self.tlvLength,self.hdr.numTLVs))
 							sbuf = b""
 							idx = 0
 							lstate = 'idle'
 							self.port.flushInput()
-							#return (False,v6,v7,v8)
-							#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-							return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+							#return (False,v6,v7,v8,v9)
+							return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 							
 					except:
+						print("TL unpack Improper Data Found:")
 						if self.dbg == True:
 							print("TL unpack Improper Data Found:")
 						self.port.flushInput()
-						#return (False,v6,v7,v8)
-						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+						#return (False,v6,v7,v8,v9)
+					
+						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 					
 					unitByteCount,lstate ,plen ,dataBytes,lenCount, numOfPoints = self.tlvTypeInfo(ttype,self.tlvLength,disp)
-					#if ttype == 6:
-					#	print("--pointCloud:((tlvLength({:d})-pointUnit(20)-tlvStruct(8))/8={:d}".format(self.tlvLength,numOfPoints))
+					#print("dataBytes={:d} lenCount={:d}".format(dataBytes , lenCount))
 					if self.sm == True:
 						print("(TL:{:d})=>({:})".format(tlvCount,lstate))
 						
 					tlvCount -= 1
 					idx = 0  
 					sbuf = b""
 			
-			elif lstate == 'V6-unit':
-				sbuf += ch
-				idx += 1
-				if idx == unitByteCount :
-					#print(":".join("{:02x}".format(c) for c in sbuf))
-					#print("unitByte:{:d}".format(len(sbuf)))
-					try:
-						self.u.elevationUnit,self.u.azimuthUnit,self.u.dopplerUnit,self.u.rangeUnit,self.u.snrUnit = struct.unpack('5f', sbuf)
-						#print("Unit  ==> elv:{:.4f} azimuth:{:.4f} doppler:{:.4f} range:{:.4f} snr:{:.4f}".format(self.u.elevationUnit,self.u.azimuthUnit,self.u.dopplerUnit,self.u.rangeUnit,self.u.snrUnit))
-						sbuf = b""
-						idx = 0
-						lstate = 'V6'				
-					except:
-						if self.dbg == True:
-							print("(6.0)Improper Type 6 unit Value structure found: ")
-						#return (False,v6,v7,v8)
-						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
-					
-					if self.sm == True:
-						print("(V6-unit:{:d})=>({:})".format(tlvCount,lstate))
-						#print("(V6-unit)=>({:})".format(lstate))
-					
 			elif lstate == 'V6': # count = Total Lentgh - 8
 				sbuf += ch
 				idx += 1
 				if (idx%dataBytes == 0):
 					try:
 						#print(":".join("{:02x}".format(c) for c in sbuf))
-						(e,a,d,r,s) = struct.unpack('2b3h', sbuf)
-						elv = e * self.u.elevationUnit
-						azi = a * self.u.azimuthUnit + self.azi_offset
-						dop = d * self.u.dopplerUnit
-						ran = r * self.u.rangeUnit
-						snr = s * self.u.snrUnit
-						#print("({:2d}:{:4d})(idx:({:4d}) elv:{:.4f} azimuth:{:.4f} doppler:{:.4f} range:{:.4f} snr:{:.4f}".format(numOfPoints,lenCount,idx,elv,azi,dop,ran,snr))
-						sz  = ran * np.sin(elv)
-						sx  = ran * np.cos(elv) * np.sin(azi)
-						sy  = ran * np.cos(elv) * np.cos(azi)
-						
+						(r,a,e,d) = struct.unpack('4f', sbuf)
+						#print("({:2d}:{:4d})(idx:({:4d}) elv:{:.4f} azimuth:{:.4f} doppler:{:.4f} range:{:.4f}".format(numOfPoints,lenCount,idx,e,a,d,r))
 						if (df == 'DataFrame'):
-							#v6df.append((self.hdr.frameNumber,'v6',elv,azi,dop,ran,snr,sx,sy,sz)) #v0.1.0
-							v6df.append((self.hdr.frameNumber,'v6',elv,azi,ran,dop,snr,sx,sy,sz)) #v0.1.1
-							 
+							sz  = r * np.sin(e)
+							sx  = r * np.cos(e) * np.sin(a)
+							sy  = r * np.cos(e) * np.cos(a)
+							#fieldNames = ['time','frameNum','type','range/px','azimuth/py','elv/vx','doppler/vy','sx/accX','sy/accY','sz/pz','na/vz','na/accZ','na/ID']
+							v6df.append((self.hdr.frameNumber,'v6',r,a,e,d,sx,sy,sz))
 						else:
-							#v6.append((elv,azi,dop,ran,snr)) 
-							v6.append((elv,azi,dop,ran,snr,sx,sy,sz)) #v2.0.1
-						
-						#print("point_cloud_2d.append:[{:d}]".format(len(point_cloud_2d)))
+							v6.append((r,a,e,d))
+							
 						sbuf = b""
-						
 					except:
 						if self.dbg == True:
 							print("(6.1)Improper Type 6 Value structure found: ")
-						#return (False,v6,v7,v8)
-						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+						#return (False,v6,v7,v8,v9)
+						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 					
 				if idx == lenCount:
 					if disp == True:
 						print("v6[{:d}]".format(len(v6)))
 					idx = 0
 					sbuf = b""
 					if tlvCount <= 0: # Back to idle
 						lstate = 'idle'
 						if self.sm == True:
-							print("(V6:{:d})=>(idle) :true".format(tlvCount))
-						#return (True,v6,v7,v8)
-						#return (True,v6,v7,v8) if (df == None) else self.list2df(True,v6df,v7df,v8df)
-						return self.list2df(True,v6df,v7df,v8df) if (df == 'DataFrame') else (True,v6,v7,v8)
+							print("(V6:tlvCnt={:d})=>(idle) :true".format(tlvCount))
+						#return (True,v6,v7,v8,v9)
+						print("(lib)v6=============SaveAppend==============")
+						return self.list2df(True,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (True,v6,v7,v8,v9)
 						
 					else: # Go to TL to get others type value
 						lstate = 'TL' #'tlTL'
 						if self.sm == True:
-							print("(V6:{:d})=>(TL)".format(tlvCount))
+							print("(V6:tlvCnt={:d})=>(TL)".format(tlvCount))
 					
 				elif idx > lenCount:
 					idx = 0
 					sbuf = b""
 					lstate = 'idle'
-					#return (False,v6,v7,v8)
-					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6,v7,v8)
-					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
-				
+					#return (False,v6,v7,v8,v9)
+					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+					
+			elif lstate == 'V9':  
+				sbuf += ch
+				idx += 1
+				if (idx%dataBytes == 0):
+					try:
+						#print(":".join("{:02x}".format(c) for c in sbuf))
+						(snr,noise) =  struct.unpack('2h', sbuf)
+						#print("lenCnt = ({:d}) snr:{:.4f} noise:{:.4f}".format(lenCount,snr,noise))
+						
+						if (df == 'DataFrame'):
+							v9df.append((self.hdr.frameNumber,'v9',snr,noise))
+						else:
+							v9.append((snr,noise))
+							
+						sbuf = b""
+					except:
+						if self.dbg == True:
+							print("(7)Improper Type 9 Value structure found: ")
+						#return (False,v6,v7,v8,v9)
+						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+						
+				if idx >= lenCount:
+					if disp == True:
+						print("count= v9[{:d}]".format(len(v9)))
+						
+					sbuf = b""
+					if tlvCount == 0:
+						lstate = 'idle'
+						if self.sm == True:
+							print("(V9)=>(idle) :true")
+						#return (True,v6,v7,v8,v9)
+						return self.list2df(True,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (True,v6,v7,v8,v9)
+						
+					else: # Go to TL to get others type value
+						lstate = 'TL'
+						idx = 0
+						if self.sm == True:
+							print("(V9)=>(TL)")
+							
+				if idx > lenCount:
+					idx = 0 
+					lstate = 'idle'
+					sbuf = b""
+					#return (False,v6,v7,v8,v9)
+					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+					
 			elif lstate == 'V7':
 				sbuf += ch
 				idx += 1
 				if (idx%dataBytes == 0):
 					#print("V7:dataBytes({:d}) lenCount({:d}) index:{:d}".format(dataBytes,lenCount,idx))
 					try:
-						#(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ) = struct.unpack('I9f', sbuf)
-						(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,confi) = struct.unpack('I27f', sbuf)
-						if (df == 'DataFrame'): 
-							v7df.append((self.hdr.frameNumber,'v7',posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,confi,tid))
-							
+						(tid,posX,posY,velX,velY,accX,accY,posZ,velZ,accZ) = struct.unpack('I9f', sbuf) 
+						#fieldNames = ['time','frameNum','type','range/px','azimuth/py','elv/vx','doppler/vy','sx/accX','sy/accY','sz/pz','na/vz','na/accZ','na/ID']
+						if (df == 'DataFrame' ):
+							v7df.append((self.hdr.frameNumber,'v7',posX,posY,velX,velY,accX,accY,posZ,velZ,accZ,tid))
 						else:
-							v7.append((tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,confi))
-						
+							v7.append((tid,posX,posY,velX,velY,accX,accY,posZ,velZ,accZ))
+							#print("tid = ({:d}) ,posX:{:.4f} posY:{:.4f} posZ:{:.4f}".format(tid,posX,posY,posZ))
 						sbuf = b""
 					except:
 						if self.dbg == True:
 							print("(7)Improper Type 7 Value structure found: ")
-						#return (False,v6,v7,v8)
-						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+						#return (False,v6,v7,v8,v9)
+						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 						
 				if idx >= lenCount:
 					if disp == True:
 						print("v7[{:d}]".format(len(v7)))
 					 
 					sbuf = b""
 					if tlvCount == 0:
 						lstate = 'idle'
 						if self.sm == True:
 							print("(V7)=>(idle) :true")
-						#return (True,v6,v7,v8)
-						#return (True,v6,v7,v8) if (df == None) else self.list2df(True,v6df,v7df,v8df)
-						return self.list2df(True,v6df,v7df,v8df) if (df == 'DataFrame') else (True,v6,v7,v8)
+						#return (True,v6,v7,v8,v9)
+						return self.list2df(True,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (True,v6,v7,v8,v9)
 						
 					else: # Go to TL to get others type value
 						lstate = 'TL'
 						idx = 0
 						if self.sm == True:
 							print("(V7)=>(TL)")
 
 				if idx > lenCount:
 					idx = 0 
 					lstate = 'idle'
 					sbuf = b""
-					#return (False,v6,v7,v8)
-					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+					#return (False,v6,v7,v8,v9)
+					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
 				
 			elif lstate == 'V8':
 				idx += 1
 				v8.append(ord(ch))
-				
 				if idx == lenCount:
 					if disp == True:
-						print("=====V8 End====")						
+						print("=====V8 End====")
 					sbuf = b""
 					idx = 0
 					lstate = 'idle'
 					if self.sm == True:
 						print("(V8:{:d})=>(idle)".format(tlvCount))
-					
-					if (df == 'DataFrame'):
-						v8df = [self.hdr.frameNumber,'v8']
-						v8df.extend(v8)
 						
-					#return (True,v6,v7,v8) if (df == None) else self.list2df(True,v6df,v7df,v8df)
-					return self.list2df(True,v6df,v7df,v8df) if (df == 'DataFrame') else (True,v6,v7,v8)
+					if (df == 'DataFrame'):
+						v8o = [self.hdr.frameNumber,'v8']
+						v8df = v8o.extend(v8)
+					#return (True,v6,v7,v8,v9)
+					return self.list2df(True,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (True,v6,v7,v8,v9)
 				
 				if idx > lenCount:
 					sbuf = b""
 					idx = 0
 					lstate = 'idle'
-					#return (False,v6,v7,v8)
-					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
-					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
-					
-	def v67Simlog(frameNum):
-		global sim_startFN,sim_stopFN
-		s_fn = frameNum + sim_startFN
-		#print("frame number:{:}".format(s_fn))
-		v6d = v6sim[v6sim['fN'] == s_fn]
-		#v6d =  v6dd[v6dd['doppler'] < 0.0]
-		#print(v6d)
-		v7d = v7sim[v7sim['fN'] == s_fn]
-		chk = 0
-		if v6d.count != 0:
-			chk = 1
-		return (chk,v6d,v7d)
-		
+					#return (False,v6,v7,v8,v9)
+					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+
 	def getRecordData(self,frameNum):
 		s_fn = frameNum + self.sim_startFN
 		#print("frame number:{:}".format(s_fn))
 		v6d = self.v6simo[self.v6simo['fN'] == s_fn]
 		#v6d =  v6dd[v6dd['doppler'] < 0.0]
 		#print(v6d)
 		v7d = self.v7simo[self.v7simo['fN'] == s_fn]
 		v8d = self.v8simo[self.v8simo['fN'] == s_fn]
+		v9d = self.v9simo[self.v9simo['fN'] == s_fn]
 		chk = 0
 		if v6d.count != 0:
 			chk = 1
-		return (chk,v6d,v7d,v8d)
+		return (chk,v6d,v7d,v8d,v9d)
+		
 		
+	'''
+		v6_col_names_rt = ['fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz'] #ok
+	v7_col_names_rt = ['fN','type','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']
+	v8_col_names_rt = ['fN','type','targetID']
+	v9_col_names_rt = ['fN','type','snr','noise']
+	
+	# read from file for trace point clouds
+	fileName = ''
+	v6_col_names = ['time','fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz']
+	v7_col_names = ['time','fN','type','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']
+	v8_col_names = ['time','fN','type','targetID']
+	v9_col_names = ['fN','type','snr','noise']
+	'''
 	def readFile(self,fileName):
 		#fileName = "pc32021-03-19-10-02-17.csv"  
 		#df = pd.read_csv(fileName, error_bad_lines=False, warn_bad_lines=False) 
 		self.fileName = fileName 
-		#          ['time','fN','type','elv','azimuth','range' ,'doppler','snr','sx', 'sy', 'sz']
-		df = pd.read_csv(self.fileName, names = self.v6_col_names, skiprows = [0,11,12]) 
+		#          ['time','fN','type','elv','azimuth','range' ,'doppler','sx', 'sy', 'sz']
+		df = pd.read_csv(self.fileName, names = self.v6_col_names, skiprows = [0,10,11,12],dtype={'fN': int,'elv': float,'azimuth':float,'range':float,'doppler':float,'sx':float,'sy':float,'sz':float}) 
 		df.dropna()
 		#print("------------------- df --------------------shape:{:}".format(df.shape))
+		print(df)
 		print(df.info())
-		print(df.info(memory_usage="deep")) 
+		#print(df.info(memory_usage="deep")) 
 		
 		v6simOri = df[(df.type == 'v6')]
-		#print("-------------------v6sim------------:{:}".format(v6simOri.shape))
-		#self.v6simo = v6simOri.loc[:,['fN','elv','azimuth','range','doppler','snr']]
-		self.v6simo = v6simOri.loc[:,['fN','type','elv','azimuth','range' ,'doppler','snr','sx', 'sy', 'sz']]
+		#print("-------------------v6simo------------:{:}".format(v6simOri.shape))
+									 
+		self.v6simo = v6simOri.loc[:,['fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz']]
+		
+		if len(self.v6simo):
+			self.sim_startFN = df['fN'].values[0]
+			self.sim_stopFN  = df['fN'].values[-1]
+		#print(self.v6simo)
+		
 		self.v6simo['elv'] = self.v6simo['elv'].astype(float, errors = 'raise') 
 		
 		df7 = pd.read_csv(self.fileName, names = self.v7_col_names, skiprows = [0])  
 		
 		v7simc = df7[df7['type'] == 'v7']
-		self.v7simo  = v7simc.loc[:,['fN','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8','ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi','tid']]
-		self.sim_startFN = df['fN'].values[0]
-		self.sim_stopFN  = df['fN'].values[-1]
-		'''
-		print("---------start frame number---------:{:}".format(self.sim_startFN))
-		print("---------stop  frame number---------:{:}".format(self.sim_stopFN))
-		print(self.v7simo)
-		print("-----v8sim data lib-----")
-		'''
+		self.v7simo  = v7simc.loc[:,['fN','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']]
+		
 		v8simc = df[df['type'] == 'v8']
-		self.v8simo  = v8simc.loc[:,['fN','type','elv']]
-		self.v8simo.columns = ['fN','type','targetID']
+		self.v8simo  = v8simc.loc[:,['fN','elv']]
 		#print(self.v8simo)
-		return (self.v6simo,self.v7simo,self.v8simo)
+		
+		v9simc = df[df['type'] == 'v9']
+		self.v9simo  = v9simc.loc[:,['fN','type','range','azimuth']]
+		self.v9simo.columns = ['fN','type','snr','noise']
+	
+		return (self.v6simo,self.v7simo,self.v8simo,self.v9simo)
```

### Comparing `mmWave-0.1.98/mmWave/pc3_vsd.py` & `mmWave-0.1.99/mmWave/pc3_vsd.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pc3_vsd_v2.py` & `mmWave-0.1.99/mmWave/pc3_vsd_v2.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pc3d.py` & `mmWave-0.1.99/mmWave/pc3d.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pc3d_kv.py` & `mmWave-0.1.99/mmWave/pc3d_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/pct.py` & `mmWave-0.1.99/mmWave/pct.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/people3D.py` & `mmWave-0.1.99/mmWave/people3D.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/peopleMB.py` & `mmWave-0.1.99/mmWave/peopleMB.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/roadwayTMD_kv.py` & `mmWave-0.1.99/mmWave/roadwayTMD_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/srradar.py` & `mmWave-0.1.99/mmWave/srradar.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/surfaceVD.py` & `mmWave-0.1.99/mmWave/surfaceVD.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/trafficMD.py` & `mmWave-0.1.99/mmWave/trafficMD_I480.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,38 @@
-# Traffic Monitor Detector Raw Data (TMD)
-# modify from LPD
-# ver:0.0.2
-# 2021/04/24
+# Traffic Monitor Detector Raw Data (TMD_I480)
+# modify from TMD
+# v6,v7,v8,v9
+#
 # parsing Traffic Monitor Detector
-# hardware:(Batman-201): ISK IWR6843 ES2.0
+# hardware:(Batman-201/601): ISK IWR6843/1843
 # company: Joybien Technologies: www.joybien.com
 # author: Zach Chen
+# ver:0.1.1 2021/09/16
+# ver:2.0.1 2022/04/28
+# ver:2.0.2 2022/05/12
+# ver:2.0.3 2022/05/12
+# ver:2.0.4 2022/05/15
+# ver:2.0.5 2023/02/10
+# ver:2.0.6 2023/03/24 header enable/disable in inital
 #===========================================
 # output: V6,V7,V8,v9 Raw data
-# v0.0.1 : 2020/04/30 release
-# v0.1.0 : 2021/04/24 release
-#    added DataFrame 
-# v0.1.1 : 2023/03/24 release
-#          header enable/disable in inital
 #
+# playback data type:
+# 	v6: list/dataFrame
+# 	v7: list/dataFrame
+# 	v8: dictionary
+# 	v9: dictionary
+
+
 import serial
 import time
 import struct
 import pandas as pd
 import numpy as np
+import csv
 
 class header:
 	version = 0
 	totalPackLen = 0
 	platform = 0
 	timeStamp = 0
 	totalPacketLen = 0
@@ -32,92 +42,160 @@
 	frameMargin = 0 
 	trackProcessTime = 0
 	uartSendTime = 0
 	numTLVs = 0
 	checksum = 0
 
 
-class TrafficMD:
+class TrafficMD_I480:
 	
-	magicWord =  [b'\x02',b'\x01',b'\x04',b'\x03',b'\x06',b'\x05',b'\x08',b'\x07',b'\0x99']
+	magicWord =  [b'\x01',b'\x02',b'\x03',b'\x04',b'\x05',b'\x06',b'\x07',b'\x08',b'\0x99']
 	port = ""
 	hdr = header
 
 	# provide csv file dataframe
 	# real-time 
 	v6_col_names_rt = ['fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz'] #ok
-	v7_col_names_rt = ['fN','type','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']
+	v7_col_names_rt = ['fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','tid']
 	v8_col_names_rt = ['fN','type','targetID']
 	v9_col_names_rt = ['fN','type','snr','noise']
 	
 	# read from file for trace point clouds
 	fileName = ''
 	v6_col_names = ['time','fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz']
-	v7_col_names = ['time','fN','type','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']
+	v7_col_names = ['time','fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','tid']
 	v8_col_names = ['time','fN','type','targetID']
-	v9_col_names = ['fN','type','snr','noise']
+	v9_col_names = ['time','fN','type','snr','noise']
 	sim_startFN = 0
 	sim_stopFN  = 0 
 	
 	v6simo = []
 	v7simo = []
-	v8simo = []
-	v9simo = []
+	v8simo = {}
+	v9simo = {}
 	
 	# add for interal use
 	tlvLength = 0
 	numOfPoints = 0
 	# for debug use 
 	dbg = False #Packet unpacket Check: True show message 
-	sm = False #Observed StateMachine: True Show message
+	sm  = False #Observed StateMachine: True Show message
 	plen = 16 
 	
 	def __init__(self,port,show = True):
 		self.port = port
 		if show:
-			print("(jb)Traffic Monitor Detector(TMD) raw Data lib initial")
-			print("(jb)For Hardware:Batman-201(ISK)")
+			print("(jb)Traffic Monitor Detector(TMD_I480) raw Data lib initial")
+			print("(jb)For Hardware:Batman-201/501/601(ISK)")
 			print("(jb)Version: v0.1.0")
-			print("(jb)Hardware: IWR-6843 ES2.0")
+			print("(jb)Hardware: IWR-6843/1843")
 			print("(jb)Firmware: TMD")
 			print("(jb)UART Baud Rate:921600")
 			print("==============Info=================")
 			print("Output: V6,V7,V8,V9 data:(RAW)")
 			print("V6: Point Cloud Spherical")
-			print("v6 structure: [(range,azimuth,elevation,doppler),......]")
+			print("V6 structure: [(range,azimuth,elevation,doppler,sx,sy,sz),......]")
 			print("V7: Target Object List")
-			print("V7 structure: [(tid,posX,posY,velX,velY,accX,accY,posZ,velZ,accZ),....]")
+			print("V7 structure: [(posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,tid),....]") #revised text change "tid" position
 			print("V8: Target Index")
 			print("V8 structure: [id1,id2....]")
 			print("V9: Point Cloud Side Info")
 			print("V9 [(snr,noise),....]")
+			print("")
+			print("tlvRead status: {0:'EMPTY',1:'inData',10:'IDLE',99:'FALSE'} ")
+			print("")
 			print("===================================")
 	 
 		
 	def useDebug(self,ft):
 		self.dbg = ft
 		
 	def stateMachine(self,ft):
 		self.sm = ft
 		
 	def getHeader(self):
 		return self.hdr
-		
+	
+	#################################################################
+	# for version manegement
+	def jb_u32ToBytes(self, v): # convert u32 as Bytes
+		A = np.zeros( (4, 1) )
+		for i in range(4):
+			A[3 - i] = int(v  % 256)
+			v = int(v / 256)
+		return int(A[0, 0]), int(A[1, 0]), int(A[2, 0]), int(A[3, 0])
+	
+	def jb_versionManagement(self):
+		# test, for example: 
+		# result as following,
+		# (1) Platform    : IWR ISK, JB, 1843
+		# (2) FW   version: V80.61R
+		# (3) TOOL version: I.04.08.00
+		#
+		# (1) Platform
+		vHardware, vMagic, vType, vRxTxNum = self.jb_u32ToBytes(self.hdr.platform)			
+		# hardware type
+		if int(vHardware / 16) == 0:
+			tmp = ''
+		elif int(vHardware / 16) == 1:
+			tmp = 'IWR '
+		elif int(vHardware / 16) == 2:
+			tmp = 'AWR '
+		else:
+			tmp = ''
+		# hardware antenna
+		if int(vHardware % 16) == 0:
+			tmp += ''
+		elif int(vHardware % 16) == 1:
+			tmp += 'ISK'
+		elif int(vHardware % 16) == 2:
+			tmp += 'AOP'
+		else:
+			tmp += ''
+		vHardware = tmp	
+		# sel magic
+		if int(vMagic % 16) == 15:
+			vMagic = 'JB'
+		else:
+			vMagic = ''			
+		print("Platform    : {}, {}, {:02x}{:02x}".format(vHardware, vMagic, vType, vRxTxNum))
+		# (2) FW version
+		vAnt, vMagic, vMajor, vMinor = self.jb_u32ToBytes(self.hdr.chirpMargin)			
+		# hardware antenna
+		if vAnt == 'I':
+			vAnt = ', Ant= ISK'
+		elif vAnt == 'A':
+			vAnt = ', Ant= AOP'
+		else:	
+			vAnt = ''
+		print("FW   version: V{:02d}.{:02d}{:c} {}".format(vMajor, vMinor, vMagic, vAnt))
+		# (3) TOOL version
+		vTool, vMajor, vMinor, vMicro = self.jb_u32ToBytes(self.hdr.frameMargin)			
+		print("TOOL version: {:c}.{:02d}.{:02d}.{:02d}".format(vTool, vMajor, vMinor, vMicro))
+	#################################################################
+				
 	def headerShow(self):
 		print("***Header***********") 
 		print("Version:     \t%x "%(self.hdr.version))
-		print("Platform:    \t%X "%(self.hdr.platform))
-		#print("TimeStamp:   \t%s "%(self.hdr.timeStamp))
+		#print("Platform:    \t%X "%(self.hdr.platform))
+		print("TimeStamp:   \t%s "%(self.hdr.timeStamp))
 		print("TotalPackLen:\t%d "%(self.hdr.totalPackLen))
 		print("PID(frame#): \t%d "%(self.hdr.frameNumber))
 		print("subframe#  : \t%d "%(self.hdr.subFrameNumber))
+	    ########################################################
+		# original
+		#print("Platform:    \t%X "%(self.hdr.platform))		
+		#print("Inter-chirp Processing Margin:\t{:d} us".format(self.hdr.chirpMargin))
+		#print("Inter-frame Processing Margin:\t{:d} us".format(self.hdr.frameMargin))
+		# new replaced
+		self.jb_versionManagement()
+	    ########################################################
+		
 		print("Inter-frame Processing Time:\t{:d} us".format(self.hdr.trackProcessTime))
 		print("UART Send Time:\t{:d} us".format(self.hdr.uartSendTime))
-		print("Inter-chirp Processing Margin:\t{:d} us".format(self.hdr.chirpMargin))
-		print("Inter-frame Processing Margin:\t{:d} us".format(self.hdr.frameMargin))
 		print("numTLVs:     \t%d "%(self.hdr.numTLVs))
 		print("Check Sum   :\t{:x}".format(self.hdr.checksum))
 		print("***End Of Header***") 
 			
 	#for class internal use
 	def tlvTypeInfo(self,dtype,count,dShow):
 		sbyte = 8  #tlvHeader Struct = 8 bytes
@@ -132,15 +210,16 @@
 			dataByte= 16    #pointStruct 8bytes:(range,azimuth,elevation,doppler)
 			pString = "DPIF Point Cloud Spherical TLV"
 			nString = ""
 			stateString = "V6"
 		elif dtype == 7:
 			unitByte = 0   #pointUnit= 0bytes 
 			sbyte = 8 	   #tlvHeader Struct = 8 bytes
-			dataByte = 40  #target struct 40 bytes:(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ)  
+			#old: dataByte = 40  #target struct 40 bytes:(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ)  # I441
+			dataByte = 112 #target struct 112 bytes:(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0..15,g,c) # I480 
 			pString = "Target Object List TLV"
 			nString = "numOfObjects:"
 			stateString = "V7"
 		elif dtype == 8:
 			unitByte = 0 #pointUnit= 0bytes 
 			sbyte = 8    #tlvHeader Struct = 8 bytes
 			dataByte = 1 #targetID = 1 byte
@@ -193,14 +272,20 @@
 # (pass_fail, v6, v7, v8, v9)
 #  pass_fail: True: Data available    False: Data not available
 #
 #  v6: DPIF point cloud Spherical infomation
 #  v7: Target Object List information
 #  v8: Target Index information
 #  v9: DPIF Point Cloud Side Infomation
+#  
+#   0: empty: tlv = 0
+#   1: data output
+#  
+#   10: idle
+#   99: error
 #
 	def tlvRead(self,disp,df = None):
 		#print("---tlvRead---")
 		#ds = dos
 		typeList = [6,7,8,9]
 		idx = 0
 		lstate = 'idle'
@@ -221,15 +306,15 @@
 		v9df = ([])
 	
 		while True:
 			try:
 				ch = self.port.read()
 			except:
 				#return (False,v6,v7,v8,v9)
-				return self.list2df(False,v6,v7,v8,v9) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+				return self.list2df(99,v6,v7,v8,v9) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 			#print(str(ch))
 			if lstate == 'idle':
 				#print(self.magicWord)
 				if ch == self.magicWord[idx]:
 					#print("*** magicWord:"+ "{:02x}".format(ord(ch)) + ":" + str(idx))
 					idx += 1
 					if idx == 8:
@@ -238,15 +323,15 @@
 						rangeProfile = b""
 						sbuf = b""
 				else:
 					#print("not: magicWord state:")
 					idx = 0
 					rangeProfile = b""
 					#return (False,v6,v7,v8,v9)
-					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+					return self.list2df(10,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (10,v6,v7,v8,v9)
 		
 			elif lstate == 'header':
 				sbuf += ch
 				idx += 1
 				if idx == 44: 
 					#print("------header-----")
 					#print(":".join("{:02x}".format(c) for c in sbuf)) 	 
@@ -258,36 +343,37 @@
 						self.hdr.chirpMargin,self.hdr.frameMargin,self.hdr.trackProcessTime,self.hdr.uartSendTime,
 						self.hdr.numTLVs,self.hdr.checksum) = struct.unpack('10I2H', sbuf)
 						
 					except:
 						if self.dbg == True:
 							print("(Header)Improper TLV structure found: ")
 						#return (False,v6,v7,v8,v9)
-						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 					
 					if disp == True:  
 						self.headerShow()
 					
 					tlvCount = self.hdr.numTLVs
 					if self.hdr.numTLVs == 0:
 						#return (False,v6,v7,v8,v9)
-						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+						#return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+						return self.list2df(0,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (0,v6,v7,v8,v9)
 						
 					if self.sm == True:
 						print("(Header)")
 						
 					sbuf = b""
 					idx = 0
 					lstate = 'TL'
 					  
 				elif idx > 48:
 					idx = 0
 					lstate = 'idle'
 					#return (False,v6,v7,v8,v9)
-					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 					
 			elif lstate == 'TL': #TLV Header type/length
 				sbuf += ch
 				idx += 1
 				if idx == 8:
 					#print(":".join("{:02x}".format(c) for c in sbuf))
 					try: 
@@ -298,24 +384,24 @@
 							if self.dbg == True:
 								print("(TL)Improper TL Length(hex):(T){:d} (L){:x} numTLVs:{:d}".format(ttype,self.tlvLength,self.hdr.numTLVs))
 							sbuf = b""
 							idx = 0
 							lstate = 'idle'
 							self.port.flushInput()
 							#return (False,v6,v7,v8,v9)
-							return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+							return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 							
 					except:
 						print("TL unpack Improper Data Found:")
 						if self.dbg == True:
 							print("TL unpack Improper Data Found:")
 						self.port.flushInput()
 						#return (False,v6,v7,v8,v9)
 					
-						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 					
 					unitByteCount,lstate ,plen ,dataBytes,lenCount, numOfPoints = self.tlvTypeInfo(ttype,self.tlvLength,disp)
 					#print("dataBytes={:d} lenCount={:d}".format(dataBytes , lenCount))
 					if self.sm == True:
 						print("(TL:{:d})=>({:})".format(tlvCount,lstate))
 						
 					tlvCount -= 1
@@ -326,54 +412,55 @@
 				sbuf += ch
 				idx += 1
 				if (idx%dataBytes == 0):
 					try:
 						#print(":".join("{:02x}".format(c) for c in sbuf))
 						(r,a,e,d) = struct.unpack('4f', sbuf)
 						#print("({:2d}:{:4d})(idx:({:4d}) elv:{:.4f} azimuth:{:.4f} doppler:{:.4f} range:{:.4f}".format(numOfPoints,lenCount,idx,e,a,d,r))
+						sz  = r * np.sin(e)
+						sx  = r * np.cos(e) * np.sin(a)
+						sy  = r * np.cos(e) * np.cos(a)
 						if (df == 'DataFrame'):
-							sz  = r * np.sin(e)
-							sx  = r * np.cos(e) * np.sin(a)
-							sy  = r * np.cos(e) * np.cos(a)
+							
 							#fieldNames = ['time','frameNum','type','range/px','azimuth/py','elv/vx','doppler/vy','sx/accX','sy/accY','sz/pz','na/vz','na/accZ','na/ID']
 							v6df.append((self.hdr.frameNumber,'v6',r,a,e,d,sx,sy,sz))
 						else:
-							v6.append((r,a,e,d))
+							v6.append((r,a,e,d,sx,sy,sz))
 							
 						sbuf = b""
 					except:
 						if self.dbg == True:
 							print("(6.1)Improper Type 6 Value structure found: ")
 						#return (False,v6,v7,v8,v9)
-						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 					
 				if idx == lenCount:
 					if disp == True:
 						print("v6[{:d}]".format(len(v6)))
 					idx = 0
 					sbuf = b""
 					if tlvCount <= 0: # Back to idle
 						lstate = 'idle'
 						if self.sm == True:
 							print("(V6:tlvCnt={:d})=>(idle) :true".format(tlvCount))
 						#return (True,v6,v7,v8,v9)
 						print("(lib)v6=============SaveAppend==============")
-						return self.list2df(True,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (True,v6,v7,v8,v9)
+						return self.list2df(1,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (1,v6,v7,v8,v9)
 						
 					else: # Go to TL to get others type value
 						lstate = 'TL' #'tlTL'
 						if self.sm == True:
 							print("(V6:tlvCnt={:d})=>(TL)".format(tlvCount))
 					
 				elif idx > lenCount:
 					idx = 0
 					sbuf = b""
 					lstate = 'idle'
 					#return (False,v6,v7,v8,v9)
-					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 					
 			elif lstate == 'V9':  
 				sbuf += ch
 				idx += 1
 				if (idx%dataBytes == 0):
 					try:
 						#print(":".join("{:02x}".format(c) for c in sbuf))
@@ -386,85 +473,86 @@
 							v9.append((snr,noise))
 							
 						sbuf = b""
 					except:
 						if self.dbg == True:
 							print("(7)Improper Type 9 Value structure found: ")
 						#return (False,v6,v7,v8,v9)
-						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 						
 				if idx >= lenCount:
 					if disp == True:
 						print("count= v9[{:d}]".format(len(v9)))
 						
 					sbuf = b""
 					if tlvCount == 0:
 						lstate = 'idle'
 						if self.sm == True:
 							print("(V9)=>(idle) :true")
 						#return (True,v6,v7,v8,v9)
-						return self.list2df(True,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (True,v6,v7,v8,v9)
+						return self.list2df(1,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (1,v6,v7,v8,v9)
 						
 					else: # Go to TL to get others type value
 						lstate = 'TL'
 						idx = 0
 						if self.sm == True:
 							print("(V9)=>(TL)")
 							
 				if idx > lenCount:
 					idx = 0 
 					lstate = 'idle'
 					sbuf = b""
 					#return (False,v6,v7,v8,v9)
-					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 					
 			elif lstate == 'V7':
 				sbuf += ch
 				idx += 1
-				if (idx%dataBytes == 0):
+				if (idx % dataBytes == 0):
+					
 					#print("V7:dataBytes({:d}) lenCount({:d}) index:{:d}".format(dataBytes,lenCount,idx))
 					try:
-						(tid,posX,posY,velX,velY,accX,accY,posZ,velZ,accZ) = struct.unpack('I9f', sbuf) 
-						#fieldNames = ['time','frameNum','type','range/px','azimuth/py','elv/vx','doppler/vy','sx/accX','sy/accY','sz/pz','na/vz','na/accZ','na/ID']
+						
+						(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,conf) = struct.unpack('I27f', sbuf) 
 						if (df == 'DataFrame' ):
-							v7df.append((self.hdr.frameNumber,'v7',posX,posY,velX,velY,accX,accY,posZ,velZ,accZ,tid))
+							v7df.append((self.hdr.frameNumber,'v7',posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,tid))
 						else:
-							v7.append((tid,posX,posY,velX,velY,accX,accY,posZ,velZ,accZ))
+							v7.append((posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,tid))
 							#print("tid = ({:d}) ,posX:{:.4f} posY:{:.4f} posZ:{:.4f}".format(tid,posX,posY,posZ))
 						sbuf = b""
 					except:
 						if self.dbg == True:
 							print("(7)Improper Type 7 Value structure found: ")
 						#return (False,v6,v7,v8,v9)
-						return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 						
 				if idx >= lenCount:
 					if disp == True:
 						print("v7[{:d}]".format(len(v7)))
 					 
 					sbuf = b""
 					if tlvCount == 0:
 						lstate = 'idle'
 						if self.sm == True:
 							print("(V7)=>(idle) :true")
 						#return (True,v6,v7,v8,v9)
-						return self.list2df(True,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (True,v6,v7,v8,v9)
+						return self.list2df(1,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (1,v6,v7,v8,v9)
 						
 					else: # Go to TL to get others type value
 						lstate = 'TL'
 						idx = 0
 						if self.sm == True:
 							print("(V7)=>(TL)")
 
 				if idx > lenCount:
 					idx = 0 
 					lstate = 'idle'
 					sbuf = b""
 					#return (False,v6,v7,v8,v9)
-					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 				
 			elif lstate == 'V8':
 				idx += 1
 				v8.append(ord(ch))
 				if idx == lenCount:
 					if disp == True:
 						print("=====V8 End====")
@@ -474,84 +562,68 @@
 					if self.sm == True:
 						print("(V8:{:d})=>(idle)".format(tlvCount))
 						
 					if (df == 'DataFrame'):
 						v8o = [self.hdr.frameNumber,'v8']
 						v8df = v8o.extend(v8)
 					#return (True,v6,v7,v8,v9)
-					return self.list2df(True,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (True,v6,v7,v8,v9)
+					return self.list2df(1,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (1,v6,v7,v8,v9)
 				
 				if idx > lenCount:
 					sbuf = b""
 					idx = 0
 					lstate = 'idle'
 					#return (False,v6,v7,v8,v9)
-					return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
+					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
 
-	def getRecordData(self,frameNum):
-		s_fn = frameNum + self.sim_startFN
-		#print("frame number:{:}".format(s_fn))
-		v6d = self.v6simo[self.v6simo['fN'] == s_fn]
-		#v6d =  v6dd[v6dd['doppler'] < 0.0]
-		#print(v6d)
-		v7d = self.v7simo[self.v7simo['fN'] == s_fn]
-		v8d = self.v8simo[self.v8simo['fN'] == s_fn]
-		v9d = self.v9simo[self.v9simo['fN'] == s_fn]
-		chk = 0
-		if v6d.count != 0:
-			chk = 1
-		return (chk,v6d,v7d,v8d,v9d)
-		
-		
-	'''
-		v6_col_names_rt = ['fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz'] #ok
-	v7_col_names_rt = ['fN','type','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']
-	v8_col_names_rt = ['fN','type','targetID']
-	v9_col_names_rt = ['fN','type','snr','noise']
 	
-	# read from file for trace point clouds
-	fileName = ''
-	v6_col_names = ['time','fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz']
-	v7_col_names = ['time','fN','type','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']
-	v8_col_names = ['time','fN','type','targetID']
-	v9_col_names = ['fN','type','snr','noise']
-	'''
+	############## for playback use #####################
 	def readFile(self,fileName):
-		#fileName = "pc32021-03-19-10-02-17.csv"  
-		#df = pd.read_csv(fileName, error_bad_lines=False, warn_bad_lines=False) 
-		self.fileName = fileName 
-		#          ['time','fN','type','elv','azimuth','range' ,'doppler','sx', 'sy', 'sz']
-		df = pd.read_csv(self.fileName, names = self.v6_col_names, skiprows = [0,10,11,12],dtype={'fN': int,'elv': float,'azimuth':float,'range':float,'doppler':float,'sx':float,'sy':float,'sz':float}) 
-		df.dropna()
-		#print("------------------- df --------------------shape:{:}".format(df.shape))
-		print(df)
-		print(df.info())
-		#print(df.info(memory_usage="deep")) 
-		
-		v6simOri = df[(df.type == 'v6')]
-		#print("-------------------v6simo------------:{:}".format(v6simOri.shape))
-									 
-		self.v6simo = v6simOri.loc[:,['fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz']]
+		with open(fileName, newline='') as csvfile:
+			rows = csv.reader(csvfile)
+			v6s = [];v7s = [];v8s = [];v9s = []
+			for row in rows:
+				if row[2] == 'v6':
+					v6s.append(row)
+				elif row[2] == 'v7':
+					v7s.append(row)
+				elif row[2] == 'v8':
+					v8s.append(row)
+				elif row[2] == 'v9':
+					v9s.append(row)
+					
+		v6_col_names = ['time','fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz']
+		self.v6simo = pd.DataFrame(v6s,columns = v6_col_names).astype({'fN': 'int32','type':str,'range':float,'azimuth':float,'elv': float,'doppler':float,'sx':float,'sy':float,'sz':float},errors = 'raise') 
 		
 		if len(self.v6simo):
-			self.sim_startFN = df['fN'].values[0]
-			self.sim_stopFN  = df['fN'].values[-1]
-		#print(self.v6simo)
-		
-		self.v6simo['elv'] = self.v6simo['elv'].astype(float, errors = 'raise') 
-		
-		df7 = pd.read_csv(self.fileName, names = self.v7_col_names, skiprows = [0])  
-		
-		v7simc = df7[df7['type'] == 'v7']
-		self.v7simo  = v7simc.loc[:,['fN','posX','posY','velX','velY','accX','accY','posZ','velZ','accZ','tid']]
-		
-		v8simc = df[df['type'] == 'v8']
-		self.v8simo  = v8simc.loc[:,['fN','elv']]
-		#print(self.v8simo)
+			#print(f"self.v6simo['fN'].values[0] = {self.v6simo['fN'].values[0]}")
+			self.sim_startFN =  self.v6simo['fN'].values[0]
+			self.sim_stopFN  =  self.v6simo['fN'].values[-1]
+			
+		v7_col_names = ['time','fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','tid'] 
+		self.v7simo = pd.DataFrame(v7s,columns = v7_col_names )
 		
-		v9simc = df[df['type'] == 'v9']
-		self.v9simo  = v9simc.loc[:,['fN','type','range','azimuth']]
-		self.v9simo.columns = ['fN','type','snr','noise']
-	
-		return (self.v6simo,self.v7simo,self.v8simo,self.v9simo)
-
+		for item in v9s:
+			hh = item[3].strip('[]').replace('(', "").replace(')','').split(',')
+			self.v9simo[int(item[1])] = [(int(hh[i]),int(hh[i+1])) for i in range(0,len(hh),2)]
+		
+		for item in v8s:
+			hh = item[3].strip('[]').split(',')
+			self.v8simo[int(item[1])] = [int(hh[i]) for i in range(len(hh))] 
+			
 
+	def getRecordData(self,frameNum):
+		s_fn = frameNum + self.sim_startFN
+		v6d = self.v6simo.loc[self.v6simo['fN'] == s_fn]  #if (len(self.v6simo) > 0) else []
+		v7d = self.v7simo.loc[self.v7simo['fN'] == s_fn]  #if (len(self.v7simo) > 0) else []
+		try:
+			v8d =  self.v8simo[s_fn]    
+		except:
+			v8d = {}
+			
+		try:
+			v9d =  self.v9simo[s_fn] 
+		except:
+			v9d = {}
+		 
+		return(1,v6d,v7d,v8d,v9d)
+
```

### Comparing `mmWave-0.1.98/mmWave/trafficMD_I480.py` & `mmWave-0.1.99/mmWave/pc3_v2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,629 +1,608 @@
-# Traffic Monitor Detector Raw Data (TMD_I480)
-# modify from TMD
-# v6,v7,v8,v9
-#
-# parsing Traffic Monitor Detector
-# hardware:(Batman-201/601): ISK IWR6843/1843
+# Overhead People Counting 3D - ISK & AOP Raw Data (OHPC)
+# ver:2.0
+# 2022/04/19
+# 
+# parsing People Counting 3D data use AOP-ISK
+# hardware:(Batman-201)ISK IWR6843 ES2.0 & BM-501 AOP
+#    Fireware version: I470
+# Fit : wall mount
 # company: Joybien Technologies: www.joybien.com
 # author: Zach Chen
-# ver:0.1.1 2021/09/16
-# ver:2.0.1 2022/04/28
-# ver:2.0.2 2022/05/12
-# ver:2.0.3 2022/05/12
-# ver:2.0.4 2022/05/15
-# ver:2.0.5 2023/02/10
-# ver:2.0.6 2023/03/24 header enable/disable in inital
 #===========================================
-# output: V6,V7,V8,v9 Raw data
+# output: V6,V7,V8 Raw data
+# v0.0.1 : 2020/06/19 release
+#          (1)Output list data
+# v0.1.0 : 2021/04/01 
+#          (1)Output DataFrame
+# v0.1.1 : 2021/08/12
+#           (doppler and range swap in V6 output)
+# v0.1.2 : 2021/09/17
+#           v7 dataframe:'tid' move to front of 'ec0'
+# v2.0 : 2022/04/19
+#          pc3_v2: add ec[16],g,confidenceLevel
+#          this version lib same as pc3OVH 
+#
+# v2.0.1: 2022/06/10 v6 add sx,sy,sz
 #
-# playback data type:
-# 	v6: list/dataFrame
-# 	v7: list/dataFrame
-# 	v8: dictionary
-# 	v9: dictionary
+# v2.0.2: 2022/06/13 added azimuth offset
+#                    azi_offset
+# v2.0.3: 2023/06/30 add playback read v2
 
 
 import serial
 import time
 import struct
 import pandas as pd
 import numpy as np
-import csv
 
 class header:
 	version = 0
 	totalPackLen = 0
 	platform = 0
-	timeStamp = 0
-	totalPacketLen = 0
 	frameNumber = 0
-	subFrameNumber = 0
+	subframeNumber = 0
 	chirpMargin = 0
 	frameMargin = 0 
 	trackProcessTime = 0
 	uartSendTime = 0
 	numTLVs = 0
 	checksum = 0
 
+class unitS:
+	elevationUnit:float = 0.0
+	azimuthUnit : float = 0.0
+	dopplerUnit :float = 0.0
+	rangeUnit :float = 0.0
+	snrUnit :float = 0.0
 
-class TrafficMD_I480:
-	
-	magicWord =  [b'\x01',b'\x02',b'\x03',b'\x04',b'\x05',b'\x06',b'\x07',b'\x08',b'\0x99']
+class Pc3_v2:
+	#magicWord =  [b'\x01',b'\x02',b'\x03',b'\x04',b'\x05',b'\x06',b'\x07',b'\x08',b'\0x99']
+	magicWord =  [b'\x02',b'\x01',b'\x04',b'\x03',b'\x06',b'\x05',b'\x08',b'\x07',b'\0x99']
 	port = ""
 	hdr = header
-
+	u = unitS
+	frameNumber = 0
+	azi_offset = 0.0
+	
 	# provide csv file dataframe
 	# real-time 
-	v6_col_names_rt = ['fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz'] #ok
-	v7_col_names_rt = ['fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','tid']
+	v6_col_names_rt = ['fN','type','elv','azimuth','range','doppler','snr','sx', 'sy', 'sz'] 
+	v7_col_names_rt = ['fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8','ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi','tid']
 	v8_col_names_rt = ['fN','type','targetID']
-	v9_col_names_rt = ['fN','type','snr','noise']
 	
 	# read from file for trace point clouds
 	fileName = ''
-	v6_col_names = ['time','fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz']
-	v7_col_names = ['time','fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','tid']
+	v6_col_names = ['time','fN','type','elv','azimuth','range','doppler','snr','sx', 'sy', 'sz']
+	#v7_col_names = ['time','fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8','ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi','tid']
+	v7_col_names = ['time','fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','tid','ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8','ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi'] #v0.1.2
 	v8_col_names = ['time','fN','type','targetID']
-	v9_col_names = ['time','fN','type','snr','noise']
 	sim_startFN = 0
 	sim_stopFN  = 0 
-	
-	v6simo = []
-	v7simo = []
-	v8simo = {}
-	v9simo = {}
-	
+	vxx_col_names = ['fN','type','i0','i1','i2','i3','i4', 'i5','i6','i7', 'i8','i9','i10','i11']
 	# add for interal use
 	tlvLength = 0
 	numOfPoints = 0
 	# for debug use 
 	dbg = False #Packet unpacket Check: True show message 
 	sm  = False #Observed StateMachine: True Show message
 	plen = 16 
 	
-	def __init__(self,port,show = True):
+	def __init__(self,port, degree = None):
 		self.port = port
-		if show:
-			print("(jb)Traffic Monitor Detector(TMD_I480) raw Data lib initial")
-			print("(jb)For Hardware:Batman-201/501/601(ISK)")
-			print("(jb)Version: v0.1.0")
-			print("(jb)Hardware: IWR-6843/1843")
-			print("(jb)Firmware: TMD")
-			print("(jb)UART Baud Rate:921600")
-			print("==============Info=================")
-			print("Output: V6,V7,V8,V9 data:(RAW)")
-			print("V6: Point Cloud Spherical")
-			print("V6 structure: [(range,azimuth,elevation,doppler,sx,sy,sz),......]")
-			print("V7: Target Object List")
-			print("V7 structure: [(posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,tid),....]") #revised text change "tid" position
-			print("V8: Target Index")
-			print("V8 structure: [id1,id2....]")
-			print("V9: Point Cloud Side Info")
-			print("V9 [(snr,noise),....]")
-			print("")
-			print("tlvRead status: {0:'EMPTY',1:'inData',10:'IDLE',99:'FALSE'} ")
-			print("")
-			print("===================================")
-	 
+		self.azi_offset = 0.0 if degree == None else degree * 3.14159/180.0
+		
+		print("(jb)People Counting 3D v2.0 (Wall Mount) initial")
+		print("(jb)vsersion:v2.0")
+		print("(jb)For Hardware:Batman-201(ISK) & BM-501 (AOP)")
+		print("(jb)Hardware: IWR-6843 & AOP")
+		print("(jb)Firmware: PC3-I470")
+		print("(jb)UART Baud Rate:921600")
+		print("Output: V6,V7,V8 data:(RAW)")
 		
 	def useDebug(self,ft):
 		self.dbg = ft
 		
 	def stateMachine(self,ft):
 		self.sm = ft
 		
 	def getHeader(self):
 		return self.hdr
-	
-	#################################################################
-	# for version manegement
-	def jb_u32ToBytes(self, v): # convert u32 as Bytes
-		A = np.zeros( (4, 1) )
-		for i in range(4):
-			A[3 - i] = int(v  % 256)
-			v = int(v / 256)
-		return int(A[0, 0]), int(A[1, 0]), int(A[2, 0]), int(A[3, 0])
-	
-	def jb_versionManagement(self):
-		# test, for example: 
-		# result as following,
-		# (1) Platform    : IWR ISK, JB, 1843
-		# (2) FW   version: V80.61R
-		# (3) TOOL version: I.04.08.00
-		#
-		# (1) Platform
-		vHardware, vMagic, vType, vRxTxNum = self.jb_u32ToBytes(self.hdr.platform)			
-		# hardware type
-		if int(vHardware / 16) == 0:
-			tmp = ''
-		elif int(vHardware / 16) == 1:
-			tmp = 'IWR '
-		elif int(vHardware / 16) == 2:
-			tmp = 'AWR '
-		else:
-			tmp = ''
-		# hardware antenna
-		if int(vHardware % 16) == 0:
-			tmp += ''
-		elif int(vHardware % 16) == 1:
-			tmp += 'ISK'
-		elif int(vHardware % 16) == 2:
-			tmp += 'AOP'
-		else:
-			tmp += ''
-		vHardware = tmp	
-		# sel magic
-		if int(vMagic % 16) == 15:
-			vMagic = 'JB'
-		else:
-			vMagic = ''			
-		print("Platform    : {}, {}, {:02x}{:02x}".format(vHardware, vMagic, vType, vRxTxNum))
-		# (2) FW version
-		vAnt, vMagic, vMajor, vMinor = self.jb_u32ToBytes(self.hdr.chirpMargin)			
-		# hardware antenna
-		if vAnt == 'I':
-			vAnt = ', Ant= ISK'
-		elif vAnt == 'A':
-			vAnt = ', Ant= AOP'
-		else:	
-			vAnt = ''
-		print("FW   version: V{:02d}.{:02d}{:c} {}".format(vMajor, vMinor, vMagic, vAnt))
-		# (3) TOOL version
-		vTool, vMajor, vMinor, vMicro = self.jb_u32ToBytes(self.hdr.frameMargin)			
-		print("TOOL version: {:c}.{:02d}.{:02d}.{:02d}".format(vTool, vMajor, vMinor, vMicro))
-	#################################################################
-				
+		
 	def headerShow(self):
-		print("***Header***********") 
+		print("******* Header ********") 
 		print("Version:     \t%x "%(self.hdr.version))
-		#print("Platform:    \t%X "%(self.hdr.platform))
-		print("TimeStamp:   \t%s "%(self.hdr.timeStamp))
+		print("Platform:    \t%X "%(self.hdr.platform))
 		print("TotalPackLen:\t%d "%(self.hdr.totalPackLen))
 		print("PID(frame#): \t%d "%(self.hdr.frameNumber))
-		print("subframe#  : \t%d "%(self.hdr.subFrameNumber))
-	    ########################################################
-		# original
-		#print("Platform:    \t%X "%(self.hdr.platform))		
-		#print("Inter-chirp Processing Margin:\t{:d} us".format(self.hdr.chirpMargin))
-		#print("Inter-frame Processing Margin:\t{:d} us".format(self.hdr.frameMargin))
-		# new replaced
-		self.jb_versionManagement()
-	    ########################################################
-		
+		print("subframe#  : \t%d "%(self.hdr.subframeNumber))
 		print("Inter-frame Processing Time:\t{:d} us".format(self.hdr.trackProcessTime))
 		print("UART Send Time:\t{:d} us".format(self.hdr.uartSendTime))
+		print("Inter-chirp Processing Margin:\t{:d} us".format(self.hdr.chirpMargin))
+		print("Inter-frame Processing Margin:\t{:d} us".format(self.hdr.frameMargin))
 		print("numTLVs:     \t%d "%(self.hdr.numTLVs))
 		print("Check Sum   :\t{:x}".format(self.hdr.checksum))
 		print("***End Of Header***") 
 			
 	#for class internal use
 	def tlvTypeInfo(self,dtype,count,dShow):
+		
 		sbyte = 8  #tlvHeader Struct = 8 bytes
 		unitByte = 20 
 		dataByte = 0
 		pString = ""
 		nString = "numOfPoints :"
-		stateString = "V6"
+		stateString = "V6-unit"
 		if dtype == 6:
-			unitByte = 0   #pointUnit= 20bytes
-			sbyte = 8      #tlvHeader Struct = 8 bytes
-			dataByte= 16    #pointStruct 8bytes:(range,azimuth,elevation,doppler)
-			pString = "DPIF Point Cloud Spherical TLV"
+			unitByte = 20  #pointUnit= 20bytes (elvUnit(4),aziUnit(4),dopplerUnit(4),rangeUnit(4),snrUnit(4))
+			sbyte = 8      #tlvHeader Struct = 8 bytes (type(4)/lenth(4))
+			dataByte= 8    #pointStruct 8bytes:(elevation(1),azimuth(1),doppler(2),range(2),snr(2))
+			pString = "Point Cloud TLV and pointUnit"
 			nString = ""
-			stateString = "V6"
 		elif dtype == 7:
 			unitByte = 0   #pointUnit= 0bytes 
-			sbyte = 8 	   #tlvHeader Struct = 8 bytes
-			#old: dataByte = 40  #target struct 40 bytes:(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ)  # I441
-			dataByte = 112 #target struct 112 bytes:(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0..15,g,c) # I480 
-			pString = "Target Object List TLV"
+			sbyte = 8 	   #tlvHeader Struct = 8 bytes (type(4)/lenth(4))
+			dataByte = 112  #target struct 112 bytes:(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,confi)  
+			pString = "Target Object TLV"
 			nString = "numOfObjects:"
 			stateString = "V7"
 		elif dtype == 8:
 			unitByte = 0 #pointUnit= 0bytes 
 			sbyte = 8    #tlvHeader Struct = 8 bytes
 			dataByte = 1 #targetID = 1 byte
 			pString = "Target Index TLV"
 			nString = "numOfIDs"
 			stateString = "V8"
-		elif dtype == 9:
-			unitByte = 0 #pointUnit= 0bytes 
-			sbyte = 8    #tlvHeader Struct = 8 bytes
-			dataByte = 4 #(snr,noise") =  4 byte
-			pString = "DPIF Point Cloud Side Info"
-			nString = "numOfIDs"
-			stateString = "V9"
 		else:
 			unitByte = 0
 			sbyte = 1
 			pString = "*** Type Error ***"
 			stateString = 'idle'
 		 
-		#retCnt = count - unitByte - sbyte
-		nPoint = count / dataByte
+		retCnt = count - unitByte -sbyte
+		nPoint = retCnt / sbyte
+		#dShow = True
 		if dShow == True:
-			print("-----[{:}] ----:{:}".format(pString,stateString))
-			print("tlv Type({:2d}Bytes):  \t{:d}".format(sbyte,dtype))
+			print("-----[{:}] ----".format(pString))
+			print("tlv Type({:2d}B):  \t{:d}".format(sbyte,dtype))
 			print("tlv length:      \t{:d}".format(count)) 
-			print("num of point:    \t{:d}".format(int(nPoint)))
-			print("value length:    \t{:d}".format(count))  
+			print("{:}      \t{:d}".format(nString,int(nPoint)))
+			print("value length:    \t{:d}".format(retCnt))  
 		
-		return unitByte,stateString, sbyte, dataByte,count, int(nPoint)
-		
-	def list2df(self,dck,l6,l7,l8,l9):
-		#print("---------------list2df: v6----------------")
-		#print(l6)
+		return unitByte,stateString, sbyte, dataByte,retCnt, int(nPoint)
 		
+	def list2df(self,dck,l6,l7,l8):
 		ll6 = pd.DataFrame(l6,columns=self.v6_col_names_rt)
 		ll7 = pd.DataFrame(l7,columns=self.v7_col_names_rt)
-		ll8 = pd.DataFrame(l8,columns=self.v8_col_names_rt)
-		ll9 = pd.DataFrame(l9,columns=self.v9_col_names_rt)
-		#print("------ll6---------list2df: v6----------------")
-		#print(ll6)
-		return (dck,ll6,ll7,ll8,ll9)
+		ll8 = l8 #pd.DataFrame(l8,columns=self.v8_col_names_rt)
+		return (dck,ll6,ll7,ll8)
 
 #
 # TLV: Type-Length-Value
 # read TLV data
 # input:
 #     disp: True:print message
 #			False: hide printing message
+#     df: 
 # output:(return parameter)
-# (pass_fail, v6, v7, v8, v9)
+# (pass_fail, v6, v7, v8)
 #  pass_fail: True: Data available    False: Data not available
-#
-#  v6: DPIF point cloud Spherical infomation
-#  v7: Target Object List information
+#  v6: point cloud infomation
+#  v7: Target Object information
 #  v8: Target Index information
-#  v9: DPIF Point Cloud Side Infomation
 #  
-#   0: empty: tlv = 0
-#   1: data output
-#  
-#   10: idle
-#   99: error
+# 
 #
 	def tlvRead(self,disp,df = None):
+		
 		#print("---tlvRead---")
 		#ds = dos
-		typeList = [6,7,8,9]
+		typeList = [6,7,8]
 		idx = 0
 		lstate = 'idle'
 		sbuf = b""
 		lenCount = 0
 		unitByteCount = 0
 		dataBytes = 0
 		numOfPoints = 0
 		tlvCount = 0
 		pbyte = 16
 		v6 = ([])
 		v7 = ([])
 		v8 = ([])
-		v9 = ([])
 		v6df = ([])
 		v7df = ([])
 		v8df = ([])
-		v9df = ([])
-	
+		
 		while True:
 			try:
 				ch = self.port.read()
 			except:
-				#return (False,v6,v7,v8,v9)
-				return self.list2df(99,v6,v7,v8,v9) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
+				#return (False,v6,v7,v8)
+				#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6,v7,v8)
+				return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+				
 			#print(str(ch))
 			if lstate == 'idle':
 				#print(self.magicWord)
 				if ch == self.magicWord[idx]:
 					#print("*** magicWord:"+ "{:02x}".format(ord(ch)) + ":" + str(idx))
 					idx += 1
 					if idx == 8:
+						 
 						idx = 0
 						lstate = 'header'
 						rangeProfile = b""
 						sbuf = b""
 				else:
 					#print("not: magicWord state:")
 					idx = 0
 					rangeProfile = b""
-					#return (False,v6,v7,v8,v9)
-					return self.list2df(10,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (10,v6,v7,v8,v9)
+					#return (False,v6,v7,v8)
+					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
 		
 			elif lstate == 'header':
 				sbuf += ch
 				idx += 1
-				if idx == 44: 
+				if idx == 40: 
 					#print("------header-----")
 					#print(":".join("{:02x}".format(c) for c in sbuf)) 	 
 					#print("len:{:d}".format(len(sbuf))) 
 					# [header - Magicword]
 					try: 
-						(self.hdr.version,self.hdr.platform,self.hdr.timeStamp,self.hdr.totalPackLen,
-						self.hdr.frameNumber,self.hdr.subFrameNumber,
+						(self.hdr.version,self.hdr.totalPackLen,self.hdr.platform,
+						self.hdr.frameNumber,self.hdr.subframeNumber,
 						self.hdr.chirpMargin,self.hdr.frameMargin,self.hdr.trackProcessTime,self.hdr.uartSendTime,
-						self.hdr.numTLVs,self.hdr.checksum) = struct.unpack('10I2H', sbuf)
-						
+						self.hdr.numTLVs,self.hdr.checksum) = struct.unpack('9I2H', sbuf)
+						self.frameNumber = self.hdr.frameNumber
 					except:
 						if self.dbg == True:
 							print("(Header)Improper TLV structure found: ")
-						#return (False,v6,v7,v8,v9)
-						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
+						#return (False,v6,v7,v8)
+						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
 					
 					if disp == True:  
 						self.headerShow()
 					
 					tlvCount = self.hdr.numTLVs
+					#print("tlvCount:{:}".format(tlvCount))
 					if self.hdr.numTLVs == 0:
-						#return (False,v6,v7,v8,v9)
-						#return self.list2df(False,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (False,v6,v7,v8,v9)
-						return self.list2df(0,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (0,v6,v7,v8,v9)
+						#return (True,v6,v7,v8)
+						#return (True,v6,v7,v8) if (df == None) else self.list2df(True,v6df,v7df,v8df)
+						return self.list2df(True,v6df,v7df,v8df) if (df == 'DataFrame') else (True,v6,v7,v8)
 						
 					if self.sm == True:
 						print("(Header)")
 						
 					sbuf = b""
 					idx = 0
 					lstate = 'TL'
 					  
-				elif idx > 48:
+				elif idx > 44:
 					idx = 0
 					lstate = 'idle'
-					#return (False,v6,v7,v8,v9)
-					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
+					#return (False,v6,v7,v8)
+					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
 					
 			elif lstate == 'TL': #TLV Header type/length
 				sbuf += ch
 				idx += 1
 				if idx == 8:
 					#print(":".join("{:02x}".format(c) for c in sbuf))
-					try: 
+					try:
 						ttype,self.tlvLength = struct.unpack('2I', sbuf)
-						#print("(TL)numTLVs({:d}): tlvCount({:d})-------ttype:tlvLength:{:d}:{:d}".format(self.hdr.numTLVs,tlvCount,ttype,self.tlvLength))
-						
+						#print("--tlvNum:{:d}: tlvCount({:d})-------ttype:tlvLength:{:d}:{:d}".format(self.hdr.numTLVs,tlvCount,ttype,self.tlvLength))
 						if ttype not in typeList or self.tlvLength > 10000:
 							if self.dbg == True:
 								print("(TL)Improper TL Length(hex):(T){:d} (L){:x} numTLVs:{:d}".format(ttype,self.tlvLength,self.hdr.numTLVs))
 							sbuf = b""
 							idx = 0
 							lstate = 'idle'
 							self.port.flushInput()
-							#return (False,v6,v7,v8,v9)
-							return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
+							#return (False,v6,v7,v8)
+							#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+							return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
 							
 					except:
-						print("TL unpack Improper Data Found:")
 						if self.dbg == True:
 							print("TL unpack Improper Data Found:")
 						self.port.flushInput()
-						#return (False,v6,v7,v8,v9)
-					
-						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
+						#return (False,v6,v7,v8)
+						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
 					
 					unitByteCount,lstate ,plen ,dataBytes,lenCount, numOfPoints = self.tlvTypeInfo(ttype,self.tlvLength,disp)
-					#print("dataBytes={:d} lenCount={:d}".format(dataBytes , lenCount))
+					#if ttype == 6:
+					#	print("--pointCloud:((tlvLength({:d})-pointUnit(20)-tlvStruct(8))/8={:d}".format(self.tlvLength,numOfPoints))
 					if self.sm == True:
 						print("(TL:{:d})=>({:})".format(tlvCount,lstate))
 						
 					tlvCount -= 1
 					idx = 0  
 					sbuf = b""
 			
+			elif lstate == 'V6-unit':
+				sbuf += ch
+				idx += 1
+				if idx == unitByteCount :
+					#print(":".join("{:02x}".format(c) for c in sbuf))
+					#print("unitByte:{:d}".format(len(sbuf)))
+					try:
+						self.u.elevationUnit,self.u.azimuthUnit,self.u.dopplerUnit,self.u.rangeUnit,self.u.snrUnit = struct.unpack('5f', sbuf)
+						#print("Unit  ==> elv:{:.4f} azimuth:{:.4f} doppler:{:.4f} range:{:.4f} snr:{:.4f}".format(self.u.elevationUnit,self.u.azimuthUnit,self.u.dopplerUnit,self.u.rangeUnit,self.u.snrUnit))
+						sbuf = b""
+						idx = 0
+						lstate = 'V6'				
+					except:
+						if self.dbg == True:
+							print("(6.0)Improper Type 6 unit Value structure found: ")
+						#return (False,v6,v7,v8)
+						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+					
+					if self.sm == True:
+						print("(V6-unit:{:d})=>({:})".format(tlvCount,lstate))
+						#print("(V6-unit)=>({:})".format(lstate))
+					
 			elif lstate == 'V6': # count = Total Lentgh - 8
 				sbuf += ch
 				idx += 1
 				if (idx%dataBytes == 0):
 					try:
 						#print(":".join("{:02x}".format(c) for c in sbuf))
-						(r,a,e,d) = struct.unpack('4f', sbuf)
-						#print("({:2d}:{:4d})(idx:({:4d}) elv:{:.4f} azimuth:{:.4f} doppler:{:.4f} range:{:.4f}".format(numOfPoints,lenCount,idx,e,a,d,r))
-						sz  = r * np.sin(e)
-						sx  = r * np.cos(e) * np.sin(a)
-						sy  = r * np.cos(e) * np.cos(a)
+						(e,a,d,r,s) = struct.unpack('2b3h', sbuf)
+						elv = e * self.u.elevationUnit
+						azi = a * self.u.azimuthUnit + self.azi_offset
+						dop = d * self.u.dopplerUnit
+						ran = r * self.u.rangeUnit
+						snr = s * self.u.snrUnit
+						#print("({:2d}:{:4d})(idx:({:4d}) elv:{:.4f} azimuth:{:.4f} doppler:{:.4f} range:{:.4f} snr:{:.4f}".format(numOfPoints,lenCount,idx,elv,azi,dop,ran,snr))
+						sz  = ran * np.sin(elv)
+						sx  = ran * np.cos(elv) * np.sin(azi)
+						sy  = ran * np.cos(elv) * np.cos(azi)
+						
 						if (df == 'DataFrame'):
-							
-							#fieldNames = ['time','frameNum','type','range/px','azimuth/py','elv/vx','doppler/vy','sx/accX','sy/accY','sz/pz','na/vz','na/accZ','na/ID']
-							v6df.append((self.hdr.frameNumber,'v6',r,a,e,d,sx,sy,sz))
+							#v6df.append((self.hdr.frameNumber,'v6',elv,azi,dop,ran,snr,sx,sy,sz)) #v0.1.0
+							v6df.append((self.hdr.frameNumber,'v6',elv,azi,ran,dop,snr,sx,sy,sz)) #v0.1.1
+							 
 						else:
-							v6.append((r,a,e,d,sx,sy,sz))
-							
+							#v6.append((elv,azi,dop,ran,snr)) 
+							v6.append((elv,azi,dop,ran,snr,sx,sy,sz)) #v2.0.1
+						
+						#print("point_cloud_2d.append:[{:d}]".format(len(point_cloud_2d)))
 						sbuf = b""
+						
 					except:
 						if self.dbg == True:
 							print("(6.1)Improper Type 6 Value structure found: ")
-						#return (False,v6,v7,v8,v9)
-						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
+						#return (False,v6,v7,v8)
+						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
 					
 				if idx == lenCount:
 					if disp == True:
 						print("v6[{:d}]".format(len(v6)))
 					idx = 0
 					sbuf = b""
 					if tlvCount <= 0: # Back to idle
 						lstate = 'idle'
 						if self.sm == True:
-							print("(V6:tlvCnt={:d})=>(idle) :true".format(tlvCount))
-						#return (True,v6,v7,v8,v9)
-						print("(lib)v6=============SaveAppend==============")
-						return self.list2df(1,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (1,v6,v7,v8,v9)
+							print("(V6:{:d})=>(idle) :true".format(tlvCount))
+						#return (True,v6,v7,v8)
+						#return (True,v6,v7,v8) if (df == None) else self.list2df(True,v6df,v7df,v8df)
+						return self.list2df(True,v6df,v7df,v8df) if (df == 'DataFrame') else (True,v6,v7,v8)
 						
 					else: # Go to TL to get others type value
 						lstate = 'TL' #'tlTL'
 						if self.sm == True:
-							print("(V6:tlvCnt={:d})=>(TL)".format(tlvCount))
+							print("(V6:{:d})=>(TL)".format(tlvCount))
 					
 				elif idx > lenCount:
 					idx = 0
 					sbuf = b""
 					lstate = 'idle'
-					#return (False,v6,v7,v8,v9)
-					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
-					
-			elif lstate == 'V9':  
-				sbuf += ch
-				idx += 1
-				if (idx%dataBytes == 0):
-					try:
-						#print(":".join("{:02x}".format(c) for c in sbuf))
-						(snr,noise) =  struct.unpack('2h', sbuf)
-						#print("lenCnt = ({:d}) snr:{:.4f} noise:{:.4f}".format(lenCount,snr,noise))
-						
-						if (df == 'DataFrame'):
-							v9df.append((self.hdr.frameNumber,'v9',snr,noise))
-						else:
-							v9.append((snr,noise))
-							
-						sbuf = b""
-					except:
-						if self.dbg == True:
-							print("(7)Improper Type 9 Value structure found: ")
-						#return (False,v6,v7,v8,v9)
-						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
-						
-				if idx >= lenCount:
-					if disp == True:
-						print("count= v9[{:d}]".format(len(v9)))
-						
-					sbuf = b""
-					if tlvCount == 0:
-						lstate = 'idle'
-						if self.sm == True:
-							print("(V9)=>(idle) :true")
-						#return (True,v6,v7,v8,v9)
-						return self.list2df(1,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (1,v6,v7,v8,v9)
-						
-					else: # Go to TL to get others type value
-						lstate = 'TL'
-						idx = 0
-						if self.sm == True:
-							print("(V9)=>(TL)")
-							
-				if idx > lenCount:
-					idx = 0 
-					lstate = 'idle'
-					sbuf = b""
-					#return (False,v6,v7,v8,v9)
-					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
-					
+					#return (False,v6,v7,v8)
+					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6,v7,v8)
+					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+				
 			elif lstate == 'V7':
 				sbuf += ch
 				idx += 1
-				if (idx % dataBytes == 0):
-					
+				if (idx%dataBytes == 0):
 					#print("V7:dataBytes({:d}) lenCount({:d}) index:{:d}".format(dataBytes,lenCount,idx))
 					try:
-						
-						(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,conf) = struct.unpack('I27f', sbuf) 
-						if (df == 'DataFrame' ):
-							v7df.append((self.hdr.frameNumber,'v7',posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,tid))
+						#(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ) = struct.unpack('I9f', sbuf)
+						(tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,confi) = struct.unpack('I27f', sbuf)
+						if (df == 'DataFrame'): 
+							v7df.append((self.hdr.frameNumber,'v7',posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,confi,tid))
+							
 						else:
-							v7.append((posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,tid))
-							#print("tid = ({:d}) ,posX:{:.4f} posY:{:.4f} posZ:{:.4f}".format(tid,posX,posY,posZ))
+							v7.append((tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ,ec0,ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,confi))
+						
 						sbuf = b""
 					except:
 						if self.dbg == True:
 							print("(7)Improper Type 7 Value structure found: ")
-						#return (False,v6,v7,v8,v9)
-						return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
+						#return (False,v6,v7,v8)
+						#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+						return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
 						
 				if idx >= lenCount:
 					if disp == True:
 						print("v7[{:d}]".format(len(v7)))
 					 
 					sbuf = b""
 					if tlvCount == 0:
 						lstate = 'idle'
 						if self.sm == True:
 							print("(V7)=>(idle) :true")
-						#return (True,v6,v7,v8,v9)
-						return self.list2df(1,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (1,v6,v7,v8,v9)
+						#return (True,v6,v7,v8)
+						#return (True,v6,v7,v8) if (df == None) else self.list2df(True,v6df,v7df,v8df)
+						return self.list2df(True,v6df,v7df,v8df) if (df == 'DataFrame') else (True,v6,v7,v8)
 						
 					else: # Go to TL to get others type value
 						lstate = 'TL'
 						idx = 0
 						if self.sm == True:
 							print("(V7)=>(TL)")
 
 				if idx > lenCount:
 					idx = 0 
 					lstate = 'idle'
 					sbuf = b""
-					#return (False,v6,v7,v8,v9)
-					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
+					#return (False,v6,v7,v8)
+					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
 				
 			elif lstate == 'V8':
 				idx += 1
 				v8.append(ord(ch))
+				
 				if idx == lenCount:
 					if disp == True:
-						print("=====V8 End====")
+						print("=====V8 End====")						
 					sbuf = b""
 					idx = 0
 					lstate = 'idle'
 					if self.sm == True:
 						print("(V8:{:d})=>(idle)".format(tlvCount))
-						
+					
 					if (df == 'DataFrame'):
-						v8o = [self.hdr.frameNumber,'v8']
-						v8df = v8o.extend(v8)
-					#return (True,v6,v7,v8,v9)
-					return self.list2df(1,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (1,v6,v7,v8,v9)
+						v8df = [self.hdr.frameNumber,'v8']
+						v8df.extend(v8)
+						
+					#return (True,v6,v7,v8) if (df == None) else self.list2df(True,v6df,v7df,v8df)
+					return self.list2df(True,v6df,v7df,v8df) if (df == 'DataFrame') else (True,v6,v7,v8)
 				
 				if idx > lenCount:
 					sbuf = b""
 					idx = 0
 					lstate = 'idle'
-					#return (False,v6,v7,v8,v9)
-					return self.list2df(99,v6df,v7df,v8df,v9df) if (df == 'DataFrame') else (99,v6,v7,v8,v9)
-
+					#return (False,v6,v7,v8)
+					#return (False,v6,v7,v8) if (df == None) else self.list2df(False,v6df,v7df,v8df)
+					return self.list2df(False,v6df,v7df,v8df) if (df == 'DataFrame') else (False,v6,v7,v8)
+					
+	def v67Simlog(frameNum):
+		global sim_startFN,sim_stopFN
+		s_fn = frameNum + sim_startFN
+		#print("frame number:{:}".format(s_fn))
+		v6d = v6sim[v6sim['fN'] == s_fn]
+		#v6d =  v6dd[v6dd['doppler'] < 0.0]
+		#print(v6d)
+		v7d = v7sim[v7sim['fN'] == s_fn]
+		chk = 0
+		if v6d.count != 0:
+			chk = 1
+		return (chk,v6d,v7d)
+		
+	def getRecordData(self,frameNum):
+		s_fn = frameNum + self.sim_startFN
+		#print("frame number:{:}".format(s_fn))
+		v6d = self.v6simo[self.v6simo['fN'] == s_fn]
+		#v6d =  v6dd[v6dd['doppler'] < 0.0]
+		#print(v6d)
+		v7d = self.v7simo[self.v7simo['fN'] == s_fn]
+		v8d = self.v8simo[self.v8simo['fN'] == s_fn]
+		chk = 0
+		if v6d.count != 0:
+			chk = 1
+		return (chk,v6d,v7d,v8d)
 	
-	############## for playback use #####################
 	def readFile(self,fileName):
-		with open(fileName, newline='') as csvfile:
-			rows = csv.reader(csvfile)
-			v6s = [];v7s = [];v8s = [];v9s = []
-			for row in rows:
-				if row[2] == 'v6':
-					v6s.append(row)
-				elif row[2] == 'v7':
-					v7s.append(row)
-				elif row[2] == 'v8':
-					v8s.append(row)
-				elif row[2] == 'v9':
-					v9s.append(row)
-					
-		v6_col_names = ['time','fN','type','range','azimuth','elv' ,'doppler','sx', 'sy', 'sz']
-		self.v6simo = pd.DataFrame(v6s,columns = v6_col_names).astype({'fN': 'int32','type':str,'range':float,'azimuth':float,'elv': float,'doppler':float,'sx':float,'sy':float,'sz':float},errors = 'raise') 
 		
-		if len(self.v6simo):
-			#print(f"self.v6simo['fN'].values[0] = {self.v6simo['fN'].values[0]}")
-			self.sim_startFN =  self.v6simo['fN'].values[0]
-			self.sim_stopFN  =  self.v6simo['fN'].values[-1]
-			
-		v7_col_names = ['time','fN','type','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','tid'] 
-		self.v7simo = pd.DataFrame(v7s,columns = v7_col_names )
+		self.fileName = fileName 
+		df = pd.read_csv(self.fileName)
+		#print("------------------- df --------------------shape:{:}".format(df.shape))
+		print(df.info())
+		#print(df.info(memory_usage="deep")) 
+		
+		#    ['fN','type','elv','azimuth','range' ,'doppler','snr','sx', 'sy', 'sz']
+		#     fN','type','elv', 'azimuth','range' ,'doppler','snr','sx', 'sy', 'sz'
+		#[time,fN,type,   posX,    posY,    posZ,    velX,   velY , velZ, accX, accY, accZ, ec0, ec1,ec2,ec3,ec4,ec5,ec6,ec7,ec8,ec9,ec10,ec11,ec12,ec13,ec14,ec15,g,confi,tid]    
+		#   0   1   2       3       4        5         6       7     8     9    10    11    12   13   14  15  16  17  18 19  20   21   22  23    24   25  26   27  28 29    30
+
+		
+		self.v6simo = df[df['type'] == 'v6'].drop(['time','accZ','ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8','ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi','tid'], 
+		axis=1).rename(columns={'posX':'elv','posY': 'azimuth','posZ': 'range' , 'velX' : 'doppler','velY': 'snr','velZ': 'sx' ,'accX':'sy','accY':'sz'})
+		
+		self.v7simo = df[df['type'] == 'v7'].drop(['time'],axis=1)
+		
+		self.v8simo = df[df['type'] == 'v8'].drop(['time','posY','posZ','velX','velY','velZ','accX','accY','accZ',
+													'ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8',
+													'ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi','tid'],axis=1).rename(columns={'posX':'targetID'})
+		
+		self.sim_startFN = int(df['fN'].values[1])
+		self.sim_stopFN  = int(df['fN'].values[-1])
+		
+		#print(f'self.sim_startFN  = {self.sim_startFN} self.sim_stopFN = {self.sim_stopFN} ')
+		return (self.v6simo,self.v7simo,self.v8simo)
+		
 		
-		for item in v9s:
-			hh = item[3].strip('[]').replace('(', "").replace(')','').split(',')
-			self.v9simo[int(item[1])] = [(int(hh[i]),int(hh[i+1])) for i in range(0,len(hh),2)]
-		
-		for item in v8s:
-			hh = item[3].strip('[]').split(',')
-			self.v8simo[int(item[1])] = [int(hh[i]) for i in range(len(hh))] 
-			
 
-	def getRecordData(self,frameNum):
-		s_fn = frameNum + self.sim_startFN
-		v6d = self.v6simo.loc[self.v6simo['fN'] == s_fn]  #if (len(self.v6simo) > 0) else []
-		v7d = self.v7simo.loc[self.v7simo['fN'] == s_fn]  #if (len(self.v7simo) > 0) else []
-		try:
-			v8d =  self.v8simo[s_fn]    
-		except:
-			v8d = {}
-			
-		try:
-			v9d =  self.v9simo[s_fn] 
-		except:
-			v9d = {}
-		 
-		return(1,v6d,v7d,v8d,v9d)
 	
+	################### v2 ############## 
+	
+		
+	def readFile_v2(self,fileName):
+		#fileName = "pc32021-03-19-10-02-17.csv"  
+		#df = pd.read_csv(fileName, error_bad_lines=False, warn_bad_lines=False) 
+		self.fileName = fileName 
+		df = pd.read_csv(self.fileName)
+		
+		#print("------------------- df --------------------shape:{:}".format(df.shape))
+		print(df.info())
+		#print(df.info(memory_usage="deep")) 
+		
+		# vxx_col_names = ['fN','type','i0','i1','i2','i3','i4', 'i5','i6','i7     , i8',   'i9' 
+		#                              (elv,azi ,dop ,ran, snr,   sx,  sy,  sz , Associate)
+		self.v6simo = df[df['type'] == 'v6'].drop(['i9'], axis=1).rename(columns={'i0': 'elv', 'i1': 'azi', 'i2': 'dop', 'i3': 'range', 'i4': 'snr',
+																					'i5': 'sx', 'i6': 'sy', 'i7' : 'sz' , 'i8':'Ass' })
+		
+		self.v7simo = df[df['type'] == 'v7'].rename(columns={'i0': 'tid', 'i1': 'posX', 'i2': 'posY', 'i3': 'posZ', 'i4': 'velX', 'i5': 'velY', 'i6': 'velZ', 'i7': 'accX', 'i8': 'accY', 'i9': 'accZ','i10':'g','i11':'c'})
+		#   
+		#print("======v7simo=========")
+		#print(self.v7simo)
+		self.sim_startFN = int(df['fN'].values[1])
+		self.sim_stopFN  = int(df['fN'].values[-1])
+		return (self.sim_startFN,self.sim_stopFN,self.v6simo,self.v7simo)
+		
+	def getRecordData_v2(self,frameNum):
+		s_fn =  frameNum + self.sim_startFN
+		#print("frame number:{:}".format(s_fn))
+		v68d = self.v6simo[(self.v6simo.fN ==  s_fn)]
+		#                     eadrsxyzif
+		#v68o = v68d.loc[:,['range','elv','azi','dop','sx','sy','sz','snr','Ass','fN']].apply(pd.to_numeric)
+		v68o = v68d.loc[:,['elv','azi','dop','range','snr','sx','sy','sz','Ass','fN']].apply(pd.to_numeric)
+		
+		v7d = self.v7simo[(self.v7simo.fN ==  s_fn)]
+		v7o = v7d.loc[:,['tid','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','fN']].apply(pd.to_numeric)
+		return(v68o,v7o)
+		
+
+	def recording_pc3_v2(self,writer= None,v68=None,v7=None,fn = None):
+		if v68 is not None: #v6 + v8
+			if len(v68) > 0:
+				v6l = v68
+				for i in v6l:
+					# vxx_col_names = ['fN','type','i0','i1','i2','i3','i4', 'i5','i6','i7     , i8',   'i9' 
+					#                               (elv,azi,dop ,ran, snr,   sx,  sy,  sz , Associate)
+					item = [fn,'v6'] + list(i)
+					writer.writerow(item)
+		
+		if v7 is not None:
+			if len(v7) > 0:
+				v7l = v7
+				for i in v7l:
+					#
+					#vxx_col_names = ['fN','type','i0','i1','i2','i3','i4', 'i5','i6','i7','i8','i9','i10','i11'    
+					#							  (tid,posX,posY,posZ,velX,velY,velZ,accX,accY,accZ ,'g' ,  'c'            
+					#  								0   1     2    3   4   5     6    7     9   10    11    12        
+					#  
+					item = [fn,'v7'] + list( tuple(i[:10]) + (i[-2],i[-1])) 
+					writer.writerow(item)
+		 
+		
+
+
```

### Comparing `mmWave-0.1.98/mmWave/trafficMD_kv.py` & `mmWave-0.1.99/mmWave/trafficMD_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/vehicleOD.py` & `mmWave-0.1.99/mmWave/vehicleOD.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/vehicleODHeatMap.py` & `mmWave-0.1.99/mmWave/vehicleODHeatMap.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/vehicleODR.py` & `mmWave-0.1.99/mmWave/vehicleODR.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/vitalsign.py` & `mmWave-0.1.99/mmWave/vitalsign.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave/vitalsign_kv.py` & `mmWave-0.1.99/mmWave/vitalsign_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/mmWave.egg-info/PKG-INFO` & `mmWave-0.1.99/mmWave.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmWave
-Version: 0.1.98
+Version: 0.1.99
 Summary: Joybien mmWave (Batman-101/201/301/501/601) library
 Home-page: http://www.joybien.com
 Download-URL: https://pypi.org/project/mmWave
 Author: Bighead Chen
 Author-email: zach_chen@joybien.com
 Project-URL: API Source Code, https://github.com/bigheadG/mmWave
 Classifier: Programming Language :: Python :: 3
@@ -118,14 +118,15 @@
 14. mmWave-1.0.77      
     2022/06/09 mrRadar added headerShowAll()
 15. mmWave-1.0.78
     2022/06/10 pc3_v2 v2.0.1, (v6 data update) add sx,sy,sz
     2022/06/13 pc3_v2 v2.0.2, added azimuth offset 
 16. mmWave-1.0.79
     2022/06/13 pc3_v2 v2.0.2, added azimuth offset 
+    2023/06/30 pc3_v2 v2.0.3, playback function
 17. mmWave-1.0.80
     2022/07/18 pc3OVH v1.0.0, added tilt,install height and (sx,sy,sz) in raw data mode     
 18. mmWave-1.0.81 
     2022/07/19 pc3OVH v1.0.1, added v6 fetch time
 19. mmWave-1.0.83 (fix 82)
     2022/07/20 v1.0.2 raw data: (elv,azi,ran,dop,snr,sx,sy,sz)..
 20. mmWave-1.0.84
```

### Comparing `mmWave-0.1.98/mmWave.egg-info/SOURCES.txt` & `mmWave-0.1.99/mmWave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.98/setup.py` & `mmWave-0.1.99/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -178,23 +178,27 @@
 # @1.0.96
 #    2023/04/07 pc3_V1884R v0.0.2  add try..except in unpack
 #
 # @1.0.97
 #   2023/05/25 pc3_oob v0.0.4 add v7 and playback
 # @1.0.98
 #   2023/05/25 pc3_oob v0.0.5 bug fix
+#
+# @1.0.99
+#   2023/06/30 pc3_v2  v2.0.3 add playback read v2
+#
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mmWave",
-    version="0.1.98",
+    version="0.1.99",
     author="Bighead Chen",
     author_email="zach_chen@joybien.com",
     description="Joybien mmWave (Batman-101/201/301/501/601) library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://www.joybien.com",
     download_url="https://pypi.org/project/mmWave",
```

