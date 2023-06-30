# Comparing `tmp/yaqd-core-2023.2.0.tar.gz` & `tmp/yaqd_core-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaqd-core-2023.2.0.tar", last modified: Thu Feb  2 23:01:51 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `yaqd-core-2023.2.0.tar` & `yaqd_core-2023.6.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0    11127 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     7651 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/LICENSE
--rw-r--r--   0        0        0      666 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/README.md
--rw-r--r--   0        0        0     1260 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/pyproject.toml
--rw-r--r--   0        0        0        6 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/AVRO_VERSION
--rw-r--r--   0        0        0        9 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/VERSION
--rw-r--r--   0        0        0      706 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/__init__.py
--rw-r--r--   0        0        0      648 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/__version__.py
--rw-r--r--   0        0        0      256 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_has_dependents.py
--rw-r--r--   0        0        0     1473 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_has_limits.py
--rw-r--r--   0        0        0     1286 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_has_mapping.py
--rw-r--r--   0        0        0     2265 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_has_measure_trigger.py
--rw-r--r--   0        0        0     1018 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_has_position.py
--rw-r--r--   0        0        0     3592 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_has_transformed_position.py
--rw-r--r--   0        0        0      334 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_has_turret.py
--rwxr-xr-x   0        0        0    14530 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_is_daemon.py
--rw-r--r--   0        0        0      875 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_is_discrete.py
--rw-r--r--   0        0        0      213 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_is_homeable.py
--rw-r--r--   0        0        0     1383 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_is_sensor.py
--rw-r--r--   0        0        0       96 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_legacy/__init__.py
--rw-r--r--   0        0        0      177 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_legacy/_base.py
--rwxr-xr-x   0        0        0      257 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_legacy/_continuous.py
--rwxr-xr-x   0        0        0      159 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_legacy/_discrete.py
--rw-r--r--   0        0        0      243 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_legacy/_sensor.py
--rw-r--r--   0        0        0     2813 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_mro.py
--rw-r--r--   0        0        0     4223 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_protocol.py
--rw-r--r--   0        0        0      541 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_state.py
--rw-r--r--   0        0        0      109 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_uses_i2c.py
--rw-r--r--   0        0        0      221 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_uses_serial.py
--rw-r--r--   0        0        0      111 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/_uses_uart.py
--rw-r--r--   0        0        0       24 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/aserial/__init__.py
--rw-r--r--   0        0        0     1570 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/aserial/_aserial.py
--rw-r--r--   0        0        0     1446 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/avrorpc/__init__.py
--rw-r--r--   0        0        0      791 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/avrorpc/avro_numpy.py
--rw-r--r--   0        0        0     3344 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/avrorpc/handshake.py
--rw-r--r--   0        0        0      121 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/avrorpc/protocol.py
--rw-r--r--   0        0        0     3985 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/avrorpc/unpacker.py
--rw-r--r--   0        0        0     1727 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/logging/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/py.typed
--rw-r--r--   0        0        0       27 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/testing/__init__.py
--rw-r--r--   0        0        0     1872 2023-02-02 23:01:38.421341 yaqd-core-2023.2.0/yaqd_core/testing/_run_daemon.py
--rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 yaqd-core-2023.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11522 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/__version__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_has_dependents.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_has_limits.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_has_mapping.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_has_measure_trigger.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_has_position.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_has_transformed_position.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_has_turret.py
+-rwxr-xr-x   0        0        0    14479 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_is_daemon.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_is_discrete.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_is_homeable.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_is_sensor.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_mro.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_protocol.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_state.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_uses_i2c.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_uses_serial.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_uses_uart.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/py.typed
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_legacy/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_legacy/_base.py
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_legacy/_continuous.py
+-rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_legacy/_discrete.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/_legacy/_sensor.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/aserial/__init__.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/aserial/_aserial.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/avrorpc/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/avrorpc/avro_numpy.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/avrorpc/handshake.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/avrorpc/protocol.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/avrorpc/unpacker.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/logging/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/testing/__init__.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/yaqd_core/testing/_run_daemon.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/.gitignore
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/LICENSE
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/README.md
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 yaqd_core-2023.6.0/PKG-INFO
```

### Comparing `yaqd-core-2023.2.0/CHANGELOG.md` & `yaqd_core-2023.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.6.0]
+
+### Added
+- fake-has-transformed-position for testing purposes
+- has-transformed-position can read native_limits as a config option
+
+### Fixed
+- Fixes has_transformed_position which had inheiritance issue
+
+### Changed
+- Upgraded appdirs to platformdirs
+- moved to hatchling build system
+
 ## [2023.2.0]
 
 ### Fixed
 - Text for two methods for has-transformed-position for pedagogical reasons
 - Wrapped call to `start_server` in `create_task` for Python 3.11 compatibility
 
 ## [2022.8.0]
@@ -320,15 +333,16 @@
 
 ### Initial release
 - The base daemon implementation
 - JSON-RPC implementation
 - Generic Client
 - Continuous hardware base daemon
 
-[Unreleased]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2023.2.0...main
+[Unreleased]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2023.6.0...main
+[2023.6.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2023.2.0...2023.6.0
 [2023.2.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2022.8.0...2023.2.0
 [2022.8.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2022.7.0...2022.8.0
 [2022.7.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2022.5.0...2022.7.0
 [2022.5.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2022.3.0...yaqd-core-2022.5.0
 [2022.3.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2021.12.0...yaqd-core-2022.3.0
 [2021.12.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2021.10.0...yaqd-core-2021.12.0
 [2021.10.0]: https://github.com/yaq-project/yaq-python/compare/yaqd-core-2021.4.0...yaqd-core-2021.10.0
```

### Comparing `yaqd-core-2023.2.0/LICENSE` & `yaqd_core-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/README.md` & `yaqd_core-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/pyproject.toml` & `yaqd_core-2023.6.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 [build-system]
-requires = ["flit_core >=2,<3.2"]
-build-backend = "flit_core.buildapi"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-[tool.flit.metadata]
-module = "yaqd_core"
-dist-name = "yaqd-core"
-author = "yaq developers"
-home-page = "https://yaq.fyi"
+[project]
+name = "yaqd-core"
+author = [{name="yaq developers"}]
 requires-python = ">=3.7"
-requires = ["appdirs", "tomli", "tomli-w", "fastavro>=1.4.0"]
-description-file="README.md"
+dependencies = ["platformdirs", "tomli", "tomli-w", "fastavro>=1.4.0"]
+readme="README.md"
+dynamic = ["version"]
+license = "LGPL-3.0-only"
 classifiers=[
-        "Development Status :: 5 - Production/Stable",
-	"Intended Audience :: Science/Research",
-	"License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
-	"Natural Language :: English",
-	"Programming Language :: Python :: 3",
-	"Programming Language :: Python :: 3.8",
-	"Programming Language :: Python :: 3.9",
-	"Programming Language :: Python :: 3.10",
-	"Programming Language :: Python :: 3.11",
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
+"Home Page" = "https://yaq.fyi"
 Documentation = "http://yaq-core-python.yaq.fyi/"
 Source = "https://github.com/yaq-project/yaq-python"
-Issues = "https://github.com/yaq-project/yaq-python/-/issues"
+Issues = "https://github.com/yaq-project/yaq-python/issues"
 
-[tool.flit.metadata.requires-extra]
+[project.optional-dependencies]
 dev = ["black", "pre-commit"]
 
+[tool.hatch.version]
+path = "yaqd_core/__version__.py"
+
 [tool.black]
 line-length = 99
 target-version = ['py37', 'py38']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
```

### Comparing `yaqd-core-2023.2.0/yaqd_core/__init__.py` & `yaqd_core-2023.6.0/yaqd_core/__init__.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/_has_limits.py` & `yaqd_core-2023.6.0/yaqd_core/_has_limits.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,34 +11,44 @@
     def __init__(
         self, name: str, config: Dict[str, Any], config_filepath: pathlib.Path
     ):
         super().__init__(name, config, config_filepath)
         self._out_of_limits = config["out_of_limits"]
 
     def get_limits(self) -> List[float]:
-        assert self._state["hw_limits"][0] < self._state["hw_limits"][1]
-        config_limits = self._config["limits"]
-        assert config_limits[0] < config_limits[1]
-        out = [
-            max(self._state["hw_limits"][0], config_limits[0]),
-            min(self._state["hw_limits"][1], config_limits[1]),
-        ]
+        # wrapper for client
+        return self.limits
+
+    @property
+    def limits(self) -> List[float]:
+        # for internal use
+        return self._joint_limit(self._state["hw_limits"], self._config["limits"])
+
+    @classmethod
+    def _joint_limit(cls, *limits: List[float]):
+        mins, maxes = [*zip(*limits)]
+        assert all([mini < maxi for mini, maxi in zip(mins, maxes)])
+        out = [max(*mins), min(*maxes)]
         assert out[0] < out[1]
         return out
 
     def in_limits(self, position: float) -> bool:
-        low, upp = self.get_limits()
+        return self._in_limits(position)
+
+    def _in_limits(self, position):
+        # for internal use
+        low, upp = self.limits
         return low <= position <= upp
 
     def set_position(self, position: float) -> None:
-        if not self.in_limits(position):
+        if not self._in_limits(position):
             if self._out_of_limits == "closest":
-                low, upp = self.get_limits()
+                low, upp = self.limits
                 if position > upp:
                     position = upp
                 elif position < low:
                     position = low
             elif self._out_of_limits == "ignore":
                 return
             else:
-                raise ValueError(f"{position} not in ranges {self.get_limits()}")
+                raise ValueError(f"{position} not in ranges {self.limits}")
         super().set_position(position)
```

### Comparing `yaqd-core-2023.2.0/yaqd_core/_has_mapping.py` & `yaqd_core-2023.6.0/yaqd_core/_has_mapping.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/_has_measure_trigger.py` & `yaqd_core-2023.6.0/yaqd_core/_has_measure_trigger.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/_has_position.py` & `yaqd_core-2023.6.0/yaqd_core/_has_position.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/_has_transformed_position.py` & `yaqd_core-2023.6.0/yaqd_core/_has_transformed_position.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 __all__ = ["HasTransformedPosition"]
 
 
 import pathlib
 from typing import Dict, Any, Optional, List
-
 from yaqd_core import HasLimits, HasPosition, IsDaemon
 
 
 class HasTransformedPosition(HasLimits, HasPosition, IsDaemon):
     def __init__(
         self, name: str, config: Dict[str, Any], config_filepath: pathlib.Path
     ):
@@ -48,32 +47,48 @@
         Note that override should still obey inversion:
         ```
         _relative_to_transformed(_transformed_to_relative(x)) == x
         ```.
         """
         return transformed_position
 
-    # --- methods for transformed positions -------------------------------------------------------
+    # --- wrap parent messages that deal with position --------------------------------------------
+    # --- clients use transformed position, but parent messages except/return native position.
 
     def set_position(self, position: float) -> None:
         super().set_position(self.to_native(position))
 
+    def set_relative(self, distance: float) -> float:
+        new = self.to_transformed(self._state["destination"]) + distance
+        self.set_position(new)
+        return new
+
     def get_position(self) -> float:
-        return self.to_transformed(super().get_position())
+        position = super().get_position()
+        return self.to_transformed(position)
 
     def get_destination(self) -> float:
         return self.to_transformed(super().get_destination())
 
     def in_limits(self, position: float) -> bool:
         return super().in_limits(self.to_native(position))
 
     def get_limits(self) -> List[float]:
-        return [self.to_transformed(lim) for lim in super().get_limits()]
+        return sorted(map(self.to_transformed, self.limits))
+
+    # --- setting or returning native coordinates -------------------------------------------------
+    # --- new messages introduce by this trait
 
-    # --- native properties -----------------------------------------------------------------------
+    @property
+    def limits(self) -> List[float]:
+        return self._joint_limit(
+            self._state["hw_limits"],
+            sorted(map(self.to_native, self._config["limits"])),
+            self._config["native_limits"],
+        )
 
     def get_native_reference(self) -> float:
         return self._state["native_reference_position"]
 
     def set_native_reference(self, native_position):
         self._state["native_reference_position"] = native_position
 
@@ -83,11 +98,11 @@
     def get_native_position(self) -> float:
         return self._state["position"]
 
     def get_native_destination(self) -> float:
         return self._state["destination"]
 
     def get_native_limits(self) -> List[float]:
-        return super().get_limits()
+        return self.limits
 
     def get_native_units(self) -> Optional[str]:
         return self._native_units
```

### Comparing `yaqd-core-2023.2.0/yaqd_core/_is_daemon.py` & `yaqd_core-2023.6.0/yaqd_core/_is_daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pathlib
 import signal
 import sys
 import time
 from typing import Dict, List, Optional, Any
 from abc import ABC
 
-import appdirs  # type: ignore
+import platformdirs  # type: ignore
 import tomli
 import tomli_w
 
 from .__version__ import __version__, __avro_version__
 from ._protocol import Protocol
 from . import logging
 from ._mro import assert_mro
@@ -55,24 +55,24 @@
             The path for the configuration (not used internally, availble to clients)
         """
 
         self.name = name
         self._config = config
         self._config_filepath = config_filepath
         self._state_filepath = (
-            pathlib.Path(appdirs.user_data_dir("yaqd-state", "yaq"))
+            platformdirs.user_data_path("yaqd-state", "yaq")
             / self._kind
             / f"{self.name}-state.toml"
         )
         self.logger = logging.getLogger(self.name)
         if "log_level" in self._config:
             self.logger.setLevel(logging.name_to_level[self._config["log_level"]])
         if self._config.get("log_to_file"):
             log_path = (
-                pathlib.Path(appdirs.user_log_dir(f"yaqd-{self._kind}", "yaq"))
+                platformdirs.user_log_path(f"yaqd-{self._kind}", "yaq")
                 / f"{self.name}-{time.strftime('%Y%m%dT%H%M%S%z')}.log"
             )
             log_path.parent.mkdir(parents=True, exist_ok=True)
             fh = logging_.FileHandler(log_path)
             fh.setFormatter(logging.formatter)
             self.logger.addHandler(fh)
         self.logger.info(f"Config File Path = {self._config_filepath}")
@@ -135,17 +135,15 @@
             )
 
         parser = argparse.ArgumentParser()
         parser.add_argument(
             "--config",
             "-c",
             default=(
-                pathlib.Path(appdirs.user_config_dir("yaqd", "yaq"))
-                / cls._kind
-                / "config.toml"
+                platformdirs.user_config_path("yaqd", "yaq") / cls._kind / "config.toml"
             ),
             action="store",
             help="Path to the configuration toml file.",
         )
         parser.add_argument(
             "--verbose",
             "-v",
```

### Comparing `yaqd-core-2023.2.0/yaqd_core/_is_discrete.py` & `yaqd_core-2023.6.0/yaqd_core/_is_discrete.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/_is_sensor.py` & `yaqd_core-2023.6.0/yaqd_core/_is_sensor.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/_mro.py` & `yaqd_core-2023.6.0/yaqd_core/_mro.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/_protocol.py` & `yaqd_core-2023.6.0/yaqd_core/_protocol.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/_state.py` & `yaqd_core-2023.6.0/yaqd_core/_state.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/aserial/_aserial.py` & `yaqd_core-2023.6.0/yaqd_core/aserial/_aserial.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/avrorpc/__init__.py` & `yaqd_core-2023.6.0/yaqd_core/avrorpc/__init__.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/avrorpc/avro_numpy.py` & `yaqd_core-2023.6.0/yaqd_core/avrorpc/avro_numpy.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/avrorpc/handshake.py` & `yaqd_core-2023.6.0/yaqd_core/avrorpc/handshake.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/avrorpc/unpacker.py` & `yaqd_core-2023.6.0/yaqd_core/avrorpc/unpacker.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/logging/__init__.py` & `yaqd_core-2023.6.0/yaqd_core/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/yaqd_core/testing/_run_daemon.py` & `yaqd_core-2023.6.0/yaqd_core/testing/_run_daemon.py`

 * *Files identical despite different names*

### Comparing `yaqd-core-2023.2.0/PKG-INFO` & `yaqd_core-2023.6.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: yaqd-core
-Version: 2023.2.0
-Summary: Core python package for implementing yaq deamons, and associated utilities.
-Home-page: https://yaq.fyi
-Author: yaq developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Version: 2023.6.0
+Project-URL: Home Page, https://yaq.fyi
+Project-URL: Documentation, http://yaq-core-python.yaq.fyi/
+Project-URL: Source, https://github.com/yaq-project/yaq-python
+Project-URL: Issues, https://github.com/yaq-project/yaq-python/issues
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: appdirs
+Requires-Python: >=3.7
+Requires-Dist: fastavro>=1.4.0
+Requires-Dist: platformdirs
 Requires-Dist: tomli
 Requires-Dist: tomli-w
-Requires-Dist: fastavro>=1.4.0
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: pre-commit ; extra == "dev"
-Project-URL: Documentation, http://yaq-core-python.yaq.fyi/
-Project-URL: Issues, https://github.com/yaq-project/yaq-python/-/issues
-Project-URL: Source, https://github.com/yaq-project/yaq-python
 Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Description-Content-Type: text/markdown
 
 # yaqd-core-python
 
 [![PyPI](https://img.shields.io/pypi/v/yaqd-core)](https://pypi.org/project/yaqd-core)
 [![Conda](https://img.shields.io/conda/vn/conda-forge/yaqd-core)](https://anaconda.org/conda-forge/yaqd-core)
 [![black](https://img.shields.io/badge/code--style-black-black)](https://black.readthedocs.io/)
 [![ver](https://img.shields.io/badge/calver-YYYY.M.MICRO-blue)](https://calver.org/)
 [![log](https://img.shields.io/badge/change-log-informational)](https://github.com/yaq-project/yaq-python/blob/main/yaqd-core/CHANGELOG.md)
 
 Core python package for implementing yaq daemons, and associated utilities.
 
 Documentation at https://yaqd-core-python.yaq.fyi
-
```

