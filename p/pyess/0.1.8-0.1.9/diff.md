# Comparing `tmp/pyess-0.1.8.tar.gz` & `tmp/pyess-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyess-0.1.8.tar", last modified: Sat May 30 17:49:17 2020, max compression
+gzip compressed data, was "dist/pyess-0.1.9.tar", last modified: Mon Jun  1 19:05:15 2020, max compression
```

## Comparing `pyess-0.1.8.tar` & `pyess-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 paulg      (501) staff       (20)        0 2020-05-30 17:49:17.744753 pyess-0.1.8/
--rw-r--r--   0 paulg      (501) staff       (20)    14814 2020-05-30 17:49:17.744495 pyess-0.1.8/PKG-INFO
--rw-r--r--   0 paulg      (501) staff       (20)    11992 2020-05-30 17:49:00.000000 pyess-0.1.8/README.rst
-drwxr-xr-x   0 paulg      (501) staff       (20)        0 2020-05-30 17:49:17.741904 pyess-0.1.8/pyess/
--rwxr-xr-x   0 paulg      (501) staff       (20)       91 2020-05-30 17:47:54.000000 pyess-0.1.8/pyess/__init__.py
--rwxr-xr-x   0 paulg      (501) staff       (20)     7717 2020-05-30 12:55:03.000000 pyess-0.1.8/pyess/aio_ess.py
--rwxr-xr-x   0 paulg      (501) staff       (20)     3233 2020-04-30 06:36:50.000000 pyess-0.1.8/pyess/cli.py
--rwxr-xr-x   0 paulg      (501) staff       (20)     1024 2020-04-30 06:36:50.000000 pyess-0.1.8/pyess/constants.py
--rwxr-xr-x   0 paulg      (501) staff       (20)     9454 2020-05-26 19:37:52.000000 pyess-0.1.8/pyess/ess.py
--rw-r--r--   0 paulg      (501) staff       (20)     6103 2020-05-30 17:45:34.000000 pyess-0.1.8/pyess/essmqtt.py
-drwxr-xr-x   0 paulg      (501) staff       (20)        0 2020-05-30 17:49:17.744061 pyess-0.1.8/pyess.egg-info/
--rw-r--r--   0 paulg      (501) staff       (20)    14814 2020-05-30 17:49:17.000000 pyess-0.1.8/pyess.egg-info/PKG-INFO
--rw-r--r--   0 paulg      (501) staff       (20)      320 2020-05-30 17:49:17.000000 pyess-0.1.8/pyess.egg-info/SOURCES.txt
--rw-r--r--   0 paulg      (501) staff       (20)        1 2020-05-30 17:49:17.000000 pyess-0.1.8/pyess.egg-info/dependency_links.txt
--rw-r--r--   0 paulg      (501) staff       (20)       72 2020-05-30 17:49:17.000000 pyess-0.1.8/pyess.egg-info/entry_points.txt
--rw-r--r--   0 paulg      (501) staff       (20)        1 2020-04-30 06:49:14.000000 pyess-0.1.8/pyess.egg-info/not-zip-safe
--rw-r--r--   0 paulg      (501) staff       (20)       70 2020-05-30 17:49:17.000000 pyess-0.1.8/pyess.egg-info/requires.txt
--rw-r--r--   0 paulg      (501) staff       (20)        6 2020-05-30 17:49:17.000000 pyess-0.1.8/pyess.egg-info/top_level.txt
--rw-r--r--   0 paulg      (501) staff       (20)       38 2020-05-30 17:49:17.744833 pyess-0.1.8/setup.cfg
--rwxr-xr-x   0 paulg      (501) staff       (20)     1066 2020-05-30 14:28:03.000000 pyess-0.1.8/setup.py
+drwxr-xr-x   0 paulg      (501) staff       (20)        0 2020-06-01 19:05:15.045866 pyess-0.1.9/
+-rw-r--r--   0 paulg      (501) staff       (20)    16087 2020-06-01 19:05:15.045571 pyess-0.1.9/PKG-INFO
+-rw-r--r--   0 paulg      (501) staff       (20)    13073 2020-06-01 19:04:13.000000 pyess-0.1.9/README.rst
+drwxr-xr-x   0 paulg      (501) staff       (20)        0 2020-06-01 19:05:15.043659 pyess-0.1.9/pyess/
+-rwxr-xr-x   0 paulg      (501) staff       (20)       91 2020-06-01 19:04:59.000000 pyess-0.1.9/pyess/__init__.py
+-rwxr-xr-x   0 paulg      (501) staff       (20)     7717 2020-05-30 12:55:03.000000 pyess-0.1.9/pyess/aio_ess.py
+-rwxr-xr-x   0 paulg      (501) staff       (20)     3233 2020-04-30 06:36:50.000000 pyess-0.1.9/pyess/cli.py
+-rwxr-xr-x   0 paulg      (501) staff       (20)     1024 2020-04-30 06:36:50.000000 pyess-0.1.9/pyess/constants.py
+-rwxr-xr-x   0 paulg      (501) staff       (20)     9454 2020-05-26 19:37:52.000000 pyess-0.1.9/pyess/ess.py
+-rw-r--r--   0 paulg      (501) staff       (20)     7648 2020-06-01 12:42:54.000000 pyess-0.1.9/pyess/essmqtt.py
+drwxr-xr-x   0 paulg      (501) staff       (20)        0 2020-06-01 19:05:15.045084 pyess-0.1.9/pyess.egg-info/
+-rw-r--r--   0 paulg      (501) staff       (20)    16087 2020-06-01 19:05:14.000000 pyess-0.1.9/pyess.egg-info/PKG-INFO
+-rw-r--r--   0 paulg      (501) staff       (20)      320 2020-06-01 19:05:14.000000 pyess-0.1.9/pyess.egg-info/SOURCES.txt
+-rw-r--r--   0 paulg      (501) staff       (20)        1 2020-06-01 19:05:14.000000 pyess-0.1.9/pyess.egg-info/dependency_links.txt
+-rw-r--r--   0 paulg      (501) staff       (20)       72 2020-06-01 19:05:14.000000 pyess-0.1.9/pyess.egg-info/entry_points.txt
+-rw-r--r--   0 paulg      (501) staff       (20)        1 2020-04-30 06:49:14.000000 pyess-0.1.9/pyess.egg-info/not-zip-safe
+-rw-r--r--   0 paulg      (501) staff       (20)       70 2020-06-01 19:05:14.000000 pyess-0.1.9/pyess.egg-info/requires.txt
+-rw-r--r--   0 paulg      (501) staff       (20)        6 2020-06-01 19:05:14.000000 pyess-0.1.9/pyess.egg-info/top_level.txt
+-rw-r--r--   0 paulg      (501) staff       (20)       38 2020-06-01 19:05:15.045946 pyess-0.1.9/setup.cfg
+-rwxr-xr-x   0 paulg      (501) staff       (20)     1066 2020-05-30 14:28:03.000000 pyess-0.1.9/setup.py
```

### Comparing `pyess-0.1.8/PKG-INFO` & `pyess-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyess
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for communicating with LG ESS solar power converters/batteries
 Home-page: https://github.com/gluap/pyess
 Author: Paul Görgen
 Author-email: pypi@pgoergen.de
 License: MIT
 Description: =====
         pyess
@@ -185,14 +185,35 @@
         The config file can contain any of the command line arguments. Example::
         
            ess_password = <your_ess_password>
            mqtt_server = <your_mqtt_server>
            mqtt_user = <your_mqtt_username>
            mqtt_password = <your_mqtt_password>
         
+        
+        essmqtt autoconfig for homeassistant
+        ....................................
+        Essmqtt can provide autoconfiguration for [homeassistant](https://www.home-assistant.io/).
+        
+        **prerequisites:** [mqtt must be set up with matt discovery in homeassistant](https://www.home-assistant.io/docs/mqtt/discovery/)
+        
+        To select the sensors that should be autodiscovered by homeassistant, provide the ``--hass_autoconfig_sensors``
+        argument with a comma separated list of all mqtt pathes you want to see as sensors in homeassistant. Some autodetection
+        of the value type is done so for instance if an mqtt path contains ``power`` it is assumed to be a power
+        value in watts. Of course this can also be configured in a config file.
+        
+        Example config file::
+        
+           ess_password = <your_ess_password>
+           mqtt_server = <your_mqtt_server>
+           mqtt_user = <your_mqtt_username>
+           mqtt_password = <your_mqtt_password>
+           hass_autoconfig_sensors= ess/common/BATT/soc,ess/home/statistics/pcs_pv_total_power,ess/common/GRID/active_power,ess/common/LOAD/load_power
+        
+        
         essmqtt as systemd service
         ..........................
         To set up ``essmqtt`` as a daemon (systemd service) it is recommended to install it in a venv first::
         
           python3.7 -m venv <path_to_venv>
           <path_to_venv>/bin/pip install pyess
         
@@ -229,14 +250,17 @@
         via the API but not yet via the CLI is the data for the daily / weekly / monthly / yearly statistics graphs that can
         be accessed via the EnerVu App.
         
         
         Changelog
         =========
         
+        **2020-06-01 0.1.9**
+         - add homeassistant auto config
+        
         **2020-05-30 0.1.8**
          - refactor uploading to MQTT to avoid accidentally trying to access a string by key (should fix #8)
         
         **2020-05-30 0.1.7**
          - add config file to allow storing settings for essmqtt
         
         **2020-05-30 0.1.6**
```

### Comparing `pyess-0.1.8/README.rst` & `pyess-0.1.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -177,14 +177,35 @@
 The config file can contain any of the command line arguments. Example::
 
    ess_password = <your_ess_password>
    mqtt_server = <your_mqtt_server>
    mqtt_user = <your_mqtt_username>
    mqtt_password = <your_mqtt_password>
 
+
+essmqtt autoconfig for homeassistant
+....................................
+Essmqtt can provide autoconfiguration for [homeassistant](https://www.home-assistant.io/).
+
+**prerequisites:** [mqtt must be set up with matt discovery in homeassistant](https://www.home-assistant.io/docs/mqtt/discovery/)
+
+To select the sensors that should be autodiscovered by homeassistant, provide the ``--hass_autoconfig_sensors``
+argument with a comma separated list of all mqtt pathes you want to see as sensors in homeassistant. Some autodetection
+of the value type is done so for instance if an mqtt path contains ``power`` it is assumed to be a power
+value in watts. Of course this can also be configured in a config file.
+
+Example config file::
+
+   ess_password = <your_ess_password>
+   mqtt_server = <your_mqtt_server>
+   mqtt_user = <your_mqtt_username>
+   mqtt_password = <your_mqtt_password>
+   hass_autoconfig_sensors= ess/common/BATT/soc,ess/home/statistics/pcs_pv_total_power,ess/common/GRID/active_power,ess/common/LOAD/load_power
+
+
 essmqtt as systemd service
 ..........................
 To set up ``essmqtt`` as a daemon (systemd service) it is recommended to install it in a venv first::
 
   python3.7 -m venv <path_to_venv>
   <path_to_venv>/bin/pip install pyess
 
@@ -221,14 +242,17 @@
 via the API but not yet via the CLI is the data for the daily / weekly / monthly / yearly statistics graphs that can
 be accessed via the EnerVu App.
 
 
 Changelog
 =========
 
+**2020-06-01 0.1.9**
+ - add homeassistant auto config
+
 **2020-05-30 0.1.8**
  - refactor uploading to MQTT to avoid accidentally trying to access a string by key (should fix #8)
 
 **2020-05-30 0.1.7**
  - add config file to allow storing settings for essmqtt
 
 **2020-05-30 0.1.6**
```

### Comparing `pyess-0.1.8/pyess/aio_ess.py` & `pyess-0.1.9/pyess/aio_ess.py`

 * *Files identical despite different names*

### Comparing `pyess-0.1.8/pyess/cli.py` & `pyess-0.1.9/pyess/cli.py`

 * *Files identical despite different names*

### Comparing `pyess-0.1.8/pyess/constants.py` & `pyess-0.1.9/pyess/constants.py`

 * *Files identical despite different names*

### Comparing `pyess-0.1.8/pyess/ess.py` & `pyess-0.1.9/pyess/ess.py`

 * *Files identical despite different names*

### Comparing `pyess-0.1.8/pyess/essmqtt.py` & `pyess-0.1.9/pyess/essmqtt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import configargparse
 import asyncio
+import configargparse
 import logging
+import json
 import sys
-from distutils.util import strtobool
 
 from asyncio_mqtt import Client
 
+from distutils.util import strtobool
+
 from pyess.aio_ess import ESS
 from pyess.ess import autodetect_ess
 
 logger = logging.getLogger(__name__)
 
 
 # The callback for when the client receives a CONNACK response from the server.
@@ -52,14 +54,46 @@
 
         i += 1
         if once:
             break
         await asyncio.sleep(interval_seconds - 1)
 
 
+def prepare_description(sensor):
+    description = {"name": sensor, "state_topic": sensor}
+    if "power" in sensor:
+        description["device_class"] = "power"
+        description["unit_of_measurement"] = "W"
+    if "enegy" in sensor or "energy" in sensor: # typo in ess json
+        description["unit_of_measuremnt"] = "Wh"
+        description["icon"] = "mdi:gauge"
+    if "soc" in sensor:
+        description["device_class"] = "battery"
+    if "current" in sensor:
+        description["unit_of_measurement"] = "A"
+        description["icon"] = "mdi:gauge"
+    if "voltage" in sensor:
+        description["unit_of_measurement"] = "V"
+        description["icon"] = "mdi:gauge"
+    return description
+
+
+async def announce_loop(client, once=False, sensors=None):
+    if sensors is None:
+        return
+    while True:
+        for sensor in sensors:
+            await client.publish(f"homeassistant/sensor/{sensor.replace('/','')}/config",
+                                 json.dumps(prepare_description(sensor)))
+        if not once:
+            await asyncio.sleep(120)
+        else:
+            return
+
+
 def main(arguments=None):
     loop = asyncio.get_event_loop()
     asyncio.run(_main(arguments))
     # .run(_main, arguments)
 
 
 async def _main(arguments=None):
@@ -79,14 +113,16 @@
     parser.add_argument("--mqtt_password", default=None, help="mqtt password")
     parser.add_argument("--mqtt_user", default=None, help="mqtt user")
     parser.add_argument("--ess_host", default=None, help="hostname or IP of mqtt host (discover via mdns if not set)")
     parser.add_argument("--once", default=False, type=bool, help="no loop, only one pass")
     parser.add_argument("--common_divisor", default=1, type=int,
                         help="multiply interval_seconds for values below 'common' by this factor")
     parser.add_argument("--interval_seconds", default=10, type=int, help="update interval (default: 10 seconds)")
+    parser.add_argument("--hass_autoconfig_sensors", default=None, help="comma-separated list of sensors to advertise"
+                                                                        "for homassistant autconfig")
 
     args = parser.parse_args(arguments)
 
     if args.ess_host is None:
         ip, name = autodetect_ess()
     else:
         ip, name = args.ess_host, args.ess_host
@@ -136,14 +172,17 @@
             asyncio.create_task(handle_control(client, switch_active, "/ess/control/active"))
 
             # also subscribe without leading slash for better style
             await client.subscribe('ess/control/#')
             asyncio.create_task(handle_control(client, switch_winter, "ess/control/winter_mode"))
             asyncio.create_task(handle_control(client, switch_fastcharge, "ess/control/fastcharge"))
             asyncio.create_task(handle_control(client, switch_active, "ess/control/active"))
+            if args.hass_autoconfig_sensors is not None:
+                asyncio.ensure_future(
+                    announce_loop(client, once=args.once, sensors=args.hass_autoconfig_sensors.split(",")))
 
             await send_loop(ess, client, once=args.once, interval_seconds=args.interval_seconds,
                             common_divisor=args.common_divisor)
 
     else:
         pass
```

### Comparing `pyess-0.1.8/pyess.egg-info/PKG-INFO` & `pyess-0.1.9/pyess.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyess
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for communicating with LG ESS solar power converters/batteries
 Home-page: https://github.com/gluap/pyess
 Author: Paul Görgen
 Author-email: pypi@pgoergen.de
 License: MIT
 Description: =====
         pyess
@@ -185,14 +185,35 @@
         The config file can contain any of the command line arguments. Example::
         
            ess_password = <your_ess_password>
            mqtt_server = <your_mqtt_server>
            mqtt_user = <your_mqtt_username>
            mqtt_password = <your_mqtt_password>
         
+        
+        essmqtt autoconfig for homeassistant
+        ....................................
+        Essmqtt can provide autoconfiguration for [homeassistant](https://www.home-assistant.io/).
+        
+        **prerequisites:** [mqtt must be set up with matt discovery in homeassistant](https://www.home-assistant.io/docs/mqtt/discovery/)
+        
+        To select the sensors that should be autodiscovered by homeassistant, provide the ``--hass_autoconfig_sensors``
+        argument with a comma separated list of all mqtt pathes you want to see as sensors in homeassistant. Some autodetection
+        of the value type is done so for instance if an mqtt path contains ``power`` it is assumed to be a power
+        value in watts. Of course this can also be configured in a config file.
+        
+        Example config file::
+        
+           ess_password = <your_ess_password>
+           mqtt_server = <your_mqtt_server>
+           mqtt_user = <your_mqtt_username>
+           mqtt_password = <your_mqtt_password>
+           hass_autoconfig_sensors= ess/common/BATT/soc,ess/home/statistics/pcs_pv_total_power,ess/common/GRID/active_power,ess/common/LOAD/load_power
+        
+        
         essmqtt as systemd service
         ..........................
         To set up ``essmqtt`` as a daemon (systemd service) it is recommended to install it in a venv first::
         
           python3.7 -m venv <path_to_venv>
           <path_to_venv>/bin/pip install pyess
         
@@ -229,14 +250,17 @@
         via the API but not yet via the CLI is the data for the daily / weekly / monthly / yearly statistics graphs that can
         be accessed via the EnerVu App.
         
         
         Changelog
         =========
         
+        **2020-06-01 0.1.9**
+         - add homeassistant auto config
+        
         **2020-05-30 0.1.8**
          - refactor uploading to MQTT to avoid accidentally trying to access a string by key (should fix #8)
         
         **2020-05-30 0.1.7**
          - add config file to allow storing settings for essmqtt
         
         **2020-05-30 0.1.6**
```

### Comparing `pyess-0.1.8/setup.py` & `pyess-0.1.9/setup.py`

 * *Files identical despite different names*

