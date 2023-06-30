# Comparing `tmp/dia-adfpro-1.6.5.tar.gz` & `tmp/dia-adfpro-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dia-adfpro-1.6.5.tar", last modified: Tue May 30 12:04:22 2023, max compression
+gzip compressed data, was "dia-adfpro-1.6.7.tar", last modified: Fri Jun 30 07:40:13 2023, max compression
```

## Comparing `dia-adfpro-1.6.5.tar` & `dia-adfpro-1.6.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:04:22.057431 dia-adfpro-1.6.5/
--rw-rw-rw-   0        0        0     1089 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/LICENSE.txt
--rw-rw-rw-   0        0        0       17 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1046 2023-05-30 12:04:22.058423 dia-adfpro-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0      685 2021-02-11 11:49:55.000000 dia-adfpro-1.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 12:04:21.715392 dia-adfpro-1.6.5/dia_adfpro.egg-info/
--rw-rw-rw-   0        0        0     1046 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 12:04:21.717398 dia-adfpro-1.6.5/diaadfpro/
--rw-rw-rw-   0        0        0      295 2023-05-30 12:03:55.000000 dia-adfpro-1.6.5/diaadfpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:04:21.910416 dia-adfpro-1.6.5/diaadfpro/adfpro/
--rw-rw-rw-   0        0        0      270 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/__init__.py
--rw-rw-rw-   0        0        0    10059 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/classify.py
--rw-rw-rw-   0        0        0    13958 2023-05-26 14:18:50.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/configuration.py
--rw-rw-rw-   0        0        0     3268 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/constants.py
--rw-rw-rw-   0        0        0     1334 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/explain.py
--rw-rw-rw-   0        0        0    31088 2023-05-30 11:55:47.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/feature_extract.py
--rw-rw-rw-   0        0        0    16597 2023-03-27 10:16:17.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/feature_extractors.py
--rw-rw-rw-   0        0        0    10096 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/golden.py
--rw-rw-rw-   0        0        0    14313 2023-04-28 12:40:42.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/model.py
--rw-rw-rw-   0        0        0     7455 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/offload.py
--rw-rw-rw-   0        0        0     7607 2023-04-28 12:40:42.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/train.py
--rw-rw-rw-   0        0        0    54884 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:04:22.055427 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/
--rw-rw-rw-   0        0        0      268 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/__init__.py
--rw-rw-rw-   0        0        0     4014 2023-05-30 12:03:46.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/constants.py
--rw-rw-rw-   0        0        0     6149 2022-08-02 08:08:38.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_anomaly_plots.py
--rw-rw-rw-   0        0        0    11741 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_app.py
--rw-rw-rw-   0        0        0    20412 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_components.py
--rw-rw-rw-   0        0        0     1167 2021-09-23 15:24:24.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_env_cfg.py
--rw-rw-rw-   0        0        0     1243 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_env_cfg.sample.py
--rw-rw-rw-   0        0        0     3677 2022-08-02 08:08:38.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_ohlc_plots.py
--rw-rw-rw-   0        0        0     6925 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_retrain.py
--rw-rw-rw-   0        0        0    10252 2022-08-02 08:08:38.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_summary_table.py
--rw-rw-rw-   0        0        0      115 2023-05-30 12:04:22.065421 dia-adfpro-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1239 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:40:13.541022 dia-adfpro-1.6.7/
+-rw-rw-rw-   0        0        0     1089 2023-05-18 08:28:18.000000 dia-adfpro-1.6.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       17 2023-05-18 08:28:18.000000 dia-adfpro-1.6.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1046 2023-06-30 07:40:13.542313 dia-adfpro-1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2021-02-11 11:49:55.000000 dia-adfpro-1.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 07:40:13.245991 dia-adfpro-1.6.7/dia_adfpro.egg-info/
+-rw-rw-rw-   0        0        0     1046 2023-06-30 07:40:12.000000 dia-adfpro-1.6.7/dia_adfpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-06-30 07:40:13.000000 dia-adfpro-1.6.7/dia_adfpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 07:40:12.000000 dia-adfpro-1.6.7/dia_adfpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 07:40:12.000000 dia-adfpro-1.6.7/dia_adfpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-30 07:40:12.000000 dia-adfpro-1.6.7/dia_adfpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 07:40:13.249991 dia-adfpro-1.6.7/diaadfpro/
+-rw-rw-rw-   0        0        0      295 2023-06-30 07:38:55.000000 dia-adfpro-1.6.7/diaadfpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:40:13.413988 dia-adfpro-1.6.7/diaadfpro/adfpro/
+-rw-rw-rw-   0        0        0      270 2022-08-01 06:46:08.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/__init__.py
+-rw-rw-rw-   0        0        0    10332 2023-06-30 07:38:36.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/classify.py
+-rw-rw-rw-   0        0        0    13958 2023-05-26 14:18:50.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/configuration.py
+-rw-rw-rw-   0        0        0     3268 2022-10-24 07:17:27.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/constants.py
+-rw-rw-rw-   0        0        0     1334 2022-08-01 06:46:08.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/explain.py
+-rw-rw-rw-   0        0        0    31088 2023-05-30 12:06:03.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/feature_extract.py
+-rw-rw-rw-   0        0        0    16597 2023-03-27 10:16:17.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/feature_extractors.py
+-rw-rw-rw-   0        0        0    10096 2022-08-01 06:46:08.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/golden.py
+-rw-rw-rw-   0        0        0    14313 2023-04-28 12:40:42.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/model.py
+-rw-rw-rw-   0        0        0     7455 2022-10-24 07:17:27.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/offload.py
+-rw-rw-rw-   0        0        0     7607 2023-04-28 12:40:42.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/train.py
+-rw-rw-rw-   0        0        0    54984 2023-06-30 07:38:36.000000 dia-adfpro-1.6.7/diaadfpro/adfpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:40:13.538995 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/
+-rw-rw-rw-   0        0        0      268 2022-08-01 06:46:08.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/__init__.py
+-rw-rw-rw-   0        0        0     4014 2023-06-30 07:38:55.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/constants.py
+-rw-rw-rw-   0        0        0     6149 2022-08-02 08:08:38.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_anomaly_plots.py
+-rw-rw-rw-   0        0        0    11741 2022-10-24 07:17:27.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_app.py
+-rw-rw-rw-   0        0        0    20412 2022-10-24 07:17:27.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_components.py
+-rw-rw-rw-   0        0        0     1167 2021-09-23 15:24:24.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_env_cfg.py
+-rw-rw-rw-   0        0        0     1243 2022-08-01 06:46:08.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_env_cfg.sample.py
+-rw-rw-rw-   0        0        0     3677 2022-08-02 08:08:38.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_ohlc_plots.py
+-rw-rw-rw-   0        0        0     6925 2022-10-24 07:17:27.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_retrain.py
+-rw-rw-rw-   0        0        0    10252 2022-08-02 08:08:38.000000 dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_summary_table.py
+-rw-rw-rw-   0        0        0      115 2023-06-30 07:40:13.544006 dia-adfpro-1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     1239 2023-05-18 08:28:18.000000 dia-adfpro-1.6.7/setup.py
```

### Comparing `dia-adfpro-1.6.5/LICENSE.txt` & `dia-adfpro-1.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/PKG-INFO` & `dia-adfpro-1.6.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dia-adfpro
-Version: 1.6.5
+Version: 1.6.7
 Summary: A Python application for anomaly detection
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_ADFPRO
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dia-adfpro-1.6.5/README.md` & `dia-adfpro-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/dia_adfpro.egg-info/PKG-INFO` & `dia-adfpro-1.6.7/dia_adfpro.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dia-adfpro
-Version: 1.6.5
+Version: 1.6.7
 Summary: A Python application for anomaly detection
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_ADFPRO
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dia-adfpro-1.6.5/dia_adfpro.egg-info/SOURCES.txt` & `dia-adfpro-1.6.7/dia_adfpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/classify.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/classify.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,27 +29,31 @@
     CLASSIFICATION_RESULT_WRITE_ERROR = 2
     COMPONENT_NOT_FOUND = 3
     UNSPECIFIED_ERROR = 1000
 
 
 class Classifier():
     @staticmethod
-    def build(modl_descriptor: ModelDescriptor, dbp, pwd, artifacts_path, cmp_descriptor_dct):
+    def build(modl_descriptor: ModelDescriptor, dbp, pwd, artifacts_path, cmp_descriptor_dct, send_notification_email = False):
         cls = Classifier()
         cls.__set_model_descriptor(modl_descriptor)
         cls.__set_db_params(dbp, pwd)
         cls.__set_artifacts_path(artifacts_path)
         cls.__set_classification_date(ADFPDateUtils.get_current_dt())
         cls.__set_cmp_descriptor_dictionary(cmp_descriptor_dct)
+        cls.__set_notification_email_enabled(send_notification_email)
         return cls
 
     def __init__(self):
         self.__diagnostics = DiagnosticsUtils()
         self.__exit_codes = []
 
+    def __set_notification_email_enabled(self, notif_email_enabled):
+        self.__notification_email_enabled = notif_email_enabled
+
     def __set_cmp_descriptor_dictionary(self, cmp_descriptor_dct):
         self.__cmp_descriptor_dct = cmp_descriptor_dct
 
     def __set_model_descriptor(self, modl_descriptor: ModelDescriptor):
         self.__model_descriptor = modl_descriptor
 
     def __set_db_params(self, dbp, pwd):
@@ -118,19 +122,19 @@
                                            error_msg=error_msg)
 
                 logger.error(">>>Error classifying equipment: {}".format(cmp_name))
                 logger.error(">>>{}".format(e))
                 self.__exit_codes.append(ClassifierExitCodes.UNSPECIFIED_ERROR)
 
         if self.__dbp[ADFPC.STR_WRITE_ENABLED]:
-            self.__diagnostics.notify(self.__dbp, self.__dbpwd)
-            logger.info("Error notification sent via email")
+            self.__diagnostics.notify(self.__dbp, self.__dbpwd, self.__notification_email_enabled)
+            logger.info("Notified errors (database/email)")
         else:
             logger.warning("Write to DB disabled")
-            logger.warning("Skipped writing diagnostics to DB and generating summary email")
+            logger.warning("Skipped writing diagnostics to DB and generating disgnostics")
 
     def classify_component(self, cmp: Component, cls_start=None, cls_end=None):
         if cmp is None:
             logger.error("Cannot classify null component")
             return
 
         logger.info("Classifying {}".format(cmp.name))
```

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/configuration.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/configuration.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/constants.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/constants.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/explain.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/explain.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/feature_extract.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/feature_extract.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/feature_extractors.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/golden.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/golden.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/model.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/model.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/offload.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/offload.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/train.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/train.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro/utils.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1040,15 +1040,15 @@
 
             logger.info("Appended to incidents_df")
             logger.info("Len of incidents_df = {}".format(len(self.__incidents_df)))
 
         except TypeError as e:
             logging.warning(str(e))
 
-    def notify(self, config_dict, dp_passw):
+    def notify(self, config_dict, dp_passw, notification_email_enabled = False):
         """
         Write incident logs to the database and creates email.html
         """
 
         table_name = config_dict[ADFPC.STR_DIAG_TABLE_NAME]
         user = config_dict[ADFPC.STR_USER]
         password = dp_passw
@@ -1058,20 +1058,21 @@
         ssl = config_dict[ADFPC.STR_SSL]
         ssl_cert = config_dict[ADFPC.STR_SSL_CERT_PATH]
 
         logger.info("Write diagnostics data to database ({})".format(table_name))
         IOUtils.write_results(df_results=self.__incidents_df, res_table_name=table_name,
                               user=user, passwd=password, host=host, port=port, db=database, ssl=ssl, ssl_cert=ssl_cert)
 
-        if len(self.__incidents_df) > 0:
-            payload = {"incidents_df": self.__incidents_df, "run_no": self.__run_no}
-            Notifier.incident_email(payload)
-        else:
-            payload = {"run_no": self.__run_no}
-            Notifier.no_incident_email(payload)
+        if notification_email_enabled:
+            if len(self.__incidents_df) > 0:
+                payload = {"incidents_df": self.__incidents_df, "run_no": self.__run_no}
+                Notifier.incident_email(payload)
+            else:
+                payload = {"run_no": self.__run_no}
+                Notifier.no_incident_email(payload)
 
 
 class ShiftHelper:
 
     def __init__(self, shifts_dct):
         assert (len(shifts_dct.keys()) == 3)
         self.__shifts_dct = shifts_dct
```

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/constants.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro_ui/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
             Manjunath C Bagewadi <bagewadi_manjunath_c@lilly.com>, 
             Henson Tauro <tauro_henson@lilly.com> 
             (MQ IDS - Data Integration and Analytics)
 License:    MIT
 """
 
 class ADFPCUI:
-    REPORT_VERSION = "1.6.5 (2023-05-30)"
+    REPORT_VERSION = "1.6.7 (2023-06-30)"
 
     #use for html id's
     ID_REFRESH = "btn-refresh"                                       #Refresh tab1
     ID_LATESTFETCH = "lbl-latestfetch"                               # latestfetch tab1
     ID_SUMMARY_TBL_CONTAINER = "div-summary-tbl-container"
     
     RETRAIN_YML = "/mnt/py/cfg.jobs/temp_retrain_job.yml"
```

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_anomaly_plots.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_anomaly_plots.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_app.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_app.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_components.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_components.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_env_cfg.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_env_cfg.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_env_cfg.sample.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_env_cfg.sample.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_ohlc_plots.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_ohlc_plots.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_retrain.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_retrain.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_summary_table.py` & `dia-adfpro-1.6.7/diaadfpro/adfpro_ui/ui_summary_table.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.5/setup.py` & `dia-adfpro-1.6.7/setup.py`

 * *Files identical despite different names*

