# Comparing `tmp/plugp100-2.5.1.tar.gz` & `tmp/plugp100-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugp100-2.5.1.tar", last modified: Mon Jan 30 22:16:07 2023, max compression
+gzip compressed data, was "plugp100-3.0.0.tar", last modified: Fri Jun 30 06:29:54 2023, max compression
```

## Comparing `plugp100-2.5.1.tar` & `plugp100-3.0.0.tar`

### file list

```diff
@@ -1,56 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.253799 plugp100-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-30 22:15:57.000000 plugp100-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-30 22:15:57.000000 plugp100-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-30 22:16:07.253799 plugp100-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-01-30 22:15:57.000000 plugp100-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.249799 plugp100-2.5.1/plugp100/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.249799 plugp100-2.5.1/plugp100/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/api/tapo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/discover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.249799 plugp100-2.5.1/plugp100/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/domain/energy_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/domain/light_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/domain/power_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/domain/tapo_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/domain/tapo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/domain/tapo_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.249799 plugp100-2.5.1/plugp100/tapo_protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.249799 plugp100-2.5.1/plugp100/tapo_protocol/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/encryption/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/encryption/key_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/encryption/tp_link_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.249799 plugp100-2.5.1/plugp100/tapo_protocol/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/get_current_power.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/get_device_info_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/get_energy_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/handshake_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/login_device_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/secure_passthrough_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/set_device_info_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/set_lighting_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/methods/taporequest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.249799 plugp100-2.5.1/plugp100/tapo_protocol/params/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/params/device_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/params/handshake_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/params/login_device_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/tapo_protocol/tapo_protocol_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.249799 plugp100-2.5.1/plugp100/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-01-30 22:15:57.000000 plugp100-2.5.1/plugp100/utils/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 22:16:07.249799 plugp100-2.5.1/plugp100.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-30 22:16:07.000000 plugp100-2.5.1/plugp100.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-30 22:16:07.000000 plugp100-2.5.1/plugp100.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 22:16:07.000000 plugp100-2.5.1/plugp100.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-30 22:16:07.000000 plugp100-2.5.1/plugp100.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-30 22:16:07.000000 plugp100-2.5.1/plugp100.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-30 22:15:57.000000 plugp100-2.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-30 22:16:07.253799 plugp100-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-01-30 22:15:57.000000 plugp100-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.495865 plugp100-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-30 06:29:42.000000 plugp100-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 06:29:42.000000 plugp100-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-30 06:29:54.495865 plugp100-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-30 06:29:42.000000 plugp100-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/ledstrip_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/light_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/light_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/light_effect_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/plug_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/api/tapo_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/common/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/functional/either.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/common/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/discover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/encryption/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/encryption/key_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/encryption/tp_link_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/handshake_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/login_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/secure_passthrough_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.495865 plugp100-3.0.0/plugp100/requests/set_device_info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/set_device_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/set_device_info/set_light_color_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/set_device_info/set_light_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/set_device_info/set_plug_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/requests/tapo_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.495865 plugp100-3.0.0/plugp100/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/child_device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/energy_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/power_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/tapo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-30 06:29:42.000000 plugp100-3.0.0/plugp100/responses/tapo_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:29:54.491865 plugp100-3.0.0/plugp100.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 06:29:54.000000 plugp100-3.0.0/plugp100.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 06:29:42.000000 plugp100-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 06:29:54.495865 plugp100-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-30 06:29:42.000000 plugp100-3.0.0/setup.py
```

### Comparing `plugp100-2.5.1/LICENSE` & `plugp100-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plugp100-2.5.1/PKG-INFO` & `plugp100-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 2.5.1
+Version: 3.0.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
@@ -22,15 +22,15 @@
 
 # Code example
 
 ```python
 import asyncio
 
 from plugp100 import TapoApiClient, TapoApiClientConfig
-from plugp100.domain.light_effect import LightEffectPreset
+from plugp100.api.light_effect import LightEffectPreset
 
 
 async def main():
     # create generic tapo api
     config = TapoApiClientConfig("<ip>", "<email>", "<passwd>")
     sw = TapoApiClient.from_config(config)
     await sw.login()
```

### Comparing `plugp100-2.5.1/README.md` & `plugp100-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Code example
 
 ```python
 import asyncio
 
 from plugp100 import TapoApiClient, TapoApiClientConfig
-from plugp100.domain.light_effect import LightEffectPreset
+from plugp100.api.light_effect import LightEffectPreset
 
 
 async def main():
     # create generic tapo api
     config = TapoApiClientConfig("<ip>", "<email>", "<passwd>")
     sw = TapoApiClient.from_config(config)
     await sw.login()
```

### Comparing `plugp100-2.5.1/plugp100/domain/energy_info.py` & `plugp100-3.0.0/plugp100/responses/energy_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,8 +11,7 @@
     current_power: float = property(lambda self: self.info["current_power"])
 
     def __init__(self, info: Dict[str, Any]):
         self.info = info
 
     def get_unmapped_state(self):
         return self.info
-
```

### Comparing `plugp100-2.5.1/plugp100/domain/light_effect.py` & `plugp100-3.0.0/plugp100/api/light_effect.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,244 +1,266 @@
 import dataclasses
-from typing import Optional
+from typing import Optional, List
 
-from plugp100.tapo_protocol.params import LightEffectData
 
-
-@dataclasses.dataclass()
-class LightEffectPreset:
+@dataclasses.dataclass
+class LightEffect:
+    id: str
     name: str
-    effect: LightEffectData
-
-    def __init__(self, effect: LightEffectData, name: Optional[str] = None):
-        self.effect = effect
-        self.name = self.effect.name.lower() if name is None else name
-
-    @staticmethod
-    def bubbling_calderon() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_6DlumDwO2NdfHppy50vJtu', name='Bubbling Cauldron', brightness=100,
-                                   display_colors=[[100, 100, 100], [270, 100, 100]], enable=1, bAdjusted=None,
-                                   brightness_range=[50, 100], backgrounds=[[270, 40, 50]], custom=0, direction=None,
-                                   duration=0, expansion_strategy=1, fadeoff=1000, hue_range=[100, 270],
-                                   init_states=[[270, 100, 100]], random_seed=24, repeat_times=None,
-                                   saturation_range=[80, 100], segment_length=None, segments=[0], sequence=None,
-                                   spread=None, transition=200, transition_range=None, type='random',
-                                   trans_sequence=None, run_time=None)
-        )
-
-    @staticmethod
-    def aurora() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_1MClvV18i15Jq3bvJVf0eP', name='Aurora', brightness=100,
-                                   display_colors=[[120, 100, 100], [240, 100, 100], [260, 100, 100], [280, 100, 100]],
-                                   enable=1, bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=4,
-                                   duration=0, expansion_strategy=1, fadeoff=None, hue_range=None, init_states=[],
-                                   random_seed=None, repeat_times=0, saturation_range=None, segment_length=None,
-                                   segments=[0],
-                                   sequence=[[120, 100, 100], [240, 100, 100], [260, 100, 100], [280, 100, 100]],
-                                   spread=7, transition=1500, transition_range=None, type='sequence',
-                                   trans_sequence=None, run_time=None)
-        )
-
-    @staticmethod
-    def candy_cane() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_6Dy0Nc45vlhFPEzG021Pe9', name='Candy Cane', brightness=100,
-                                   display_colors=[[0, 0, 100], [360, 81, 100]], enable=1, bAdjusted=None,
-                                   brightness_range=[], backgrounds=[], custom=0, direction=1, duration=700,
-                                   expansion_strategy=1, fadeoff=None, hue_range=None, init_states=[], random_seed=None,
-                                   repeat_times=0, saturation_range=None, segment_length=None,
-                                   segments=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15],
-                                   sequence=[[0, 0, 100], [0, 0, 100], [360, 81, 100], [0, 0, 100], [0, 0, 100],
-                                             [360, 81, 100], [360, 81, 100], [0, 0, 100], [0, 0, 100], [360, 81, 100],
-                                             [360, 81, 100], [360, 81, 100], [360, 81, 100], [0, 0, 100], [0, 0, 100],
-                                             [360, 81, 100]], spread=1, transition=500, transition_range=None,
-                                   type='sequence')
-        )
-
-    @staticmethod
-    def christmas() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_5zkiG6avJ1IbhjiZbRlWvh', name='Christmas', brightness=100,
-                                   display_colors=[[136, 98, 100], [350, 97, 100]], enable=1, bAdjusted=None,
-                                   brightness_range=[50, 100],
-                                   backgrounds=[[136, 98, 75], [136, 0, 0], [350, 0, 100], [350, 97, 94]], custom=0,
-                                   direction=None, duration=5000, expansion_strategy=1, fadeoff=2000,
-                                   hue_range=[136, 146], init_states=[[136, 0, 100]], random_seed=100,
-                                   repeat_times=None, saturation_range=[90, 100], segment_length=None, segments=[0],
-                                   sequence=None, spread=None, transition=0, transition_range=None, type='random')
-        )
-
-    @staticmethod
-    def flicker() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_4HVKmMc6vEzjm36jXaGwMs', name='Flicker', brightness=100,
-                                   display_colors=[[30, 81, 100], [40, 100, 100]], enable=1, bAdjusted=None,
-                                   brightness_range=[50, 100], backgrounds=[], custom=0, direction=None, duration=0,
-                                   expansion_strategy=1, fadeoff=None, hue_range=[30, 40], init_states=[[30, 81, 80]],
-                                   random_seed=None, repeat_times=None, saturation_range=[100, 100],
-                                   segment_length=None, segments=[1], sequence=None, spread=None, transition=0,
-                                   transition_range=[375, 500], type='random')
-        )
-
-    @staticmethod
-    def christmas_light() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_3Gk6CmXOXbjCiwz9iD543C', name="Grandma's Christmas Lights",
-                                   brightness=100,
-                                   display_colors=[[30, 100, 100], [240, 100, 100], [130, 100, 100], [0, 100, 100]],
-                                   enable=1, bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=1,
-                                   duration=5000, expansion_strategy=1, fadeoff=None, hue_range=None, init_states=[],
-                                   random_seed=None, repeat_times=0, saturation_range=None, segment_length=None,
-                                   segments=[0],
-                                   sequence=[[30, 100, 100], [30, 0, 0], [30, 0, 0], [240, 100, 100], [240, 0, 0],
-                                             [240, 0, 0], [240, 0, 100], [240, 0, 0], [240, 0, 0], [130, 100, 100],
-                                             [130, 0, 0], [130, 0, 0], [0, 100, 100], [0, 0, 0], [0, 0, 0]], spread=1,
-                                   transition=100, transition_range=None, type='sequence')
-        )
-
-    @staticmethod
-    def hanukkah() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_2YTk4wramLKv5XZ9KFDVYm', name='Hanukkah', brightness=100,
-                                   display_colors=[[200, 100, 100]], enable=1, bAdjusted=None,
-                                   brightness_range=[50, 100], backgrounds=[], custom=0, direction=None, duration=1500,
-                                   expansion_strategy=1, fadeoff=None, hue_range=[200, 210], init_states=[[35, 81, 80]],
-                                   random_seed=None, repeat_times=None, saturation_range=[0, 100], segment_length=None,
-                                   segments=[1], sequence=None, spread=None, transition=0, transition_range=[400, 500],
-                                   type='random')
-        )
-
-    @staticmethod
-    def haunted_mansion() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_4rJ6JwC7I9st3tQ8j4lwlI', name='Haunted Mansion', brightness=100,
-                                   display_colors=[[45, 10, 100]], enable=1, bAdjusted=None, brightness_range=[0, 80],
-                                   backgrounds=[[45, 10, 100]], custom=0, direction=None, duration=0,
-                                   expansion_strategy=2, fadeoff=200, hue_range=[45, 45], init_states=[[45, 10, 100]],
-                                   random_seed=1, repeat_times=None, saturation_range=[10, 10], segment_length=None,
-                                   segments=[80], sequence=None, spread=None, transition=0, transition_range=[50, 1500],
-                                   type='random')
-        )
-
-    @staticmethod
-    def icicle() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_7UcYLeJbiaxVIXCxr21tpx', name='Icicle', brightness=100,
-                                   display_colors=[[190, 100, 100]], enable=1, bAdjusted=None, brightness_range=[],
-                                   backgrounds=[], custom=0, direction=4, duration=0, expansion_strategy=1,
-                                   fadeoff=None, hue_range=None, init_states=[], random_seed=None, repeat_times=0,
-                                   saturation_range=None, segment_length=None, segments=[0],
-                                   sequence=[[190, 100, 70], [190, 100, 70], [190, 30, 50], [190, 100, 70],
-                                             [190, 100, 70]], spread=3, transition=400, transition_range=None,
-                                   type='sequence')
-        )
-
-    @staticmethod
-    def lightning() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_7OGzfSfnOdhoO2ri4gOHWn', name='Lightning', brightness=100,
-                                   display_colors=[[210, 10, 100], [200, 50, 100], [200, 100, 100]], enable=1,
-                                   bAdjusted=None, brightness_range=[90, 100],
-                                   backgrounds=[[200, 100, 100], [200, 50, 10], [210, 10, 50], [240, 10, 0]], custom=0,
-                                   direction=None, duration=0, expansion_strategy=1, fadeoff=150, hue_range=[240, 240],
-                                   init_states=[[240, 30, 100]], random_seed=600, repeat_times=None,
-                                   saturation_range=[10, 11], segment_length=None,
-                                   segments=[7, 20, 23, 32, 34, 35, 49, 65, 66, 74, 80], sequence=None, spread=None,
-                                   transition=50, transition_range=None, type='random')
-        )
-
-    @staticmethod
-    def ocean() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_0fOleCdwSgR0nfjkReeYfw', name='Ocean', brightness=100,
-                                   display_colors=[[198, 84, 100]], enable=1, bAdjusted=None, brightness_range=[],
-                                   backgrounds=[], custom=0, direction=3, duration=0, expansion_strategy=1,
-                                   fadeoff=None, hue_range=None, init_states=[], random_seed=None, repeat_times=0,
-                                   saturation_range=None, segment_length=None, segments=[0],
-                                   sequence=[[198, 84, 30], [198, 70, 30], [198, 10, 30]], spread=16, transition=2000,
-                                   transition_range=None, type='sequence')
-        )
-
-    @staticmethod
-    def rainbow() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_7CC5y4lsL8pETYvmz7UOpQ', name='Rainbow', brightness=100,
-                                   display_colors=[[0, 100, 100], [100, 100, 100], [200, 100, 100], [300, 100, 100]],
-                                   enable=1, bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=1,
-                                   duration=0, expansion_strategy=1, fadeoff=None, hue_range=None, init_states=[],
-                                   random_seed=None, repeat_times=0, saturation_range=None, segment_length=None,
-                                   segments=[0],
-                                   sequence=[[0, 100, 100], [100, 100, 100], [200, 100, 100], [300, 100, 100]],
-                                   spread=12, transition=1500, transition_range=None, type='sequence')
-        )
-
-    @staticmethod
-    def raindrop() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_1t2nWlTBkV8KXBZ0TWvBjs', name='Raindrop', brightness=100,
-                                   display_colors=[[200, 10, 100], [200, 20, 100]], enable=1, bAdjusted=None,
-                                   brightness_range=[10, 30], backgrounds=[[200, 40, 0]], custom=0, direction=None,
-                                   duration=0, expansion_strategy=1, fadeoff=1000, hue_range=[200, 200],
-                                   init_states=[[200, 40, 100]], random_seed=24, repeat_times=None,
-                                   saturation_range=[10, 20], segment_length=None, segments=[0], sequence=None,
-                                   spread=None, transition=1000, transition_range=None, type='random')
-        )
-
-    @staticmethod
-    def spring() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_1nL6GqZ5soOxj71YDJOlZL', name='Spring', brightness=100,
-                                   display_colors=[[0, 30, 100], [130, 100, 100]], enable=1, bAdjusted=None,
-                                   brightness_range=[90, 100], backgrounds=[[130, 100, 40]], custom=0, direction=None,
-                                   duration=600, expansion_strategy=1, fadeoff=1000, hue_range=[0, 90],
-                                   init_states=[[80, 30, 100]], random_seed=20, repeat_times=None,
-                                   saturation_range=[30, 100], segment_length=None, segments=[0], sequence=None,
-                                   spread=None, transition=0, transition_range=[2000, 6000], type='random')
-        )
-
-    @staticmethod
-    def sunrise() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_1OVSyXIsDxrt4j7OxyRvqi', name='Sunrise', brightness=100,
-                                   display_colors=[[30, 0, 100], [30, 95, 100], [0, 100, 100]], enable=1,
-                                   bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=1,
-                                   duration=600, expansion_strategy=2, fadeoff=None, hue_range=None, init_states=[],
-                                   random_seed=None, repeat_times=1, saturation_range=None, segment_length=None,
-                                   segments=[0],
-                                   sequence=[[0, 100, 5], [0, 100, 5], [10, 100, 6], [15, 100, 7], [20, 100, 8],
-                                             [20, 100, 10], [30, 100, 12], [30, 95, 15], [30, 90, 20], [30, 80, 25],
-                                             [30, 75, 30], [30, 70, 40], [30, 60, 50], [30, 50, 60], [30, 20, 70],
-                                             [30, 0, 100]], spread=1, transition=60000, transition_range=None,
-                                   type='pulse', trans_sequence=[], run_time=0)
-        )
-
-    @staticmethod
-    def sunset() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_5NiN0Y8GAUD78p4neKk9EL', name='Sunset', brightness=100,
-                                   display_colors=[[0, 100, 100], [30, 95, 100], [30, 0, 100]], enable=1,
-                                   bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=1,
-                                   duration=600, expansion_strategy=2, fadeoff=None, hue_range=None, init_states=[],
-                                   random_seed=None, repeat_times=1, saturation_range=None, segment_length=None,
-                                   segments=[0],
-                                   sequence=[[30, 0, 100], [30, 20, 100], [30, 50, 99], [30, 60, 98], [30, 70, 97],
-                                             [30, 75, 95], [30, 80, 93], [30, 90, 90], [30, 95, 85], [30, 100, 80],
-                                             [20, 100, 70], [20, 100, 60], [15, 100, 50], [10, 100, 40], [0, 100, 30],
-                                             [0, 100, 0]], spread=1, transition=60000, transition_range=None,
-                                   type='pulse', trans_sequence=[], run_time=0)
-        )
-
-    @staticmethod
-    def valentines() -> 'LightEffectPreset':
-        return LightEffectPreset(
-            effect=LightEffectData(id='TapoStrip_2q1Vio9sSjHmaC7JS9d30l', name='Valentines', brightness=100,
-                                   display_colors=[[340, 20, 100], [20, 50, 100], [0, 100, 100], [340, 40, 100]],
-                                   enable=1, bAdjusted=None, brightness_range=[90, 100],
-                                   backgrounds=[[340, 20, 50], [20, 50, 50], [0, 100, 50]], custom=0, direction=None,
-                                   duration=600, expansion_strategy=1, fadeoff=3000, hue_range=[340, 340],
-                                   init_states=[[340, 30, 100]], random_seed=100, repeat_times=None,
-                                   saturation_range=[30, 40], segment_length=None, segments=[0], sequence=None,
-                                   spread=None, transition=2000, transition_range=None, type='random',
-                                   trans_sequence=None, run_time=None)
+    brightness: int
+    display_colors: List[List[int]]
+    enable: int
+    bAdjusted: Optional[int] = None
+    brightness_range: List[int] = dataclasses.field(default_factory=list)
+    backgrounds: List[List[int]] = dataclasses.field(default_factory=list)
+    custom: Optional[int] = None
+    direction: Optional[int] = None
+    duration: Optional[int] = None
+    expansion_strategy: Optional[int] = None
+    fadeoff: Optional[int] = None
+    hue_range: Optional[List[int]] = None
+    init_states: List[List[int]] = dataclasses.field(default_factory=list)
+    random_seed: Optional[int] = None
+    repeat_times: Optional[int] = None
+    saturation_range: Optional[List[int]] = None
+    segment_length: Optional[int] = None
+    segments: Optional[List[int]] = None
+    sequence: Optional[List[List[int]]] = None
+    spread: Optional[int] = None
+    transition: Optional[int] = None
+    transition_range: Optional[List[int]] = None
+    type: Optional[str] = None
+    trans_sequence: Optional[List[int]] = None
+    run_time: Optional[int] = None
+
+    def as_dict(self):  # custom as_dict that remove None fields
+        return {k: v for k, v in dataclasses.asdict(self).items() if v is not None}
+
+    @staticmethod
+    def bubbling_calderon() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_6DlumDwO2NdfHppy50vJtu', name='Bubbling Cauldron', brightness=100,
+            display_colors=[[100, 100, 100], [270, 100, 100]], enable=1, bAdjusted=None,
+            brightness_range=[50, 100], backgrounds=[[270, 40, 50]], custom=0, direction=None,
+            duration=0, expansion_strategy=1, fadeoff=1000, hue_range=[100, 270],
+            init_states=[[270, 100, 100]], random_seed=24, repeat_times=None,
+            saturation_range=[80, 100], segment_length=None, segments=[0], sequence=None,
+            spread=None, transition=200, transition_range=None, type='random',
+            trans_sequence=None, run_time=None
+        )
+
+    @staticmethod
+    def aurora() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_1MClvV18i15Jq3bvJVf0eP', name='Aurora', brightness=100,
+            display_colors=[[120, 100, 100], [240, 100, 100], [260, 100, 100], [280, 100, 100]],
+            enable=1, bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=4,
+            duration=0, expansion_strategy=1, fadeoff=None, hue_range=None, init_states=[],
+            random_seed=None, repeat_times=0, saturation_range=None, segment_length=None,
+            segments=[0],
+            sequence=[[120, 100, 100], [240, 100, 100], [260, 100, 100], [280, 100, 100]],
+            spread=7, transition=1500, transition_range=None, type='sequence',
+            trans_sequence=None, run_time=None
+        )
+
+    @staticmethod
+    def candy_cane() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_6Dy0Nc45vlhFPEzG021Pe9', name='Candy Cane', brightness=100,
+            display_colors=[[0, 0, 100], [360, 81, 100]], enable=1, bAdjusted=None,
+            brightness_range=[], backgrounds=[], custom=0, direction=1, duration=700,
+            expansion_strategy=1, fadeoff=None, hue_range=None, init_states=[], random_seed=None,
+            repeat_times=0, saturation_range=None, segment_length=None,
+            segments=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15],
+            sequence=[[0, 0, 100], [0, 0, 100], [360, 81, 100], [0, 0, 100], [0, 0, 100],
+                      [360, 81, 100], [360, 81, 100], [0, 0, 100], [0, 0, 100], [360, 81, 100],
+                      [360, 81, 100], [360, 81, 100], [360, 81, 100], [0, 0, 100], [0, 0, 100],
+                      [360, 81, 100]], spread=1, transition=500, transition_range=None,
+            type='sequence'
+        )
+
+    @staticmethod
+    def christmas() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_5zkiG6avJ1IbhjiZbRlWvh', name='Christmas', brightness=100,
+            display_colors=[[136, 98, 100], [350, 97, 100]], enable=1, bAdjusted=None,
+            brightness_range=[50, 100],
+            backgrounds=[[136, 98, 75], [136, 0, 0], [350, 0, 100], [350, 97, 94]], custom=0,
+            direction=None, duration=5000, expansion_strategy=1, fadeoff=2000,
+            hue_range=[136, 146], init_states=[[136, 0, 100]], random_seed=100,
+            repeat_times=None, saturation_range=[90, 100], segment_length=None, segments=[0],
+            sequence=None, spread=None, transition=0, transition_range=None, type='random'
+        )
+
+    @staticmethod
+    def flicker() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_4HVKmMc6vEzjm36jXaGwMs', name='Flicker', brightness=100,
+            display_colors=[[30, 81, 100], [40, 100, 100]], enable=1, bAdjusted=None,
+            brightness_range=[50, 100], backgrounds=[], custom=0, direction=None, duration=0,
+            expansion_strategy=1, fadeoff=None, hue_range=[30, 40], init_states=[[30, 81, 80]],
+            random_seed=None, repeat_times=None, saturation_range=[100, 100],
+            segment_length=None, segments=[1], sequence=None, spread=None, transition=0,
+            transition_range=[375, 500], type='random'
+        )
+
+    @staticmethod
+    def christmas_light() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_3Gk6CmXOXbjCiwz9iD543C', name="Grandma's Christmas Lights",
+            brightness=100,
+            display_colors=[[30, 100, 100], [240, 100, 100], [130, 100, 100], [0, 100, 100]],
+            enable=1, bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=1,
+            duration=5000, expansion_strategy=1, fadeoff=None, hue_range=None, init_states=[],
+            random_seed=None, repeat_times=0, saturation_range=None, segment_length=None,
+            segments=[0],
+            sequence=[[30, 100, 100], [30, 0, 0], [30, 0, 0], [240, 100, 100], [240, 0, 0],
+                      [240, 0, 0], [240, 0, 100], [240, 0, 0], [240, 0, 0], [130, 100, 100],
+                      [130, 0, 0], [130, 0, 0], [0, 100, 100], [0, 0, 0], [0, 0, 0]], spread=1,
+            transition=100, transition_range=None, type='sequence'
+        )
+
+    @staticmethod
+    def hanukkah() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_2YTk4wramLKv5XZ9KFDVYm', name='Hanukkah', brightness=100,
+            display_colors=[[200, 100, 100]], enable=1, bAdjusted=None,
+            brightness_range=[50, 100], backgrounds=[], custom=0, direction=None, duration=1500,
+            expansion_strategy=1, fadeoff=None, hue_range=[200, 210], init_states=[[35, 81, 80]],
+            random_seed=None, repeat_times=None, saturation_range=[0, 100], segment_length=None,
+            segments=[1], sequence=None, spread=None, transition=0, transition_range=[400, 500],
+            type='random'
+        )
+
+    @staticmethod
+    def haunted_mansion() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_4rJ6JwC7I9st3tQ8j4lwlI', name='Haunted Mansion', brightness=100,
+            display_colors=[[45, 10, 100]], enable=1, bAdjusted=None, brightness_range=[0, 80],
+            backgrounds=[[45, 10, 100]], custom=0, direction=None, duration=0,
+            expansion_strategy=2, fadeoff=200, hue_range=[45, 45], init_states=[[45, 10, 100]],
+            random_seed=1, repeat_times=None, saturation_range=[10, 10], segment_length=None,
+            segments=[80], sequence=None, spread=None, transition=0, transition_range=[50, 1500],
+            type='random'
+        )
+
+    @staticmethod
+    def icicle() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_7UcYLeJbiaxVIXCxr21tpx', name='Icicle', brightness=100,
+            display_colors=[[190, 100, 100]], enable=1, bAdjusted=None, brightness_range=[],
+            backgrounds=[], custom=0, direction=4, duration=0, expansion_strategy=1,
+            fadeoff=None, hue_range=None, init_states=[], random_seed=None, repeat_times=0,
+            saturation_range=None, segment_length=None, segments=[0],
+            sequence=[[190, 100, 70], [190, 100, 70], [190, 30, 50], [190, 100, 70],
+                      [190, 100, 70]], spread=3, transition=400, transition_range=None,
+            type='sequence'
+        )
+
+    @staticmethod
+    def lightning() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_7OGzfSfnOdhoO2ri4gOHWn', name='Lightning', brightness=100,
+            display_colors=[[210, 10, 100], [200, 50, 100], [200, 100, 100]], enable=1,
+            bAdjusted=None, brightness_range=[90, 100],
+            backgrounds=[[200, 100, 100], [200, 50, 10], [210, 10, 50], [240, 10, 0]], custom=0,
+            direction=None, duration=0, expansion_strategy=1, fadeoff=150, hue_range=[240, 240],
+            init_states=[[240, 30, 100]], random_seed=600, repeat_times=None,
+            saturation_range=[10, 11], segment_length=None,
+            segments=[7, 20, 23, 32, 34, 35, 49, 65, 66, 74, 80], sequence=None, spread=None,
+            transition=50, transition_range=None, type='random'
+        )
+
+    @staticmethod
+    def ocean() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_0fOleCdwSgR0nfjkReeYfw', name='Ocean', brightness=100,
+            display_colors=[[198, 84, 100]], enable=1, bAdjusted=None, brightness_range=[],
+            backgrounds=[], custom=0, direction=3, duration=0, expansion_strategy=1,
+            fadeoff=None, hue_range=None, init_states=[], random_seed=None, repeat_times=0,
+            saturation_range=None, segment_length=None, segments=[0],
+            sequence=[[198, 84, 30], [198, 70, 30], [198, 10, 30]], spread=16, transition=2000,
+            transition_range=None, type='sequence'
+        )
+
+    @staticmethod
+    def rainbow() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_7CC5y4lsL8pETYvmz7UOpQ', name='Rainbow', brightness=100,
+            display_colors=[[0, 100, 100], [100, 100, 100], [200, 100, 100], [300, 100, 100]],
+            enable=1, bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=1,
+            duration=0, expansion_strategy=1, fadeoff=None, hue_range=None, init_states=[],
+            random_seed=None, repeat_times=0, saturation_range=None, segment_length=None,
+            segments=[0],
+            sequence=[[0, 100, 100], [100, 100, 100], [200, 100, 100], [300, 100, 100]],
+            spread=12, transition=1500, transition_range=None, type='sequence'
+        )
+
+    @staticmethod
+    def raindrop() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_1t2nWlTBkV8KXBZ0TWvBjs', name='Raindrop', brightness=100,
+            display_colors=[[200, 10, 100], [200, 20, 100]], enable=1, bAdjusted=None,
+            brightness_range=[10, 30], backgrounds=[[200, 40, 0]], custom=0, direction=None,
+            duration=0, expansion_strategy=1, fadeoff=1000, hue_range=[200, 200],
+            init_states=[[200, 40, 100]], random_seed=24, repeat_times=None,
+            saturation_range=[10, 20], segment_length=None, segments=[0], sequence=None,
+            spread=None, transition=1000, transition_range=None, type='random'
+        )
+
+    @staticmethod
+    def spring() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_1nL6GqZ5soOxj71YDJOlZL', name='Spring', brightness=100,
+            display_colors=[[0, 30, 100], [130, 100, 100]], enable=1, bAdjusted=None,
+            brightness_range=[90, 100], backgrounds=[[130, 100, 40]], custom=0, direction=None,
+            duration=600, expansion_strategy=1, fadeoff=1000, hue_range=[0, 90],
+            init_states=[[80, 30, 100]], random_seed=20, repeat_times=None,
+            saturation_range=[30, 100], segment_length=None, segments=[0], sequence=None,
+            spread=None, transition=0, transition_range=[2000, 6000], type='random'
+        )
+
+    @staticmethod
+    def sunrise() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_1OVSyXIsDxrt4j7OxyRvqi', name='Sunrise', brightness=100,
+            display_colors=[[30, 0, 100], [30, 95, 100], [0, 100, 100]], enable=1,
+            bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=1,
+            duration=600, expansion_strategy=2, fadeoff=None, hue_range=None, init_states=[],
+            random_seed=None, repeat_times=1, saturation_range=None, segment_length=None,
+            segments=[0],
+            sequence=[[0, 100, 5], [0, 100, 5], [10, 100, 6], [15, 100, 7], [20, 100, 8],
+                      [20, 100, 10], [30, 100, 12], [30, 95, 15], [30, 90, 20], [30, 80, 25],
+                      [30, 75, 30], [30, 70, 40], [30, 60, 50], [30, 50, 60], [30, 20, 70],
+                      [30, 0, 100]], spread=1, transition=60000, transition_range=None,
+            type='pulse', trans_sequence=[], run_time=0
+        )
+
+    @staticmethod
+    def sunset() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_5NiN0Y8GAUD78p4neKk9EL', name='Sunset', brightness=100,
+            display_colors=[[0, 100, 100], [30, 95, 100], [30, 0, 100]], enable=1,
+            bAdjusted=None, brightness_range=[], backgrounds=[], custom=0, direction=1,
+            duration=600, expansion_strategy=2, fadeoff=None, hue_range=None, init_states=[],
+            random_seed=None, repeat_times=1, saturation_range=None, segment_length=None,
+            segments=[0],
+            sequence=[[30, 0, 100], [30, 20, 100], [30, 50, 99], [30, 60, 98], [30, 70, 97],
+                      [30, 75, 95], [30, 80, 93], [30, 90, 90], [30, 95, 85], [30, 100, 80],
+                      [20, 100, 70], [20, 100, 60], [15, 100, 50], [10, 100, 40], [0, 100, 30],
+                      [0, 100, 0]], spread=1, transition=60000, transition_range=None,
+            type='pulse', trans_sequence=[], run_time=0
+        )
+
+    @staticmethod
+    def valentines() -> 'LightEffect':
+        return LightEffect(
+            id='TapoStrip_2q1Vio9sSjHmaC7JS9d30l', name='Valentines', brightness=100,
+            display_colors=[[340, 20, 100], [20, 50, 100], [0, 100, 100], [340, 40, 100]],
+            enable=1, bAdjusted=None, brightness_range=[90, 100],
+            backgrounds=[[340, 20, 50], [20, 50, 50], [0, 100, 50]], custom=0, direction=None,
+            duration=600, expansion_strategy=1, fadeoff=3000, hue_range=[340, 340],
+            init_states=[[340, 30, 100]], random_seed=100, repeat_times=None,
+            saturation_range=[30, 40], segment_length=None, segments=[0], sequence=None,
+            spread=None, transition=2000, transition_range=None, type='random',
+            trans_sequence=None, run_time=None
         )
```

### Comparing `plugp100-2.5.1/plugp100/domain/tapo_exception.py` & `plugp100-3.0.0/plugp100/responses/tapo_exception.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+from typing import Optional
 
 
 class TapoError(Enum):
     INVALID_PUBLIC_KEY = -1010
     INVALID_CREDENTIAL = -1501
     INVALID_REQUEST = -1002
     INVALID_JSON = -1003
@@ -16,17 +17,17 @@
 }
 
 
 class TapoException(Exception):
     error_code: int
 
     @staticmethod
-    def from_error_code(error_code):
+    def from_error_code(error_code, msg: Optional[str]):
         try:
             tapo_error = TapoError(error_code)
             return TapoException(error_code, f"Returned error_code: {tapo_error}: {_error_message[tapo_error]}")
         except ValueError:
-            return TapoException(error_code, f"Returned unknown error_code: {error_code}")
+            return TapoException(error_code, f"Returned unknown error_code: {error_code}  msg: {msg}")
 
     def __init__(self, error_code, msg):
         super(TapoException, self).__init__(msg)
         self.error_code = error_code
```

### Comparing `plugp100-2.5.1/plugp100/tapo_protocol/encryption/key_pair.py` & `plugp100-3.0.0/plugp100/encryption/key_pair.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import base64
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.primitives import serialization
 
-from plugp100.tapo_protocol.encryption.helpers import Base64str
+from plugp100.encryption.helpers import Base64str
 
 
 class KeyPair(object):
 
     @staticmethod
     def create_key_pair() -> 'KeyPair':
         private_key = rsa.generate_private_key(public_exponent=65537, key_size=1024)
```

### Comparing `plugp100-2.5.1/plugp100/tapo_protocol/encryption/tp_link_cipher.py` & `plugp100-3.0.0/plugp100/encryption/tp_link_cipher.py`

 * *Files identical despite different names*

### Comparing `plugp100-2.5.1/plugp100/utils/http_client.py` & `plugp100-3.0.0/plugp100/common/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-2.5.1/plugp100.egg-info/PKG-INFO` & `plugp100-3.0.0/plugp100.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 2.5.1
+Version: 3.0.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
@@ -22,15 +22,15 @@
 
 # Code example
 
 ```python
 import asyncio
 
 from plugp100 import TapoApiClient, TapoApiClientConfig
-from plugp100.domain.light_effect import LightEffectPreset
+from plugp100.api.light_effect import LightEffectPreset
 
 
 async def main():
     # create generic tapo api
     config = TapoApiClientConfig("<ip>", "<email>", "<passwd>")
     sw = TapoApiClient.from_config(config)
     await sw.login()
```

### Comparing `plugp100-2.5.1/setup.py` & `plugp100-3.0.0/setup.py`

 * *Files identical despite different names*

