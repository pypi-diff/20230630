# Comparing `tmp/arivo-settings_models-0.0.1rc3.tar.gz` & `tmp/arivo-settings_models-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arivo-settings_models-0.0.1rc3.tar", last modified: Wed Jun 28 13:41:44 2023, max compression
+gzip compressed data, was "dist/arivo-settings_models-0.0.1rc4.tar", last modified: Fri Jun 30 09:21:26 2023, max compression
```

## Comparing `arivo-settings_models-0.0.1rc3.tar` & `arivo-settings_models-0.0.1rc4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc3/.coveragerc
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/AUTHORS
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/settings_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc3/settings_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc3/settings_models/validators.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc3/settings_models/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/settings_models/settings/
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc3/settings_models/settings/gate_control.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc3/settings_models/settings/intercom.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc3/settings_models/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc3/settings_models/settings/enforcement.py
--rw-rw-rw-   0 root         (0) root         (0)    20238 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc3/settings_models/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc3/settings_models/settings/device_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc3/settings_models/_combat.py
--rw-rw-rw-   0 root         (0) root         (0)     6344 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc3/settings_models/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc3/tox.ini
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-22 11:55:45.000000 arivo-settings_models-0.0.1rc3/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/tools/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc3/tools/pages.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc3/tests/test_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)    38588 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc3/tests/test_validation.py
--rw-rw-rw-   0 root         (0) root         (0)    11501 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc3/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc3/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc3/README.md
--rw-r--r--   0 root         (0) root         (0)     1318 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc3/test-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/docs/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc3/docs/migrations.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      922 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-28 13:41:44.000000 arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      707 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      922 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/settings_models/
+-rw-rw-rw-   0 root         (0) root         (0)     6344 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/intercom.py
+-rw-rw-rw-   0 root         (0) root         (0)    20317 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/gate_control.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/enforcement.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/settings/device_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/doc.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/_combat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/settings_models/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tox.ini
+-rw-r--r--   0 root         (0) root         (0)      707 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/docs/migrations.md
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/test-requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11501 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    37784 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tests/test_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tests/test_serialization.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/ChangeLog
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 09:21:26.000000 arivo-settings_models-0.0.1rc4/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-30 09:21:10.000000 arivo-settings_models-0.0.1rc4/tools/pages.py
```

### Comparing `arivo-settings_models-0.0.1rc3/settings_models/validators.py` & `arivo-settings_models-0.0.1rc4/settings_models/validators.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc3/settings_models/settings/gate_control.py` & `arivo-settings_models-0.0.1rc4/settings_models/settings/gate_control.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc3/settings_models/settings/common.py` & `arivo-settings_models-0.0.1rc4/settings_models/settings/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 
     door = "door"
     """
     Door: Gate without LPR where people can walk into the parking lot. 
     No check-in or check-out, only access check
     """
 
-    transit_freeflow = "transit_freeflow"
+    transit_access_check = "transit_access_check"
     """
-    Gate separating parts within a parking lot. No check-in, check-out or access check. 
-    Movements are used in passage control (someone is not parking in the wrong area) and for logging
+    Gate with barrier where vehicles can pass depending on access rights specified by the gate list in parksetting or
+    shortterm_gates in parking_area. This is a well defined functionality of the controller.
     """
 
-    transit_barrier = "transit_barrier"
+    transit_custom = "transit_custom"
     """
-    Gate with barrier separating parts within a parking lot. No check-in, check-out. 
-    Access check is done at the gate, so only permitted users can enter an area within the parking lot
-    Movements are used in passage control (someone is not parking in the wrong area) and for logging
+    Gates with custom behavior. These gates might or might not have a barrier. Examples are: 
+      - Passage check gates (permanent parkers must pass this gate or gets fined)
+      - Gate with shortterm count check (e.g. only 10 shortterm parkers are allowed at the same time)
+      - automatic gates (e.g. exit of restricted subarea)
+    Behavior of those gates is not implemented by the controller
     """
 
 
 class RefsModel(SettingsModel):
     """
     Model for used keys of a Dict setting like parksettings
     """
@@ -217,17 +219,16 @@
 class Parksetting(SettingsModel):
     """
     Defines the terms and conditions for parking sessions of registered users. This is not used for registered
     shortterm parkers.
     """
     id: str = Field(..., description="Id of the parksetting. UUID string in canonical textual representation")
     name: str = Field(..., description="Name for UIs", max_length=126)
-    gates: Optional[List[str]] = Field(..., description="Gates this parksetting is valid for (only types entry, exit, "
-                                                        "bidirectional or transit_barrier/transit_access_check",
-                                       min_items=1)
+    gates: List[str] = Field(..., description="Gates this parksetting is valid for (only types entry, exit, "
+                                              "bidirectional or transit_barrier/transit_access_check", min_items=1)
     default_cost_entries: List[CostEntryData] = Field(..., description="Default cost entries added on entry. "
                                                                        "Empty list is free.")
 
     id_validator = uuid_validator("id")
 
     @validator('default_cost_entries', each_item=True)
     def cost_entry_validator(cls, cost_entry):
```

### Comparing `arivo-settings_models-0.0.1rc3/settings_models/settings/device_keys.py` & `arivo-settings_models-0.0.1rc4/settings_models/settings/device_keys.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc3/settings_models/serialization.py` & `arivo-settings_models-0.0.1rc4/settings_models/serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc3/PKG-INFO` & `arivo-settings_models-0.0.1rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings_models
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-0.0.1rc3/.gitlab-ci.yml` & `arivo-settings_models-0.0.1rc4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc3/setup.cfg` & `arivo-settings_models-0.0.1rc4/setup.cfg`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc3/tests/test_serialization.py` & `arivo-settings_models-0.0.1rc4/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc3/tests/test_validation.py` & `arivo-settings_models-0.0.1rc4/tests/test_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,29 +46,14 @@
                 "gates": ["gate1"],
                 "default_cost_entries": [{"entry_type": "static_cost", "value": 123,
                                           "group": "parking_default", "account_id": "0"}]}
         })
         res = parse_setting("common/parksettings2", gt)
         self.assert_result(dump_setting(res), gt)
 
-    def test_parksettings_gates_none_success(self):
-        self.maxDiff = None
-        gt = dump_setting({
-            "896150c9-5616-4406-a544-84c3824cfea9": {
-                "id": "896150c9-5616-4406-a544-84c3824cfea9", "name": "Dauerparker mit variablen Kosten",
-                "gates": None, "default_cost_entries": []},
-            "12e8a7e2-be78-488e-8d1a-1486f7da2179": {
-                "id": "12e8a7e2-be78-488e-8d1a-1486f7da2179", "name": "Dauerparker ohne Kosten",
-                "gates": None,
-                "default_cost_entries": [{"entry_type": "static_cost", "value": 123,
-                                          "group": "parking_default", "account_id": "0"}]}
-        })
-        res = parse_setting("common/parksettings2", gt)
-        self.assert_result(dump_setting(res), gt)
-
     def test_parksettings_gates_no_empty_list(self):
         self.maxDiff = None
         with self.assertRaises(ValidationError) as e:
             gt = dump_setting({
                 "896150c9-5616-4406-a544-84c3824cfea9": {
                     "id": "896150c9-5616-4406-a544-84c3824cfea9", "name": "Dauerparker mit variablen Kosten",
                     "gates": [], "default_cost_entries": []}})
```

### Comparing `arivo-settings_models-0.0.1rc3/tests/test_models.py` & `arivo-settings_models-0.0.1rc4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc3/tests/utils.py` & `arivo-settings_models-0.0.1rc4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc3/ChangeLog` & `arivo-settings_models-0.0.1rc4/ChangeLog`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+v0.0.1rc4
+---------
+
+* parksettings must have gates specified (again) changed comments for gate types
+* renamed GateType enums
+
 v0.0.1rc3
 ---------
 
 * Parksettings with null gates allowed
 
 v0.0.1rc2
 ---------
@@ -54,9 +60,7 @@
 
 * added testcase for refs
 * coverage fix
 * removing pages stage because no documentation yet
 * settings models and parsing/serializing
 * committing before weekend [skip ci]
 * test something
-* npm version check
-* trying ci and pages and first part of implementation
```

### Comparing `arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/PKG-INFO` & `arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings-models
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-0.0.1rc3/arivo_settings_models.egg-info/SOURCES.txt` & `arivo-settings_models-0.0.1rc4/arivo_settings_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

