# Comparing `tmp/esgcet-5.2.0.tar.gz` & `tmp/esgcet-5.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ames4/git-repos/esg-publisher/src/python/dist/.tmp-f2j01_w1/esgcet-5.2.0.tar", last modified: Fri Jun 30 00:07:33 2023, max compression
+gzip compressed data, was "/Users/ames4/tmpgit/esg-publisher/pkg/dist/.tmp-w67g62ms/esgcet-5.2.0rc2.tar", last modified: Fri May 12 20:42:53 2023, max compression
```

## Comparing `esgcet-5.2.0.tar` & `esgcet-5.2.0rc2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ames4    (36337)    36337        0 2023-06-30 00:07:33.947952 esgcet-5.2.0/
--rw-r--r--   0 ames4    (36337)    36337      166 2023-06-30 00:07:33.947526 esgcet-5.2.0/PKG-INFO
--rw-r--r--   0 ames4    (36337)    36337      680 2023-06-30 00:05:55.000000 esgcet-5.2.0/esg.yaml
-drwxr-xr-x   0 ames4    (36337)    36337        0 2023-06-30 00:07:33.941269 esgcet-5.2.0/esgcet/
--rw-r--r--   0 ames4    (36337)    36337       22 2023-06-29 23:31:47.000000 esgcet-5.2.0/esgcet/__init__.py
--rw-r--r--   0 ames4    (36337)    36337     2949 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/activity_check.py
--rw-r--r--   0 ames4    (36337)    36337    12705 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/args.py
--rw-r--r--   0 ames4    (36337)    36337     2356 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/cmip5.py
--rw-r--r--   0 ames4    (36337)    36337     3679 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/cmip6.py
--rw-r--r--   0 ames4    (36337)    36337     3534 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/create_ip.py
--rw-r--r--   0 ames4    (36337)    36337      192 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/e3sm.py
--rw-r--r--   0 ames4    (36337)    36337     4620 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/esgindexpub.py
--rw-r--r--   0 ames4    (36337)    36337     2315 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/esgmapconv.py
--rw-r--r--   0 ames4    (36337)    36337     5815 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/esgmigrate.py
--rw-r--r--   0 ames4    (36337)    36337     7354 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/esgmkpubrec.py
--rw-r--r--   0 ames4    (36337)    36337     3856 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/esgpidcitepub.py
--rw-r--r--   0 ames4    (36337)    36337     6406 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/esgunpublish.py
--rw-r--r--   0 ames4    (36337)    36337     3645 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/esgupdate.py
--rw-r--r--   0 ames4    (36337)    36337     3446 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/generic_netcdf.py
--rw-r--r--   0 ames4    (36337)    36337     3631 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/generic_pub.py
--rw-r--r--   0 ames4    (36337)    36337     1102 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/handler_base.py
--rw-r--r--   0 ames4    (36337)    36337     3059 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/index_pub.py
--rw-r--r--   0 ames4    (36337)    36337     1604 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/input4mips.py
--rw-r--r--   0 ames4    (36337)    36337     2756 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/list2json.py
--rw-r--r--   0 ames4    (36337)    36337      798 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/logger.py
--rw-r--r--   0 ames4    (36337)    36337     2206 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/mapfile.py
--rw-r--r--   0 ames4    (36337)    36337     1682 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/migratecmd.py
--rw-r--r--   0 ames4    (36337)    36337    16357 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/mk_dataset.py
--rw-r--r--   0 ames4    (36337)    36337     4594 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/mk_dataset_autoc.py
--rw-r--r--   0 ames4    (36337)    36337     2349 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/mk_dataset_xarray.py
--rw-r--r--   0 ames4    (36337)    36337     1480 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/mkd_cmip5.py
--rw-r--r--   0 ames4    (36337)    36337     4774 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/mkd_create_ip.py
--rw-r--r--   0 ames4    (36337)    36337     1578 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/mkd_input4mips.py
--rw-r--r--   0 ames4    (36337)    36337     2995 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/mkd_non_nc.py
--rw-r--r--   0 ames4    (36337)    36337     8953 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/pid_cite_pub.py
--rw-r--r--   0 ames4    (36337)    36337     3966 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/pub_client.py
--rw-r--r--   0 ames4    (36337)    36337     3513 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/pub_internal.py
--rw-r--r--   0 ames4    (36337)    36337      463 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/pub_test.py
--rw-r--r--   0 ames4    (36337)    36337     4479 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/publish_script.py
--rw-r--r--   0 ames4    (36337)    36337     2272 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/search_check.py
--rw-r--r--   0 ames4    (36337)    36337     4736 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/settings.py
--rw-r--r--   0 ames4    (36337)    36337     2420 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/unpublish.py
--rw-r--r--   0 ames4    (36337)    36337     4029 2023-06-29 17:29:02.000000 esgcet-5.2.0/esgcet/update.py
-drwxr-xr-x   0 ames4    (36337)    36337        0 2023-06-30 00:07:33.946132 esgcet-5.2.0/esgcet.egg-info/
--rw-r--r--   0 ames4    (36337)    36337      166 2023-06-30 00:07:33.000000 esgcet-5.2.0/esgcet.egg-info/PKG-INFO
--rw-r--r--   0 ames4    (36337)    36337     1050 2023-06-30 00:07:33.000000 esgcet-5.2.0/esgcet.egg-info/SOURCES.txt
--rw-r--r--   0 ames4    (36337)    36337        1 2023-06-30 00:07:33.000000 esgcet-5.2.0/esgcet.egg-info/dependency_links.txt
--rw-r--r--   0 ames4    (36337)    36337      320 2023-06-30 00:07:33.000000 esgcet-5.2.0/esgcet.egg-info/entry_points.txt
--rw-r--r--   0 ames4    (36337)    36337        1 2023-06-29 23:44:36.000000 esgcet-5.2.0/esgcet.egg-info/not-zip-safe
--rw-r--r--   0 ames4    (36337)    36337       69 2023-06-30 00:07:33.000000 esgcet-5.2.0/esgcet.egg-info/requires.txt
--rw-r--r--   0 ames4    (36337)    36337        7 2023-06-30 00:07:33.000000 esgcet-5.2.0/esgcet.egg-info/top_level.txt
--rw-r--r--   0 ames4    (36337)    36337       38 2023-06-30 00:07:33.948113 esgcet-5.2.0/setup.cfg
--rwxr-xr-x   0 ames4    (36337)    36337     3091 2023-06-29 17:29:02.000000 esgcet-5.2.0/setup.py
+drwxr-xr-x   0 ames4    (36337)    36337        0 2023-05-12 20:42:53.226019 esgcet-5.2.0rc2/
+-rw-r--r--   0 ames4    (36337)    36337      169 2023-05-12 20:42:53.225594 esgcet-5.2.0rc2/PKG-INFO
+-rw-r--r--   0 ames4    (36337)    36337     2438 2022-06-23 14:22:51.000000 esgcet-5.2.0rc2/esg.ini
+drwxr-xr-x   0 ames4    (36337)    36337        0 2023-05-12 20:42:53.219987 esgcet-5.2.0rc2/esgcet/
+-rw-r--r--   0 ames4    (36337)    36337       25 2023-04-11 17:57:32.000000 esgcet-5.2.0rc2/esgcet/__init__.py
+-rw-r--r--   0 ames4    (36337)    36337     2640 2022-03-08 15:37:48.000000 esgcet-5.2.0rc2/esgcet/activity_check.py
+-rw-r--r--   0 ames4    (36337)    36337    12383 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/args.py
+-rw-r--r--   0 ames4    (36337)    36337     2499 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/cmip5.py
+-rw-r--r--   0 ames4    (36337)    36337     3736 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/cmip6.py
+-rw-r--r--   0 ames4    (36337)    36337     3694 2023-04-19 15:55:00.000000 esgcet-5.2.0rc2/esgcet/create_ip.py
+-rw-r--r--   0 ames4    (36337)    36337      192 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/e3sm.py
+-rw-r--r--   0 ames4    (36337)    36337     4614 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgindexpub.py
+-rw-r--r--   0 ames4    (36337)    36337     2309 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgmapconv.py
+-rw-r--r--   0 ames4    (36337)    36337     5809 2023-04-14 23:57:26.000000 esgcet-5.2.0rc2/esgcet/esgmigrate.py
+-rw-r--r--   0 ames4    (36337)    36337     7348 2023-04-26 23:13:35.000000 esgcet-5.2.0rc2/esgcet/esgmkpubrec.py
+-rw-r--r--   0 ames4    (36337)    36337     3850 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgpidcitepub.py
+-rw-r--r--   0 ames4    (36337)    36337     6400 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgunpublish.py
+-rw-r--r--   0 ames4    (36337)    36337     3639 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgupdate.py
+-rw-r--r--   0 ames4    (36337)    36337     3440 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/generic_netcdf.py
+-rw-r--r--   0 ames4    (36337)    36337     3625 2022-06-23 14:22:51.000000 esgcet-5.2.0rc2/esgcet/generic_pub.py
+-rw-r--r--   0 ames4    (36337)    36337     1102 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/handler_base.py
+-rw-r--r--   0 ames4    (36337)    36337     2808 2022-06-23 14:22:51.000000 esgcet-5.2.0rc2/esgcet/index_pub.py
+-rw-r--r--   0 ames4    (36337)    36337     1598 2023-05-12 20:41:14.000000 esgcet-5.2.0rc2/esgcet/input4mips.py
+-rw-r--r--   0 ames4    (36337)    36337     2756 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/list2json.py
+-rw-r--r--   0 ames4    (36337)    36337      613 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/logger.py
+-rw-r--r--   0 ames4    (36337)    36337     2200 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/mapfile.py
+-rw-r--r--   0 ames4    (36337)    36337     1676 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/migratecmd.py
+-rw-r--r--   0 ames4    (36337)    36337    16351 2023-04-24 16:37:31.000000 esgcet-5.2.0rc2/esgcet/mk_dataset.py
+-rw-r--r--   0 ames4    (36337)    36337     4594 2023-04-24 16:37:57.000000 esgcet-5.2.0rc2/esgcet/mk_dataset_autoc.py
+-rw-r--r--   0 ames4    (36337)    36337     2349 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/mk_dataset_xarray.py
+-rw-r--r--   0 ames4    (36337)    36337     1474 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/mkd_cmip5.py
+-rw-r--r--   0 ames4    (36337)    36337     4768 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/mkd_create_ip.py
+-rw-r--r--   0 ames4    (36337)    36337     1572 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/mkd_input4mips.py
+-rw-r--r--   0 ames4    (36337)    36337     2989 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/mkd_non_nc.py
+-rw-r--r--   0 ames4    (36337)    36337     8947 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/pid_cite_pub.py
+-rw-r--r--   0 ames4    (36337)    36337     3960 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/pub_client.py
+-rw-r--r--   0 ames4    (36337)    36337     3553 2023-01-06 00:49:50.000000 esgcet-5.2.0rc2/esgcet/pub_internal.py
+-rw-r--r--   0 ames4    (36337)    36337      463 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/pub_test.py
+-rw-r--r--   0 ames4    (36337)    36337     4479 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/publish_script.py
+-rw-r--r--   0 ames4    (36337)    36337     2266 2022-03-14 16:31:36.000000 esgcet-5.2.0rc2/esgcet/search_check.py
+-rw-r--r--   0 ames4    (36337)    36337     4736 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/settings.py
+-rw-r--r--   0 ames4    (36337)    36337     2414 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/unpublish.py
+-rw-r--r--   0 ames4    (36337)    36337     4023 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/update.py
+drwxr-xr-x   0 ames4    (36337)    36337        0 2023-05-12 20:42:53.224982 esgcet-5.2.0rc2/esgcet.egg-info/
+-rw-r--r--   0 ames4    (36337)    36337      169 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/PKG-INFO
+-rw-r--r--   0 ames4    (36337)    36337     1049 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/SOURCES.txt
+-rw-r--r--   0 ames4    (36337)    36337        1 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/dependency_links.txt
+-rw-r--r--   0 ames4    (36337)    36337      320 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/entry_points.txt
+-rw-r--r--   0 ames4    (36337)    36337        1 2023-02-16 00:31:46.000000 esgcet-5.2.0rc2/esgcet.egg-info/not-zip-safe
+-rw-r--r--   0 ames4    (36337)    36337       69 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/requires.txt
+-rw-r--r--   0 ames4    (36337)    36337        7 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/top_level.txt
+-rw-r--r--   0 ames4    (36337)    36337       38 2023-05-12 20:42:53.226142 esgcet-5.2.0rc2/setup.cfg
+-rwxr-xr-x   0 ames4    (36337)    36337     3091 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/setup.py
```

### Comparing `esgcet-5.2.0/esgcet/activity_check.py` & `esgcet-5.2.0rc2/esgcet/activity_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-import json
+import sys, json, os
 import esgcet.logger as logger
+
 from esgcet.settings import SOURCE_ID_LIMITS
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 
 class FieldCheck(object):
-    """
-    Container for CV attribute agreement checks.
-    For now this is specific to CMIP6.
-    """
+
     def __init__(self, cmor_path, silent=False):
-        """
-        Constuctor.
-        cmor_path (string)  Required path to CV files from a CMOR table repo
-        silent (bool)  Run with out INFO messages
-        """
-        # TODO make this configurable per project
         cv_path = "{}/CMIP6_CV.json".format(cmor_path)
         jobj = json.load(open(cv_path))["CV"]
         self.sid_dict = jobj["source_id"]
         self.silent = silent
         self.idx = -1
         self.publog = log.return_logger('Activity Check', silent=silent)
         self.project_key = "cmip6"
         self.project_str = "CMIP6"
 
+
     def check_activity(self, source_id, activity_id):
 
         if source_id not in self.sid_dict:
             return False
         rec = self.sid_dict[source_id]
 
         return activity_id in rec["activity_participation"]
@@ -50,15 +43,15 @@
         if not src_id in self.sid_dict: 
             self.publog.error("Source_id {} is unregistered with the {} Controlled Vocabulary (CV). Publication halted".format(src_id, self.project_str))
             self.publog.error("If you think this message has been received in error, please update your CV source repository")
             raise UserWarning
 
         if self.project_key in SOURCE_ID_LIMITS and len(src_id) > SOURCE_ID_LIMITS[self.project_key]:
             self.publog.error(f"Source_id {src_id} exceeds the {SOURCE_ID_LIMITS[self.project_key]} character limit for project {self.project_str}. Publication halted.")
-            raise UserWarning
+            raise UserWarning          
 
         if not self.check_activity(src_id, act_id):
             self.publog.error("Source_id {} is not registered for participation in CMIP6 activity {}. Publication halted".format(src_id, act_id))
             self.publog.error("If you think this message has been received in error, please update your CV source repository")
             raise UserWarning
         if not self.check_institution(src_id, inst_id):
             self.publog.error("Institution_id {} is not registered to contribute to source_id {}. Publication halted".format(inst_id, src_id))
```

### Comparing `esgcet-5.2.0/esgcet/args.py` & `esgcet-5.2.0rc2/esgcet/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import argparse
 from pathlib import Path
-import os
+import os, sys, json
 import esgcet.esgmigrate as em
+from esgcet.settings import *
 import esgcet.logger as logger
 import yaml
 
-log = logger.ESGPubLogger()
+import esgcet
+
+import esgcet
+
+log = logger.Logger()
 publog = log.return_logger('Settings')
 
 DEFAULT_ESGINI = '/esg/config/esgcet'
 
 
 class PublisherArgs:
-    """  Reconcile command line argumenets and config file settings.
-    """
+
     def __init__(self):
         pass
 
     def get_args(self):
-        """ Wrap argument parser
-        """
         parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
 
         # ANY FILE NAME INPUT: check first to make sure it exists
         home = str(Path.home())
         def_config = home + "/.esg/esg.yaml"
         parser.add_argument("--test", dest="test", action="store_true", help="PID registration will run in 'test' mode. Use this mode unless you are performing 'production' publications.")
         # replica stuff new... hard-coded, modify mk dataset so that it imports it instead
@@ -47,34 +49,27 @@
         parser.add_argument("--xarray", dest="xarray", action="store_true", help="Use Xarray to extract metadata even if Autocurator is configured.") 
 
         pub = parser.parse_args()
 
         return pub
 
     def load_config(self, config_path):
-        """
-        Load the configuration file from specified path
-        config_path : string  config file path cannot be empty
-        """
         config_file = None
         try:
             config_file = open(config_path, 'r')  # or "a+", whatever you need
         except IOError:
             publog.error("Could not open file, please provide correct path to yaml config file.")
             quit(1)
 
         with config_file as fd:
             conf = yaml.load(fd, Loader=yaml.SafeLoader)
         return conf
 
-    def get_dict(self,  fn_project):
-        """
-        Return a dict containing the publisher arguments to use:
-        fn_project (string)  Specified project if pre-parsed.
-        """
+    def get_dict(self, fullmap, fn_project):
+
         pub = self.get_args()
         json_file = pub.json
 
         if pub.migrate:
             em.run(DEFAULT_ESGINI, False, False)
 
         config_file = pub.cfg
@@ -252,15 +247,15 @@
 
         if globus == "none" and not silent:
             publog.info("No Globus UUID defined.")
 
         if dtn == "none" and not silent:
             publog.info("No data transfer node defined.")
 
-        argdict = { "silent": silent, "verbose": verbose,
+        argdict = {"fullmap": fullmap, "silent": silent, "verbose": verbose,
                    "cert": cert,
                    "autoc_command": autocurator, "index_node": index_node, "data_node": data_node,
                    "data_roots": data_roots, "globus": globus, "dtn": dtn, "replica": replica,
                    "json_file": json_file, "test": test, "user_project_config": proj_config, "verify": verify,
                    "auth": auth, "skip_prepare": skip_prepare, "force_prepare": force_prepare,
                    "non_nc": non_nc, "mountpoints": mountpoints}
```

### Comparing `esgcet-5.2.0/esgcet/cmip5.py` & `esgcet-5.2.0rc2/esgcet/cmip5.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-import os
+import sys, os
 from esgcet.create_ip import CreateIP
 from esgcet.mkd_cmip5 import ESGPubMKDCmip5
 from esgcet.settings import VARIABLE_LIMIT
+import logging
 import tempfile
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 
 class cmip5(CreateIP):
 
     def __init__(self, argdict):
         super().__init__(argdict)
         self.variable_limit = 100
         self.autoc_args = ' --out_pretty --out_json {} --files "{}/*.nc"'
         self.publog = log.return_logger('CMIP5', self.silent, self.verbose)
 
     def autocurator(self, map_json_data):
         datafile = map_json_data[0][1]
+
         destpath = os.path.dirname(datafile)
+        outname = os.path.basename(datafile)
+        idx = outname.rfind('.')  # was this needed for something?
 
         autstr = self.autoc_command + self.autoc_args
         files = os.listdir(destpath)
         for f in files:
             var = f.split('_')[0]
             if var not in self.variables:
                 self.variables.append(var)
@@ -42,15 +46,15 @@
         limit = False
         mkd = ESGPubMKDCmip5(self.data_node, self.index_node, self.replica, self.globus, self.data_roots,
                                 self.dtn, self.silent, self.verbose, limit_exceeded)
         for scan in self.scans:
             try:
                 out_json_data = mkd.get_records(map_json_data, scan.name, self.json_file)
                 self.datasets.append(out_json_data)
-            except:
+            except Exception as ex:
                 self.publog.exception("Occured while making dataset.")
                 self.cleanup()
                 exit(1)
             # only use first scan file if more than 75 variables
             if len(self.variables) > self.variable_limit:
                 limit = True
                 break
```

### Comparing `esgcet-5.2.0/esgcet/cmip6.py` & `esgcet-5.2.0rc2/esgcet/cmip6.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from esgcet.pid_cite_pub import ESGPubPidCite
 from esgcet.activity_check import FieldCheck
 import tempfile
+import json
+
+from esgcet.generic_pub import BasePublisher
 from esgcet.generic_netcdf import GenericPublisher
-import os
+import sys, os
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 
 class cmip6(GenericPublisher):
 
     scan_file = tempfile.NamedTemporaryFile()  # create a temporary file which is deleted afterward for autocurator
     scanfn = scan_file.name
     files = [scan_file, ]
```

### Comparing `esgcet-5.2.0/esgcet/create_ip.py` & `esgcet-5.2.0rc2/esgcet/create_ip.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import os
+import sys, os
+import json
+from esgcet.generic_pub import BasePublisher
 from esgcet.generic_netcdf import GenericPublisher
 from esgcet.mkd_create_ip import ESGPubMKDCreateIP
 from esgcet.update import ESGPubUpdate
 from esgcet.index_pub import ESGPubIndex
 import tempfile
 from esgcet.settings import VARIABLE_LIMIT
 from copy import deepcopy
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
-
+log = logger.Logger()
 
 class CreateIP(GenericPublisher):
 
     def __init__(self, argdict):
         super().__init__(argdict)
 
         self.scans = []
@@ -26,15 +27,18 @@
 
     def cleanup(self):
         for scan in self.scans:
             scan.close()
 
     def autocurator(self, map_json_data):
         datafile = map_json_data[0][1]
+
         destpath = os.path.dirname(datafile)
+        outname = os.path.basename(datafile)
+        idx = outname.rfind('.')  # was this needed for something?
 
         autstr = self.autoc_command + self.autoc_args
         files = os.listdir(destpath)
         for f in files:
             var = f.split('_')[0]
             if var not in self.variables:
                 self.variables.append(var)
@@ -55,35 +59,36 @@
         mkd = ESGPubMKDCreateIP(self.data_node, self.index_node, self.replica, self.globus, self.data_roots,
                                 self.dtn, self.silent, self.verbose, limit_exceeded)
         for scan in self.scans:
             try: 
                 out_json_data = mkd.get_records(map_json_data, scan.name, self.json_file)
                 self.datasets.append(deepcopy(out_json_data)) # herein lies the issue, copy hasn't fixed it
             except Exception as ex:
-                self.publog.exception(f"Failed to make dataset: {ex}")
+                self.publog.exception("Failed to make dataset")
                 self.cleanup()
                 exit(1)
             # only use first scan file if more than 75 variables
             if len(self.variables) > self.variable_limit:
                 limit = True
                 break
+            
 
         self.master_dataset = mkd.aggregate_datasets(self.datasets, limit)
         return 0
 
     def update(self, placeholder):
         up = ESGPubUpdate(self.index_node, self.cert, silent=self.silent, verbose=self.verbose, verify=self.verify, auth=self.auth)
         try:
             up.run(self.master_dataset)
         except Exception as ex:
-            self.publog.exception(f"Failed to update record: {ex}")
+            self.publog.exception("Failed to update record")
             self.cleanup()
             exit(1)
 
     def index_pub(self, placeholder):
         ip = ESGPubIndex(self.index_node, self.cert, silent=self.silent, verbose=self.verbose, verify=self.verify, auth=self.auth)
         try:
             ip.do_publish(self.master_dataset)
         except Exception as ex:
-            self.publog.exception(f"Failed to publish to index node: {ex}")
+            self.publog.exception("Failed to publish to index node")
             self.cleanup()
             exit(1)
```

### Comparing `esgcet-5.2.0/esgcet/esgindexpub.py` & `esgcet-5.2.0rc2/esgcet/esgindexpub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys, json, os
 from esgcet.index_pub import ESGPubIndex
 import argparse
 from pathlib import Path
 import esgcet.logger as logger
 import esgcet.args as pub_args
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 publog = log.return_logger('esgindexpub')
 
 
 def get_args():
     parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
 
     home = str(Path.home())
```

### Comparing `esgcet-5.2.0/esgcet/esgmapconv.py` & `esgcet-5.2.0rc2/esgcet/esgmapconv.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import os
 import argparse
 from pathlib import Path
 import esgcet.logger as logger
 import esgcet.args as pub_args
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 publog = log.return_logger('esgmapconv')
 
 
 def get_args():
     parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
 
     home = str(Path.home())
```

### Comparing `esgcet-5.2.0/esgcet/esgmigrate.py` & `esgcet-5.2.0rc2/esgcet/esgmigrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import shutil
 from datetime import date
 from pathlib import Path
 import json
 import esgcet.logger as logger
 import yaml
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 DEFAULT_ESGINI = '/esg/config/esgcet/'
 CONFIG_FN_DEST = "~/.esg/esg.yaml"
 
 # These are the keys that 
 MIGRATE_KEYS = ['pid_creds', 'data_roots', 'user_project_config']
```

### Comparing `esgcet-5.2.0/esgcet/esgmkpubrec.py` & `esgcet-5.2.0rc2/esgcet/esgmkpubrec.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 import sys
 import esgcet.args as pub_args
 import json
 import os
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 publog = log.return_logger('esgmkpubrec')
 
 from esgcet.mk_dataset_autoc import ESGPubAutocHandler
 from esgcet.mk_dataset_xarray import ESGPubXArrayHandler
 
 def get_args():
     parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
```

### Comparing `esgcet-5.2.0/esgcet/esgpidcitepub.py` & `esgcet-5.2.0rc2/esgcet/esgpidcitepub.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import json
 from pathlib import Path
 import os
 import esgcet.args as pub_args
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 publog = log.return_logger('esgpidcitepub')
 
 
 def get_args():
     parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
     home = str(Path.home())
     def_config = home + "/.esg/esg.yaml"
```

### Comparing `esgcet-5.2.0/esgcet/esgunpublish.py` & `esgcet-5.2.0rc2/esgcet/esgunpublish.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import argparse
 from pathlib import Path
 import esgcet.args as pub_args
 import esgcet.logger as logger
 
 from esgcet.mapfile import ESGPubMapConv
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 publog = log.return_logger('esgunpublish')
 
 import esgcet
 
 def get_args():
     parser = argparse.ArgumentParser(description="Unpublish data sets from ESGF databases.")
```

### Comparing `esgcet-5.2.0/esgcet/esgupdate.py` & `esgcet-5.2.0rc2/esgcet/esgupdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import json
 import argparse
 from pathlib import Path
 import esgcet.args as pub_args
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 publog = log.return_logger('esgupdate')
 
 
 def get_args():
     parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
 
     home = str(Path.home())
```

### Comparing `esgcet-5.2.0/esgcet/generic_netcdf.py` & `esgcet-5.2.0rc2/esgcet/generic_netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import json, os, sys
 import tempfile
 from esgcet.generic_pub import BasePublisher
 import traceback
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 class GenericPublisher(BasePublisher):
 
     scan_file = tempfile.NamedTemporaryFile()  # create a temporary file which is deleted afterward for autocurator
     scanfn = scan_file.name
 
     def __init__(self, argdict):
```

### Comparing `esgcet-5.2.0/esgcet/generic_pub.py` & `esgcet-5.2.0rc2/esgcet/generic_pub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from esgcet.mapfile import ESGPubMapConv
 from esgcet.mkd_non_nc import ESGPubMKDNonNC
 from esgcet.update import ESGPubUpdate
 from esgcet.index_pub import ESGPubIndex
 import sys
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 
 class BasePublisher(object):
 
     def __init__(self, argdict):
         self.argdict = argdict
         self.fullmap = argdict["fullmap"]
```

### Comparing `esgcet-5.2.0/esgcet/handler_base.py` & `esgcet-5.2.0rc2/esgcet/handler_base.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.2.0/esgcet/index_pub.py` & `esgcet-5.2.0rc2/esgcet/index_pub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from esgcet.pub_client import publisherClient
 import esgcet.logger as logger
+
 import os
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 
 class ESGPubIndex:
-    """
-    Wrapper class for push-publishing of records to the index node.
-    """
+
     def __init__(self, hostname, cert_fn, verbose=False, silent=False, verify=False, auth=True, arch_cfg=None):
-        """
-        Constructor, creates a "client" object
-        """
         self.silent = silent
         self.verbose = verbose
         self.pubCli = publisherClient(cert_fn, hostname, verify=verify, verbose=self.verbose, silent=self.silent, auth=auth)
         self.publog = log.return_logger('Index Publication', silent, verbose)
         self.arch_cfg = arch_cfg
 
+
     def gen_xml(self, d):
         out = []
         out.append("<doc>\n")
 
         for key in d:
 
             val = d[key]
@@ -33,18 +30,17 @@
                 for vv in val:
                     out.append('  <field name="{}">{}</field>\n'.format(key, vv))
             else:
                 out.append('  <field name="{}">{}</field>\n'.format(key, val))
         out.append("</doc>\n")
         return ''.join(out)
 
+
     def do_publish(self, dataset):
-        """ handle dataset publishing
-        dataset (list) of dictionary records
-        """
+
         rc = True
         for rec in dataset:
 
             new_xml = self.gen_xml(rec)
 
             if self.arch_cfg:
                 resp = self.archive_rec(rec, new_xml)
```

### Comparing `esgcet-5.2.0/esgcet/input4mips.py` & `esgcet-5.2.0rc2/esgcet/input4mips.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from esgcet.mkd_input4mips import ESGPubMKDinput4MIPs
 from esgcet.pid_cite_pub import ESGPubPidCite
 from esgcet.cmip6 import cmip6
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 class input4mips(cmip6):
 
     def __init__(self, argdict):
         super().__init__(argdict)
         self.MKD_Construct = ESGPubMKDinput4MIPs
         self.publog = log.return_logger('input4MIPs', self.silent, self.verbose)
```

### Comparing `esgcet-5.2.0/esgcet/list2json.py` & `esgcet-5.2.0rc2/esgcet/list2json.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.2.0/esgcet/logger.py` & `esgcet-5.2.0rc2/esgcet/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import logging
 
 
-class ESGPubLogger:
-    """
-    Logger wrapper class
-    """
+class Logger:
+
     def __init__(self):
-        """ Constructor
-        """
         pass
 
     def return_logger(self, name, silent=False, verbose=False):
-        """
-        Logger 'factory' method allows for the naming and level specification.
-        """
         publog = logging.getLogger(name)
         if silent:
             publog.setLevel(logging.WARNING)
         elif verbose:
             publog.setLevel(logging.DEBUG)
         else:
             publog.setLevel(logging.INFO)
```

### Comparing `esgcet-5.2.0/esgcet/mapfile.py` & `esgcet-5.2.0rc2/esgcet/mapfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from datetime import datetime
 import traceback
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 class ESGPubMapConv:
 
     def __init__(self, mapfilename, project=None, silent=False):
 
         self.mapfilename = mapfilename
         self.project = project
```

### Comparing `esgcet-5.2.0/esgcet/migratecmd.py` & `esgcet-5.2.0rc2/esgcet/migratecmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from esgcet.esgmigrate import ESGPubMigrate
 import argparse, sys, os
 from pathlib import Path
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 publog = log.return_logger('esgmigrate')
 
 
 DEFAULT_ESGINI = '/esg/config/esgcet/'
 home = str(Path.home())
```

### Comparing `esgcet-5.2.0/esgcet/mk_dataset.py` & `esgcet-5.2.0rc2/esgcet/mk_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from datetime import datetime, timedelta
 
 from esgcet.settings import *
 from pathlib import Path
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 class ESGPubMakeDataset:
     """
     Base class (abstract) to assemble the ESGF index records (dataset and file records).
     """
     def init_project(self, proj):
         """
```

### Comparing `esgcet-5.2.0/esgcet/mk_dataset_autoc.py` & `esgcet-5.2.0rc2/esgcet/mk_dataset_autoc.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.2.0/esgcet/mk_dataset_xarray.py` & `esgcet-5.2.0rc2/esgcet/mk_dataset_xarray.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.2.0/esgcet/mkd_cmip5.py` & `esgcet-5.2.0rc2/esgcet/mkd_cmip5.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from esgcet.settings import *
 from pathlib import Path
 from esgcet.mk_dataset import ESGPubMakeDataset
 from esgcet.mkd_create_ip import ESGPubMKDCreateIP
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 
 class ESGPubMKDCmip5(ESGPubMKDCreateIP):
 
     def init_project(self):
 
         self.DRS = DRS["cmip5"]
```

### Comparing `esgcet-5.2.0/esgcet/mkd_create_ip.py` & `esgcet-5.2.0rc2/esgcet/mkd_create_ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime, timedelta
 
 from esgcet.settings import *
 from pathlib import Path
 from esgcet.mk_dataset import ESGPubMakeDataset
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 
 class ESGPubMKDCreateIP(ESGPubMakeDataset):
 
     def init_project(self, s, l):
 
         self.project = "CREATE-IP"
```

### Comparing `esgcet-5.2.0/esgcet/mkd_input4mips.py` & `esgcet-5.2.0rc2/esgcet/mkd_input4mips.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from esgcet.mk_dataset import ESGPubMakeDataset
 from esgcet.settings import GA, GA_DELIMITED
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 
 class ESGPubMKDinput4MIPs(ESGPubMakeDataset):
 
     def __init__(self, data_node, index_node, replica, globus, data_roots, dtn, silent=False, verbose=False, limit_exceeded=False, user_project=None):
         super().__init__(data_node, index_node, replica, globus, data_roots, dtn, silent, verbose, limit_exceeded, user_project)
         self.publog = log.return_logger('Make Dataset input4MIPs', silent, verbose)
```

### Comparing `esgcet-5.2.0/esgcet/mkd_non_nc.py` & `esgcet-5.2.0rc2/esgcet/mkd_non_nc.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import configparser as cfg
 from esgcet.mk_dataset import ESGPubMakeDataset
 from datetime import datetime, timedelta
 from esgcet.settings import *
 from pathlib import Path
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 
 class ESGPubMKDNonNC(ESGPubMakeDataset):
 
     def __init__(self, data_node, index_node, replica, globus, data_roots, dtn, silent=False, verbose=False, limit_exceeded=False, user_project=None):
         super().__init__(data_node, index_node, replica, globus, data_roots, dtn, silent, verbose, limit_exceeded,
                          user_project)
```

### Comparing `esgcet-5.2.0/esgcet/pid_cite_pub.py` & `esgcet-5.2.0rc2/esgcet/pid_cite_pub.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys, json
 from esgcet.settings import PID_PREFIX, PID_EXCHANGE, HTTP_SERVICE, CITATION_URLS, PID_URL
 import traceback
 import esgcet.logger as logger
 
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 silent = False
 verbose = False
 pid_creds = {}
 import traceback
 
 class ESGPubPidCite(object):
```

### Comparing `esgcet-5.2.0/esgcet/pub_client.py` & `esgcet-5.2.0rc2/esgcet/pub_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 class publisherClient(object):
     """  REST API wrapper for the esg-seach/ws APIs
         User must supply API parameters in xml form for publish and updates, dataset_ids for retract/delete
     """
     
     def __init__(self, cert_fn, hostname, verify=False, verbose=False, silent=False, auth=True):
```

### Comparing `esgcet-5.2.0/esgcet/pub_internal.py` & `esgcet-5.2.0rc2/esgcet/pub_internal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from esgcet.args import PublisherArgs
+import esgcet.esgmigrate as migrate
 import os
+import json
 import sys
+from esgcet.settings import *
+import configparser as cfg
+from pathlib import Path
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
-publog = log.return_logger('Publisher-Main')
+log = logger.Logger()
+publog = log.return_logger('Publisher')
 
 
 def check_files(files):
     for file in files:
         try:
             myfile = open(file, 'r')
             myfile.close()
@@ -19,29 +24,28 @@
 
 def run(fullmap, pub_args):
 
     # SETUP
     split_map = fullmap.split("/")
     fname = split_map[-1]
     fname_split = fname.split(".")
-    project_name = fname_split[0]
+    p = fname_split[0]
 
     files = []
     files.append(fullmap)
 
     check_files(files)
 
-    argdict = pub_args.get_dict(project_name)
-    argdict["fullmap"] = fullmap
+    argdict = pub_args.get_dict(fullmap, p)
 
     if "proj" in argdict:
-        project_name = argdict["proj"]
+        p = argdict["proj"]
     else:
-        argdict["proj"] = project_name
-    project = project_name.lower()
+        argdict["proj"] = p
+    project = p.lower()
     user_defined = False
     if argdict["user_project_config"]:
         user_defined = True
     non_netcdf = False
     if argdict["non_nc"]:
         non_netcdf = True
 
@@ -74,14 +78,15 @@
 
     # ___________________________________________
     # WORKFLOW - one line call
 
     return proj.workflow()
 
 
+
 def main():
     pub_args = PublisherArgs()
     pub = pub_args.get_args()
     maps = pub.map  # full mapfile path
     if maps is None:
         publog.error("Missing argument --map, use " + sys.argv[0] + " --help for usage.")
         exit(1)
@@ -111,11 +116,10 @@
             myfile.close()
             if ismap:
                 rc = rc and run(m, pub_args)
 
     if not rc:
         exit(1)
 
-
 if __name__ == '__main__':
     sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
     main()
```

### Comparing `esgcet-5.2.0/esgcet/publish_script.py` & `esgcet-5.2.0rc2/esgcet/publish_script.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.2.0/esgcet/search_check.py` & `esgcet-5.2.0rc2/esgcet/search_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys, json, requests
 from datetime import datetime
 from pathlib import Path
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 ''' Handles setting latest=false for previously published versions, includes finding those in the index
 '''
 class ESGSearchCheck():
 
 
     def __init__(self, index_node,  silent=False, verbose=False, verify=True):
```

### Comparing `esgcet-5.2.0/esgcet/settings.py` & `esgcet-5.2.0rc2/esgcet/settings.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.2.0/esgcet/unpublish.py` & `esgcet-5.2.0rc2/esgcet/unpublish.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from esgcet.pid_cite_pub import ESGPubPidCite
 from esgcet.search_check import ESGSearchCheck
 
 
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 def check_for_pid_proj(dset_arr):
 
     for dset in dset_arr:
 
         parts = dset.split('.')
         if parts[0].lower() in ["cmip6", "input4mips"]:
```

### Comparing `esgcet-5.2.0/esgcet/update.py` & `esgcet-5.2.0rc2/esgcet/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from esgcet.pub_client import publisherClient
 import sys, json, requests
 from datetime import datetime
 from pathlib import Path
 import esgcet.logger as logger
 
-log = logger.ESGPubLogger()
+log = logger.Logger()
 
 ''' Handles setting latest=false for previously published versions, includes finding those in the index
 '''
 class ESGPubUpdate():
 
 
     def __init__(self, index_node, cert_fn, silent=False, verbose=False, verify=False, auth=True):
```

### Comparing `esgcet-5.2.0/esgcet.egg-info/SOURCES.txt` & `esgcet-5.2.0rc2/esgcet.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-esg.yaml
+esg.ini
 setup.py
 esgcet/__init__.py
 esgcet/activity_check.py
 esgcet/args.py
 esgcet/cmip5.py
 esgcet/cmip6.py
 esgcet/create_ip.py
```

### Comparing `esgcet-5.2.0/setup.py` & `esgcet-5.2.0rc2/setup.py`

 * *Files identical despite different names*

