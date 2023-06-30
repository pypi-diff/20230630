# Comparing `tmp/yaqd-fakes-2022.5.0.tar.gz` & `tmp/yaqd_fakes-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaqd-fakes-2022.5.0.tar", last modified: Thu May 19 21:47:41 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `yaqd-fakes-2022.5.0.tar` & `yaqd_fakes-2023.6.0.tar`

### file list

```diff
@@ -1,30 +1,36 @@
--rw-r--r--   0        0        0     3921 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     7633 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/LICENSE
--rw-r--r--   0        0        0     1128 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/README.md
--rw-r--r--   0        0        0     1700 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/pyproject.toml
--rw-r--r--   0        0        0        9 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/VERSION
--rw-r--r--   0        0        0       74 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/__init__.py
--rw-r--r--   0        0        0      515 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/__version__.py
--rw-r--r--   0        0        0     1848 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/_fake_camera.py
--rw-r--r--   0        0        0     1387 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/_fake_continuous_hardware.py
--rw-r--r--   0        0        0     1132 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/_fake_discrete_hardware.py
--rw-r--r--   0        0        0     1955 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/_fake_has_turret.py
--rw-r--r--   0        0        0     1516 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/_fake_sensor.py
--rw-r--r--   0        0        0     1692 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/_fake_spectrometer.py
--rw-r--r--   0        0        0     1369 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/_fake_triggered_sensor.py
--rw-r--r--   0        0        0      486 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/_signal_generators.py
--rw-r--r--   0        0        0     9262 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-camera.avpr
--rw-r--r--   0        0        0      711 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-camera.toml
--rw-r--r--   0        0        0     9152 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-continuous-hardware.avpr
--rw-r--r--   0        0        0      643 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-continuous-hardware.toml
--rw-r--r--   0        0        0     9868 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-discrete-hardware.avpr
--rw-r--r--   0        0        0      735 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-discrete-hardware.toml
--rw-r--r--   0        0        0    10858 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-has-turret.avpr
--rw-r--r--   0        0        0      734 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-has-turret.toml
--rw-r--r--   0        0        0     7100 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-sensor.avpr
--rw-r--r--   0        0        0      742 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-sensor.toml
--rw-r--r--   0        0        0     9788 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-spectrometer.avpr
--rw-r--r--   0        0        0      939 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-spectrometer.toml
--rw-r--r--   0        0        0     7751 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-triggered-sensor.avpr
--rw-r--r--   0        0        0      635 2022-05-19 21:47:25.612257 yaqd-fakes-2022.5.0/yaqd_fakes/fake-triggered-sensor.toml
--rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 yaqd-fakes-2022.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/__init__.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/__version__.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_fake_camera.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_fake_continuous_hardware.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_fake_discrete_hardware.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_fake_furnace.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_fake_has_transformed_position.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_fake_has_turret.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_fake_sensor.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_fake_spectrometer.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_fake_triggered_sensor.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/_signal_generators.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-camera.avpr
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-camera.toml
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-continuous-hardware.avpr
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-continuous-hardware.toml
+-rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-discrete-hardware.avpr
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-discrete-hardware.toml
+-rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-furnace.avpr
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-furnace.toml
+-rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-has-transformed-position.avpr
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-has-transformed-position.toml
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-has-turret.avpr
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-has-turret.toml
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-sensor.avpr
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-sensor.toml
+-rw-r--r--   0        0        0     9788 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-spectrometer.avpr
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-spectrometer.toml
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-triggered-sensor.avpr
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/yaqd_fakes/fake-triggered-sensor.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/.gitignore
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/LICENSE
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/README.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 yaqd_fakes-2023.6.0/PKG-INFO
```

### Comparing `yaqd-fakes-2022.5.0/CHANGELOG.md` & `yaqd_fakes-2023.6.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.6.0]
+
+### Added
+- new fake-furnace daemon, useful for prototyping chemical engineering setups
+- new fake-has-transformed-position daemon
+
+### Changed
+- moved to hatchling build system
+
 ## [2022.5.0]
 
 ### Changed
 - moved to github
 - rerendered avprs for updated has-position trait
 
 ## [2022.3.1]
@@ -104,15 +113,16 @@
 - include avpr and toml files in the distributed version
 
 ## [2020.06.0]
 
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2022.5.0...main
+[Unreleased]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2023.6.0...main
+[2023.6.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2022.5.0...yaqd-fakes-2023.6.0
 [2022.5.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2022.3.1...yaqd-fakes-2022.5.0
 [2022.3.1]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2022.3.0...yaqd-fakes-2022.3.1
 [2022.3.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2021.10.0...yaqd-fakes-2022.3.0
 [2021.10.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2021.8.0...yaqd-fakes-2021.10.0
 [2021.8.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2021.3.0...yaqd-fakes-2021.8.0
 [2021.3.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2021.2.0...yaqd-fakes-2021.3.0
 [2021.2.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-fakes-2021.1.0...yaqd-fakes-2021.2.0
```

### Comparing `yaqd-fakes-2022.5.0/LICENSE` & `yaqd_fakes-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/README.md` & `yaqd_fakes-2023.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,11 +9,14 @@
 
 fake yaq daemons, for testing purposes
 
 This package contains the following daemon(s):
 
 - [fake-camera](https://yaq.fyi/daemons/fake-camera)
 - [fake-continuous-hardware](https://yaq.fyi/daemons/fake-continuous-hardware)
+- [fake-has-transformed-position](https://yaq.fyi/daemons/fake-has-transformed-position)
 - [fake-discrete-hardware](https://yaq.fyi/daemons/fake-discrete-hardware)
+- [fake-furnace](https://yaq.fyi/daemons/fake-furnace)
 - [fake-has-turret](https://yaq.fyi/daemons/fake-has-turret)
+- [fake-sensor](https://yaq.fyi/daemons/fake-sensor)
 - [fake-spectrometer](https://yaq.fyi/daemons/fake-spectrometer) (requires numpy)
 - [fake-triggered-sensor](https://yaq.fyi/daemons/fake-triggered-sensor)
```

### Comparing `yaqd-fakes-2022.5.0/pyproject.toml` & `yaqd_fakes-2023.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 [build-system]
-requires = ["flit_core >=2,<4"]
-build-backend = "flit_core.buildapi"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-[tool.flit.metadata]
-module = "yaqd_fakes"
-dist-name = "yaqd-fakes"
-author = "yaq developers"
-home-page = "https://yaq.fyi"
+[project]
+name = "yaqd-fakes"
+authors = [{name="yaq developers"}]
 requires-python = ">=3.7"
-requires = ["yaqd-core>=2022.3.0"]
-description-file="README.md"
+dependencies = ["yaqd-core>=2022.3.0"]
+readme="README.md"
+license="LGPL-3.0-only"
+dynamic=["version"]
 classifiers=[
-        "Development Status :: 5 - Production/Stable",
-	"Intended Audience :: Science/Research",
-	"License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
-	"Natural Language :: English",
-	"Programming Language :: Python :: 3",
-	"Programming Language :: Python :: 3.8",
-	"Programming Language :: Python :: 3.9",
-	"Programming Language :: Python :: 3.10",
-	"Topic :: Scientific/Engineering",
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Topic :: Scientific/Engineering",
 ]
 
-[tool.flit.metadata.urls]
+[project.urls]
+"Home page" = "https://yaq.fyi"
 Source = "https://github.com/yaq-project/yaq-python"
 Issues = "https://github.com/yaq-project/yaq-python/issues"
 
-[tool.flit.metadata.requires-extra]
+[project.optional-dependencies]
 dev = ["black", "pre-commit"]
 
-[tool.flit.scripts]
+[project.scripts]
 yaqd-fake-continuous-hardware="yaqd_fakes._fake_continuous_hardware:FakeContinuousHardware.main"
 yaqd-fake-discrete-hardware="yaqd_fakes._fake_discrete_hardware:FakeDiscreteHardware.main"
+yaqd-fake-furnace="yaqd_fakes._fake_furnace:FakeFurnace.main"
 yaqd-fake-triggered-sensor="yaqd_fakes._fake_triggered_sensor:FakeTriggeredSensor.main"
 yaqd-fake-has-turret="yaqd_fakes._fake_has_turret:FakeHasTurret.main"
 yaqd-fake-sensor="yaqd_fakes._fake_sensor:FakeSensor.main"
 yaqd-fake-spectrometer="yaqd_fakes._fake_spectrometer:FakeSpectrometer.main"
 yaqd-fake-camera="yaqd_fakes._fake_camera:FakeCamera.main"
+yaqd-fake-has-transformed-position="yaqd_fakes._fake_has_transformed_position:FakeHasTransformedPosition.main"
+
+[tool.hatch.version]
+path="yaqd_fakes/__version__.py"
 
 [tool.black]
 line-length = 99
 target-version = ['py37', 'py38']
 include = '\.pyi?$'
 exclude = '''
 /(
```

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/_fake_camera.py` & `yaqd_fakes-2023.6.0/yaqd_fakes/_fake_camera.py`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/_fake_continuous_hardware.py` & `yaqd_fakes-2023.6.0/yaqd_fakes/_fake_continuous_hardware.py`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/_fake_discrete_hardware.py` & `yaqd_fakes-2023.6.0/yaqd_fakes/_fake_discrete_hardware.py`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/_fake_has_turret.py` & `yaqd_fakes-2023.6.0/yaqd_fakes/_fake_has_turret.py`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/_fake_sensor.py` & `yaqd_fakes-2023.6.0/yaqd_fakes/_fake_sensor.py`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/_fake_spectrometer.py` & `yaqd_fakes-2023.6.0/yaqd_fakes/_fake_spectrometer.py`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/_fake_triggered_sensor.py` & `yaqd_fakes-2023.6.0/yaqd_fakes/_fake_triggered_sensor.py`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-camera.avpr` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-camera.avpr`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-camera.toml` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-camera.toml`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-continuous-hardware.avpr` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-continuous-hardware.avpr`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         }
     },
     "properties": {
         "destination": {
             "control_kind": "hinted",
             "dynamic": true,
             "getter": "get_destination",
-            "limits_getter": null,
+            "limits_getter": "get_limits",
             "options_getter": null,
             "record_kind": "data",
             "setter": "set_position",
             "type": "double",
             "units_getter": "get_units"
         },
         "position": {
```

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-continuous-hardware.toml` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-continuous-hardware.toml`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-discrete-hardware.avpr` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-discrete-hardware.avpr`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-discrete-hardware.toml` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-discrete-hardware.toml`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-has-turret.avpr` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-has-turret.avpr`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         }
     },
     "properties": {
         "destination": {
             "control_kind": "hinted",
             "dynamic": true,
             "getter": "get_destination",
-            "limits_getter": null,
+            "limits_getter": "get_limits",
             "options_getter": null,
             "record_kind": "data",
             "setter": "set_position",
             "type": "double",
             "units_getter": "get_units"
         },
         "position": {
```

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-has-turret.toml` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-has-turret.toml`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-sensor.avpr` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-sensor.avpr`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-sensor.toml` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-sensor.toml`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-spectrometer.avpr` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-spectrometer.avpr`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-spectrometer.toml` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-spectrometer.toml`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-triggered-sensor.avpr` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-triggered-sensor.avpr`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/yaqd_fakes/fake-triggered-sensor.toml` & `yaqd_fakes-2023.6.0/yaqd_fakes/fake-triggered-sensor.toml`

 * *Files identical despite different names*

### Comparing `yaqd-fakes-2022.5.0/PKG-INFO` & `yaqd_fakes-2023.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: yaqd-fakes
-Version: 2022.5.0
-Summary: fake yaq daemons, for testing purposes
-Home-page: https://yaq.fyi
+Version: 2023.6.0
+Project-URL: Home page, https://yaq.fyi
+Project-URL: Source, https://github.com/yaq-project/yaq-python
+Project-URL: Issues, https://github.com/yaq-project/yaq-python/issues
 Author: yaq developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+License-Expression: LGPL-3.0-only
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
 Requires-Dist: yaqd-core>=2022.3.0
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: pre-commit ; extra == "dev"
-Project-URL: Issues, https://github.com/yaq-project/yaq-python/issues
-Project-URL: Source, https://github.com/yaq-project/yaq-python
 Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Description-Content-Type: text/markdown
 
 # yaqd-fakes
 
 [![PyPI](https://img.shields.io/pypi/v/yaqd-fakes)](https://pypi.org/project/yaqd-fakes)
 [![Conda](https://img.shields.io/conda/vn/conda-forge/yaqd-fakes)](https://anaconda.org/conda-forge/yaqd-fakes)
 [![yaq](https://img.shields.io/badge/framework-yaq-orange)](https://yaq.fyi/)
 [![black](https://img.shields.io/badge/code--style-black-black)](https://black.readthedocs.io/)
@@ -33,12 +35,14 @@
 
 fake yaq daemons, for testing purposes
 
 This package contains the following daemon(s):
 
 - [fake-camera](https://yaq.fyi/daemons/fake-camera)
 - [fake-continuous-hardware](https://yaq.fyi/daemons/fake-continuous-hardware)
+- [fake-has-transformed-position](https://yaq.fyi/daemons/fake-has-transformed-position)
 - [fake-discrete-hardware](https://yaq.fyi/daemons/fake-discrete-hardware)
+- [fake-furnace](https://yaq.fyi/daemons/fake-furnace)
 - [fake-has-turret](https://yaq.fyi/daemons/fake-has-turret)
+- [fake-sensor](https://yaq.fyi/daemons/fake-sensor)
 - [fake-spectrometer](https://yaq.fyi/daemons/fake-spectrometer) (requires numpy)
 - [fake-triggered-sensor](https://yaq.fyi/daemons/fake-triggered-sensor)
-
```

