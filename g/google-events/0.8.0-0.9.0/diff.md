# Comparing `tmp/google-events-0.8.0.tar.gz` & `tmp/google-events-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-events-0.8.0.tar", last modified: Tue Jun 27 19:41:27 2023, max compression
+gzip compressed data, was "google-events-0.9.0.tar", last modified: Thu Jun 29 22:32:57 2023, max compression
```

## Comparing `google-events-0.8.0.tar` & `google-events-0.9.0.tar`

### file list

```diff
@@ -1,487 +1,487 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.602782 google-events-0.8.0/
--rw-rw-r--   0 root         (0)     1003    11357 2023-06-27 19:38:25.000000 google-events-0.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-27 19:38:25.000000 google-events-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     1811 2023-06-27 19:41:27.602782 google-events-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003      893 2023-06-27 19:38:25.000000 google-events-0.8.0/README.md
--rw-rw-r--   0 root         (0)     1003       94 2023-06-27 19:38:25.000000 google-events-0.8.0/pyproject.toml
--rw-rw-r--   0 root         (0)     1003     1040 2023-06-27 19:41:27.602782 google-events-0.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003       70 2023-06-27 19:38:25.000000 google-events-0.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.542774 google-events-0.8.0/src/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.526772 google-events-0.8.0/src/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.542774 google-events-0.8.0/src/google/events/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.542774 google-events-0.8.0/src/google/events/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.546774 google-events-0.8.0/src/google/events/cloud/alloydb/
--rw-rw-r--   0 root         (0)     1003     1977 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/alloydb/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/alloydb/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.546774 google-events-0.8.0/src/google/events/cloud/alloydb_v1/
--rw-rw-r--   0 root         (0)     1003     1509 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/alloydb_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/alloydb_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.546774 google-events-0.8.0/src/google/events/cloud/alloydb_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/alloydb_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.546774 google-events-0.8.0/src/google/events/cloud/alloydb_v1/types/
--rw-rw-r--   0 root         (0)     1003     1199 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/alloydb_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    50757 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/alloydb_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.546774 google-events-0.8.0/src/google/events/cloud/apigateway/
--rw-rw-r--   0 root         (0)     1003     1258 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigateway/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigateway/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.546774 google-events-0.8.0/src/google/events/cloud/apigateway_v1/
--rw-rw-r--   0 root         (0)     1003     1044 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigateway_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigateway_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.546774 google-events-0.8.0/src/google/events/cloud/apigateway_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigateway_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.546774 google-events-0.8.0/src/google/events/cloud/apigateway_v1/types/
--rw-rw-r--   0 root         (0)     1003      851 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigateway_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    15346 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigateway_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.546774 google-events-0.8.0/src/google/events/cloud/apigeeregistry/
--rw-rw-r--   0 root         (0)     1003     1690 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigeeregistry/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigeeregistry/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/
--rw-rw-r--   0 root         (0)     1003     1288 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/types/
--rw-rw-r--   0 root         (0)     1003     1031 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    24076 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/audit/
--rw-rw-r--   0 root         (0)     1003     1637 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/audit/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/audit/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/audit_v1/
--rw-rw-r--   0 root         (0)     1003     1325 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/audit_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/audit_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/audit_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/audit_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/audit_v1/types/
--rw-rw-r--   0 root         (0)     1003     1077 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/audit_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    26222 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/audit_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.530772 google-events-0.8.0/src/google/events/cloud/beyondcorp/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections/
--rw-rw-r--   0 root         (0)     1003      979 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/
--rw-rw-r--   0 root         (0)     1003      883 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/
--rw-rw-r--   0 root         (0)     1003      735 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     8799 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.550775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors/
--rw-rw-r--   0 root         (0)     1003     1180 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/
--rw-rw-r--   0 root         (0)     1003      984 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/
--rw-rw-r--   0 root         (0)     1003      807 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     8405 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways/
--rw-rw-r--   0 root         (0)     1003      958 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/
--rw-rw-r--   0 root         (0)     1003      868 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/
--rw-rw-r--   0 root         (0)     1003      723 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7047 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices/
--rw-rw-r--   0 root         (0)     1003     1042 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/
--rw-rw-r--   0 root         (0)     1003      928 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/
--rw-rw-r--   0 root         (0)     1003      771 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     9372 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.554775 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways/
--rw-rw-r--   0 root         (0)     1003      979 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/
--rw-rw-r--   0 root         (0)     1003      883 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/
--rw-rw-r--   0 root         (0)     1003      735 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4243 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/certificatemanager/
--rw-rw-r--   0 root         (0)     1003     2008 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/certificatemanager/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/certificatemanager/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/
--rw-rw-r--   0 root         (0)     1003     1521 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/types/
--rw-rw-r--   0 root         (0)     1003     1245 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    35465 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/cloudbuild/
--rw-rw-r--   0 root         (0)     1003     2002 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/cloudbuild/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/cloudbuild/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/
--rw-rw-r--   0 root         (0)     1003     1455 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/types/
--rw-rw-r--   0 root         (0)     1003     1127 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    38251 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.558776 google-events-0.8.0/src/google/events/cloud/clouddms/
--rw-rw-r--   0 root         (0)     1003     2732 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/clouddms/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/clouddms/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/clouddms_v1/
--rw-rw-r--   0 root         (0)     1003     2040 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/clouddms_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/clouddms_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/clouddms_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/clouddms_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/clouddms_v1/types/
--rw-rw-r--   0 root         (0)     1003     1639 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/clouddms_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    45706 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/clouddms_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/dataflow/
--rw-rw-r--   0 root         (0)     1003     3397 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataflow/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataflow/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/
--rw-rw-r--   0 root         (0)     1003     2330 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/types/
--rw-rw-r--   0 root         (0)     1003     1819 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    46656 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/datafusion/
--rw-rw-r--   0 root         (0)     1003     1562 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datafusion/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datafusion/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/datafusion_v1/
--rw-rw-r--   0 root         (0)     1003     1237 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datafusion_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datafusion_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/datafusion_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datafusion_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/datafusion_v1/types/
--rw-rw-r--   0 root         (0)     1003      999 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datafusion_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    20801 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datafusion_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/dataplex/
--rw-rw-r--   0 root         (0)     1003     3826 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataplex/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataplex/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.562776 google-events-0.8.0/src/google/events/cloud/dataplex_v1/
--rw-rw-r--   0 root         (0)     1003     2644 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataplex_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataplex_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/dataplex_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataplex_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/dataplex_v1/types/
--rw-rw-r--   0 root         (0)     1003     2033 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataplex_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003   134352 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/dataplex_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/datastore/
--rw-rw-r--   0 root         (0)     1003     1399 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastore/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastore/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/datastore_v1/
--rw-rw-r--   0 root         (0)     1003     1119 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastore_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/datastore_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastore_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/datastore_v1/types/
--rw-rw-r--   0 root         (0)     1003      897 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastore_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    17836 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastore_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/datastream/
--rw-rw-r--   0 root         (0)     1003     4598 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastream/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastream/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/datastream_v1/
--rw-rw-r--   0 root         (0)     1003     3126 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastream_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastream_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/datastream_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastream_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/datastream_v1/types/
--rw-rw-r--   0 root         (0)     1003     2423 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastream_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    52030 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/datastream_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.566777 google-events-0.8.0/src/google/events/cloud/eventarc/
--rw-rw-r--   0 root         (0)     1003     1864 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/eventarc/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/eventarc/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/eventarc_v1/
--rw-rw-r--   0 root         (0)     1003     1417 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/eventarc_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/eventarc_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/eventarc_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/eventarc_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/eventarc_v1/types/
--rw-rw-r--   0 root         (0)     1003     1121 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/eventarc_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    21783 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/eventarc_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/firestore/
--rw-rw-r--   0 root         (0)     1003     1241 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/firestore/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/firestore/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/firestore_v1/
--rw-rw-r--   0 root         (0)     1003     1033 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/firestore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/firestore_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/firestore_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/firestore_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/firestore_v1/types/
--rw-rw-r--   0 root         (0)     1003      841 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/firestore_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10821 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/firestore_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/functions/
--rw-rw-r--   0 root         (0)     1003     1969 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/functions/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/functions/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/functions_v2/
--rw-rw-r--   0 root         (0)     1003     1473 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/functions_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/functions_v2/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/functions_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/functions_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/functions_v2/types/
--rw-rw-r--   0 root         (0)     1003     1161 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/functions_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    36858 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/functions_v2/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.570777 google-events-0.8.0/src/google/events/cloud/gkebackup/
--rw-rw-r--   0 root         (0)     1003     1914 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkebackup/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkebackup/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/gkebackup_v1/
--rw-rw-r--   0 root         (0)     1003     1454 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkebackup_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkebackup_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/gkebackup_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkebackup_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/gkebackup_v1/types/
--rw-rw-r--   0 root         (0)     1003     1157 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkebackup_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    54614 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkebackup_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/gkehub/
--rw-rw-r--   0 root         (0)     1003     3260 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkehub/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkehub/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/gkehub_v1/
--rw-rw-r--   0 root         (0)     1003     2377 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkehub_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkehub_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/gkehub_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkehub_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/gkehub_v1/types/
--rw-rw-r--   0 root         (0)     1003     1873 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkehub_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    42166 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/gkehub_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/iot/
--rw-rw-r--   0 root         (0)     1003     2770 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/iot/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/iot/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/iot_v1/
--rw-rw-r--   0 root         (0)     1003     2088 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/iot_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/iot_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/iot_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/iot_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/iot_v1/types/
--rw-rw-r--   0 root         (0)     1003     1647 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/iot_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    31987 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/iot_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.574778 google-events-0.8.0/src/google/events/cloud/memcache/
--rw-rw-r--   0 root         (0)     1003     1412 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/memcache/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/memcache/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/memcache_v1/
--rw-rw-r--   0 root         (0)     1003     1175 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/memcache_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/memcache_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/memcache_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/memcache_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/memcache_v1/types/
--rw-rw-r--   0 root         (0)     1003      969 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/memcache_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    17718 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/memcache_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/metastore/
--rw-rw-r--   0 root         (0)     1003     2809 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/metastore/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/metastore/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/metastore_v1/
--rw-rw-r--   0 root         (0)     1003     2025 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/metastore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/metastore_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/metastore_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/metastore_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/metastore_v1/types/
--rw-rw-r--   0 root         (0)     1003     1593 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/metastore_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    44965 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/metastore_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/networkconnectivity/
--rw-rw-r--   0 root         (0)     1003     2981 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkconnectivity/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkconnectivity/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/
--rw-rw-r--   0 root         (0)     1003     2069 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/types/
--rw-rw-r--   0 root         (0)     1003     1657 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    40382 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.578778 google-events-0.8.0/src/google/events/cloud/networkmanagement/
--rw-rw-r--   0 root         (0)     1003     3460 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkmanagement/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkmanagement/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/
--rw-rw-r--   0 root         (0)     1003     2280 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/types/
--rw-rw-r--   0 root         (0)     1003     1765 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    83302 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/notebooks/
--rw-rw-r--   0 root         (0)     1003     3049 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/notebooks/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/notebooks/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/notebooks_v1/
--rw-rw-r--   0 root         (0)     1003     2193 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/notebooks_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/notebooks_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/notebooks_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/notebooks_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/notebooks_v1/types/
--rw-rw-r--   0 root         (0)     1003     1731 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/notebooks_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    92217 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/notebooks_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/pubsub/
--rw-rw-r--   0 root         (0)     1003      918 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/pubsub/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/pubsub/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/pubsub_v1/
--rw-rw-r--   0 root         (0)     1003      860 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/pubsub_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/pubsub_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/pubsub_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/pubsub_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/pubsub_v1/types/
--rw-rw-r--   0 root         (0)     1003      731 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/pubsub_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2943 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/pubsub_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.582779 google-events-0.8.0/src/google/events/cloud/redis/
--rw-rw-r--   0 root         (0)     1003     1461 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/redis/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/redis/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/redis_v1/
--rw-rw-r--   0 root         (0)     1003     1213 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/redis_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/redis_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/redis_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/redis_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/redis_v1/types/
--rw-rw-r--   0 root         (0)     1003      995 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/redis_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    27814 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/redis_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/scheduler/
--rw-rw-r--   0 root         (0)     1003      828 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/scheduler/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/scheduler/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/scheduler_v1/
--rw-rw-r--   0 root         (0)     1003      800 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/scheduler_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/scheduler_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/scheduler_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/scheduler_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/scheduler_v1/types/
--rw-rw-r--   0 root         (0)     1003      683 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/scheduler_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1199 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/scheduler_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/storage/
--rw-rw-r--   0 root         (0)     1003      826 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/storage/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/storage/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/storage_v1/
--rw-rw-r--   0 root         (0)     1003      800 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/storage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/storage_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/storage_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/storage_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/storage_v1/types/
--rw-rw-r--   0 root         (0)     1003      685 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/storage_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     9246 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/storage_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.538773 google-events-0.8.0/src/google/events/cloud/video/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/video/transcoder/
--rw-rw-r--   0 root         (0)     1003     2608 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/video/transcoder/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/video/transcoder/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.586779 google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/
--rw-rw-r--   0 root         (0)     1003     1756 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/types/
--rw-rw-r--   0 root         (0)     1003     1347 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    81133 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/visionai/
--rw-rw-r--   0 root         (0)     1003     5786 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/visionai/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/visionai/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/visionai_v1/
--rw-rw-r--   0 root         (0)     1003     3939 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/visionai_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/visionai_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/visionai_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/visionai_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/visionai_v1/types/
--rw-rw-r--   0 root         (0)     1003     3043 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/visionai_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    92567 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/visionai_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/vmmigration/
--rw-rw-r--   0 root         (0)     1003     5696 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/vmmigration/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/vmmigration/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/vmmigration_v1/
--rw-rw-r--   0 root         (0)     1003     3842 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/vmmigration_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/vmmigration_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/vmmigration_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/vmmigration_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/vmmigration_v1/types/
--rw-rw-r--   0 root         (0)     1003     3003 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/vmmigration_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    88598 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/vmmigration_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.590780 google-events-0.8.0/src/google/events/cloud/workflows/
--rw-rw-r--   0 root         (0)     1003      911 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/workflows/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/workflows/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/cloud/workflows_v1/
--rw-rw-r--   0 root         (0)     1003      847 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/workflows_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/workflows_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/cloud/workflows_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/workflows_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/cloud/workflows_v1/types/
--rw-rw-r--   0 root         (0)     1003      715 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/workflows_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6226 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/cloud/workflows_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.542774 google-events-0.8.0/src/google/events/firebase/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/analytics/
--rw-rw-r--   0 root         (0)     1003     1754 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/analytics/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/analytics/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/analytics_v1/
--rw-rw-r--   0 root         (0)     1003     1333 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/analytics_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/analytics_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/analytics_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/analytics_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/analytics_v1/types/
--rw-rw-r--   0 root         (0)     1003     1063 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/analytics_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    14151 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/analytics_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/auth/
--rw-rw-r--   0 root         (0)     1003      984 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/auth/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/auth/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/auth_v1/
--rw-rw-r--   0 root         (0)     1003      890 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/auth_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/auth_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/auth_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/auth_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/auth_v1/types/
--rw-rw-r--   0 root         (0)     1003      745 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/auth_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4622 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/auth_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/database/
--rw-rw-r--   0 root         (0)     1003      836 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/database/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/database/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.594781 google-events-0.8.0/src/google/events/firebase/database_v1/
--rw-rw-r--   0 root         (0)     1003      806 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/database_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/database_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/database_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/database_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/database_v1/types/
--rw-rw-r--   0 root         (0)     1003      687 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/database_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1545 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/database_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/firebasealerts/
--rw-rw-r--   0 root         (0)     1003      830 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/firebasealerts/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/firebasealerts/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/
--rw-rw-r--   0 root         (0)     1003      794 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/types/
--rw-rw-r--   0 root         (0)     1003      669 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2025 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/remoteconfig/
--rw-rw-r--   0 root         (0)     1003     1187 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/remoteconfig/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/remoteconfig/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/
--rw-rw-r--   0 root         (0)     1003     1027 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/types/
--rw-rw-r--   0 root         (0)     1003      859 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5002 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/testlab/
--rw-rw-r--   0 root         (0)     1003     1192 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/testlab/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/testlab/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/testlab_v1/
--rw-rw-r--   0 root         (0)     1003     1015 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/testlab_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/testlab_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.598781 google-events-0.8.0/src/google/events/firebase/testlab_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/testlab_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.602782 google-events-0.8.0/src/google/events/firebase/testlab_v1/types/
--rw-rw-r--   0 root         (0)     1003      837 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/testlab_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6673 2023-06-27 19:38:25.000000 google-events-0.8.0/src/google/events/firebase/testlab_v1/types/data.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.602782 google-events-0.8.0/src/google_events.egg-info/
--rw-r--r--   0 root         (0)     1003     1811 2023-06-27 19:41:27.000000 google-events-0.8.0/src/google_events.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    16482 2023-06-27 19:41:27.000000 google-events-0.8.0/src/google_events.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-27 19:41:27.000000 google-events-0.8.0/src/google_events.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       36 2023-06-27 19:41:27.000000 google-events-0.8.0/src/google_events.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-27 19:41:27.000000 google-events-0.8.0/src/google_events.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-27 19:41:27.602782 google-events-0.8.0/tests/
--rw-rw-r--   0 root         (0)     1003       14 2023-06-27 19:38:25.000000 google-events-0.8.0/tests/requirements.txt
--rw-rw-r--   0 root         (0)     1003     6107 2023-06-27 19:38:25.000000 google-events-0.8.0/tests/test_cloudevents_data_parsing.py
--rw-rw-r--   0 root         (0)     1003     1094 2023-06-27 19:38:25.000000 google-events-0.8.0/tests/util.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.093005 google-events-0.9.0/
+-rw-rw-r--   0 root         (0)     1003    11357 2023-06-29 22:29:55.000000 google-events-0.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-29 22:29:55.000000 google-events-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     1811 2023-06-29 22:32:57.093005 google-events-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003      893 2023-06-29 22:29:55.000000 google-events-0.9.0/README.md
+-rw-rw-r--   0 root         (0)     1003       94 2023-06-29 22:29:55.000000 google-events-0.9.0/pyproject.toml
+-rw-rw-r--   0 root         (0)     1003     1040 2023-06-29 22:32:57.093005 google-events-0.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003       70 2023-06-29 22:29:55.000000 google-events-0.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.028999 google-events-0.9.0/src/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.008998 google-events-0.9.0/src/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.024999 google-events-0.9.0/src/google/events/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.024999 google-events-0.9.0/src/google/events/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.028999 google-events-0.9.0/src/google/events/cloud/alloydb/
+-rw-rw-r--   0 root         (0)     1003     1977 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/alloydb/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/alloydb/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.028999 google-events-0.9.0/src/google/events/cloud/alloydb_v1/
+-rw-rw-r--   0 root         (0)     1003     1509 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/alloydb_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/alloydb_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.028999 google-events-0.9.0/src/google/events/cloud/alloydb_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/alloydb_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.028999 google-events-0.9.0/src/google/events/cloud/alloydb_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1199 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/alloydb_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    50757 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/alloydb_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/apigateway/
+-rw-rw-r--   0 root         (0)     1003     1258 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigateway/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigateway/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/apigateway_v1/
+-rw-rw-r--   0 root         (0)     1003     1044 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigateway_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigateway_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/apigateway_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigateway_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/apigateway_v1/types/
+-rw-rw-r--   0 root         (0)     1003      851 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigateway_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15346 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigateway_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/apigeeregistry/
+-rw-rw-r--   0 root         (0)     1003     1690 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigeeregistry/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigeeregistry/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/
+-rw-rw-r--   0 root         (0)     1003     1288 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1031 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24076 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/audit/
+-rw-rw-r--   0 root         (0)     1003     1637 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/audit/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/audit/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.033000 google-events-0.9.0/src/google/events/cloud/audit_v1/
+-rw-rw-r--   0 root         (0)     1003     1325 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/audit_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/audit_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/audit_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/audit_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/audit_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1077 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/audit_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26222 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/audit_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.012998 google-events-0.9.0/src/google/events/cloud/beyondcorp/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections/
+-rw-rw-r--   0 root         (0)     1003      979 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/
+-rw-rw-r--   0 root         (0)     1003      883 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/
+-rw-rw-r--   0 root         (0)     1003      735 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8799 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors/
+-rw-rw-r--   0 root         (0)     1003     1180 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/
+-rw-rw-r--   0 root         (0)     1003      984 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/
+-rw-rw-r--   0 root         (0)     1003      807 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8405 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.037000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways/
+-rw-rw-r--   0 root         (0)     1003      958 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/
+-rw-rw-r--   0 root         (0)     1003      868 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/
+-rw-rw-r--   0 root         (0)     1003      723 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7047 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices/
+-rw-rw-r--   0 root         (0)     1003     1042 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/
+-rw-rw-r--   0 root         (0)     1003      928 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/
+-rw-rw-r--   0 root         (0)     1003      771 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9372 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways/
+-rw-rw-r--   0 root         (0)     1003      979 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/
+-rw-rw-r--   0 root         (0)     1003      883 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.041000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/
+-rw-rw-r--   0 root         (0)     1003      735 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4243 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/certificatemanager/
+-rw-rw-r--   0 root         (0)     1003     2008 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/certificatemanager/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/certificatemanager/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/
+-rw-rw-r--   0 root         (0)     1003     1521 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1245 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35465 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/cloudbuild/
+-rw-rw-r--   0 root         (0)     1003     2002 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/cloudbuild/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/cloudbuild/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/
+-rw-rw-r--   0 root         (0)     1003     1455 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1127 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38251 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/clouddms/
+-rw-rw-r--   0 root         (0)     1003     2732 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/clouddms/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/clouddms/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.045001 google-events-0.9.0/src/google/events/cloud/clouddms_v1/
+-rw-rw-r--   0 root         (0)     1003     2040 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/clouddms_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/clouddms_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/clouddms_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/clouddms_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/clouddms_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1639 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/clouddms_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    45706 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/clouddms_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/dataflow/
+-rw-rw-r--   0 root         (0)     1003     3397 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataflow/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataflow/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/
+-rw-rw-r--   0 root         (0)     1003     2330 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/types/
+-rw-rw-r--   0 root         (0)     1003     1819 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46656 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/datafusion/
+-rw-rw-r--   0 root         (0)     1003     1562 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datafusion/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datafusion/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/datafusion_v1/
+-rw-rw-r--   0 root         (0)     1003     1237 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datafusion_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datafusion_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/datafusion_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datafusion_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/datafusion_v1/types/
+-rw-rw-r--   0 root         (0)     1003      999 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datafusion_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20801 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datafusion_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.049001 google-events-0.9.0/src/google/events/cloud/dataplex/
+-rw-rw-r--   0 root         (0)     1003     3826 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataplex/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataplex/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/dataplex_v1/
+-rw-rw-r--   0 root         (0)     1003     2644 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataplex_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataplex_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/dataplex_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataplex_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/dataplex_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2033 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataplex_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003   134352 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/dataplex_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/datastore/
+-rw-rw-r--   0 root         (0)     1003     1399 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastore/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastore/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/datastore_v1/
+-rw-rw-r--   0 root         (0)     1003     1119 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastore_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/datastore_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastore_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/datastore_v1/types/
+-rw-rw-r--   0 root         (0)     1003      897 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastore_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17836 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastore_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/datastream/
+-rw-rw-r--   0 root         (0)     1003     4598 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastream/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastream/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/datastream_v1/
+-rw-rw-r--   0 root         (0)     1003     3126 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastream_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastream_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.053001 google-events-0.9.0/src/google/events/cloud/datastream_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastream_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/datastream_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2423 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastream_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    52030 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/datastream_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/eventarc/
+-rw-rw-r--   0 root         (0)     1003     1864 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/eventarc/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/eventarc/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/eventarc_v1/
+-rw-rw-r--   0 root         (0)     1003     1417 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/eventarc_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/eventarc_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/eventarc_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/eventarc_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/eventarc_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1121 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/eventarc_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21783 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/eventarc_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/firestore/
+-rw-rw-r--   0 root         (0)     1003     1241 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/firestore/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/firestore/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/firestore_v1/
+-rw-rw-r--   0 root         (0)     1003     1033 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/firestore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/firestore_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/firestore_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/firestore_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/firestore_v1/types/
+-rw-rw-r--   0 root         (0)     1003      841 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/firestore_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10821 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/firestore_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/functions/
+-rw-rw-r--   0 root         (0)     1003     1969 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/functions/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/functions/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.057002 google-events-0.9.0/src/google/events/cloud/functions_v2/
+-rw-rw-r--   0 root         (0)     1003     1473 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/functions_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/functions_v2/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/functions_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/functions_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/functions_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1161 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/functions_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    36858 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/functions_v2/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/gkebackup/
+-rw-rw-r--   0 root         (0)     1003     1914 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkebackup/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkebackup/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/gkebackup_v1/
+-rw-rw-r--   0 root         (0)     1003     1454 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkebackup_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkebackup_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/gkebackup_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkebackup_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/gkebackup_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1157 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkebackup_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54614 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkebackup_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/gkehub/
+-rw-rw-r--   0 root         (0)     1003     3260 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkehub/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkehub/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/gkehub_v1/
+-rw-rw-r--   0 root         (0)     1003     2377 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkehub_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkehub_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/gkehub_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkehub_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.061002 google-events-0.9.0/src/google/events/cloud/gkehub_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1873 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkehub_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    42166 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/gkehub_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/iot/
+-rw-rw-r--   0 root         (0)     1003     2770 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/iot/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/iot/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/iot_v1/
+-rw-rw-r--   0 root         (0)     1003     2088 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/iot_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/iot_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/iot_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/iot_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1647 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/iot_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    31987 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/iot_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/memcache/
+-rw-rw-r--   0 root         (0)     1003     1412 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/memcache/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/memcache/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/memcache_v1/
+-rw-rw-r--   0 root         (0)     1003     1175 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/memcache_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/memcache_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/memcache_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/memcache_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/memcache_v1/types/
+-rw-rw-r--   0 root         (0)     1003      969 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/memcache_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17718 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/memcache_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/metastore/
+-rw-rw-r--   0 root         (0)     1003     2809 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/metastore/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/metastore/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/metastore_v1/
+-rw-rw-r--   0 root         (0)     1003     2025 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/metastore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/metastore_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/metastore_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/metastore_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.065002 google-events-0.9.0/src/google/events/cloud/metastore_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1593 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/metastore_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    44965 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/metastore_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/networkconnectivity/
+-rw-rw-r--   0 root         (0)     1003     2981 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkconnectivity/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkconnectivity/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/
+-rw-rw-r--   0 root         (0)     1003     2069 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1657 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    40382 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/networkmanagement/
+-rw-rw-r--   0 root         (0)     1003     3460 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkmanagement/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkmanagement/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/
+-rw-rw-r--   0 root         (0)     1003     2280 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1765 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83302 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/notebooks/
+-rw-rw-r--   0 root         (0)     1003     3049 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/notebooks/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/notebooks/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.069003 google-events-0.9.0/src/google/events/cloud/notebooks_v1/
+-rw-rw-r--   0 root         (0)     1003     2193 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/notebooks_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/notebooks_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/notebooks_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/notebooks_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/notebooks_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1731 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/notebooks_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    92217 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/notebooks_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/pubsub/
+-rw-rw-r--   0 root         (0)     1003      918 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/pubsub/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/pubsub/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/pubsub_v1/
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/pubsub_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/pubsub_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/pubsub_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/pubsub_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/pubsub_v1/types/
+-rw-rw-r--   0 root         (0)     1003      731 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/pubsub_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2943 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/pubsub_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/redis/
+-rw-rw-r--   0 root         (0)     1003     1461 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/redis/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/redis/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/redis_v1/
+-rw-rw-r--   0 root         (0)     1003     1213 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/redis_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/redis_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/redis_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/redis_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/redis_v1/types/
+-rw-rw-r--   0 root         (0)     1003      995 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/redis_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27814 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/redis_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.073003 google-events-0.9.0/src/google/events/cloud/scheduler/
+-rw-rw-r--   0 root         (0)     1003      828 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/scheduler/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/scheduler/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/scheduler_v1/
+-rw-rw-r--   0 root         (0)     1003      800 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/scheduler_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/scheduler_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/scheduler_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/scheduler_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/scheduler_v1/types/
+-rw-rw-r--   0 root         (0)     1003      683 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/scheduler_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1199 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/scheduler_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/storage/
+-rw-rw-r--   0 root         (0)     1003      826 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/storage/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/storage/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/storage_v1/
+-rw-rw-r--   0 root         (0)     1003      800 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/storage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/storage_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/storage_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/storage_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/storage_v1/types/
+-rw-rw-r--   0 root         (0)     1003      685 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/storage_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9246 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/storage_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.020999 google-events-0.9.0/src/google/events/cloud/video/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/video/transcoder/
+-rw-rw-r--   0 root         (0)     1003     2608 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/video/transcoder/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/video/transcoder/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/
+-rw-rw-r--   0 root         (0)     1003     1756 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.077003 google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1347 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    81133 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/visionai/
+-rw-rw-r--   0 root         (0)     1003     5786 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/visionai/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/visionai/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/visionai_v1/
+-rw-rw-r--   0 root         (0)     1003     3939 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/visionai_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/visionai_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/visionai_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/visionai_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/visionai_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3043 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/visionai_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    92567 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/visionai_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/vmmigration/
+-rw-rw-r--   0 root         (0)     1003     5696 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/vmmigration/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/vmmigration/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/vmmigration_v1/
+-rw-rw-r--   0 root         (0)     1003     3842 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/vmmigration_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/vmmigration_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/vmmigration_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/vmmigration_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/vmmigration_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3003 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/vmmigration_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    88598 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/vmmigration_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/workflows/
+-rw-rw-r--   0 root         (0)     1003      911 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/workflows/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/workflows/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/workflows_v1/
+-rw-rw-r--   0 root         (0)     1003      847 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/workflows_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/workflows_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.081004 google-events-0.9.0/src/google/events/cloud/workflows_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/workflows_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/cloud/workflows_v1/types/
+-rw-rw-r--   0 root         (0)     1003      715 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/workflows_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6226 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/cloud/workflows_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.028999 google-events-0.9.0/src/google/events/firebase/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/firebase/analytics/
+-rw-rw-r--   0 root         (0)     1003     1754 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/analytics/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/analytics/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/firebase/analytics_v1/
+-rw-rw-r--   0 root         (0)     1003     1333 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/analytics_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/analytics_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/firebase/analytics_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/analytics_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/firebase/analytics_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1063 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/analytics_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14151 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/analytics_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/firebase/auth/
+-rw-rw-r--   0 root         (0)     1003      984 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/auth/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/auth/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/firebase/auth_v1/
+-rw-rw-r--   0 root         (0)     1003      890 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/auth_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/auth_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/firebase/auth_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/auth_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/firebase/auth_v1/types/
+-rw-rw-r--   0 root         (0)     1003      745 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/auth_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4622 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/auth_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.085004 google-events-0.9.0/src/google/events/firebase/database/
+-rw-rw-r--   0 root         (0)     1003      836 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/database/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/database/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/database_v1/
+-rw-rw-r--   0 root         (0)     1003      806 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/database_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/database_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/database_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/database_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/database_v1/types/
+-rw-rw-r--   0 root         (0)     1003      687 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/database_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1545 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/database_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/firebasealerts/
+-rw-rw-r--   0 root         (0)     1003      830 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/firebasealerts/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/firebasealerts/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/
+-rw-rw-r--   0 root         (0)     1003      794 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/types/
+-rw-rw-r--   0 root         (0)     1003      669 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2025 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/remoteconfig/
+-rw-rw-r--   0 root         (0)     1003     1187 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/remoteconfig/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/remoteconfig/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/
+-rw-rw-r--   0 root         (0)     1003     1027 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/types/
+-rw-rw-r--   0 root         (0)     1003      859 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5002 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.089004 google-events-0.9.0/src/google/events/firebase/testlab/
+-rw-rw-r--   0 root         (0)     1003     1192 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/testlab/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/testlab/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.093005 google-events-0.9.0/src/google/events/firebase/testlab_v1/
+-rw-rw-r--   0 root         (0)     1003     1015 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/testlab_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/testlab_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.093005 google-events-0.9.0/src/google/events/firebase/testlab_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/testlab_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.093005 google-events-0.9.0/src/google/events/firebase/testlab_v1/types/
+-rw-rw-r--   0 root         (0)     1003      837 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/testlab_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6673 2023-06-29 22:29:55.000000 google-events-0.9.0/src/google/events/firebase/testlab_v1/types/data.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.093005 google-events-0.9.0/src/google_events.egg-info/
+-rw-r--r--   0 root         (0)     1003     1811 2023-06-29 22:32:56.000000 google-events-0.9.0/src/google_events.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    16482 2023-06-29 22:32:56.000000 google-events-0.9.0/src/google_events.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-29 22:32:56.000000 google-events-0.9.0/src/google_events.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       36 2023-06-29 22:32:56.000000 google-events-0.9.0/src/google_events.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-29 22:32:56.000000 google-events-0.9.0/src/google_events.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 22:32:57.093005 google-events-0.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003       14 2023-06-29 22:29:55.000000 google-events-0.9.0/tests/requirements.txt
+-rw-rw-r--   0 root         (0)     1003     6107 2023-06-29 22:29:55.000000 google-events-0.9.0/tests/test_cloudevents_data_parsing.py
+-rw-rw-r--   0 root         (0)     1003     1094 2023-06-29 22:29:55.000000 google-events-0.9.0/tests/util.py
```

### Comparing `google-events-0.8.0/LICENSE` & `google-events-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/MANIFEST.in` & `google-events-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/PKG-INFO` & `google-events-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-events
-Version: 0.8.0
+Version: 0.9.0
 Summary: Google Cloudevents library
 Home-page: https://github.com/googleapis/google-cloudevents-python/
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache License 2.0
 Platform: Posix
 Platform: MacOS X
```

### Comparing `google-events-0.8.0/README.md` & `google-events-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/setup.cfg` & `google-events-0.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = google-events
-version = 0.8.0
+version = 0.9.0
 author = Google LLC
 author_email = googleapis-packages@google.com
 description = Google Cloudevents library
 long_description = file: README.md
 long_description_content_type = text/markdown
 home-page = https://github.com/googleapis/google-cloudevents-python/
 license = Apache License 2.0
```

### Comparing `google-events-0.8.0/src/google/events/cloud/alloydb/__init__.py` & `google-events-0.9.0/src/google/events/cloud/alloydb/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/alloydb/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/alloydb/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/alloydb_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/alloydb_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/alloydb_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/alloydb_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/alloydb_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/alloydb_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/alloydb_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/alloydb_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/alloydb_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/alloydb_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigateway/__init__.py` & `google-events-0.9.0/src/google/events/cloud/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigateway/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/apigateway/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/apigateway_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/apigateway_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigateway_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/apigateway_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/apigateway_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/apigateway_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigateway_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/apigateway_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigateway_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/apigateway_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigeeregistry/__init__.py` & `google-events-0.9.0/src/google/events/cloud/apigeeregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigeeregistry/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/apigeeregistry/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/apigeeregistry_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/apigeeregistry_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/audit/__init__.py` & `google-events-0.9.0/src/google/events/cloud/audit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/audit/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/audit/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/audit_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/audit_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/audit_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/audit_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/audit_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/audit_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/audit_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/audit_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/audit_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/audit_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnections_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appconnectors_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/appgateways_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientconnectorservices_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/beyondcorp/clientgateways_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/certificatemanager/__init__.py` & `google-events-0.9.0/src/google/events/cloud/certificatemanager/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/certificatemanager/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/certificatemanager/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/certificatemanager_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/certificatemanager_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/cloudbuild/__init__.py` & `google-events-0.9.0/src/google/events/cloud/cloudbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/cloudbuild/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/cloudbuild/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/cloudbuild_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/cloudbuild_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/clouddms/__init__.py` & `google-events-0.9.0/src/google/events/cloud/clouddms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/clouddms/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/clouddms/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/clouddms_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/clouddms_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/clouddms_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/clouddms_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/clouddms_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/clouddms_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/clouddms_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/clouddms_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/clouddms_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/clouddms_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataflow/__init__.py` & `google-events-0.9.0/src/google/events/cloud/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataflow/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/dataflow/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/__init__.py` & `google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataflow_v1beta3/types/data.py` & `google-events-0.9.0/src/google/events/cloud/dataflow_v1beta3/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datafusion/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datafusion/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/datafusion/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/datafusion_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datafusion_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datafusion_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/datafusion_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/datafusion_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datafusion_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datafusion_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datafusion_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datafusion_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/datafusion_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataplex/__init__.py` & `google-events-0.9.0/src/google/events/cloud/dataplex/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataplex/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/dataplex/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/dataplex_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/dataplex_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataplex_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/dataplex_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/dataplex_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/dataplex_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataplex_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/dataplex_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/dataplex_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/dataplex_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastore/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastore/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/datastore/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/datastore_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datastore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastore_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/datastore_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/datastore_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datastore_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastore_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datastore_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastore_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/datastore_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastream/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datastream/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastream/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/datastream/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/datastream_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datastream_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastream_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/datastream_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/datastream_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datastream_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastream_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/datastream_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/datastream_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/datastream_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/eventarc/__init__.py` & `google-events-0.9.0/src/google/events/cloud/eventarc/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/eventarc/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/eventarc/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/eventarc_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/eventarc_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/eventarc_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/eventarc_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/eventarc_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/eventarc_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/eventarc_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/eventarc_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/eventarc_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/eventarc_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/firestore/__init__.py` & `google-events-0.9.0/src/google/events/cloud/firestore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/firestore/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/firestore/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/firestore_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/firestore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/firestore_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/firestore_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/firestore_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/firestore_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/firestore_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/firestore_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/firestore_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/firestore_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/functions/__init__.py` & `google-events-0.9.0/src/google/events/cloud/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/functions/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/functions/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/functions_v2/__init__.py` & `google-events-0.9.0/src/google/events/cloud/functions_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/functions_v2/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/functions_v2/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/functions_v2/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/functions_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/functions_v2/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/functions_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/functions_v2/types/data.py` & `google-events-0.9.0/src/google/events/cloud/functions_v2/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkebackup/__init__.py` & `google-events-0.9.0/src/google/events/cloud/gkebackup/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkebackup/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/gkebackup/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/gkebackup_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/gkebackup_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkebackup_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/gkebackup_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/gkebackup_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/gkebackup_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkebackup_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/gkebackup_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkebackup_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/gkebackup_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkehub/__init__.py` & `google-events-0.9.0/src/google/events/cloud/gkehub/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkehub/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/gkehub/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/gkehub_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/gkehub_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkehub_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/gkehub_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/gkehub_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/gkehub_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkehub_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/gkehub_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/gkehub_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/gkehub_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/iot/__init__.py` & `google-events-0.9.0/src/google/events/cloud/iot/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/iot/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/iot/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/iot_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/iot_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/iot_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/iot_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/iot_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/iot_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/iot_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/iot_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/iot_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/memcache/__init__.py` & `google-events-0.9.0/src/google/events/cloud/memcache/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/memcache/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/memcache/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/memcache_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/memcache_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/memcache_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/memcache_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/memcache_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/memcache_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/memcache_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/memcache_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/memcache_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/memcache_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/metastore/__init__.py` & `google-events-0.9.0/src/google/events/cloud/metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/metastore/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/metastore/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/metastore_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/metastore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/metastore_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/metastore_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/metastore_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/metastore_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/metastore_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/metastore_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/metastore_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/metastore_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkconnectivity/__init__.py` & `google-events-0.9.0/src/google/events/cloud/networkconnectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkconnectivity/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/networkconnectivity/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkconnectivity_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/networkconnectivity_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkmanagement/__init__.py` & `google-events-0.9.0/src/google/events/cloud/networkmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkmanagement/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/networkmanagement/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/networkmanagement_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/networkmanagement_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/notebooks/__init__.py` & `google-events-0.9.0/src/google/events/cloud/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/notebooks/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/notebooks/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/notebooks_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/notebooks_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/notebooks_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/notebooks_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/notebooks_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/notebooks_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/notebooks_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/notebooks_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/notebooks_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/notebooks_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/pubsub/__init__.py` & `google-events-0.9.0/src/google/events/cloud/pubsub/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/pubsub/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/pubsub/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/pubsub_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/pubsub_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/pubsub_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/pubsub_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/pubsub_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/pubsub_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/pubsub_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/pubsub_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/pubsub_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/pubsub_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/redis/__init__.py` & `google-events-0.9.0/src/google/events/cloud/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/redis/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/redis/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/redis_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/redis_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/redis_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/redis_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/redis_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/redis_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/redis_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/redis_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/redis_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/redis_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/scheduler/__init__.py` & `google-events-0.9.0/src/google/events/cloud/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/scheduler/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/scheduler/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/scheduler_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/scheduler_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/scheduler_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/scheduler_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/scheduler_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/scheduler_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/scheduler_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/scheduler_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/scheduler_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/scheduler_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/storage/__init__.py` & `google-events-0.9.0/src/google/events/cloud/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/storage/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/storage/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/storage_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/storage_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/storage_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/storage_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/storage_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/storage_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/storage_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/storage_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/storage_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/storage_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/video/transcoder/__init__.py` & `google-events-0.9.0/src/google/events/cloud/video/transcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/video/transcoder/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/video/transcoder/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/video/transcoder_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/video/transcoder_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/visionai/__init__.py` & `google-events-0.9.0/src/google/events/cloud/visionai/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/visionai/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/visionai/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/visionai_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/visionai_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/visionai_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/visionai_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/visionai_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/visionai_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/visionai_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/visionai_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/visionai_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/visionai_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/vmmigration/__init__.py` & `google-events-0.9.0/src/google/events/cloud/vmmigration/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/vmmigration/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/vmmigration/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/vmmigration_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/vmmigration_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/vmmigration_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/vmmigration_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/vmmigration_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/vmmigration_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/vmmigration_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/vmmigration_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/vmmigration_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/vmmigration_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/workflows/__init__.py` & `google-events-0.9.0/src/google/events/cloud/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/workflows/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/workflows/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/workflows_v1/__init__.py` & `google-events-0.9.0/src/google/events/cloud/workflows_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/workflows_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/cloud/workflows_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/cloud/workflows_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/cloud/workflows_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/workflows_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/cloud/workflows_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/cloud/workflows_v1/types/data.py` & `google-events-0.9.0/src/google/events/cloud/workflows_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/analytics/__init__.py` & `google-events-0.9.0/src/google/events/firebase/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/analytics/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/analytics/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/analytics_v1/__init__.py` & `google-events-0.9.0/src/google/events/firebase/analytics_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/analytics_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/analytics_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/analytics_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/firebase/analytics_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/analytics_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/firebase/analytics_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/analytics_v1/types/data.py` & `google-events-0.9.0/src/google/events/firebase/analytics_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/auth/__init__.py` & `google-events-0.9.0/src/google/events/firebase/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/auth/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/auth/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/auth_v1/__init__.py` & `google-events-0.9.0/src/google/events/firebase/auth_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/auth_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/auth_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/auth_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/firebase/auth_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/auth_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/firebase/auth_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/auth_v1/types/data.py` & `google-events-0.9.0/src/google/events/firebase/auth_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/database/__init__.py` & `google-events-0.9.0/src/google/events/firebase/database/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/database/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/database/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/database_v1/__init__.py` & `google-events-0.9.0/src/google/events/firebase/database_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/database_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/database_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/database_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/firebase/database_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/database_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/firebase/database_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/database_v1/types/data.py` & `google-events-0.9.0/src/google/events/firebase/database_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/firebasealerts/__init__.py` & `google-events-0.9.0/src/google/events/firebase/firebasealerts/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/firebasealerts/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/firebasealerts/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/__init__.py` & `google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/firebasealerts_v1/types/data.py` & `google-events-0.9.0/src/google/events/firebase/firebasealerts_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/remoteconfig/__init__.py` & `google-events-0.9.0/src/google/events/firebase/remoteconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/remoteconfig/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/remoteconfig/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/__init__.py` & `google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/remoteconfig_v1/types/data.py` & `google-events-0.9.0/src/google/events/firebase/remoteconfig_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/testlab/__init__.py` & `google-events-0.9.0/src/google/events/firebase/testlab/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/testlab/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/testlab/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/testlab_v1/__init__.py` & `google-events-0.9.0/src/google/events/firebase/testlab_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/testlab_v1/gapic_version.py` & `google-events-0.9.0/src/google/events/firebase/testlab_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.0.0"  # {x-release-please-version}
```

### Comparing `google-events-0.8.0/src/google/events/firebase/testlab_v1/services/__init__.py` & `google-events-0.9.0/src/google/events/firebase/testlab_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/testlab_v1/types/__init__.py` & `google-events-0.9.0/src/google/events/firebase/testlab_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google/events/firebase/testlab_v1/types/data.py` & `google-events-0.9.0/src/google/events/firebase/testlab_v1/types/data.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/src/google_events.egg-info/PKG-INFO` & `google-events-0.9.0/src/google_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-events
-Version: 0.8.0
+Version: 0.9.0
 Summary: Google Cloudevents library
 Home-page: https://github.com/googleapis/google-cloudevents-python/
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache License 2.0
 Platform: Posix
 Platform: MacOS X
```

### Comparing `google-events-0.8.0/src/google_events.egg-info/SOURCES.txt` & `google-events-0.9.0/src/google_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/tests/test_cloudevents_data_parsing.py` & `google-events-0.9.0/tests/test_cloudevents_data_parsing.py`

 * *Files identical despite different names*

### Comparing `google-events-0.8.0/tests/util.py` & `google-events-0.9.0/tests/util.py`

 * *Files identical despite different names*

