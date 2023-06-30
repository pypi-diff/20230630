# Comparing `tmp/netbox-cisco-support-plugin-0.0.8.tar.gz` & `tmp/netbox-cisco-support-plugin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-support-plugin-0.0.8.tar", last modified: Fri Jun 23 14:53:19 2023, max compression
+gzip compressed data, was "netbox-cisco-support-plugin-0.0.9.tar", last modified: Fri Jun 23 15:12:12 2023, max compression
```

## Comparing `netbox-cisco-support-plugin-0.0.8.tar` & `netbox-cisco-support-plugin-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.840448 netbox-cisco-support-plugin-0.0.8/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     5431 2023-06-23 14:53:19.840448 netbox-cisco-support-plugin-0.0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4785 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.836448 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1665 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.836448 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/api/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2424 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/api/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/api/urls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      695 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/api/views.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4395 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/filtersets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10150 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.836448 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.836448 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    43551 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.840448 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)     3497 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)      400 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/0003_rename_model_ciscodevicesupport_pid.py
--rw-r--r--   0 vsts      (1001) docker     (123)      832 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1101 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6845 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/navigation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3925 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1844 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.832448 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.840448 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)     6359 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     3458 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.840448 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2714 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1105 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/urls.py
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1739 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/views.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 14:53:19.836448 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5431 2023-06-23 14:53:19.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1851 2023-06-23 14:53:19.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-23 14:53:19.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-23 14:53:19.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-23 14:53:19.000000 netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-23 14:53:19.840448 netbox-cisco-support-plugin-0.0.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1568 2023-06-23 14:53:02.000000 netbox-cisco-support-plugin-0.0.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.510300 netbox-cisco-support-plugin-0.0.9/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     5431 2023-06-23 15:12:12.510300 netbox-cisco-support-plugin-0.0.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4785 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.502299 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      645 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1665 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.506300 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2424 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/api/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/api/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      695 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/api/views.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4395 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/filtersets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10150 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.506300 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.506300 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    43551 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.510300 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3497 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      400 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/0003_rename_model_ciscodevicesupport_pid.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      832 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1101 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6845 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/navigation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3925 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1844 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.498299 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.510300 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6359 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3458 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.510300 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2688 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1105 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1739 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/views.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-23 15:12:12.506300 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5431 2023-06-23 15:12:12.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1851 2023-06-23 15:12:12.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-23 15:12:12.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-23 15:12:12.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-06-23 15:12:12.000000 netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-23 15:12:12.510300 netbox-cisco-support-plugin-0.0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1568 2023-06-23 15:11:55.000000 netbox-cisco-support-plugin-0.0.9/setup.py
```

### Comparing `netbox-cisco-support-plugin-0.0.8/LICENSE` & `netbox-cisco-support-plugin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/PKG-INFO` & `netbox-cisco-support-plugin-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-support-plugin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-support-plugin-0.0.8/README.md` & `netbox-cisco-support-plugin-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/__init__.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/admin.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/api/serializers.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/api/views.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/filtersets.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/forms.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/0001_initial.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/models.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/tables.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/template_content.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/templatetags/filters.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/templatetags/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 @register.filter(is_safe=True)
 def coverage_class(value):
     """
     Set CSS class for text fields
     """
-    if not value or value == "None" or value is None or "Not covered" in value:
+    if not value or value == "None" or value is None:
         return mark_safe('class="danger"')
 
 
 @register.filter(is_safe=True)
 def coverage_class_boolian(value):
     """
     Set CSS class for boolian fields to display a green thick or a red cross
```

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/urls.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin/views.py` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin.egg-info/PKG-INFO` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-support-plugin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-support-plugin-0.0.8/netbox_cisco_support_plugin.egg-info/SOURCES.txt` & `netbox-cisco-support-plugin-0.0.9/netbox_cisco_support_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.8/setup.py` & `netbox-cisco-support-plugin-0.0.9/setup.py`

 * *Files identical despite different names*

