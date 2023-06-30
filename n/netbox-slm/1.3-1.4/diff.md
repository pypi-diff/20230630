# Comparing `tmp/netbox-slm-1.3.tar.gz` & `tmp/netbox-slm-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-slm-1.3.tar", last modified: Wed Apr 19 08:25:32 2023, max compression
+gzip compressed data, was "netbox-slm-1.4.tar", last modified: Fri Jun 30 13:14:42 2023, max compression
```

## Comparing `netbox-slm-1.3.tar` & `netbox-slm-1.4.tar`

### file list

```diff
@@ -1,43 +1,55 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:32.056067 netbox-slm-1.3/
--rwxrwxrwx   0 user      (1000) user      (1000)      557 2022-09-12 10:32:39.000000 netbox-slm-1.3/LICENSE
--rwxrwxrwx   0 user      (1000) user      (1000)      108 2023-04-19 08:14:46.000000 netbox-slm-1.3/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)      858 2023-04-19 08:25:32.058042 netbox-slm-1.3/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)     8170 2023-03-31 08:03:01.000000 netbox-slm-1.3/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.117380 netbox-slm-1.3/netbox_slm/
--rwxrwxrwx   0 user      (1000) user      (1000)      451 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/admin.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.440583 netbox-slm-1.3/netbox_slm/api/
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/api/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1811 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/api/serializers.py
--rwxrwxrwx   0 user      (1000) user      (1000)      531 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/api/urls.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1317 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/api/views.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1951 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/filtersets.py
--rwxrwxrwx   0 user      (1000) user      (1000)     5405 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/forms.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.687302 netbox-slm-1.3/netbox_slm/migrations/
--rwxrwxrwx   0 user      (1000) user      (1000)     3820 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/0001_initial.py
--rwxrwxrwx   0 user      (1000) user      (1000)      596 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/0002_alter_softwareproduct_manufacturer.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1479 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/0003_auto_20220407_1209.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1922 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/0004_auto_20220415_0705.py
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/migrations/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2954 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/models.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2347 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/navigation.py
--rwxrwxrwx   0 user      (1000) user      (1000)     4902 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/tables.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:30.672999 netbox-slm-1.3/netbox_slm/templates/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.875513 netbox-slm-1.3/netbox_slm/templates/netbox_slm/
--rwxrwxrwx   0 user      (1000) user      (1000)     1595 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproduct.html
--rwxrwxrwx   0 user      (1000) user      (1000)     1619 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproductinstallation.html
--rwxrwxrwx   0 user      (1000) user      (1000)     1222 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproductversion.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.925514 netbox-slm-1.3/netbox_slm/templatetags/
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-09-12 10:32:39.000000 netbox-slm-1.3/netbox_slm/templatetags/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:32.016329 netbox-slm-1.3/netbox_slm/tests/
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2023-03-29 20:01:01.000000 netbox-slm-1.3/netbox_slm/tests/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1914 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/tests/test_models.py
--rwxrwxrwx   0 user      (1000) user      (1000)     4006 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/urls.py
--rwxrwxrwx   0 user      (1000) user      (1000)     5425 2023-04-19 08:14:46.000000 netbox-slm-1.3/netbox_slm/views.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-19 08:25:31.253863 netbox-slm-1.3/netbox_slm.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      858 2023-04-19 08:25:30.000000 netbox-slm-1.3/netbox_slm.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      992 2023-04-19 08:25:30.000000 netbox-slm-1.3/netbox_slm.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-19 08:25:30.000000 netbox-slm-1.3/netbox_slm.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       11 2023-04-19 08:25:30.000000 netbox-slm-1.3/netbox_slm.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1000) user      (1000)      803 2023-04-19 08:25:32.068239 netbox-slm-1.3/setup.cfg
--rwxrwxrwx   0 user      (1000) user      (1000)       41 2023-04-19 08:14:46.000000 netbox-slm-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.924749 netbox-slm-1.4/
+-rw-rw-rw-   0        0        0      557 2022-09-12 10:32:39.000000 netbox-slm-1.4/LICENSE
+-rw-rw-rw-   0        0        0      108 2023-04-19 08:14:46.000000 netbox-slm-1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      932 2023-06-30 13:14:42.924749 netbox-slm-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8170 2023-03-31 08:03:01.000000 netbox-slm-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.790952 netbox-slm-1.4/netbox_slm/
+-rw-rw-rw-   0        0        0      451 2023-06-30 13:03:59.000000 netbox-slm-1.4/netbox_slm/__init__.py
+-rw-rw-rw-   0        0        0      222 2023-06-27 09:22:21.000000 netbox-slm-1.4/netbox_slm/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.811128 netbox-slm-1.4/netbox_slm/api/
+-rw-rw-rw-   0        0        0        0 2022-09-12 10:32:39.000000 netbox-slm-1.4/netbox_slm/api/__init__.py
+-rw-rw-rw-   0        0        0     2485 2023-06-28 21:09:43.000000 netbox-slm-1.4/netbox_slm/api/serializers.py
+-rw-rw-rw-   0        0        0      621 2023-06-27 09:28:51.000000 netbox-slm-1.4/netbox_slm/api/urls.py
+-rw-rw-rw-   0        0        0     1616 2023-06-27 09:28:51.000000 netbox-slm-1.4/netbox_slm/api/views.py
+-rw-rw-rw-   0        0        0     2725 2023-06-28 21:07:38.000000 netbox-slm-1.4/netbox_slm/filtersets.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.841311 netbox-slm-1.4/netbox_slm/forms/
+-rw-rw-rw-   0        0        0      153 2023-06-27 08:49:52.000000 netbox-slm-1.4/netbox_slm/forms/__init__.py
+-rw-rw-rw-   0        0        0     2671 2023-06-27 09:05:37.000000 netbox-slm-1.4/netbox_slm/forms/software_license.py
+-rw-rw-rw-   0        0        0     1278 2023-06-27 08:59:01.000000 netbox-slm-1.4/netbox_slm/forms/software_product.py
+-rw-rw-rw-   0        0        0     3249 2023-06-27 08:59:01.000000 netbox-slm-1.4/netbox_slm/forms/software_product_installation.py
+-rw-rw-rw-   0        0        0     1567 2023-06-27 08:59:01.000000 netbox-slm-1.4/netbox_slm/forms/software_product_version.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.874636 netbox-slm-1.4/netbox_slm/migrations/
+-rw-rw-rw-   0        0        0     3820 2022-09-12 10:32:39.000000 netbox-slm-1.4/netbox_slm/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      596 2022-09-12 10:32:39.000000 netbox-slm-1.4/netbox_slm/migrations/0002_alter_softwareproduct_manufacturer.py
+-rw-rw-rw-   0        0        0     1479 2022-09-12 10:32:39.000000 netbox-slm-1.4/netbox_slm/migrations/0003_auto_20220407_1209.py
+-rw-rw-rw-   0        0        0     1922 2022-09-12 10:32:39.000000 netbox-slm-1.4/netbox_slm/migrations/0004_auto_20220415_0705.py
+-rw-rw-rw-   0        0        0     2712 2023-06-27 09:25:04.000000 netbox-slm-1.4/netbox_slm/migrations/0005_add_software_license.py
+-rw-rw-rw-   0        0        0        0 2022-09-12 10:32:39.000000 netbox-slm-1.4/netbox_slm/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4084 2023-06-28 20:59:37.000000 netbox-slm-1.4/netbox_slm/models.py
+-rw-rw-rw-   0        0        0     3049 2023-06-27 09:16:50.000000 netbox-slm-1.4/netbox_slm/navigation.py
+-rw-rw-rw-   0        0        0     6395 2023-06-28 21:06:07.000000 netbox-slm-1.4/netbox_slm/tables.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.774296 netbox-slm-1.4/netbox_slm/templates/
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.891317 netbox-slm-1.4/netbox_slm/templates/netbox_slm/
+-rw-rw-rw-   0        0        0     2285 2023-06-30 13:02:31.000000 netbox-slm-1.4/netbox_slm/templates/netbox_slm/softwarelicense.html
+-rw-rw-rw-   0        0        0     1888 2023-06-27 09:40:48.000000 netbox-slm-1.4/netbox_slm/templates/netbox_slm/softwareproduct.html
+-rw-rw-rw-   0        0        0     1505 2023-06-27 09:40:48.000000 netbox-slm-1.4/netbox_slm/templates/netbox_slm/softwareproductinstallation.html
+-rw-rw-rw-   0        0        0     1168 2023-06-27 09:35:09.000000 netbox-slm-1.4/netbox_slm/templates/netbox_slm/softwareproductversion.html
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.891317 netbox-slm-1.4/netbox_slm/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-09-12 10:32:39.000000 netbox-slm-1.4/netbox_slm/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.891317 netbox-slm-1.4/netbox_slm/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-29 20:01:01.000000 netbox-slm-1.4/netbox_slm/tests/__init__.py
+-rw-rw-rw-   0        0        0     2376 2023-06-28 21:18:57.000000 netbox-slm-1.4/netbox_slm/tests/test_models.py
+-rw-rw-rw-   0        0        0     5260 2023-06-27 09:15:23.000000 netbox-slm-1.4/netbox_slm/urls.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.924749 netbox-slm-1.4/netbox_slm/views/
+-rw-rw-rw-   0        0        0      153 2023-06-27 08:50:18.000000 netbox-slm-1.4/netbox_slm/views/__init__.py
+-rw-rw-rw-   0        0        0     1576 2023-06-27 08:35:32.000000 netbox-slm-1.4/netbox_slm/views/software_license.py
+-rw-rw-rw-   0        0        0     1786 2023-06-27 08:35:31.000000 netbox-slm-1.4/netbox_slm/views/software_product.py
+-rw-rw-rw-   0        0        0     1924 2023-06-27 08:35:32.000000 netbox-slm-1.4/netbox_slm/views/software_product_installation.py
+-rw-rw-rw-   0        0        0     1952 2023-06-27 08:35:32.000000 netbox-slm-1.4/netbox_slm/views/software_product_version.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:14:42.811128 netbox-slm-1.4/netbox_slm.egg-info/
+-rw-rw-rw-   0        0        0      932 2023-06-30 13:14:42.000000 netbox-slm-1.4/netbox_slm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2023-06-30 13:14:42.000000 netbox-slm-1.4/netbox_slm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 13:14:42.000000 netbox-slm-1.4/netbox_slm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 13:14:42.000000 netbox-slm-1.4/netbox_slm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      834 2023-06-30 13:14:42.924749 netbox-slm-1.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-19 08:14:46.000000 netbox-slm-1.4/setup.py
```

### Comparing `netbox-slm-1.3/LICENSE` & `netbox-slm-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-slm-1.3/PKG-INFO` & `netbox-slm-1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-Metadata-Version: 2.1
-Name: netbox-slm
-Version: 1.3
-Summary: Software Lifecycle Management Netbox Plugin.
-Author: ICTU
-Author-email: open-source-projects@ictu.nl
-License: Apache 2.0
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.9
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: netbox-slm
+Version: 1.4
+Summary: Software Lifecycle Management Netbox Plugin.
+Home-page: UNKNOWN
+Author: ICTU
+Author-email: open-source-projects@ictu.nl
+License: Apache 2.0
+Platform: UNKNOWN
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.9
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `netbox-slm-1.3/README.md` & `netbox-slm-1.4/README.md`

 * *Files identical despite different names*

### Comparing `netbox-slm-1.3/netbox_slm/api/serializers.py` & `netbox-slm-1.4/netbox_slm/api/serializers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from rest_framework import serializers
 
 from netbox.api.serializers import NetBoxModelSerializer
-from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
+from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation, SoftwareLicense
 
 
 class SoftwareProductSerializer(NetBoxModelSerializer):
     display = serializers.SerializerMethodField()
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_slm-api:softwareproduct-detail"
     )
 
     class Meta:
         model = SoftwareProduct
         fields = [
-            'id', 'display', 'url', 'name', 'tags', 'custom_field_data', 'created', 'last_updated',
+            'id', 'display', 'url', 'name',
+            'tags', 'custom_field_data', 'created', 'last_updated',
         ]
 
     def get_display(self, obj):
         return f"{obj.manufacturer} - {obj}"
 
 
 class SoftwareProductVersionSerializer(NetBoxModelSerializer):
@@ -25,15 +26,16 @@
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_slm-api:softwareproductversion-detail"
     )
 
     class Meta:
         model = SoftwareProductVersion
         fields = [
-            'id', 'display', 'url', 'name', 'software_product', 'tags', 'custom_field_data', 'created', 'last_updated',
+            'id', 'display', 'url', 'name', 'software_product',
+            'tags', 'custom_field_data', 'created', 'last_updated',
         ]
 
     def get_display(self, obj):
         return f"{obj}"
 
 
 class SoftwareProductInstallationSerializer(NetBoxModelSerializer):
@@ -41,13 +43,31 @@
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_slm-api:softwareproductinstallation-detail"
     )
 
     class Meta:
         model = SoftwareProductInstallation
         fields = [
-            'id', 'display', 'url', 'device', 'virtualmachine', 'software_product', 'version', 'tags',
-            'custom_field_data', 'created', 'last_updated',
+            'id', 'display', 'url', 'device', 'virtualmachine', 'software_product', 'version',
+            'tags', 'custom_field_data', 'created', 'last_updated',
+        ]
+
+    def get_display(self, obj):
+        return f"{obj}"
+
+
+class SoftwareLicenseSerializer(NetBoxModelSerializer):
+    display = serializers.SerializerMethodField()
+    url = serializers.HyperlinkedIdentityField(
+        view_name="plugins-api:netbox_slm-api:softwarelicense-detail"
+    )
+
+    class Meta:
+        model = SoftwareLicense
+        fields = [
+            'id', 'display', 'url', 'name', 'description', 'type', 'stored_location',
+            'start_date', 'expiration_date', 'software_product', 'version', 'installation',
+            'tags', 'custom_field_data', 'created', 'last_updated',
         ]
 
     def get_display(self, obj):
         return f"{obj}"
```

### Comparing `netbox-slm-1.3/netbox_slm/api/views.py` & `netbox-slm-1.4/netbox_slm/forms/software_product.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-from rest_framework.routers import APIRootView
+from django import forms
 
-from netbox.api.viewsets import NetBoxModelViewSet
-from netbox_slm.api.serializers import (
-    SoftwareProductSerializer, SoftwareProductVersionSerializer, SoftwareProductInstallationSerializer,
-)
-from netbox_slm.filtersets import (
-    SoftwareProductFilterSet, SoftwareProductVersionFilterSet, SoftwareProductInstallationFilterSet,
-)
-from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
+from dcim.models import Manufacturer
+from netbox.forms import NetBoxModelForm, NetBoxModelImportForm, NetBoxModelBulkEditForm, NetBoxModelFilterSetForm
+from netbox_slm.models import SoftwareProduct
+from utilities.forms import DynamicModelChoiceField, TagFilterField
 
 
-class NetboxSLMRootView(APIRootView):
-    """
-    NetboxSLM API root view
-    """
+class SoftwareProductForm(NetBoxModelForm):
+    """Form for creating a new SoftwareProduct object."""
 
-    def get_view_name(self):
-        return "NetboxSLM"
+    manufacturer = DynamicModelChoiceField(
+        queryset=Manufacturer.objects.all(),
+        required=True,
+    )
 
+    class Meta:
+        model = SoftwareProduct
+        fields = ("name", "manufacturer", "description", "tags")
 
-class SoftwareProductViewSet(NetBoxModelViewSet):
-    queryset = SoftwareProduct.objects.all()
-    serializer_class = SoftwareProductSerializer
-    filterset_class = SoftwareProductFilterSet
 
+class SoftwareProductFilterForm(NetBoxModelFilterSetForm):
+    model = SoftwareProduct
+    fieldsets = (
+        (None, ('q', 'tag')),
+    )
 
-class SoftwareProductVersionViewSet(NetBoxModelViewSet):
-    queryset = SoftwareProductVersion.objects.all()
-    serializer_class = SoftwareProductVersionSerializer
-    filterset_class = SoftwareProductVersionFilterSet
+    tag = TagFilterField(model)
 
 
-class SoftwareProductInstallationViewSet(NetBoxModelViewSet):
-    queryset = SoftwareProductInstallation.objects.all()
-    serializer_class = SoftwareProductInstallationSerializer
-    filterset_class = SoftwareProductInstallationFilterSet
+class SoftwareProductImportForm(NetBoxModelImportForm):
+    class Meta:
+        model = SoftwareProduct
+        fields = ("name", "manufacturer",)
+
+
+class SoftwareProductBulkEditForm(NetBoxModelBulkEditForm):
+    pk = forms.ModelMultipleChoiceField(
+        queryset=SoftwareProduct.objects.all(),
+        widget=forms.MultipleHiddenInput(),
+    )
+
+    class Meta:
+        model = SoftwareProduct
+        nullable_fields = []
```

### Comparing `netbox-slm-1.3/netbox_slm/filtersets.py` & `netbox-slm-1.4/netbox_slm/filtersets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.db.models import Q
 
 from netbox.filtersets import NetBoxModelFilterSet
-from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
+from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation, SoftwareLicense
 
 
 class SoftwareProductFilterSet(NetBoxModelFilterSet):
     """Filter capabilities for SoftwareProduct instances."""
 
     class Meta:
         model = SoftwareProduct
@@ -39,17 +39,38 @@
 
 
 class SoftwareProductInstallationFilterSet(NetBoxModelFilterSet):
     """Filter capabilities for SoftwareProductInstallation instances."""
 
     class Meta:
         model = SoftwareProductInstallation
-        fields = tuple()
+        fields = (
+            "software_product",
+        )
 
     def search(self, queryset, name, value):
         """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = Q(software_product__name__icontains=value) | \
                     Q(software_product__manufacturer__name__icontains=value) | \
                     Q(version__name__icontains=value)
         return queryset.filter(qs_filter)
+
+
+class SoftwareLicenseFilterSet(NetBoxModelFilterSet):
+    """Filter capabilities for SoftwareLicense instances."""
+
+    class Meta:
+        model = SoftwareLicense
+        fields = tuple()
+
+    def search(self, queryset, name, value):
+        """Perform the filtered search."""
+        if not value.strip():
+            return queryset
+        qs_filter = Q(name__icontains=value) | \
+                    Q(software_product__name__icontains=value) | \
+                    Q(version__name__icontains=value) | \
+                    Q(installation__device__name__icontains=value) | \
+                    Q(installation__virtualmachine__name__icontains=value)
+        return queryset.filter(qs_filter)
```

### Comparing `netbox-slm-1.3/netbox_slm/forms.py` & `netbox-slm-1.4/netbox_slm/forms/software_product_installation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,18 @@
 from django import forms
 from django.urls import reverse_lazy
 from django.utils.translation import gettext as _
 
-from dcim.models import Manufacturer, Device
-from netbox.forms import NetBoxModelForm, NetBoxModelCSVForm, NetBoxModelBulkEditForm, NetBoxModelFilterSetForm
-from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
+from dcim.models import Device
+from netbox.forms import NetBoxModelForm, NetBoxModelImportForm, NetBoxModelBulkEditForm, NetBoxModelFilterSetForm
+from netbox_slm.models import SoftwareProductInstallation, SoftwareProduct, SoftwareProductVersion
 from utilities.forms import DynamicModelChoiceField, APISelect, TagFilterField
 from virtualization.models import VirtualMachine
 
 
-class SoftwareProductForm(NetBoxModelForm):
-    """Form for creating a new SoftwareProduct object."""
-
-    manufacturer = DynamicModelChoiceField(
-        queryset=Manufacturer.objects.all(),
-        required=True,
-    )
-
-    class Meta:
-        model = SoftwareProduct
-        fields = ("name", "manufacturer", "description", "tags")
-
-
-class SoftwareProductFilterForm(NetBoxModelFilterSetForm):
-    model = SoftwareProduct
-    fieldsets = (
-        (None, ('q', 'tag')),
-    )
-
-    tag = TagFilterField(model)
-
-
-class SoftwareProductCSVForm(NetBoxModelCSVForm):
-    class Meta:
-        model = SoftwareProduct
-        fields = ("name", "manufacturer",)
-
-
-class SoftwareProductBulkEditForm(NetBoxModelBulkEditForm):
-    pk = forms.ModelMultipleChoiceField(
-        queryset=SoftwareProduct.objects.all(),
-        widget=forms.MultipleHiddenInput(),
-    )
-
-    class Meta:
-        model = SoftwareProduct
-        nullable_fields = []
-
-
-class SoftwareProductVersionForm(NetBoxModelForm):
-    """Form for creating a new SoftwareProductVersion object."""
-    name = forms.CharField(label=_("Version"))
-
-    software_product = DynamicModelChoiceField(
-        queryset=SoftwareProduct.objects.all(),
-        widget=APISelect(
-            attrs={"data-url": reverse_lazy("plugins-api:netbox_slm-api:softwareproduct-list")}
-        ),
-    )
-
-    class Meta:
-        model = SoftwareProductVersion
-        fields = ("name", "software_product", "tags")
-
-
-class SoftwareProductVersionFilterForm(NetBoxModelFilterSetForm):
-    model = SoftwareProductVersion
-    fieldsets = (
-        (None, ('q', 'tag')),
-    )
-
-    tag = TagFilterField(model)
-
-
-class SoftwareProductVersionCSVForm(NetBoxModelCSVForm):
-    class Meta:
-        model = SoftwareProductVersion
-        fields = ("name",)
-
-
-class SoftwareProductVersionBulkEditForm(NetBoxModelBulkEditForm):
-    pk = forms.ModelMultipleChoiceField(
-        queryset=SoftwareProduct.objects.all(),
-        widget=forms.MultipleHiddenInput(),
-    )
-
-    class Meta:
-        model = SoftwareProductVersion
-        nullable_fields = []
-
-
 class SoftwareProductInstallationForm(NetBoxModelForm):
     """Form for creating a new SoftwareProductInstallation object."""
 
     device = DynamicModelChoiceField(
         queryset=Device.objects.all(),
         required=False,
     )
@@ -142,15 +61,15 @@
     fieldsets = (
         (None, ('q', 'tag',)),
     )
 
     tag = TagFilterField(model)
 
 
-class SoftwareProductInstallationCSVForm(NetBoxModelCSVForm):
+class SoftwareProductInstallationImportForm(NetBoxModelImportForm):
     class Meta:
         model = SoftwareProductInstallation
         fields = tuple()
 
 
 class SoftwareProductInstallationBulkEditForm(NetBoxModelBulkEditForm):
     software_product = DynamicModelChoiceField(
```

### Comparing `netbox-slm-1.3/netbox_slm/migrations/0001_initial.py` & `netbox-slm-1.4/netbox_slm/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-slm-1.3/netbox_slm/migrations/0002_alter_softwareproduct_manufacturer.py` & `netbox-slm-1.4/netbox_slm/migrations/0002_alter_softwareproduct_manufacturer.py`

 * *Files identical despite different names*

### Comparing `netbox-slm-1.3/netbox_slm/migrations/0003_auto_20220407_1209.py` & `netbox-slm-1.4/netbox_slm/migrations/0003_auto_20220407_1209.py`

 * *Files identical despite different names*

### Comparing `netbox-slm-1.3/netbox_slm/migrations/0004_auto_20220415_0705.py` & `netbox-slm-1.4/netbox_slm/migrations/0004_auto_20220415_0705.py`

 * *Files identical despite different names*

### Comparing `netbox-slm-1.3/netbox_slm/navigation.py` & `netbox-slm-1.4/netbox_slm/navigation.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,8 +58,28 @@
                 "Import",
                 "mdi mdi-upload",
                 ButtonColorChoices.CYAN,
                 permissions=["netbox_slm.add_softwareproductinstallation"],
             ),
         )
     ),
+    PluginMenuItem(
+        link='plugins:netbox_slm:softwarelicense_list',
+        link_text='Licenses',
+        buttons=(
+            PluginMenuButton(
+                "plugins:netbox_slm:softwarelicense_add",
+                "Add",
+                "mdi mdi-plus-thick",
+                ButtonColorChoices.GREEN,
+                permissions=["netbox_slm.add_softwarelicense"],
+            ),
+            PluginMenuButton(
+                "plugins:netbox_slm:softwarelicense_import",
+                "Import",
+                "mdi mdi-upload",
+                ButtonColorChoices.CYAN,
+                permissions=["netbox_slm.add_softwarelicense"],
+            ),
+        )
+    ),
 )
```

### Comparing `netbox-slm-1.3/netbox_slm/tables.py` & `netbox-slm-1.4/netbox_slm/tables.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import django_tables2 as tables
 from django.db.models import Count
 from django_tables2.utils import Accessor
 
 from netbox.tables import NetBoxTable, ToggleColumn, columns
-from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
+from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation, SoftwareLicense
 
 
 class SoftwareProductTable(NetBoxTable):
     """Table for displaying SoftwareProduct objects."""
 
     pk = ToggleColumn()
     name = tables.LinkColumn()
@@ -114,15 +114,15 @@
         linkify=True
     )
     virtualmachine = tables.Column(
         accessor=Accessor('virtualmachine'),
         linkify=True
     )
     platform = tables.Column(
-        accessor='get_platform',
+        accessor=Accessor('platform'),
         linkify=True
     )
     type = tables.Column(accessor='render_type')
     software_product = tables.Column(
         accessor=Accessor('software_product'),
         linkify=True
     )
@@ -161,7 +161,62 @@
 
     def order_type(self, queryset, is_descending):
         queryset = queryset.order_by(("device" if is_descending else "virtualmachine"))
         return queryset, True
 
     def render_software_product(self, value, **kwargs):
         return f"{kwargs['record'].software_product.manufacturer.name} - {value}"
+
+
+class SoftwareLicenseTable(NetBoxTable):
+    """Table for displaying SoftwareLicense objects."""
+
+    pk = ToggleColumn()
+    name = tables.LinkColumn()
+
+    type = tables.Column(accessor='render_type')
+    software_product = tables.Column(
+        accessor=Accessor('software_product'),
+        linkify=True
+    )
+    version = tables.Column(
+        accessor=Accessor('version'),
+        linkify=True
+    )
+    installation = tables.Column(
+        accessor=Accessor('installation'),
+        linkify=True
+    )
+
+    tags = columns.TagColumn(
+        url_name="plugins:netbox_slm:softwarelicense_list",
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = SoftwareLicense
+        fields = (
+            "pk",
+            "name",
+            "description",
+            "type",
+            "stored_location",
+            "start_date",
+            "expiration_date",
+            "software_product",
+            "version",
+            "installation",
+            "tags",
+        )
+        default_columns = (
+            "pk",
+            "name",
+            "expiration_date",
+            "software_product",
+            "installation",
+            "tags",
+        )
+
+    def render_software_product(self, value, **kwargs):
+        return f"{kwargs['record'].software_product.manufacturer.name} - {value}"
+
+    def render_installation(self, **kwargs):
+        return f"{kwargs['record'].installation.platform}"
```

### Comparing `netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproduct.html` & `netbox-slm-1.4/netbox_slm/templates/netbox_slm/softwarelicense.html`

 * *Files 26% similar despite different names*

```diff
@@ -5,40 +5,59 @@
 {% load plugins %}
 
 {% block content %}
 <div class="row my-3">
 	<div class="col col-md-6">
         <div class="card">
             <h5 class="card-header">
-                Software Product
+                Software License
             </h5>
             <div class="card-body">
                 <table class="table table-hover attr-table">
                     <tr>
                         <th scope="row">Name</th>
-                        <td>{{ object }}</td>
+                        <td>{{ object.name }}</td>
                     </tr>
                     <tr>
-                        <th scope="row">Versions</th>
-                        <td>
-                        {% for version in object.softwareproduct_versions.all %}
-                            <a href="{% url 'plugins:netbox_slm:softwareproductversion' pk=version.pk %}">
-                                <span class="badge" style="color: #ffffff; background-color: #9e9e9e">{{ version }}</span>
-                            </a>
-                        {% empty %}
-                            n/a
-                        {% endfor %}
-                        </td>
+                        <th scope="row">Description</th>
+                        <td>{{ object.description }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Type</th>
+                        <td>{{ object.type }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Stored location</th>
+                        <td>{{ object.stored_location }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Start date</th>
+                        <td>{{ object.start_date }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Expiration date</th>
+                        <td>{{ object.expiration_date }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Software Product</th>
+                        <td>{{ object.software_product }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Version</th>
+                        <td>{{ object.version }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Installation</th>
+                        <td>{{ object.installation }}</td>
                     </tr>
                 </table>
             </div>
         </div>
         {% include 'inc/panels/custom_fields.html' %}
         {% include 'inc/panels/tags.html' %}
-{#        {% include 'inc/panels/comments.html' %}#}
         {% plugin_left_page object %}
     </div>
 </div>
 <div class="row">
     <div class="col col-md-12">
         {% plugin_full_width_page object %}
     </div>
```

#### html2text {}

```diff
@@ -1,10 +1,16 @@
 {% extends 'generic/object.html' %} {% load buttons %} {% load static %} {%
 load helpers %} {% load plugins %} {% block content %}
-** Software Product **
-Name     {{ object }}
-Versions {% for version in object.softwareproduct_versions.all %} {{_version_}}
-         {% empty %} n/a {% endfor %}
+** Software License **
+Name             {{ object.name }}
+Description      {{ object.description }}
+Type             {{ object.type }}
+Stored location  {{ object.stored_location }}
+Start date       {{ object.start_date }}
+Expiration date  {{ object.expiration_date }}
+Software Product {{ object.software_product }}
+Version          {{ object.version }}
+Installation     {{ object.installation }}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
-%} {# {% include 'inc/panels/comments.html' %}#} {% plugin_left_page object %}
+%} {% plugin_left_page object %}
 {% plugin_full_width_page object %}
 {% endblock %}
```

### Comparing `netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproductinstallation.html` & `netbox-slm-1.4/netbox_slm/templates/netbox_slm/softwareproductversion.html`

 * *Files 14% similar despite different names*

```diff
@@ -5,43 +5,33 @@
 {% load plugins %}
 
 {% block content %}
 <div class="row my-3">
 	<div class="col col-md-6">
         <div class="card">
             <h5 class="card-header">
-                Software Product Installation
+                Software Product Version
             </h5>
             <div class="card-body">
                 <table class="table table-hover attr-table">
-                    {% if object.device %}
                     <tr>
-                        <th scope="row">Device</th>
-                        <td>{{ object.device }}</td>
+                        <th scope="row">Name</th>
+                        <td>{{ object.name }}</td>
                     </tr>
-                    {% else %}
                     <tr>
-                        <th scope="row">Virtualmachine</th>
-                        <td>{{ object.virtualmachine }}</td>
-                    </tr>
-                    {% endif %}
-                    <tr>
-                        <th scope="row">Software Product</th>
-                        <td>{{ object.software_product }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Version</th>
-                        <td>{{ object.version }}</td>
+                        <th scope="row">Installations</th>
+                        <td>
+                            {{ object.get_installation_count }}
+                        </td>
                     </tr>
                 </table>
             </div>
         </div>
         {% include 'inc/panels/custom_fields.html' %}
         {% include 'inc/panels/tags.html' %}
-{#        {% include 'inc/panels/comments.html' %}#}
         {% plugin_left_page object %}
     </div>
 </div>
 <div class="row">
     <div class="col col-md-12">
         {% plugin_full_width_page object %}
     </div>
```

#### html2text {}

```diff
@@ -1,11 +1,9 @@
 {% extends 'generic/object.html' %} {% load buttons %} {% load static %} {%
 load helpers %} {% load plugins %} {% block content %}
-** Software Product Installation **
-Device           {{ object.device }}
-Virtualmachine   {{ object.virtualmachine }}
-Software Product {{ object.software_product }}
-Version          {{ object.version }}
+** Software Product Version **
+Name          {{ object.name }}
+Installations {{ object.get_installation_count }}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
-%} {# {% include 'inc/panels/comments.html' %}#} {% plugin_left_page object %}
+%} {% plugin_left_page object %}
 {% plugin_full_width_page object %}
 {% endblock %}
```

### Comparing `netbox-slm-1.3/netbox_slm/templates/netbox_slm/softwareproductversion.html` & `netbox-slm-1.4/netbox_slm/templates/netbox_slm/softwareproduct.html`

 * *Files 25% similar despite different names*

```diff
@@ -5,34 +5,47 @@
 {% load plugins %}
 
 {% block content %}
 <div class="row my-3">
 	<div class="col col-md-6">
         <div class="card">
             <h5 class="card-header">
-                Software Product Version
+                Software Product
             </h5>
             <div class="card-body">
                 <table class="table table-hover attr-table">
                     <tr>
                         <th scope="row">Name</th>
                         <td>{{ object.name }}</td>
                     </tr>
                     <tr>
-                        <th scope="row">Installations</th>
+                        <th scope="row">Description</th>
+                        <td>{{ object.description }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Manufacturer</th>
+                        <td>{{ object.manufacturer }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Versions</th>
                         <td>
-                            {{ object.get_installation_count }}
+                        {% for version in object.softwareproduct_versions.all %}
+                            <a href="{% url 'plugins:netbox_slm:softwareproductversion' pk=version.pk %}">
+                                <span class="badge" style="color: #ffffff; background-color: #9e9e9e">{{ version }}</span>
+                            </a>
+                        {% empty %}
+                            n/a
+                        {% endfor %}
                         </td>
                     </tr>
                 </table>
             </div>
         </div>
         {% include 'inc/panels/custom_fields.html' %}
         {% include 'inc/panels/tags.html' %}
-{#        {% include 'inc/panels/comments.html' %}#}
         {% plugin_left_page object %}
     </div>
 </div>
 <div class="row">
     <div class="col col-md-12">
         {% plugin_full_width_page object %}
     </div>
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
 {% extends 'generic/object.html' %} {% load buttons %} {% load static %} {%
 load helpers %} {% load plugins %} {% block content %}
-** Software Product Version **
-Name          {{ object.name }}
-Installations {{ object.get_installation_count }}
+** Software Product **
+Name         {{ object.name }}
+Description  {{ object.description }}
+Manufacturer {{ object.manufacturer }}
+Versions     {% for version in object.softwareproduct_versions.all %} {
+             {_version_}} {% empty %} n/a {% endfor %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/tags.html'
-%} {# {% include 'inc/panels/comments.html' %}#} {% plugin_left_page object %}
+%} {% plugin_left_page object %}
 {% plugin_full_width_page object %}
 {% endblock %}
```

### Comparing `netbox-slm-1.3/netbox_slm/tests/test_models.py` & `netbox-slm-1.4/netbox_slm/tests/test_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from django.test import TestCase
 
-from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
+from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation, SoftwareLicense
 
 
 class ModelTestCase(TestCase):
     def setUp(self):
         self.p_name = "test product"
         self.v_name = "test version"
+        self.l_name = "test license"
 
         self.software_product = SoftwareProduct.objects.create(name=self.p_name)
         self.software_product_version = SoftwareProductVersion.objects.create(
             name=self.v_name, software_product=self.software_product
         )
         self.software_product_installation = SoftwareProductInstallation.objects.create(
             software_product=self.software_product, version=self.software_product_version
         )
+        self.software_license = SoftwareLicense.objects.create(
+            name=self.l_name, software_product=self.software_product,
+            version=self.software_product_version, installation=self.software_product_installation
+        )
 
     def test_model_name(self):
         self.assertEqual(self.p_name, str(self.software_product))
         self.assertEqual(self.v_name, str(self.software_product_version))
-        self.assertTrue(str(self.software_product_installation).isnumeric())  # should be PK
+        self.assertTrue(str(self.software_product_installation)[0].isdigit())  # starts with PK
+        self.assertEqual(self.l_name, str(self.software_license))
 
     def test_absolute_url(self):
         self.assertEqual("/plugins/slm/software-products/1/", self.software_product.get_absolute_url())
         self.assertEqual("/plugins/slm/versions/1/", self.software_product_version.get_absolute_url())
         self.assertEqual("/plugins/slm/installations/1/", self.software_product_installation.get_absolute_url())
+        self.assertEqual("/plugins/slm/licenses/1/", self.software_license.get_absolute_url())
 
     def test_get_installation_count(self):
         installation_ss = '<a href="/plugins/slm/installations/?q={}">1</a>'
         self.assertEqual(installation_ss.format(self.p_name), self.software_product.get_installation_count())
         self.assertEqual(installation_ss.format(self.v_name), self.software_product_version.get_installation_count())
 
     def test_product_installation_methods(self):
         self.assertEqual("virtualmachine", self.software_product_installation.render_type())
-        self.assertIsNone(self.software_product_installation.get_platform())
+        self.assertIsNone(self.software_product_installation.platform)
```

#### html2text {}

```diff
@@ -1,26 +1,30 @@
 from django.test import TestCase from netbox_slm.models import SoftwareProduct,
-SoftwareProductVersion, SoftwareProductInstallation class ModelTestCase
-(TestCase): def setUp(self): self.p_name = "test product" self.v_name = "test
-version" self.software_product = SoftwareProduct.objects.create
-(name=self.p_name) self.software_product_version =
-SoftwareProductVersion.objects.create( name=self.v_name,
-software_product=self.software_product ) self.software_product_installation =
-SoftwareProductInstallation.objects.create
+SoftwareProductVersion, SoftwareProductInstallation, SoftwareLicense class
+ModelTestCase(TestCase): def setUp(self): self.p_name = "test product"
+self.v_name = "test version" self.l_name = "test license" self.software_product
+= SoftwareProduct.objects.create(name=self.p_name)
+self.software_product_version = SoftwareProductVersion.objects.create
+( name=self.v_name, software_product=self.software_product )
+self.software_product_installation = SoftwareProductInstallation.objects.create
 ( software_product=self.software_product, version=self.software_product_version
-) def test_model_name(self): self.assertEqual(self.p_name, str
-(self.software_product)) self.assertEqual(self.v_name, str
-(self.software_product_version)) self.assertTrue(str
-(self.software_product_installation).isnumeric()) # should be PK def
-test_absolute_url(self): self.assertEqual("/plugins/slm/software-products/1/",
+) self.software_license = SoftwareLicense.objects.create( name=self.l_name,
+software_product=self.software_product, version=self.software_product_version,
+installation=self.software_product_installation ) def test_model_name(self):
+self.assertEqual(self.p_name, str(self.software_product)) self.assertEqual
+(self.v_name, str(self.software_product_version)) self.assertTrue(str
+(self.software_product_installation)[0].isdigit()) # starts with PK
+self.assertEqual(self.l_name, str(self.software_license)) def test_absolute_url
+(self): self.assertEqual("/plugins/slm/software-products/1/",
 self.software_product.get_absolute_url()) self.assertEqual("/plugins/slm/
 versions/1/", self.software_product_version.get_absolute_url())
 self.assertEqual("/plugins/slm/installations/1/",
-self.software_product_installation.get_absolute_url()) def
+self.software_product_installation.get_absolute_url()) self.assertEqual("/
+plugins/slm/licenses/1/", self.software_license.get_absolute_url()) def
 test_get_installation_count(self): installation_ss = '1' self.assertEqual
 (installation_ss.format(self.p_name),
 self.software_product.get_installation_count()) self.assertEqual
 (installation_ss.format(self.v_name),
 self.software_product_version.get_installation_count()) def
 test_product_installation_methods(self): self.assertEqual("virtualmachine",
 self.software_product_installation.render_type()) self.assertIsNone
-(self.software_product_installation.get_platform())
+(self.software_product_installation.platform)
```

### Comparing `netbox-slm-1.3/netbox_slm/urls.py` & `netbox-slm-1.4/netbox_slm/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 from django.urls import path
 
 from netbox.views.generic import ObjectChangeLogView
 from netbox_slm import views
-from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation
+from netbox_slm.models import SoftwareProduct, SoftwareProductVersion, SoftwareProductInstallation, SoftwareLicense
 
 urlpatterns = [
-    # Software Products
-    path("software-products/", views.SoftwareProductListView.as_view(), name='softwareproduct_list'),
-    path("software-products/add/", views.SoftwareProductEditView.as_view(), name='softwareproduct_add'),
-    path("software-products/import/", views.SoftwareProductBulkImportView.as_view(), name="softwareproduct_import"),
-    path("software-products/edit/", views.SoftwareProductBulkEditView.as_view(), name="softwareproduct_bulk_edit"),
+    # SoftwareProduct
+    path("software-products/", views.SoftwareProductListView.as_view(),
+         name='softwareproduct_list'),
+    path("software-products/add/", views.SoftwareProductEditView.as_view(),
+         name='softwareproduct_add'),
+    path("software-products/import/", views.SoftwareProductBulkImportView.as_view(),
+         name="softwareproduct_import"),
+    path("software-products/edit/", views.SoftwareProductBulkEditView.as_view(),
+         name="softwareproduct_bulk_edit"),
     path("software-products/delete/", views.SoftwareProductBulkDeleteView.as_view(),
          name="softwareproduct_bulk_delete"),
-    path("software-products/<int:pk>/", views.SoftwareProductView.as_view(), name="softwareproduct"),
+    path("software-products/<int:pk>/", views.SoftwareProductView.as_view(),
+         name="softwareproduct"),
     path("software-products/<int:pk>/delete/", views.SoftwareProductDeleteView.as_view(),
          name="softwareproduct_delete"),
-    path("software-products/<int:pk>/edit/", views.SoftwareProductEditView.as_view(), name="softwareproduct_edit"),
+    path("software-products/<int:pk>/edit/", views.SoftwareProductEditView.as_view(),
+         name="softwareproduct_edit"),
     path(
         "software-products/<int:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="softwareproduct_changelog",
         kwargs={"model": SoftwareProduct},
     ),
 
-    # Software Product Versions
-    path("versions/", views.SoftwareProductVersionListView.as_view(), name='softwareproductversion_list'),
-    path("versions/add/", views.SoftwareProductVersionEditView.as_view(), name='softwareproductversion_add'),
+    # SoftwareProductVersion
+    path("versions/", views.SoftwareProductVersionListView.as_view(),
+         name='softwareproductversion_list'),
+    path("versions/add/", views.SoftwareProductVersionEditView.as_view(),
+         name='softwareproductversion_add'),
     path("versions/import/", views.SoftwareProductVersionBulkImportView.as_view(),
          name="softwareproductversion_import"),
-    path("versions/edit/", views.SoftwareProductVersionBulkEditView.as_view(), name="softwareproductversion_bulk_edit"),
+    path("versions/edit/", views.SoftwareProductVersionBulkEditView.as_view(),
+         name="softwareproductversion_bulk_edit"),
     path("versions/delete/", views.SoftwareProductVersionBulkDeleteView.as_view(),
          name="softwareproductversion_bulk_delete"),
-    path("versions/<int:pk>/", views.SoftwareProductVersionView.as_view(), name="softwareproductversion"),
+    path("versions/<int:pk>/", views.SoftwareProductVersionView.as_view(),
+         name="softwareproductversion"),
     path("versions/<int:pk>/delete/", views.SoftwareProductVersionDeleteView.as_view(),
          name="softwareproductversion_delete"),
-    path("versions/<int:pk>/edit/", views.SoftwareProductVersionEditView.as_view(), name="softwareproductversion_edit"),
+    path("versions/<int:pk>/edit/", views.SoftwareProductVersionEditView.as_view(),
+         name="softwareproductversion_edit"),
     path(
         "versions/<int:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="softwareproductversion_changelog",
         kwargs={"model": SoftwareProductVersion},
     ),
 
-    # Software Product Versions
+    # SoftwareProductInstallation
     path("installations/", views.SoftwareProductInstallationListView.as_view(),
          name='softwareproductinstallation_list'),
     path("installations/add/", views.SoftwareProductInstallationEditView.as_view(),
          name='softwareproductinstallation_add'),
     path("installations/import/", views.SoftwareProductInstallationBulkImportView.as_view(),
          name="softwareproductinstallation_import"),
     path("installations/edit/", views.SoftwareProductInstallationBulkEditView.as_view(),
@@ -61,8 +72,32 @@
          name="softwareproductinstallation_edit"),
     path(
         "installations/<int:pk>/changelog/",
         ObjectChangeLogView.as_view(),
         name="softwareproductinstallation_changelog",
         kwargs={"model": SoftwareProductInstallation},
     ),
+
+    # SoftwareLicense
+    path("licenses/", views.SoftwareLicenseListView.as_view(),
+         name='softwarelicense_list'),
+    path("licenses/add/", views.SoftwareLicenseEditView.as_view(),
+         name='softwarelicense_add'),
+    path("licenses/import/", views.SoftwareLicenseBulkImportView.as_view(),
+         name="softwarelicense_import"),
+    path("licenses/edit/", views.SoftwareLicenseBulkEditView.as_view(),
+         name="softwarelicense_bulk_edit"),
+    path("licenses/delete/", views.SoftwareLicenseBulkDeleteView.as_view(),
+         name="softwarelicense_bulk_delete"),
+    path("licenses/<int:pk>/", views.SoftwareLicenseView.as_view(),
+         name="softwarelicense"),
+    path("licenses/<int:pk>/delete/", views.SoftwareLicenseDeleteView.as_view(),
+         name="softwarelicense_delete"),
+    path("licenses/<int:pk>/edit/", views.SoftwareLicenseEditView.as_view(),
+         name="softwarelicense_edit"),
+    path(
+        "licenses/<int:pk>/changelog/",
+        ObjectChangeLogView.as_view(),
+        name="softwarelicense_changelog",
+        kwargs={"model": SoftwareLicense},
+    ),
 ]
```

### Comparing `netbox-slm-1.3/netbox_slm.egg-info/PKG-INFO` & `netbox-slm-1.4/netbox_slm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-Metadata-Version: 2.1
-Name: netbox-slm
-Version: 1.3
-Summary: Software Lifecycle Management Netbox Plugin.
-Author: ICTU
-Author-email: open-source-projects@ictu.nl
-License: Apache 2.0
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.9
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: netbox-slm
+Version: 1.4
+Summary: Software Lifecycle Management Netbox Plugin.
+Home-page: UNKNOWN
+Author: ICTU
+Author-email: open-source-projects@ictu.nl
+License: Apache 2.0
+Platform: UNKNOWN
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Python: >=3.9
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `netbox-slm-1.3/netbox_slm.egg-info/SOURCES.txt` & `netbox-slm-1.4/netbox_slm.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,32 +2,42 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 netbox_slm/__init__.py
 netbox_slm/admin.py
 netbox_slm/filtersets.py
-netbox_slm/forms.py
 netbox_slm/models.py
 netbox_slm/navigation.py
 netbox_slm/tables.py
 netbox_slm/urls.py
-netbox_slm/views.py
 netbox_slm.egg-info/PKG-INFO
 netbox_slm.egg-info/SOURCES.txt
 netbox_slm.egg-info/dependency_links.txt
 netbox_slm.egg-info/top_level.txt
 netbox_slm/api/__init__.py
 netbox_slm/api/serializers.py
 netbox_slm/api/urls.py
 netbox_slm/api/views.py
+netbox_slm/forms/__init__.py
+netbox_slm/forms/software_license.py
+netbox_slm/forms/software_product.py
+netbox_slm/forms/software_product_installation.py
+netbox_slm/forms/software_product_version.py
 netbox_slm/migrations/0001_initial.py
 netbox_slm/migrations/0002_alter_softwareproduct_manufacturer.py
 netbox_slm/migrations/0003_auto_20220407_1209.py
 netbox_slm/migrations/0004_auto_20220415_0705.py
+netbox_slm/migrations/0005_add_software_license.py
 netbox_slm/migrations/__init__.py
+netbox_slm/templates/netbox_slm/softwarelicense.html
 netbox_slm/templates/netbox_slm/softwareproduct.html
 netbox_slm/templates/netbox_slm/softwareproductinstallation.html
 netbox_slm/templates/netbox_slm/softwareproductversion.html
 netbox_slm/templatetags/__init__.py
 netbox_slm/tests/__init__.py
-netbox_slm/tests/test_models.py
+netbox_slm/tests/test_models.py
+netbox_slm/views/__init__.py
+netbox_slm/views/software_license.py
+netbox_slm/views/software_product.py
+netbox_slm/views/software_product_installation.py
+netbox_slm/views/software_product_version.py
```

### Comparing `netbox-slm-1.3/setup.cfg` & `netbox-slm-1.4/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6e65 7462 6f78 2d73 6c6d 0a76 6572  = netbox-slm.ver
-00000020: 7369 6f6e 203d 2031 2e33 0a64 6573 6372  sion = 1.3.descr
-00000030: 6970 7469 6f6e 203d 2053 6f66 7477 6172  iption = Softwar
-00000040: 6520 4c69 6665 6379 636c 6520 4d61 6e61  e Lifecycle Mana
-00000050: 6765 6d65 6e74 204e 6574 626f 7820 506c  gement Netbox Pl
-00000060: 7567 696e 2e0a 6175 7468 6f72 203d 2049  ugin..author = I
-00000070: 4354 550a 6175 7468 6f72 5f65 6d61 696c  CTU.author_email
-00000080: 203d 206f 7065 6e2d 736f 7572 6365 2d70   = open-source-p
-00000090: 726f 6a65 6374 7340 6963 7475 2e6e 6c0a  rojects@ictu.nl.
-000000a0: 6c69 6365 6e73 6520 3d20 4170 6163 6865  license = Apache
-000000b0: 2032 2e30 0a63 6c61 7373 6966 6965 7273   2.0.classifiers
-000000c0: 203d 200a 0945 6e76 6972 6f6e 6d65 6e74   = ..Environment
-000000d0: 203a 3a20 5765 6220 456e 7669 726f 6e6d   :: Web Environm
-000000e0: 656e 740a 0946 7261 6d65 776f 726b 203a  ent..Framework :
-000000f0: 3a20 446a 616e 676f 0a09 496e 7465 6e64  : Django..Intend
-00000100: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-00000110: 6576 656c 6f70 6572 730a 094c 6963 656e  evelopers..Licen
-00000120: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000130: 6564 203a 3a20 4170 6163 6865 2053 6f66  ed :: Apache Sof
-00000140: 7477 6172 6520 4c69 6365 6e73 650a 094f  tware License..O
-00000150: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000160: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000170: 740a 0950 726f 6772 616d 6d69 6e67 204c  t..Programming L
-00000180: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000190: 6e0a 0950 726f 6772 616d 6d69 6e67 204c  n..Programming L
-000001a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001b0: 6e20 3a3a 2033 0a09 5072 6f67 7261 6d6d  n :: 3..Programm
-000001c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001d0: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
-000001e0: 6e6c 790a 0950 726f 6772 616d 6d69 6e67  nly..Programming
-000001f0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000200: 686f 6e20 3a3a 2033 2e39 0a09 5072 6f67  hon :: 3.9..Prog
-00000210: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000220: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000230: 3130 0a09 5072 6f67 7261 6d6d 696e 6720  10..Programming 
-00000240: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000250: 6f6e 203a 3a20 332e 3131 0a09 546f 7069  on :: 3.11..Topi
-00000260: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-00000270: 2057 5757 2f48 5454 500a 0954 6f70 6963   WWW/HTTP..Topic
-00000280: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
-00000290: 5757 572f 4854 5450 203a 3a20 4479 6e61  WWW/HTTP :: Dyna
-000002a0: 6d69 6320 436f 6e74 656e 740a 0a5b 6f70  mic Content..[op
-000002b0: 7469 6f6e 735d 0a69 6e63 6c75 6465 5f70  tions].include_p
-000002c0: 6163 6b61 6765 5f64 6174 6120 3d20 7472  ackage_data = tr
-000002d0: 7565 0a70 6163 6b61 6765 7320 3d20 6669  ue.packages = fi
-000002e0: 6e64 3a0a 7079 7468 6f6e 5f72 6571 7569  nd:.python_requi
-000002f0: 7265 7320 3d20 3e3d 332e 390a 0a5b 6567  res = >=3.9..[eg
-00000300: 675f 696e 666f 5d0a 7461 675f 6275 696c  g_info].tag_buil
-00000310: 6420 3d20 0a74 6167 5f64 6174 6520 3d20  d = .tag_date = 
-00000320: 300a 0a                                  0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 206e 6574 626f 782d 736c 6d0d 0a76   = netbox-slm..v
+00000020: 6572 7369 6f6e 203d 2031 2e34 0d0a 6465  ersion = 1.4..de
+00000030: 7363 7269 7074 696f 6e20 3d20 536f 6674  scription = Soft
+00000040: 7761 7265 204c 6966 6563 7963 6c65 204d  ware Lifecycle M
+00000050: 616e 6167 656d 656e 7420 4e65 7462 6f78  anagement Netbox
+00000060: 2050 6c75 6769 6e2e 0d0a 6175 7468 6f72   Plugin...author
+00000070: 203d 2049 4354 550d 0a61 7574 686f 725f   = ICTU..author_
+00000080: 656d 6169 6c20 3d20 6f70 656e 2d73 6f75  email = open-sou
+00000090: 7263 652d 7072 6f6a 6563 7473 4069 6374  rce-projects@ict
+000000a0: 752e 6e6c 0d0a 6c69 6365 6e73 6520 3d20  u.nl..license = 
+000000b0: 4170 6163 6865 2032 2e30 0d0a 636c 6173  Apache 2.0..clas
+000000c0: 7369 6669 6572 7320 3d20 0d0a 0945 6e76  sifiers = ...Env
+000000d0: 6972 6f6e 6d65 6e74 203a 3a20 5765 6220  ironment :: Web 
+000000e0: 456e 7669 726f 6e6d 656e 740d 0a09 4672  Environment...Fr
+000000f0: 616d 6577 6f72 6b20 3a3a 2044 6a61 6e67  amework :: Djang
+00000100: 6f0d 0a09 496e 7465 6e64 6564 2041 7564  o...Intended Aud
+00000110: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00000120: 6572 730d 0a09 4c69 6365 6e73 6520 3a3a  ers...License ::
+00000130: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000140: 2041 7061 6368 6520 536f 6674 7761 7265   Apache Software
+00000150: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+00000160: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00000170: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
+00000180: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000190: 7561 6765 203a 3a20 5079 7468 6f6e 0d0a  uage :: Python..
+000001a0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000001b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000001c0: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
+000001d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001e0: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
+000001f0: 6c79 0d0a 0950 726f 6772 616d 6d69 6e67  ly...Programming
+00000200: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000210: 686f 6e20 3a3a 2033 2e39 0d0a 0950 726f  hon :: 3.9...Pro
+00000220: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000230: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000240: 2e31 300d 0a09 5072 6f67 7261 6d6d 696e  .10...Programmin
+00000250: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000260: 7468 6f6e 203a 3a20 332e 3131 0d0a 0954  thon :: 3.11...T
+00000270: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+00000280: 203a 3a20 5757 572f 4854 5450 0d0a 0954   :: WWW/HTTP...T
+00000290: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+000002a0: 203a 3a20 5757 572f 4854 5450 203a 3a20   :: WWW/HTTP :: 
+000002b0: 4479 6e61 6d69 6320 436f 6e74 656e 740d  Dynamic Content.
+000002c0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 696e  ...[options]..in
+000002d0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+000002e0: 7461 203d 2074 7275 650d 0a70 6163 6b61  ta = true..packa
+000002f0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+00000300: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000310: 3d33 2e39 0d0a 0d0a 5b65 6767 5f69 6e66  =3.9....[egg_inf
+00000320: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000330: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000340: 0d0a                                     ..
```

