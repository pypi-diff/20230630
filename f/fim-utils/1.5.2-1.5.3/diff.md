# Comparing `tmp/fim_utils-1.5.2.tar.gz` & `tmp/fim_utils-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim_utils-1.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fim_utils-1.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fim_utils-1.5.2.tar` & `fim_utils-1.5.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1955 2023-06-14 13:08:12.061187 fim_utils-1.5.2/.gitignore
--rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.2/LICENSE
--rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.2/MANIFEST.in
--rw-r--r--   0        0        0     7348 2023-06-14 13:08:12.061836 fim_utils-1.5.2/README.md
--rw-r--r--   0        0        0      156 2023-06-14 19:58:07.843935 fim_utils-1.5.2/fimutil/__init__.py
--rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.2/fimutil/al2s/__init__.py
--rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.2/fimutil/al2s/arm.py
--rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.2/fimutil/al2s/cloud_cfg.py
--rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.2/fimutil/al2s/oess.py
--rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.2/fimutil/netam/__init__.py
--rw-r--r--   0        0        0    19815 2023-06-14 13:08:12.063296 fim_utils-1.5.2/fimutil/netam/arm.py
--rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.2/fimutil/netam/nso.py
--rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.2/fimutil/netam/sr_pce.py
--rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.2/fimutil/ralph/__init__.py
--rw-r--r--   0        0        0     3456 2023-06-14 19:22:11.396659 fim_utils-1.5.2/fimutil/ralph/asset.py
--rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.2/fimutil/ralph/dp_switch.py
--rw-r--r--   0        0        0     3991 2023-06-14 13:08:12.064708 fim_utils-1.5.2/fimutil/ralph/ethernetport.py
--rw-r--r--   0        0        0    21991 2023-06-14 13:08:12.065444 fim_utils-1.5.2/fimutil/ralph/fim_helper.py
--rw-r--r--   0        0        0     2574 2023-06-14 19:54:12.053408 fim_utils-1.5.2/fimutil/ralph/fpga.py
--rw-r--r--   0        0        0     1304 2023-06-14 19:54:22.381741 fim_utils-1.5.2/fimutil/ralph/gpu.py
--rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.2/fimutil/ralph/model.py
--rw-r--r--   0        0        0     1666 2023-06-14 13:08:12.067133 fim_utils-1.5.2/fimutil/ralph/nvme.py
--rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.2/fimutil/ralph/ralph_uri.py
--rw-r--r--   0        0        0     5825 2023-05-10 02:03:36.805547 fim_utils-1.5.2/fimutil/ralph/site.py
--rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.2/fimutil/ralph/storage.py
--rw-r--r--   0        0        0    10922 2023-06-14 19:23:06.279493 fim_utils-1.5.2/fimutil/ralph/worker_node.py
--rw-r--r--   0        0        0        0 2023-06-14 13:08:12.067791 fim_utils-1.5.2/fimutil/utilities/__init__.py
--rw-r--r--   0        0        0     6183 2023-06-14 13:08:12.068611 fim_utils-1.5.2/fimutil/utilities/generate_instance_flavors.py
--rw-r--r--   0        0        0     1717 2023-06-14 13:08:12.069196 fim_utils-1.5.2/fimutil/utilities/scan_net.py
--rw-r--r--   0        0        0     1351 2023-06-14 13:08:12.069677 fim_utils-1.5.2/fimutil/utilities/scan_oess.py
--rw-r--r--   0        0        0     5594 2023-06-14 19:50:45.471475 fim_utils-1.5.2/fimutil/utilities/scan_site.py
--rw-r--r--   0        0        0     2121 2023-06-14 19:57:09.799801 fim_utils-1.5.2/fimutil/utilities/scan_worker.py
--rw-r--r--   0        0        0     1008 2023-06-14 13:08:12.071273 fim_utils-1.5.2/pyproject.toml
--rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.2/setup.py
--rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.2/test/al2s_test.py
--rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.2/test/netam_test.py
--rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.2/test/ralph_test.py
--rw-r--r--   0        0        0     8070 1970-01-01 00:00:00.000000 fim_utils-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1955 2023-06-14 13:08:12.061187 fim_utils-1.5.3/.gitignore
+-rw-r--r--   0        0        0     1071 2021-03-24 00:22:11.944263 fim_utils-1.5.3/LICENSE
+-rw-r--r--   0        0        0      201 2022-08-11 21:42:55.301280 fim_utils-1.5.3/MANIFEST.in
+-rw-r--r--   0        0        0     7348 2023-06-14 13:08:12.061836 fim_utils-1.5.3/README.md
+-rw-r--r--   0        0        0      156 2023-06-30 20:01:29.261689 fim_utils-1.5.3/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2022-10-26 01:51:00.888375 fim_utils-1.5.3/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0     9526 2023-05-10 02:03:58.408283 fim_utils-1.5.3/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2023-05-10 02:03:58.408621 fim_utils-1.5.3/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0    11301 2023-05-10 02:03:58.409043 fim_utils-1.5.3/fimutil/al2s/oess.py
+-rw-r--r--   0        0        0        2 2021-10-19 20:02:19.089826 fim_utils-1.5.3/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    19815 2023-06-14 13:08:12.063296 fim_utils-1.5.3/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2023-01-08 20:10:10.091848 fim_utils-1.5.3/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2021-09-17 00:59:00.932312 fim_utils-1.5.3/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2022-02-22 22:46:07.359348 fim_utils-1.5.3/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3456 2023-06-14 20:11:33.885819 fim_utils-1.5.3/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2022-11-09 23:04:15.007880 fim_utils-1.5.3/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2023-06-14 13:08:12.064708 fim_utils-1.5.3/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    21991 2023-06-14 13:08:12.065444 fim_utils-1.5.3/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2574 2023-06-14 20:11:33.888572 fim_utils-1.5.3/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     1304 2023-06-14 20:11:33.889490 fim_utils-1.5.3/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2022-10-26 01:51:00.892729 fim_utils-1.5.3/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1666 2023-06-14 13:08:12.067133 fim_utils-1.5.3/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1384 2021-09-27 19:32:26.474769 fim_utils-1.5.3/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     6407 2023-06-30 19:52:17.512322 fim_utils-1.5.3/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2021-07-02 19:22:05.667481 fim_utils-1.5.3/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    10922 2023-06-14 20:11:33.890225 fim_utils-1.5.3/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:08:12.067791 fim_utils-1.5.3/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6183 2023-06-14 13:08:12.068611 fim_utils-1.5.3/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1717 2023-06-14 13:08:12.069196 fim_utils-1.5.3/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     1351 2023-06-14 13:08:12.069677 fim_utils-1.5.3/fimutil/utilities/scan_oess.py
+-rw-r--r--   0        0        0     5594 2023-06-14 20:11:33.890832 fim_utils-1.5.3/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2121 2023-06-14 20:11:33.891406 fim_utils-1.5.3/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0     1008 2023-06-14 13:08:12.071273 fim_utils-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      984 2022-08-11 21:42:55.305204 fim_utils-1.5.3/setup.py
+-rw-r--r--   0        0        0      464 2022-10-26 01:51:00.894625 fim_utils-1.5.3/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2022-02-23 20:02:20.197422 fim_utils-1.5.3/test/netam_test.py
+-rw-r--r--   0        0        0      326 2021-03-31 20:43:55.831882 fim_utils-1.5.3/test/ralph_test.py
+-rw-r--r--   0        0        0     8070 1970-01-01 00:00:00.000000 fim_utils-1.5.3/PKG-INFO
```

### Comparing `fim_utils-1.5.2/.gitignore` & `fim_utils-1.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/LICENSE` & `fim_utils-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/README.md` & `fim_utils-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/al2s/arm.py` & `fim_utils-1.5.3/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/al2s/cloud_cfg.py` & `fim_utils-1.5.3/fimutil/al2s/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/al2s/oess.py` & `fim_utils-1.5.3/fimutil/al2s/oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/netam/arm.py` & `fim_utils-1.5.3/fimutil/netam/arm.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/netam/nso.py` & `fim_utils-1.5.3/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/netam/sr_pce.py` & `fim_utils-1.5.3/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/asset.py` & `fim_utils-1.5.3/fimutil/ralph/asset.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/dp_switch.py` & `fim_utils-1.5.3/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/ethernetport.py` & `fim_utils-1.5.3/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/fim_helper.py` & `fim_utils-1.5.3/fimutil/ralph/fim_helper.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/fpga.py` & `fim_utils-1.5.3/fimutil/ralph/fpga.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/gpu.py` & `fim_utils-1.5.3/fimutil/ralph/gpu.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/model.py` & `fim_utils-1.5.3/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/nvme.py` & `fim_utils-1.5.3/fimutil/ralph/nvme.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/ralph_uri.py` & `fim_utils-1.5.3/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/site.py` & `fim_utils-1.5.3/fimutil/ralph/site.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,23 +63,32 @@
             self.dp_switch.parse()
         except ValueError:
             logging.warning('Unable to find a dataplane switch in site, continuing')
 
         query = {'hostname': f'{self.name.lower()}-time' + self.domain}
         results = self.ralph.get_json_object(self.ralph.base_uri + 'data-center-assets/?' +
                                              urlencode(query))
-        ptp_url = None
-        try:
-            ptp_url = pyjq.one('[ .results[0].url ]', results)[0]
-            logging.info(f'Identified PTP server {ptp_url=}')
-            if not ptp_url:
-                raise ValueError
-            self.ptp = True
-        except ValueError:
-            logging.warning('Unable to find PTP server in site, continuing')
+
+        if self.config and self.config.get(self.name) and self.config.get(self.name).get('ptp'):
+            ptp_override = self.config.get(self.name).get('ptp')
+            if not isinstance(ptp_override, bool):
+                logging.error(f'Config file does not specify ptp override as a boolean for site {self.name}')
+                raise RuntimeError('Unable to continue')
+            logging.info(f'Overriding {self.name} PTP setting with {ptp_override} from static configuration file')
+            self.ptp = ptp_override
+        else:
+            ptp_url = None
+            try:
+                ptp_url = pyjq.one('[ .results[0].url ]', results)[0]
+                logging.info(f'Identified PTP server {ptp_url=}')
+                if not ptp_url:
+                    raise ValueError
+                self.ptp = True
+            except ValueError:
+                logging.warning('Unable to find PTP server in site, continuing')
 
         query = {'hostname__regex': f'{self.name.lower()}-w[1234567890]+' + self.domain}
         results = self.ralph.get_json_object(self.ralph.base_uri + 'data-center-assets/?' +
                                              urlencode(query))
 
         worker_urls = pyjq.one('[ .results[].url ]', results)
         logging.info(f'Identified {len(worker_urls)} workers')
```

### Comparing `fim_utils-1.5.2/fimutil/ralph/storage.py` & `fim_utils-1.5.3/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/ralph/worker_node.py` & `fim_utils-1.5.3/fimutil/ralph/worker_node.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/utilities/generate_instance_flavors.py` & `fim_utils-1.5.3/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/utilities/scan_net.py` & `fim_utils-1.5.3/fimutil/utilities/scan_net.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/utilities/scan_oess.py` & `fim_utils-1.5.3/fimutil/utilities/scan_oess.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/utilities/scan_site.py` & `fim_utils-1.5.3/fimutil/utilities/scan_site.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/fimutil/utilities/scan_worker.py` & `fim_utils-1.5.3/fimutil/utilities/scan_worker.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/pyproject.toml` & `fim_utils-1.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/setup.py` & `fim_utils-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/test/netam_test.py` & `fim_utils-1.5.3/test/netam_test.py`

 * *Files identical despite different names*

### Comparing `fim_utils-1.5.2/PKG-INFO` & `fim_utils-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fim-utils
-Version: 1.5.2
+Version: 1.5.3
 Summary: This is a package of Information Model utilitied for FABRIC
 Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>, Hussamuddin Nasir <nasir@netlab.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

