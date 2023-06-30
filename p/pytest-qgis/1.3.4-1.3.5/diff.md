# Comparing `tmp/pytest-qgis-1.3.4.tar.gz` & `tmp/pytest-qgis-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-qgis-1.3.4.tar", last modified: Fri Jun  9 12:32:21 2023, max compression
+gzip compressed data, was "pytest-qgis-1.3.5.tar", last modified: Fri Jun 30 09:17:16 2023, max compression
```

## Comparing `pytest-qgis-1.3.4.tar` & `pytest-qgis-1.3.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.542595 pytest-qgis-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/src/pytest_qgis/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/mock_qgis_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16365 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/pytest_qgis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/qgis_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/qgis_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/src/pytest_qgis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 12:32:21.000000 pytest-qgis-1.3.4/src/pytest_qgis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:32:21.546595 pytest-qgis-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/tests/test_ini.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/tests/test_pytest_qgis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/tests/test_qgis_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-09 12:32:12.000000 pytest-qgis-1.3.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:16.665632 pytest-qgis-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-06-30 09:17:16.665632 pytest-qgis-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 09:17:16.665632 pytest-qgis-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:16.661632 pytest-qgis-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:16.661632 pytest-qgis-1.3.5/src/pytest_qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/src/pytest_qgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/src/pytest_qgis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/src/pytest_qgis/mock_qgis_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/src/pytest_qgis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/src/pytest_qgis/pytest_qgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/src/pytest_qgis/qgis_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/src/pytest_qgis/qgis_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/src/pytest_qgis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:16.665632 pytest-qgis-1.3.5/src/pytest_qgis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-06-30 09:17:16.000000 pytest-qgis-1.3.5/src/pytest_qgis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-30 09:17:16.000000 pytest-qgis-1.3.5/src/pytest_qgis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:17:16.000000 pytest-qgis-1.3.5/src/pytest_qgis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 09:17:16.000000 pytest-qgis-1.3.5/src/pytest_qgis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 09:17:16.000000 pytest-qgis-1.3.5/src/pytest_qgis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 09:17:16.000000 pytest-qgis-1.3.5/src/pytest_qgis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:17:16.665632 pytest-qgis-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/tests/test_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/tests/test_pytest_qgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/tests/test_qgis_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-30 09:17:01.000000 pytest-qgis-1.3.5/tests/test_utils.py
```

### Comparing `pytest-qgis-1.3.4/LICENSE` & `pytest-qgis-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.4/PKG-INFO` & `pytest-qgis-1.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-qgis
-Version: 1.3.4
+Version: 1.3.5
 Summary: A pytest plugin for testing QGIS python plugins
 Home-page: https://github.com/GispoCoding/pytest-qgis
 Author: Joona Laine
 Author-email: info@gispo.fi
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 License: GNU GPL v2.0
@@ -64,20 +64,20 @@
   calls `processing.run(...)`.
 * `qgis_version` returns QGIS version number as integer.
 * `qgis_world_map_geopackage` returns Path to the world_map.gpkg that ships with QGIS
 * `qgis_countries_layer` returns Natural Earth countries layer from world.map.gpkg as QgsVectorLayer
 
 ### Markers
 
-* `qgis_show_map` lets developer inspect the QGIS map visually at the teardown of the test. Full signature of the marker
+* `qgis_show_map` lets developer inspect the QGIS map visually during the test and also at the teardown of the test. Full signature of the marker
   is:
   ```python
   @pytest.mark.qgis_show_map(timeout: int = 30, add_basemap: bool = False, zoom_to_common_extent: bool = True, extent: QgsRectangle = None)
   ```
-    * `timeout` is the time in seconds until the map is closed.
+    * `timeout` is the time in seconds until the map is closed. If timeout is zero, the map will be closed in teardown.
     * `add_basemap` when set to True, adds Natural Earth countries layer as the basemap for the map.
     * `zoom_to_common_extent` when set to True, centers the map around all layers in the project.
     * `extent` is alternative to `zoom_to_common_extent` and lets user specify the extent
       as [`QgsRectangle`](https://qgis.org/pyqgis/master/core/QgsRectangle.html)
 
 Check the marker api [documentation](https://docs.pytest.org/en/latest/mark.html)
 and [examples](https://docs.pytest.org/en/latest/example/markers.html#marking-whole-classes-or-modules) for the ways
```

### Comparing `pytest-qgis-1.3.4/README.md` & `pytest-qgis-1.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,20 @@
   calls `processing.run(...)`.
 * `qgis_version` returns QGIS version number as integer.
 * `qgis_world_map_geopackage` returns Path to the world_map.gpkg that ships with QGIS
 * `qgis_countries_layer` returns Natural Earth countries layer from world.map.gpkg as QgsVectorLayer
 
 ### Markers
 
-* `qgis_show_map` lets developer inspect the QGIS map visually at the teardown of the test. Full signature of the marker
+* `qgis_show_map` lets developer inspect the QGIS map visually during the test and also at the teardown of the test. Full signature of the marker
   is:
   ```python
   @pytest.mark.qgis_show_map(timeout: int = 30, add_basemap: bool = False, zoom_to_common_extent: bool = True, extent: QgsRectangle = None)
   ```
-    * `timeout` is the time in seconds until the map is closed.
+    * `timeout` is the time in seconds until the map is closed. If timeout is zero, the map will be closed in teardown.
     * `add_basemap` when set to True, adds Natural Earth countries layer as the basemap for the map.
     * `zoom_to_common_extent` when set to True, centers the map around all layers in the project.
     * `extent` is alternative to `zoom_to_common_extent` and lets user specify the extent
       as [`QgsRectangle`](https://qgis.org/pyqgis/master/core/QgsRectangle.html)
 
 Check the marker api [documentation](https://docs.pytest.org/en/latest/mark.html)
 and [examples](https://docs.pytest.org/en/latest/example/markers.html#marking-whole-classes-or-modules) for the ways
```

### Comparing `pytest-qgis-1.3.4/setup.cfg` & `pytest-qgis-1.3.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = pytest-qgis
 author = Joona Laine
 author_email = info@gispo.fi
 maintainer = Gispo Ltd.
 maintainer_email = info@gispo.fi
-version = 1.3.4
+version = 1.3.5
 description = A pytest plugin for testing QGIS python plugins
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = pytest,qgis,QGIS,PyQGIS
 url = https://github.com/GispoCoding/pytest-qgis
 license = GNU GPL v2.0
 classifiers = 
@@ -59,14 +59,15 @@
 	src/pytest_qgis/pytest_qgis.py:QGS105
 	src/pytest_qgis/qgis_interface.py:N802,N803
 	tests/*:ANN001,ANN201
 extend-ignore = 
 	E203,
 	ANN101,
 	PT004
+ban-relative-imports = true
 
 [isort]
 profile = black
 multi_line_output = 3
 
 [mypy]
 disable_error_code = misc
```

### Comparing `pytest-qgis-1.3.4/setup.py` & `pytest-qgis-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.4/src/pytest_qgis/__init__.py` & `pytest-qgis-1.3.5/src/pytest_qgis/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.4/src/pytest_qgis/_version.py` & `pytest-qgis-1.3.5/src/pytest_qgis/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with pytest-qgis.  If not, see <https://www.gnu.org/licenses/>.
 
 
-__version__ = "1.3.2"
+__version__ = "1.3.5"
```

### Comparing `pytest-qgis-1.3.4/src/pytest_qgis/mock_qgis_classes.py` & `pytest-qgis-1.3.5/src/pytest_qgis/mock_qgis_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (C) 2021 pytest-qgis Contributors.
+#  Copyright (C) 2021-2023 pytest-qgis Contributors.
 #
 #
 #  This file is part of pytest-qgis.
 #
 #  pytest-qgis is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 2 of the License, or
@@ -35,13 +35,13 @@
             Qgis.Success: [],
         }
 
     def get_messages(self, level: int) -> List[str]:
         """Used to test which messages have been logged."""
         return self.messages[level]
 
-    def pushMessage(  # noqa N802
+    def pushMessage(  # noqa: N802
         self, title: str, text: str, level: int, duration: int
     ) -> None:
         """A mocked method for pushing a message to the bar."""
         msg = f"{title}:{text}"
         self.messages[level].append(msg)
```

### Comparing `pytest-qgis-1.3.4/src/pytest_qgis/pytest_qgis.py` & `pytest-qgis-1.3.5/src/pytest_qgis/pytest_qgis.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with pytest-qgis.  If not, see <https://www.gnu.org/licenses/>.
 
-
+import contextlib
 import os.path
 import shutil
 import sys
 import tempfile
 import time
 import warnings
 from collections import namedtuple
@@ -151,15 +151,17 @@
 
     if not request.config._plugin_settings.qgis_init_disabled:
         assert _APP
         if not sip.isdeleted(_CANVAS) and _CANVAS is not None:
             _CANVAS.deleteLater()
         _APP.exitQgis()
         if _QGIS_CONFIG_PATH and _QGIS_CONFIG_PATH.exists():
-            shutil.rmtree(_QGIS_CONFIG_PATH)
+            # TODO: https://github.com/GispoCoding/pytest-qgis/issues/43
+            with contextlib.suppress(PermissionError):
+                shutil.rmtree(_QGIS_CONFIG_PATH)
 
 
 @pytest.fixture(scope="session")
 def qgis_parent(qgis_app: QgsApplication) -> QWidget:
     return _PARENT
 
 
@@ -184,23 +186,23 @@
     """
     Initializes QGIS processing framework
     """
     _initialize_processing(qgis_app)
 
 
 @pytest.fixture()
-def qgis_new_project(qgis_iface: QgisInterface) -> None:  # noqa QGS105
+def qgis_new_project(qgis_iface: QgisInterface) -> None:  # noqa: QGS105
     """
     Initializes new QGIS project by removing layers and relations etc.
     """
     qgis_iface.newProject()
 
 
 @pytest.fixture()
-def new_project(qgis_iface: QgisInterface) -> None:  # noqa QGS105
+def new_project(qgis_iface: QgisInterface) -> None:  # noqa: QGS105
     """
     Initializes new QGIS project by removing layers and relations etc.
 
     Deprecated: use qgis_new_project instead.
     """
     warnings.warn(
         "new_project fixture will be deprecated. " "Use qgis_new_project instead.",
@@ -260,14 +262,18 @@
     """
     Shows QGIS map if qgis_show_map marker is used.
     """
     show_map_marker = request.node.get_closest_marker(SHOW_MAP_MARKER)
     common_settings: Settings = request.config._plugin_settings  # type: ignore
 
     if show_map_marker:
+        # Assign the bridge to have correct layer order and visibilities
+        bridge = QgsLayerTreeMapCanvasBridge(  # noqa: F841, this needs to be assigned
+            QgsProject.instance().layerTreeRoot(), qgis_iface.mapCanvas()
+        )
         _show_qgis_dlg(common_settings, qgis_parent)
 
     yield
 
     if (
         show_map_marker
         and common_settings.gui_enabled
@@ -292,14 +298,15 @@
 
     if not settings.qgis_init_disabled:
         _APP = QgsApplication([], GUIenabled=settings.gui_enabled)
         _APP.initQgis()
         QgsGui.editorWidgetRegistry().initEditors()
     _PARENT = QMainWindow()
     _CANVAS = QgsMapCanvas(_PARENT)
+    _PARENT.resize(QtCore.QSize(settings.canvas_width, settings.canvas_height))
     _CANVAS.resize(QtCore.QSize(settings.canvas_width, settings.canvas_height))
 
     # QgisInterface is a stub implementation of the QGIS plugin interface
     _IFACE = QgisInterface(_CANVAS, MockMessageBar(), _PARENT)
 
     # Patching imported iface (evaluated as None in tests) with iface.
     # This only works with QGIS >= 3.18 since before that
@@ -317,42 +324,44 @@
         sys.path.append(python_plugins_path)
     from processing.core.Processing import Processing
 
     Processing.initialize()
 
 
 def _show_qgis_dlg(common_settings: Settings, qgis_parent: QWidget) -> None:
-    if common_settings.gui_enabled and not common_settings.qgis_init_disabled:
+    if not common_settings.qgis_init_disabled:
         qgis_parent.setWindowTitle("Test QGIS dialog opened by Pytest-qgis")
         qgis_parent.show()
-    elif not common_settings.gui_enabled:
-        warnings.warn(
-            "Cannot show QGIS map because the GUI is not enabled. "
-            "Set qgis_qui_enabled=True in pytest.ini.",
-            stacklevel=1,
-        )
     elif common_settings.qgis_init_disabled:
         warnings.warn(
             "Cannot show QGIS map because QGIS is not initialized. "
             "Run the tests without --qgis_disable_init to enable QGIS map.",
             stacklevel=1,
         )
+    if not common_settings.gui_enabled:
+        warnings.warn(
+            "QGIS map is not visible because the GUI is not enabled. "
+            "Set qgis_qui_enabled=True in pytest.ini to see the window.",
+            stacklevel=1,
+        )
 
 
 def _configure_qgis_map(
     qgis_app: QgsApplication,
     qgis_iface: QgisInterface,
     qgis_parent: QWidget,
     settings: ShowMapSettings,
     tmp_path: Path,
 ) -> None:
+    if settings.timeout == 0:
+        qgis_parent.close()
+        return
+
     message_box = QMessageBox(qgis_parent)
-    bridge = QgsLayerTreeMapCanvasBridge(  # noqa: F841, this needs to be assigned
-        QgsProject.instance().layerTreeRoot(), qgis_iface.mapCanvas()
-    )
+
     try:
         # Change project CRS to most common CRS if it is not set
         if not QgsProject.instance().crs().isValid():
             set_map_crs_based_on_layers()
 
         extent = settings.extent
         if settings.zoom_to_common_extent and extent is None:
@@ -379,18 +388,15 @@
 
         message_box.setWindowTitle("pytest-qgis")
         message_box.setText(
             "Click close to close the map and to end the test.\n"
             f"It will close automatically in {settings.timeout} seconds."
         )
         message_box.addButton(QMessageBox.Close)
-        message_box.move(
-            message_box.mapToGlobal(qgis_parent.rect().topLeft())
-            - QtCore.QPoint(message_box.width(), 0)
-        )
+        message_box.move(QgsApplication.instance().primaryScreen().geometry().topLeft())
         message_box.setWindowModality(QtCore.Qt.NonModal)
         message_box.show()
 
         t = time.time()
         while time.time() - t < settings.timeout and message_box.isVisible():
             QCoreApplication.processEvents()
     finally:
@@ -469,16 +475,15 @@
     """Copy geopackage to the temporary directory and return the copy."""
     world_map_gpkg = Path(
         QgsApplication.pkgDataPath(), "resources", "data", "world_map.gpkg"
     )
     assert world_map_gpkg.exists(), world_map_gpkg
 
     # Copy the geopackage to allow modifications
-    path_to_copied_geopackage = Path(shutil.copy(world_map_gpkg, tmp_path))
-    return path_to_copied_geopackage
+    return Path(shutil.copy(world_map_gpkg, tmp_path))
 
 
 def _get_countries_layer(geopackage: Path) -> QgsVectorLayer:
     countries_layer = QgsVectorLayer(
         f"{geopackage}|layername=countries",
         "Natural Earth Countries",
         "ogr",
```

### Comparing `pytest-qgis-1.3.4/src/pytest_qgis/qgis_bot.py` & `pytest-qgis-1.3.5/src/pytest_qgis/qgis_bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (C) 2021-2022 pytest-qgis Contributors.
+#  Copyright (C) 2021-2023 pytest-qgis Contributors.
 #
 #
 #  This file is part of pytest-qgis.
 #
 #  pytest-qgis is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 2 of the License, or
@@ -101,19 +101,21 @@
         Gets recursively all attribute dialog widgets by name.
         :param widget: QgsAttributeDialog for the first time, afterwards QWidget.
         :return: Dictionary with field names as keys and corresponding
         QWidgets as values.
         """
         widgets_by_name = {}
         for child in widget.children():
-            if isinstance(child, QLabel):
-                if child.text() != "" and child.toolTip() != "":
-                    related_widget = child.buddy()
-                    if related_widget is not None:
-                        widgets_by_name[child.text()] = child.buddy()
+            if (
+                isinstance(child, QLabel)
+                and child.text() != ""
+                and child.toolTip() != ""
+                and child.buddy() is not None
+            ):
+                widgets_by_name[child.text()] = child.buddy()
             if hasattr(child, "children"):
                 widgets_by_name = {
                     **widgets_by_name,
                     **QgisBot.get_qgs_attribute_dialog_widgets_by_name(child),
                 }
 
         return widgets_by_name
```

### Comparing `pytest-qgis-1.3.4/src/pytest_qgis/qgis_interface.py` & `pytest-qgis-1.3.5/src/pytest_qgis/qgis_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 __author__ = "tim@linfiniti.com"
 __revision__ = "$Format:%H$"
 __date__ = "10/01/2011"
 __copyright__ = (
     "Copyright (c) 2010 by Ivan Mincik, ivan.mincik@gista.sk and "
     "Copyright (c) 2011 German Carrillo, geotux_tuxman@linuxmail.org"
     "Copyright (c) 2014 Tim Sutton, tim@linfiniti.com"
-    "Copyright (c) 2021 pytest-qgis Contributors"
+    "Copyright (c) 2021-2023 pytest-qgis Contributors"
 )
 
 import logging
 from typing import Dict, List, Optional, Union
 
-import sip
 from qgis.core import (
     QgsLayerTree,
     QgsMapLayer,
     QgsProject,
     QgsRelationManager,
     QgsVectorLayer,
 )
 from qgis.gui import QgsMapCanvas
+from qgis.PyQt import sip
 from qgis.PyQt.QtCore import QObject, pyqtSignal, pyqtSlot
 from qgis.PyQt.QtWidgets import (
     QAction,
     QDockWidget,
     QMainWindow,
     QMenuBar,
     QToolBar,
@@ -57,16 +57,16 @@
 class QgisInterface(QObject):
     """Class to expose QGIS objects and functions to plugins.
 
     This class is here for enabling us to run unit tests only,
     so most methods are simply stubs.
     """
 
-    currentLayerChanged = pyqtSignal(QgsMapCanvas)  # noqa N802
-    newProjectCreated = pyqtSignal()  # noqa N802
+    currentLayerChanged = pyqtSignal(QgsMapCanvas)  # noqa: N815
+    newProjectCreated = pyqtSignal()  # noqa: N815
 
     def __init__(
         self, canvas: QgsMapCanvas, messageBar: MockMessageBar, mainWindow: QMainWindow
     ) -> None:
         """Constructor
         :param canvas:
         """
@@ -138,27 +138,23 @@
         self._layers = []
         self.newProjectCreated.emit()
 
     # ---------------- API Mock for QgsInterface follows -------------------
 
     def zoomFull(self) -> None:
         """Zoom to the map full extent."""
-        pass
 
     def zoomToPrevious(self) -> None:
         """Zoom to previous view extent."""
-        pass
 
     def zoomToNext(self) -> None:
         """Zoom to next view extent."""
-        pass
 
     def zoomToActiveLayer(self) -> None:
         """Zoom to extent of active layer."""
-        pass
 
     def addVectorLayer(
         self, path: str, base_name: str, provider_key: str
     ) -> QgsVectorLayer:
         """Add a vector layer.
 
         :param path: Path to layer.
@@ -179,15 +175,14 @@
 
         :param path: Path to layer.
         :type path: str
 
         :param base_name: Base name for layer.
         :type base_name: str
         """
-        pass
 
     def activeLayer(self) -> Optional[QgsMapLayer]:
         """Get pointer to the active layer (layer selected in the legend)."""
         return (
             QgsProject.instance().mapLayer(self._active_layer_id)
             if self._active_layer_id
             else None
@@ -198,31 +193,28 @@
 
         :param name: Name of the menu item
         :type name: str
 
         :param action: Action to add to menu.
         :type action: QAction
         """
-        pass
 
     def addToolBarIcon(self, action: QAction) -> None:
         """Add an icon to the plugins toolbar.
 
         :param action: Action to add to the toolbar.
         :type action: QAction
         """
-        pass
 
     def removeToolBarIcon(self, action: QAction) -> None:
         """Remove an action (icon) from the plugin toolbar.
 
         :param action: Action to add to the toolbar.
         :type action: QAction
         """
-        pass
 
     def addToolBar(self, toolbar: Union[str, QToolBar]) -> QToolBar:
         """Add toolbar with specified name.
 
         :param toolbar: Name for the toolbar or QToolBar object.
         """
         if isinstance(toolbar, str):
@@ -241,26 +233,23 @@
     def mainWindow(self) -> QWidget:
         """Return a pointer to the main window.
 
         In case of QGIS it returns an instance of QgisApp.
         """
         return self._mainWindow
 
-    def addDockWidget(
-        self, area: int, dock_widget: QDockWidget
-    ) -> None:  # noqa: ANN001
+    def addDockWidget(self, area: int, dock_widget: QDockWidget) -> None:
         """Add a dock widget to the main window.
 
         :param area: Where in the ui the dock should be placed.
         :type area: Qt.DockWidgetArea
 
         :param dock_widget: A dock widget to add to the UI.
         :type dock_widget: QDockWidget
         """
-        pass
 
     def legendInterface(self) -> QgsMapCanvas:
         """Get the legend."""
         return self.canvas
 
     def messageBar(self) -> MockMessageBar:
         """Get the messagebar"""
```

### Comparing `pytest-qgis-1.3.4/src/pytest_qgis/utils.py` & `pytest-qgis-1.3.5/src/pytest_qgis/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (C) 2021 pytest-qgis Contributors.
+#  Copyright (C) 2021-2023 pytest-qgis Contributors.
 #
 #
 #  This file is part of pytest-qgis.
 #
 #  pytest-qgis is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 2 of the License, or
@@ -17,28 +17,28 @@
 #  along with pytest-qgis.  If not, see <https://www.gnu.org/licenses/>.
 #
 from collections import Counter
 from functools import wraps
 from pathlib import Path
 from typing import Any, Callable, List, Optional
 
-import sip
 from osgeo import gdal
 from qgis.core import (
     QgsCoordinateReferenceSystem,
     QgsCoordinateTransform,
     QgsLayerTree,
     QgsLayerTreeGroup,
     QgsLayerTreeLayer,
     QgsMapLayer,
     QgsProject,
     QgsRasterLayer,
     QgsRectangle,
     QgsVectorLayer,
 )
+from qgis.PyQt import sip
 
 DEFAULT_RASTER_FORMAT = "tif"
 
 DEFAULT_CRS = QgsCoordinateReferenceSystem("EPSG:4326")
 
 
 def get_common_extent_from_all_layers() -> Optional[QgsRectangle]:
@@ -83,16 +83,15 @@
         return rectangle
 
     transform = QgsCoordinateTransform(
         QgsCoordinateReferenceSystem(in_crs),
         QgsCoordinateReferenceSystem(out_crs),
         QgsProject.instance(),
     )
-    box = transform.transformBoundingBox(rectangle)
-    return box
+    return transform.transformBoundingBox(rectangle)
 
 
 def get_layers_with_different_crs() -> List[QgsMapLayer]:
     map_crs = QgsProject.instance().crs()
     return [
         layer
         for layer in QgsProject.instance().mapLayers().values()
@@ -133,15 +132,15 @@
             output_raster = str(
                 Path(output_path, f"{input_layer.name()}.{DEFAULT_RASTER_FORMAT}")
             )
             warp = gdal.Warp(
                 output_raster, input_layer.source(), dstSRS=map_crs.authid()
             )
         finally:
-            warp = None  # noqa F841
+            warp = None  # noqa: F841
 
         copy_layer_style_and_position(
             input_layer, QgsRasterLayer(output_raster), output_path
         )
 
     # Remove originals from project
     QgsProject.instance().removeMapLayers([layer.id() for layer in layers])
```

### Comparing `pytest-qgis-1.3.4/src/pytest_qgis.egg-info/PKG-INFO` & `pytest-qgis-1.3.5/src/pytest_qgis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-qgis
-Version: 1.3.4
+Version: 1.3.5
 Summary: A pytest plugin for testing QGIS python plugins
 Home-page: https://github.com/GispoCoding/pytest-qgis
 Author: Joona Laine
 Author-email: info@gispo.fi
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 License: GNU GPL v2.0
@@ -64,20 +64,20 @@
   calls `processing.run(...)`.
 * `qgis_version` returns QGIS version number as integer.
 * `qgis_world_map_geopackage` returns Path to the world_map.gpkg that ships with QGIS
 * `qgis_countries_layer` returns Natural Earth countries layer from world.map.gpkg as QgsVectorLayer
 
 ### Markers
 
-* `qgis_show_map` lets developer inspect the QGIS map visually at the teardown of the test. Full signature of the marker
+* `qgis_show_map` lets developer inspect the QGIS map visually during the test and also at the teardown of the test. Full signature of the marker
   is:
   ```python
   @pytest.mark.qgis_show_map(timeout: int = 30, add_basemap: bool = False, zoom_to_common_extent: bool = True, extent: QgsRectangle = None)
   ```
-    * `timeout` is the time in seconds until the map is closed.
+    * `timeout` is the time in seconds until the map is closed. If timeout is zero, the map will be closed in teardown.
     * `add_basemap` when set to True, adds Natural Earth countries layer as the basemap for the map.
     * `zoom_to_common_extent` when set to True, centers the map around all layers in the project.
     * `extent` is alternative to `zoom_to_common_extent` and lets user specify the extent
       as [`QgsRectangle`](https://qgis.org/pyqgis/master/core/QgsRectangle.html)
 
 Check the marker api [documentation](https://docs.pytest.org/en/latest/mark.html)
 and [examples](https://docs.pytest.org/en/latest/example/markers.html#marking-whole-classes-or-modules) for the ways
```

### Comparing `pytest-qgis-1.3.4/src/pytest_qgis.egg-info/SOURCES.txt` & `pytest-qgis-1.3.5/src/pytest_qgis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.4/tests/test_ini.py` & `pytest-qgis-1.3.5/tests/test_ini.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.4/tests/test_pytest_qgis.py` & `pytest-qgis-1.3.5/tests/test_pytest_qgis.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import TYPE_CHECKING
 
 import pytest
 from qgis.core import Qgis, QgsProcessing, QgsProject, QgsVectorLayer
 from qgis.PyQt.QtWidgets import QToolBar
 from qgis.utils import iface
 
-from .utils import QGIS_VERSION
+from tests.utils import QGIS_VERSION
 
 if TYPE_CHECKING:
     pass
 
 # DO not use this directly, this is only meant to be used with
 # replace_iface_with_qgis_iface fixture
 __iface = None
@@ -41,15 +41,14 @@
 @pytest.mark.usefixtures("replace_iface_with_qgis_iface")
 def test_a_teardown():
     """
     When replacing imported or passed QgisInterface inside a fixture,
     it might cause problems with pytest_qgis.qgis_interface.removeAllLayers
     when qgis_app is exiting.
     """
-    pass
 
 
 def test_add_layer():
     layer = QgsVectorLayer("Polygon", "dummy_polygon_layer", "memory")
     QgsProject.instance().addMapLayer(layer)
     assert set(QgsProject.instance().mapLayers().values()) == {layer}
```

### Comparing `pytest-qgis-1.3.4/tests/test_qgis_bot.py` & `pytest-qgis-1.3.5/tests/test_qgis_bot.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.4/tests/test_utils.py` & `pytest-qgis-1.3.5/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (C) 2021 pytest-qgis Contributors.
+#  Copyright (C) 2021-2023 pytest-qgis Contributors.
 #
 #
 #  This file is part of pytest-qgis.
 #
 #  pytest-qgis is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 2 of the License, or
@@ -13,26 +13,25 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with pytest-qgis.  If not, see <https://www.gnu.org/licenses/>.
 
 import pytest
-import sip
 from qgis.core import QgsCoordinateReferenceSystem, QgsProject, QgsVectorLayer
+from qgis.PyQt import sip
 
 from pytest_qgis.utils import (
     clean_qgis_layer,
     get_common_extent_from_all_layers,
     get_layers_with_different_crs,
     replace_layers_with_reprojected_clones,
     set_map_crs_based_on_layers,
 )
-
-from .utils import QGIS_VERSION
+from tests.utils import QGIS_VERSION
 
 EPSG_4326 = "EPSG:4326"
 EPSG_3067 = "EPSG:3067"
 
 DEFAULT_CRS = QgsCoordinateReferenceSystem(EPSG_4326)
```

