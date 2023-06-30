# Comparing `tmp/xrdPlanner-1.0.2.tar.gz` & `tmp/xrdPlanner-2023.6.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrdPlanner-1.0.2.tar", last modified: Fri Jun 30 08:43:25 2023, max compression
+gzip compressed data, was "xrdPlanner-2023.6.21.tar", last modified: Wed Jun 21 08:08:53 2023, max compression
```

## Comparing `xrdPlanner-1.0.2.tar` & `xrdPlanner-2023.6.21.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2023-06-30 08:43:25.935605 xrdPlanner-1.0.2/
--rw-rw-r--   0 au577597 (1644281986) staff       (20)    35149 2023-06-21 09:32:27.000000 xrdPlanner-1.0.2/LICENSE
--rw-r--r--   0 au577597 (1644281986) staff       (20)     5925 2023-06-30 08:43:25.935476 xrdPlanner-1.0.2/PKG-INFO
--rw-rw-r--   0 au577597 (1644281986) staff       (20)     5219 2023-06-30 08:41:44.000000 xrdPlanner-1.0.2/README.md
--rw-r--r--   0 au577597 (1644281986) staff       (20)       38 2023-06-30 08:43:25.935648 xrdPlanner-1.0.2/setup.cfg
--rw-r--r--   0 au577597 (1644281986) staff       (20)     1252 2023-06-30 08:38:31.000000 xrdPlanner-1.0.2/setup.py
-drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2023-06-30 08:43:25.934305 xrdPlanner-1.0.2/xrdPlanner/
--rw-r--r--   0 au577597 (1644281986) staff       (20)       75 2023-06-30 08:38:12.000000 xrdPlanner-1.0.2/xrdPlanner/__init__.py
--rw-r--r--   0 au577597 (1644281986) staff       (20)    55868 2023-06-30 08:37:53.000000 xrdPlanner-1.0.2/xrdPlanner/classes.py
--rw-r--r--   0 au577597 (1644281986) staff       (20)    93475 2023-06-21 07:00:20.000000 xrdPlanner-1.0.2/xrdPlanner/resources.py
--rw-rw-r--   0 au577597 (1644281986) staff       (20)      256 2023-06-21 06:49:34.000000 xrdPlanner-1.0.2/xrdPlanner/run_xrdPlanner.py
-drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2023-06-30 08:43:25.935266 xrdPlanner-1.0.2/xrdPlanner.egg-info/
--rw-r--r--   0 au577597 (1644281986) staff       (20)     5925 2023-06-30 08:43:25.000000 xrdPlanner-1.0.2/xrdPlanner.egg-info/PKG-INFO
--rw-r--r--   0 au577597 (1644281986) staff       (20)      330 2023-06-30 08:43:25.000000 xrdPlanner-1.0.2/xrdPlanner.egg-info/SOURCES.txt
--rw-r--r--   0 au577597 (1644281986) staff       (20)        1 2023-06-30 08:43:25.000000 xrdPlanner-1.0.2/xrdPlanner.egg-info/dependency_links.txt
--rw-r--r--   0 au577597 (1644281986) staff       (20)       62 2023-06-30 08:43:25.000000 xrdPlanner-1.0.2/xrdPlanner.egg-info/entry_points.txt
--rw-r--r--   0 au577597 (1644281986) staff       (20)       77 2023-06-30 08:43:25.000000 xrdPlanner-1.0.2/xrdPlanner.egg-info/requires.txt
--rw-r--r--   0 au577597 (1644281986) staff       (20)       11 2023-06-30 08:43:25.000000 xrdPlanner-1.0.2/xrdPlanner.egg-info/top_level.txt
+drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2023-06-21 08:08:53.647622 xrdPlanner-2023.6.21/
+-rw-rw-r--   0 au577597 (1644281986) staff       (20)    18092 2023-06-16 09:45:06.000000 xrdPlanner-2023.6.21/LICENSE
+-rw-r--r--   0 au577597 (1644281986) staff       (20)     4640 2023-06-21 08:08:53.647515 xrdPlanner-2023.6.21/PKG-INFO
+-rw-rw-r--   0 au577597 (1644281986) staff       (20)     3930 2023-06-21 08:06:37.000000 xrdPlanner-2023.6.21/README.md
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       38 2023-06-21 08:08:53.647656 xrdPlanner-2023.6.21/setup.cfg
+-rw-r--r--   0 au577597 (1644281986) staff       (20)     1257 2023-06-21 08:06:42.000000 xrdPlanner-2023.6.21/setup.py
+drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2023-06-21 08:08:53.646614 xrdPlanner-2023.6.21/xrdPlanner/
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       80 2023-06-21 08:07:18.000000 xrdPlanner-2023.6.21/xrdPlanner/__init__.py
+-rw-rw-r--   0 au577597 (1644281986) staff       (20)    50103 2023-06-21 07:56:07.000000 xrdPlanner-2023.6.21/xrdPlanner/classes.py
+-rw-r--r--   0 au577597 (1644281986) staff       (20)    93475 2023-06-21 07:00:20.000000 xrdPlanner-2023.6.21/xrdPlanner/resources.py
+-rw-rw-r--   0 au577597 (1644281986) staff       (20)      256 2023-06-21 06:49:34.000000 xrdPlanner-2023.6.21/xrdPlanner/run_xrdPlanner.py
+drwxr-xr-x   0 au577597 (1644281986) staff       (20)        0 2023-06-21 08:08:53.647364 xrdPlanner-2023.6.21/xrdPlanner.egg-info/
+-rw-r--r--   0 au577597 (1644281986) staff       (20)     4640 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/PKG-INFO
+-rw-r--r--   0 au577597 (1644281986) staff       (20)      330 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/SOURCES.txt
+-rw-r--r--   0 au577597 (1644281986) staff       (20)        1 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/dependency_links.txt
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       62 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/entry_points.txt
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       77 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/requires.txt
+-rw-r--r--   0 au577597 (1644281986) staff       (20)       11 2023-06-21 08:08:53.000000 xrdPlanner-2023.6.21/xrdPlanner.egg-info/top_level.txt
```

### Comparing `xrdPlanner-1.0.2/PKG-INFO` & `xrdPlanner-2023.6.21/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrdPlanner
-Version: 1.0.2
+Version: 2023.6.21
 Summary: A tool to project X-ray diffraction cones on a detector screen at different geometries (tilt, rotation, offset) and X-ray energies.
 Home-page: https://github.com/LennardKrause/xrdPlanner/
 Author: Lennard Krause
 Author-email: lkrause@chem.au.dk
 License: GNU GENERAL PUBLIC LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -15,48 +15,31 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xrdPlanner
 #### A tool to project X-ray diffraction cones on a detector screen at different geometries (tilt, rotation, offset) and X-ray energies
  - Main application is to visualize the maximum achievable resolution at a given geometry.
  - Is able to project diffraction cones for standard samples or directly from cif files.
- - Can turn out valuable when planning beamtimes at synchrotron facilities (e.g. [DanMAX](https://www.maxiv.lu.se/beamlines-accelerators/beamlines/danmax/)).
- - Helps in deciding on the geometry of an experiment.
+ - Can turn out valuable when planning beamtimes and deciding on the geometry of the experiment.
  - The math used is not meant to bring people to the moon but to provide a quick and simple preview.
- - The module building code is designed for [Dectris](https://www.dectris.com) [PILATUS3](https://www.dectris.com/detectors/x-ray-detectors/pilatus3/) / [EIGER2](https://www.dectris.com/detectors/x-ray-detectors/eiger2/) or [SACLA](https://sacla.xfel.jp/?lang=en) MPCCD Detectors (central hole geometry) but one-module systems like the [Bruker](https://www.bruker.com/en.html) [Photon II](https://www.bruker.com/en/products-and-solutions/diffractometers-and-scattering-systems/single-crystal-x-ray-diffractometers/sc-xrd-components/detectors.html) and [Rayonix](https://www.rayonix.com/) [MX-HS](https://www.rayonix.com/rayonix-mx-hs-series/) are possible as well.
+ - The module building code is designed for [Dectris](https://www.dectris.com) [PILATUS3](https://www.dectris.com/detectors/x-ray-detectors/pilatus3/) / [EIGER2](https://www.dectris.com/detectors/x-ray-detectors/eiger2/) and [SACLA](https://sacla.xfel.jp/?lang=en) MPCCD Detectors (central hole geometry) but one-module systems like the [Bruker](https://www.bruker.com/en.html) [Photon II](https://www.bruker.com/en/products-and-solutions/diffractometers-and-scattering-systems/single-crystal-x-ray-diffractometers/sc-xrd-components/detectors.html) are possible as well.
  - It uses [python3](https://www.python.org), [numpy](https://numpy.org), [pyqt6](https://www.riverbankcomputing.com/software/pyqt/), [pyqtgraph](https://pyqtgraph.readthedocs.io/en/latest/), [pyFAI](https://pyfai.readthedocs.io/en/v2023.1/) and [Dans_Diffraction](https://github.com/DanPorter/Dans_Diffraction).
 
 ## Short how-to:
- - pip install xrdPlanner.
  - Type _xrdPlanner_ in a terminal and hit enter.
  - Choose a detector and a model from the _Detector_ menu.
  - Pick a reference from the _Reference_ menu to plot its contours ([pyFAI](https://pyfai.readthedocs.io/en/v2023.1/)).
  - Drop a .cif file onto the window to draw its contours ([Dans_Diffraction](https://github.com/DanPorter/Dans_Diffraction)), click a contour to get a hkl tooltip.
  - Use the units from the _Units_ menu you are the most comfortable with.
  - Hover over the grey line at the top to show the sliders. Click it to make it stay open.
  - Drag the sliders to change energy and geometry.
-
-## Customisation:
-  - Edit the _settings.json_ file and the _detector_db.json_ files.
-  - Use _Settings_ -> _Edit Settings_ or _Edit Detector db_.
-  - A click on _Apply Changes_ lets you see the difference.
-  - _"geo"_ determines the startup defaults.
-  - _"plo"_ customises the general layout and visuals.
-  - _"lmt"_ sets the limiting values of the geometry/energy sliders.
-  - Add all the missing detectors to the _detector_db.json_.
-  - I hope the variable naming is self-explanatory.
-
-## Known Bugs:
-  - Overwriting defaults while in darkmode requires a reset to go back to light mode.
+ - Edit the _settings.json_ file to suit your needs.
+ - Add all the missing detectors to the _detectors.json_ file.
 
 ## Latest updates:
-  - 2023-06-30 Update: Reference hkl intensity determines linewidth (irel).
-  - 2023-06-30 Bugfix: Reference lines stay after settings reload.
-  - 2023-06-23 Bugfix: Fixed several bugs with regard to the reloading of the settings file.
-  - 2023-06-21 Update: Settings files accessible from menu, changes can be applied on the fly.
   - 2023-06-14 Update: Big speed update.
   - 2023-06-01 Update: countourpy was dropped, the conics are now calculated directly instead of being evaluated on a grid.
   - 2023-05-25 Update: Dans_Diffraction is used in favour of gemmi as it allows the direct calculation of intensities from the cif.
   - 2023-04-26 Update: A hkl tooltip is shown on click on a contour (only for cif contours).
   - 2023-04-25 Bugfix: Segmented contours are now drawn properly.
   - 2023-04-20 Bugfix: Confined slider window mobility to main window area.
   - 2023-04-10 Bugfix: Main window aspect ratio on Windows (menu bar within window).
@@ -68,16 +51,10 @@
 ## Older updates
   - 2023-03-23 Update: Settings are saved to (if doesn't exist) or loaded from (if exists) a 'settings.json' file.
   - 2023-03-23 Update: Added horizontal offset support and slider.
   - 2022-06-07 Update: Added functionality to plot Standard (LaB6, CeO2, ...) contours (needs [pyFAI](https://pyfai.readthedocs.io/en/master/)).
   - 2022-04-28 Update: Changed contour line generation to accept a list of 2-theta values as input.
   - 2022-04-27 Update: Added support for [SACLA](https://sacla.xfel.jp/?lang=en) MPCCD Detectors (central hole geometry).
   - 2022-04-25 Bugfix: Calculation of the beamcenter (rotation and tilt).
-
-## Examples
-#### A PILATUS3 2M detector and a Silicon sample.
-![Preview](https://github.com/LennardKrause/xrdPlanner/blob/main/examples/PILATUS3_2M_Si.png)
-
-#### A rotated EIGER2 4M detector and a Aluminium sample (darkmode).
-![Preview](https://github.com/LennardKrause/xrdPlanner/blob/main/examples/EIGER2_4M_Al.png)
+  - 2022-04-25 Bugfix: Unresponsive radio buttons / redrawing the figure.
 
 #### I hope this turns out to be useful for someone!
```

### Comparing `xrdPlanner-1.0.2/README.md` & `xrdPlanner-2023.6.21/xrdPlanner.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
+Metadata-Version: 2.1
+Name: xrdPlanner
+Version: 2023.6.21
+Summary: A tool to project X-ray diffraction cones on a detector screen at different geometries (tilt, rotation, offset) and X-ray energies.
+Home-page: https://github.com/LennardKrause/xrdPlanner/
+Author: Lennard Krause
+Author-email: lkrause@chem.au.dk
+License: GNU GENERAL PUBLIC LICENSE
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Topic :: Education
+Classifier: Topic :: Scientific/Engineering
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # xrdPlanner
 #### A tool to project X-ray diffraction cones on a detector screen at different geometries (tilt, rotation, offset) and X-ray energies
  - Main application is to visualize the maximum achievable resolution at a given geometry.
  - Is able to project diffraction cones for standard samples or directly from cif files.
- - Can turn out valuable when planning beamtimes at synchrotron facilities (e.g. [DanMAX](https://www.maxiv.lu.se/beamlines-accelerators/beamlines/danmax/)).
- - Helps in deciding on the geometry of an experiment.
+ - Can turn out valuable when planning beamtimes and deciding on the geometry of the experiment.
  - The math used is not meant to bring people to the moon but to provide a quick and simple preview.
- - The module building code is designed for [Dectris](https://www.dectris.com) [PILATUS3](https://www.dectris.com/detectors/x-ray-detectors/pilatus3/) / [EIGER2](https://www.dectris.com/detectors/x-ray-detectors/eiger2/) or [SACLA](https://sacla.xfel.jp/?lang=en) MPCCD Detectors (central hole geometry) but one-module systems like the [Bruker](https://www.bruker.com/en.html) [Photon II](https://www.bruker.com/en/products-and-solutions/diffractometers-and-scattering-systems/single-crystal-x-ray-diffractometers/sc-xrd-components/detectors.html) and [Rayonix](https://www.rayonix.com/) [MX-HS](https://www.rayonix.com/rayonix-mx-hs-series/) are possible as well.
+ - The module building code is designed for [Dectris](https://www.dectris.com) [PILATUS3](https://www.dectris.com/detectors/x-ray-detectors/pilatus3/) / [EIGER2](https://www.dectris.com/detectors/x-ray-detectors/eiger2/) and [SACLA](https://sacla.xfel.jp/?lang=en) MPCCD Detectors (central hole geometry) but one-module systems like the [Bruker](https://www.bruker.com/en.html) [Photon II](https://www.bruker.com/en/products-and-solutions/diffractometers-and-scattering-systems/single-crystal-x-ray-diffractometers/sc-xrd-components/detectors.html) are possible as well.
  - It uses [python3](https://www.python.org), [numpy](https://numpy.org), [pyqt6](https://www.riverbankcomputing.com/software/pyqt/), [pyqtgraph](https://pyqtgraph.readthedocs.io/en/latest/), [pyFAI](https://pyfai.readthedocs.io/en/v2023.1/) and [Dans_Diffraction](https://github.com/DanPorter/Dans_Diffraction).
 
 ## Short how-to:
- - pip install xrdPlanner.
  - Type _xrdPlanner_ in a terminal and hit enter.
  - Choose a detector and a model from the _Detector_ menu.
  - Pick a reference from the _Reference_ menu to plot its contours ([pyFAI](https://pyfai.readthedocs.io/en/v2023.1/)).
  - Drop a .cif file onto the window to draw its contours ([Dans_Diffraction](https://github.com/DanPorter/Dans_Diffraction)), click a contour to get a hkl tooltip.
  - Use the units from the _Units_ menu you are the most comfortable with.
  - Hover over the grey line at the top to show the sliders. Click it to make it stay open.
  - Drag the sliders to change energy and geometry.
-
-## Customisation:
-  - Edit the _settings.json_ file and the _detector_db.json_ files.
-  - Use _Settings_ -> _Edit Settings_ or _Edit Detector db_.
-  - A click on _Apply Changes_ lets you see the difference.
-  - _"geo"_ determines the startup defaults.
-  - _"plo"_ customises the general layout and visuals.
-  - _"lmt"_ sets the limiting values of the geometry/energy sliders.
-  - Add all the missing detectors to the _detector_db.json_.
-  - I hope the variable naming is self-explanatory.
-
-## Known Bugs:
-  - Overwriting defaults while in darkmode requires a reset to go back to light mode.
+ - Edit the _settings.json_ file to suit your needs.
+ - Add all the missing detectors to the _detectors.json_ file.
 
 ## Latest updates:
-  - 2023-06-30 Update: Reference hkl intensity determines linewidth (irel).
-  - 2023-06-30 Bugfix: Reference lines stay after settings reload.
-  - 2023-06-23 Bugfix: Fixed several bugs with regard to the reloading of the settings file.
-  - 2023-06-21 Update: Settings files accessible from menu, changes can be applied on the fly.
   - 2023-06-14 Update: Big speed update.
   - 2023-06-01 Update: countourpy was dropped, the conics are now calculated directly instead of being evaluated on a grid.
   - 2023-05-25 Update: Dans_Diffraction is used in favour of gemmi as it allows the direct calculation of intensities from the cif.
   - 2023-04-26 Update: A hkl tooltip is shown on click on a contour (only for cif contours).
   - 2023-04-25 Bugfix: Segmented contours are now drawn properly.
   - 2023-04-20 Bugfix: Confined slider window mobility to main window area.
   - 2023-04-10 Bugfix: Main window aspect ratio on Windows (menu bar within window).
@@ -51,16 +51,10 @@
 ## Older updates
   - 2023-03-23 Update: Settings are saved to (if doesn't exist) or loaded from (if exists) a 'settings.json' file.
   - 2023-03-23 Update: Added horizontal offset support and slider.
   - 2022-06-07 Update: Added functionality to plot Standard (LaB6, CeO2, ...) contours (needs [pyFAI](https://pyfai.readthedocs.io/en/master/)).
   - 2022-04-28 Update: Changed contour line generation to accept a list of 2-theta values as input.
   - 2022-04-27 Update: Added support for [SACLA](https://sacla.xfel.jp/?lang=en) MPCCD Detectors (central hole geometry).
   - 2022-04-25 Bugfix: Calculation of the beamcenter (rotation and tilt).
-
-## Examples
-#### A PILATUS3 2M detector and a Silicon sample.
-![Preview](https://github.com/LennardKrause/xrdPlanner/blob/main/examples/PILATUS3_2M_Si.png)
-
-#### A rotated EIGER2 4M detector and a Aluminium sample (darkmode).
-![Preview](https://github.com/LennardKrause/xrdPlanner/blob/main/examples/EIGER2_4M_Al.png)
+  - 2022-04-25 Bugfix: Unresponsive radio buttons / redrawing the figure.
 
 #### I hope this turns out to be useful for someone!
```

### Comparing `xrdPlanner-1.0.2/setup.py` & `xrdPlanner-2023.6.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='xrdPlanner',
-    version='1.0.2',
+    version='2023.06.21',
     description='A tool to project X-ray diffraction cones on a detector screen at different geometries (tilt, rotation, offset) and X-ray energies.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/LennardKrause/xrdPlanner/',
     author='Lennard Krause',
     author_email='lkrause@chem.au.dk',
     license='GNU GENERAL PUBLIC LICENSE',
```

### Comparing `xrdPlanner-1.0.2/xrdPlanner/classes.py` & `xrdPlanner-2023.6.21/xrdPlanner/classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,33 +11,79 @@
 class MainWindow(QtWidgets.QMainWindow):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # set path home
         self.path = os.path.dirname(__file__)
         # add an icon
         self.setWindowIcon(QtGui.QIcon(':/icons/xrdPlanner.png'))
-        # enable antialiasing
-        pg.setConfigOptions(antialias=True)
 
         # Drag-and-Drop cif-file
         #  dropEvent()
         #  - check dropped file is a cif
         #  get_cif_reference()
         #  - use gemmi to get cell, centring and crystal  system from cif
         #  - use pyFAI get_d_spacings() to create contours
         self.setAcceptDrops(True)
         
         # set path to settings file
-        self.path_settings = os.path.join(self.path, 'settings.json')
-        # set path to detector database
-        self.path_detdb = os.path.join(self.path, 'detector_db.json')
-
-        # save/load parameters to/from file
+        self.file_dump = os.path.join(self.path, 'settings.json')
+        # save parameters to file
         self.init_par()
 
+        # experimental darkmode?
+        if self.plo.darkmode:
+            self.init_darkmode()
+        
+        # set window color
+        pg.setConfigOptions(background=self.plo.plot_bg_color, antialias=True)
+
+        ###########
+        # CONTOUR #
+        ###########
+        # generate contour levels
+        self.cont_geom_num = np.linspace(self.plo.conic_tth_min, self.plo.conic_tth_max, self.plo.conic_tth_num)
+
+        # get colormap
+        self.cont_cmap = pg.colormap.get(self.plo.conic_colormap)
+        
+        # reverse the colormap useful to increase visibility in darkmode
+        if self.plo.reverse_cmap:
+            self.cont_cmap.reverse()
+        
+        # What standards should be available as reference
+        # The d spacings will be imported from pyFAI
+        self.geo.ref_library = calibrant.names()
+        # dict to store custom reference data
+        self.geo.ref_custom = {}
+        self.geo.ref_custom_hkl = {}
+        
+        # get the detector specs
+        # - update: overwrite existing file after load
+        # - reset: overwrite existing file with defaults
+        self.detectors = self.get_det_library(update=self.plo.update_det_bank, reset=self.plo.reset_det_bank)
+
+        # pick current detector
+        self.det = self.get_specs_det(self.detectors, self.geo.det_type, self.geo.det_size)
+
+        # translate unit for plot title
+        self.geo.unit_names = ['2\U0001D6F3 [\u00B0]', 'd [\u212B\u207B\u00B9]', 'q [\u212B]', 'sin(\U0001D6F3)/\U0001D706 [\u212B]']
+        if self.geo.unit >= len(self.geo.unit_names):
+            print(f'Error: Valid geo.unit range is from 0 to {len(self.geo.unit_names)-1}, geo.unit={self.geo.unit}')
+            raise SystemExit
+
+        # init the hkl tooltip
+        font = QtGui.QFont()
+        font.setPixelSize(self.plo.conic_hkl_label_size)
+        font.setBold(True)
+        QtWidgets.QToolTip.setFont(font)
+
+        ###########
+        # GENERAL #
+        ###########
+
         # menubar is displayed within the main window on Windows
         # so we need to make space for it
         # no idea about other OS, if there are issues fix them here
         if sys.platform == 'win32':
             self.offset_win32 = self.menuBar().height() - int(round(self.plo.slider_margin/2, 0))
         else:
             self.offset_win32 = 0
@@ -60,75 +106,22 @@
         # added to avoid the error:
         # qt.pointer.dispatch: skipping QEventPoint(id=0 ts=0 pos=0,0 scn=482.023,246.011
         # gbl=482.023,246.011 Released ellipse=(1x1 ∡ 0) vel=0,0 press=-482.023,-246.011
         # last=-482.023,-246.011 Δ 482.023,246.011) : no target window
         self.ax.viewport().setAttribute(QtCore.Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
         self.layout.addWidget(self.ax)
 
-        # What standards should be available as reference
-        # The d spacings will be imported from pyFAI
-        self.ref_library = calibrant.names()
-        # dict to store custom reference data
-        self.ref_custom = {}
-        self.ref_custom_hkl = {}
-        
-        # initialise all that depends on the settings
-        # call this function to apply changes were made
-        # to the settings file -> change_settings()
-        self.init_modifiables()
-        
         # populate the menus with detectors, references and units
         self.init_menus()
         
         # initialize the screen
         self.init_screen()
 
         # add the slider frame
-        # this calls draw_conics(), 
-        # make sure that everything
-        # that is needed is initialised
-        self.sliderWidget = SliderWidget(self)
-
-    def init_modifiables(self):
-        # experimental darkmode?
-        if self.plo.darkmode:
-            self.init_darkmode()
-        
-        # set window color
-        self.ax.setBackground(self.plo.plot_bg_color)
-
-        # generate contour levels
-        self.cont_geom_num = np.linspace(self.plo.conic_tth_min, self.plo.conic_tth_max, self.plo.conic_tth_num)
-
-        # translate unit for plot title
-        self.unit_names = ['2\U0001D6F3 [\u00B0]', 'd [\u212B\u207B\u00B9]', 'q [\u212B]', 'sin(\U0001D6F3)/\U0001D706 [\u212B]']
-        if self.geo.unit >= len(self.unit_names):
-            print(f'Error: Valid geo.unit range is from 0 to {len(self.unit_names)-1}, geo.unit={self.geo.unit}')
-            raise SystemExit
-
-        # get colormap
-        self.cont_cmap = pg.colormap.get(self.plo.conic_colormap, skipCache=True)
-        
-        # reverse the colormap useful to increase visibility in darkmode
-        if self.plo.reverse_cmap:
-            self.cont_cmap.reverse()
-        
-        # get the detector specs
-        # - update: overwrite existing file after load
-        # - reset: overwrite existing file with defaults
-        self.detector_db = self.get_det_library(update=self.plo.update_det_bank, reset=self.plo.reset_det_bank)
-
-        # pick current detector
-        self.det = self.get_specs_det()
-
-        # init the hkl tooltip
-        font = QtGui.QFont()
-        font.setPixelSize(self.plo.conic_hkl_label_size)
-        font.setBold(True)
-        QtWidgets.QToolTip.setFont(font)
+        self.sliderWidget = SliderWidget(self, self.geo, self.plo, self.lmt)
 
     def init_darkmode(self):
         # set window color
         self.plo.conic_label_fill = '#000000'    # [str]    Contour label fill color
         # - reference contour section - 
         self.plo.conic_ref_color = '#202020'     # [color]  Reference contour color
         self.plo.det_module_color = '#EEEEEE'    # [color]  Detector module border color
@@ -217,19 +210,20 @@
         self.setMenuBar(menuBar)
 
         menu_det = menuBar.addMenu('Detector')
         group_det = QtGui.QActionGroup(self)
         group_det.setExclusive(True)
 
         # menu Detectors
-        for d in self.detector_db:
+        for d in self.detectors:
             d = d.upper()
             d_menu = QtWidgets.QMenu(d, self)
+            d_menu.setStatusTip('')
             menu_det.addMenu(d_menu)
-            for s in self.detector_db[d]['size']:
+            for s in self.detectors[d]['size']:
                 s = s.upper()
                 det_action = QtGui.QAction(s, self, checkable=True)
                 self.set_menu_action(det_action, self.change_detector, d, s)
                 d_menu.addAction(det_action)
                 group_det.addAction(det_action)
                 if d == self.geo.det_type.upper() and s == self.geo.det_size.upper():
                     det_action.setChecked(True)
@@ -246,92 +240,59 @@
         if 'None' == self.geo.reference:
             ref_action.setChecked(True)
         
         # menu Reference: add pyFAI library
         self.sub_menu_pyFAI = QtWidgets.QMenu('pyFAI', self)
         self.sub_menu_pyFAI.setStatusTip('')
         self.menu_ref.addMenu(self.sub_menu_pyFAI)
-        for ref_name in self.ref_library:
+        for ref_name in self.geo.ref_library:
             ref_action = QtGui.QAction(ref_name, self, checkable=True)
             self.set_menu_action(ref_action, self.change_reference, ref_name)
             self.sub_menu_pyFAI.addAction(ref_action)
             self.group_ref.addAction(ref_action)
             if ref_name == self.geo.reference:
                 ref_action.setChecked(True)
 
         # menu Reference: add Custom
         self.sub_menu_custom = QtWidgets.QMenu('Custom', self)
         self.sub_menu_custom.setStatusTip('Drag and Drop *.cif files.')
         self.menu_ref.addMenu(self.sub_menu_custom)
         
         # menu Units
-        menu_unit = menuBar.addMenu('Unit')
+        menu_unit = menuBar.addMenu('Units')
         group_unit = QtGui.QActionGroup(self)
         group_unit.setExclusive(True)
-        for unit_index, unit_name in enumerate(self.unit_names):
+        for unit_index, unit_name in enumerate(self.geo.unit_names):
             unit_action = QtGui.QAction(unit_name, self, checkable=True)
             self.set_menu_action(unit_action, self.change_units, unit_index)
             menu_unit.addAction(unit_action)
             group_unit.addAction(unit_action)
             if unit_index == self.geo.unit:
                 unit_action.setChecked(True)
-        
-        # menu Settings
-        menu_edit = menuBar.addMenu('Settings')
-        if sys.platform == 'win32':
-            tokens = [('Edit Detector db file', os.system, f'notepad {self.path_detdb}'),
-                      ('Edit Settings file', os.system, f'notepad {self.path_settings}'),
-                      ('Reload Settings', self.change_settings, None)]
-        elif sys.platform == 'linux':
-            tokens = [('Edit Detector db', os.system, f'xdg-open {self.path_detdb}'),
-                      ('Edit Settings', os.system, f'xdg-open {self.path_settings}'),
-                      ('Reload Settings', self.change_settings, None)]
-        else:
-            tokens = [('Edit Detector db', os.system, f'open -t {self.path_detdb}'),
-                      ('Edit Settings', os.system, f'open -t {self.path_settings}'),
-                      ('Reload Settings', self.change_settings, None)]
-        for (name, funct, command) in tokens:
-            edit_action = QtGui.QAction(name, self)
-            if command:
-                self.set_menu_action(edit_action, funct, command)
-            else:
-                self.set_menu_action(edit_action, funct)
-            menu_edit.addAction(edit_action)
-        
-        # menu Default
-        # save new default values
-        menu_edit.addSeparator()
-        menu_default = menu_edit.addMenu('Defaults')
-        default_action = QtGui.QAction('Save current settings', self)
-        self.set_menu_action(default_action, self.save_par)
-        menu_default.addAction(default_action)
-        default_action = QtGui.QAction('Reset default settings', self)
-        self.set_menu_action(default_action, self.reset_to_default)
-        menu_default.addAction(default_action)
-    
+
     def add_unit_label(self):
         font = QtGui.QFont()
         font.setPixelSize(self.plo.unit_label_size)
         self.unit_label = pg.TextItem(anchor=(0.0,0.0), color=self.plo.unit_label_color, fill=self.plo.unit_label_fill)
-        self.unit_label.setText(self.unit_names[self.geo.unit])
+        self.unit_label.setText(self.geo.unit_names[self.geo.unit])
         self.unit_label.setFont(font)
         self.ax.addItem(self.unit_label)
-        self.unit_label.setPos(-self.xdim, self.ydim)
+        self.unit_label.setPos(-self.plo.xdim, self.plo.ydim)
 
     def resize_window(self):
         # figure out proper plot dimensions
-        self.xdim = (self.det.hms * self.det.hmn + self.det.pxs * self.det.hgp * self.det.hmn + self.det.cbh)/2
-        self.ydim = (self.det.vms * self.det.vmn + self.det.pxs * self.det.vgp * self.det.vmn + self.det.cbh)/2
+        self.plo.xdim = (self.det.hms * self.det.hmn + self.det.pxs * self.det.hgp * self.det.hmn + self.det.cbh)/2
+        self.plo.ydim = (self.det.vms * self.det.vmn + self.det.pxs * self.det.vgp * self.det.vmn + self.det.cbh)/2
         
         # limit the axis x and y
-        self.ax.setXRange(-self.xdim, self.xdim, padding=0, update=True)
-        self.ax.setYRange(-self.ydim, self.ydim, padding=0, update=True)
+        self.ax.setXRange(-self.plo.xdim, self.plo.xdim, padding=0, update=True)
+        self.ax.setYRange(-self.plo.ydim, self.plo.ydim, padding=0, update=True)
 
         # get proper dimensions
-        width = int(np.ceil(self.plo.plot_size * self.xdim / self.ydim))
+        width = int(np.ceil(self.plo.plot_size * self.plo.xdim / self.plo.ydim))
         height = self.plo.plot_size + self.plo.slider_margin//2 + self.offset_win32
 
         # fix the window size
         if self.plo.plot_size_fixed:
             self.setMaximumHeight(height)
             self.setMinimumHeight(height)
             self.setMaximumWidth(width)
@@ -345,43 +306,24 @@
 
     def set_window_title(self):
         if self.geo.reference == 'None':
             self.setWindowTitle(self.det.name)
         else:
             self.setWindowTitle(f'{self.det.name} - {self.geo.reference}')
 
-    def change_settings(self):
-        # apply changes
-        self.load_par(skip=['geo'])
-        self.init_modifiables()
-        # clear the screen
-        self.ax.clear()
-        # re-initialise
-        self.init_screen()
-        # center the slider frame
-        self.sliderWidget.apply_style()
-        self.sliderWidget.update_sliders()
-        self.sliderWidget.center_frame()
-
     def change_detector(self, det_name, det_size):
-        self.geo.det_type = det_name
-        self.geo.det_size = det_size
-        # get new detector specs
-        self.det = self.get_specs_det()
-        # clear the screen
+        self.det = self.get_specs_det(self.detectors, det_name, det_size)
         self.ax.clear()
-        # re-initialise
         self.init_screen()
-        # center the slider frame
         self.sliderWidget.center_frame()
 
     def change_units(self, unit_index):
         self.geo.unit = unit_index
-        self.unit_label.setText(self.unit_names[unit_index])
-        self.draw_conics()
+        self.unit_label.setText(self.geo.unit_names[unit_index])
+        self.draw_contours()
 
     def change_reference(self, ref_name):
         self.geo.reference = ref_name
         self.get_reference()
         self.draw_reference()
 
     def get_cif_reference(self, fpath):
@@ -395,48 +337,51 @@
         # mean rejects many, add adjustable multiplicator?
         used = reflections[reflections[:,4] > reflections[:,4].max() * self.plo.conic_ref_min_int]
         # sort by intensity -> ascending -> flip
         ordered = used[used[:, 4].argsort()][::-1]
         # pick the strongest
         ordered = ordered[:self.plo.conic_ref_num]
         # assign dspacing
-        self.cont_ref_dsp = ordered[:,3]
+        self.plo.cont_ref_dsp = ordered[:,3]
         # hkl -> integer
         # cast hkl array to list of tuples (for easy display)
-        irel = ordered[:,4]/ordered[:,4].max()
-        self.cont_ref_hkl = list(zip(ordered[:,0], ordered[:,1], ordered[:,2], ordered[:,4], irel))
+        hkl = ordered[:,:3].astype(int)
+        if self.plo.conic_hkl_show_int:
+            self.plo.cont_ref_hkl = list(zip(hkl[:,0], hkl[:,1], hkl[:,2], ordered[:,4].astype(int)))
+        else:
+            self.plo.cont_ref_hkl = list(zip(hkl[:,0], hkl[:,1], hkl[:,2]))
 
         self.geo.reference = os.path.basename(fpath)
-        self.ref_custom[self.geo.reference] = self.cont_ref_dsp
-        self.ref_custom_hkl[self.geo.reference] = self.cont_ref_hkl
+        self.geo.ref_custom[self.geo.reference] = self.plo.cont_ref_dsp
+        self.geo.ref_custom_hkl[self.geo.reference] = self.plo.cont_ref_hkl
 
         ref_action = QtGui.QAction(self.geo.reference, self, checkable=True)
         self.set_menu_action(ref_action, self.change_reference, self.geo.reference)
         self.sub_menu_custom.addAction(ref_action)
         self.group_ref.addAction(ref_action)
         ref_action.setChecked(True)
         
         # update window title
         self.set_window_title()
 
         self.draw_reference()
 
     def get_reference(self):
-        if self.geo.reference in self.ref_library:
+        if self.geo.reference in self.geo.ref_library:
             # get the d spacings for the calibrtant from pyFAI
-            self.cont_ref_dsp = np.array(calibrant.get_calibrant(self.geo.reference).get_dSpacing()[:self.plo.conic_ref_num])
-            self.cont_ref_hkl = None
-        elif self.geo.reference in self.ref_custom:
+            self.plo.cont_ref_dsp = np.array(calibrant.get_calibrant(self.geo.reference).get_dSpacing()[:self.plo.conic_ref_num])
+            self.plo.cont_ref_hkl = None
+        elif self.geo.reference in self.geo.ref_custom:
             # get custom d spacings
-            self.cont_ref_dsp = self.ref_custom[self.geo.reference]
-            self.cont_ref_hkl = self.ref_custom_hkl[self.geo.reference]
+            self.plo.cont_ref_dsp = self.geo.ref_custom[self.geo.reference]
+            self.plo.cont_ref_hkl = self.geo.ref_custom_hkl[self.geo.reference]
         else:
             # set all d-spacings to -1
-            self.cont_ref_dsp = np.zeros(self.plo.conic_ref_num)
-            self.cont_ref_hkl = None
+            self.plo.cont_ref_dsp = np.zeros(self.plo.conic_ref_num)
+            self.plo.cont_ref_hkl = None
         # update window title
         self.set_window_title()
 
     def get_specs_geo(self):
         ######################
         # Setup the geometry #
         ######################
@@ -465,27 +410,25 @@
         plo = container()
         # - geometry contour section - 
         plo.conic_tth_min = 5               # [int]    Minimum 2-theta contour line
         plo.conic_tth_max = 150             # [int]    Maximum 2-theta contour line
         plo.conic_tth_num = 30              # [int]    Number of contour lines
         plo.beamcenter_marker = 'o'         # [marker] Beam center marker
         plo.beamcenter_size = 6             # [int]    Beam center size
-        plo.conic_linewidth = 4.0           # [float]  Contour linewidth
+        plo.conic_linewidth = 3.0           # [float]  Contour linewidth
         plo.conic_label_size = 14           # [int]    Contour label size
         plo.conic_label_fill = '#FFFFFF'    # [str]    Contour label fill color
         plo.conic_colormap = 'viridis'      # [cmap]   Contour colormap
         # - reference contour section - 
         plo.conic_ref_color = '#DCDCDC'     # [color]  Reference contour color
         plo.conic_ref_linewidth = 12.0      # [float]  Reference contour linewidth
         plo.conic_ref_num = 100             # [int]    Number of reference contours
         plo.conic_ref_min_int = 0.01        # [int]    Minimum display intensity (cif)
-        plo.conic_ref_use_irel = True       # [int]    Linewidth relative to intensity
-        plo.conic_ref_irel_lw_min = 2.0     # [int]    Minimum linewidth when using irel
         plo.conic_hkl_label_size = 14       # [int]    Font size of hkl tooltip
-        plo.conic_hkl_show_int = False      # [bool]   Show intensity in hkl tooltip
+        plo.conic_hkl_show_int = False      # [bool]   Include intensity in hkl tooltip
         # - module section - 
         plo.det_module_alpha = 0.20         # [float]  Detector module alpha
         plo.det_module_width = 1            # [float]  Detector module border width
         plo.det_module_color = '#404040'    # [color]  Detector module border color
         plo.det_module_fill = '#404040'     # [color]  Detector module background color
         # - general section - 
         plo.conic_steps = 100               # [int]    Conic resolution
@@ -554,36 +497,36 @@
         # geo: geometry and detector specs
         self.geo = self.get_specs_geo()
         # plo: plot details
         self.plo = self.get_specs_plo()
         # lmt: geometry limits
         self.lmt = self.get_specs_lmt()
 
-    def get_specs_det(self):
-        det_type = self.geo.det_type.upper()
-        det_size = self.geo.det_size.upper()
+    def get_specs_det(self, detectors, det_type, det_size):
+        det_type = det_type.upper()
+        det_size = det_size.upper()
 
-        if det_type not in self.detector_db.keys():
+        if det_type not in detectors.keys():
             print(f'Unknown detector type: {det_type}')
-            print(f'Current databank entries: {", ".join(self.detector_db.keys())}.')
+            print(f'Current databank entries: {", ".join(detectors.keys())}.')
             raise SystemExit
         
-        if det_size not in self.detector_db[det_type]['size'].keys():
+        if det_size not in detectors[det_type]['size'].keys():
             print(f'Unknown detector type/size combination: {det_type}/{det_size}')
-            print(f'Current {det_type} databank sizes: {", ".join(self.detector_db[det_type]["size"].keys())}.')
+            print(f'Current {det_type} databank sizes: {", ".join(detectors[det_type]["size"].keys())}.')
             raise SystemExit
         
         det = container()
-        det.hms = self.detector_db[det_type]['hms']
-        det.vms = self.detector_db[det_type]['vms']
-        det.pxs = self.detector_db[det_type]['pxs']
-        det.hgp = self.detector_db[det_type]['hgp']
-        det.vgp = self.detector_db[det_type]['vgp']
-        det.cbh = self.detector_db[det_type]['cbh']
-        det.hmn, det.vmn = self.detector_db[det_type]['size'][det_size]
+        det.hms = detectors[det_type]['hms']
+        det.vms = detectors[det_type]['vms']
+        det.pxs = detectors[det_type]['pxs']
+        det.hgp = detectors[det_type]['hgp']
+        det.vgp = detectors[det_type]['vgp']
+        det.cbh = detectors[det_type]['cbh']
+        det.hmn, det.vmn = detectors[det_type]['size'][det_size]
         det.name = f'{det_type} {det_size}'
 
         return det
 
     def get_det_library(self, update=True, reset=False):
         ###########################
         # Detector Specifications #
@@ -680,24 +623,25 @@
             'hgp' : 0,      # [pix] Gap between modules (horizontal)
             'vgp' : 0,      # [pix] Gap between modules (vertical)
             'cbh' : 0,      # [mm]  Central beam hole
             'size' : {'7':(1,1),'14':(1,2)},
             }
         
         # make file dump
-        if not os.path.exists(self.path_detdb) or reset:
-            with open(self.path_detdb, 'w') as wf:
+        det_db = os.path.join(self.path, 'detector_db.json')
+        if not os.path.exists(det_db) or reset:
+            with open(det_db, 'w') as wf:
                 json.dump(detectors, wf, indent=4)
         else:
-            with open(self.path_detdb, 'r') as of:
+            with open(det_db, 'r') as of:
                 for key, vals in json.load(of).items():
                     detectors[key] = vals
         
         if update:
-            with open(self.path_detdb, 'w') as wf:
+            with open(det_db, 'w') as wf:
                 json.dump(detectors, wf, indent=4)
         
         return detectors
 
     def build_detector(self):
         # build detector modules
         # beam position is between the modules (even) or at the center module (odd)
@@ -723,15 +667,15 @@
                 # add the module
                 rect_item = QtWidgets.QGraphicsRectItem(origin_x, origin_y,  self.det.hms, self.det.vms)
                 rect_item.setPen(pg.mkPen(color = self.plo.det_module_color, width = self.plo.det_module_width))
                 rect_item.setBrush(pg.mkBrush(color = self.plo.det_module_fill))
                 rect_item.setOpacity(self.plo.det_module_alpha)
                 self.ax.addItem(rect_item)
 
-    def draw_conics(self):
+    def draw_contours(self):
         # calculate the offset of the contours resulting from yoff and rotation
         # shift the grid to draw the cones, to make sure the contours are drawn
         # within the visible area
         _comp_shift = -(self.geo.yoff + np.tan(np.deg2rad(self.geo.rota))*self.geo.dist)
         # update beam center
         self.patches['beamcenter'].setData([self.geo.xoff],[_comp_shift],
                                             symbol = self.plo.beamcenter_marker,
@@ -778,16 +722,16 @@
 
     def draw_reference(self):
         # plot reference contour lines
         # standard contour lines are to be drawn
         for _n in range(self.plo.conic_ref_num):
             self.patches['reference'][_n].setVisible(False)
             # number of d-spacings might be lower than the maximum number of allowed contours
-            if _n < len(self.cont_ref_dsp):
-                _d = self.cont_ref_dsp[_n]
+            if _n < len(self.plo.cont_ref_dsp):
+                _d = self.plo.cont_ref_dsp[_n]
                 # None adds a list of zeros
                 # catch those here
                 if _d <= 0:
                     continue
                 # lambda = 2 * d * sin(theta)
                 # 2-theta = 2 * (lambda / 2*d)
                 # lambda -> (12.398/geo_energy)
@@ -805,34 +749,25 @@
                 
                 # calculate the conic section corresponding to the theta angle
                 # :returns False is conic is outside of visiblee area
                 x, y, _ = self.calc_conic(omega, theta, steps=self.plo.conic_steps)
                 if x is False:
                     continue
 
+                # plot the conic section
+                self.patches['reference'][_n].setData(x, y, pen=pg.mkPen(self.plo.conic_ref_color, width=self.plo.conic_ref_linewidth))
+                self.patches['reference'][_n].setVisible(True)
+                
                 # if hkl are available
                 # put them in the proper container for the contour
                 # so indexing gets it right
-                irel = 1.0
-                if self.cont_ref_hkl:
-                    h, k, l, itot, irel = self.cont_ref_hkl[_n]
-                    if self.plo.conic_hkl_show_int:
-                        self.patches['reference'][_n].name = f'({h: 2.0f} {k: 2.0f} {l: 2.0f}) {round(itot, 0):.0f}'
-                    else:
-                        self.patches['reference'][_n].name = f'({h: 2.0f} {k: 2.0f} {l: 2.0f})'
-                    if not self.plo.conic_ref_use_irel:
-                        irel = 1.0
+                if self.plo.cont_ref_hkl:
+                    self.patches['reference'][_n].name = self.plo.cont_ref_hkl[_n]
                 else:
                     self.patches['reference'][_n].name = None
-                
-                # plot the conic section
-                self.patches['reference'][_n].setData(x, y, pen=pg.mkPen(self.plo.conic_ref_color,
-                                                                         width=max(self.plo.conic_ref_irel_lw_min, 
-                                                                                   self.plo.conic_ref_linewidth * irel)))
-                self.patches['reference'][_n].setVisible(True)
     
     def calc_conic(self, omega, theta, steps=100):
         # skip drawing smaller/larger +-90 deg contours
         # reject overlap of the 'backscattering'
         # -> limitation of the current implementation
         if theta > np.pi/2 + abs(omega):
             return False, False, False
@@ -857,23 +792,23 @@
         # add x/y offsets
         # revert tilt rotation
         y0 = dy_cone - self.geo.yoff + comp_tilt 
         x0 = self.geo.xoff
 
         # add margin to slightly extend
         # conics outside of visible area
-        _xdim = self.xdim * 1.05
-        _ydim = self.ydim * 1.05
+        _xdim = self.plo.xdim * 1.05
+        _ydim = self.plo.ydim * 1.05
         # evaluate the eccentricity and parameterise
         # the resulting conic accordingly
         if abs(ecc) == 0:
             # circle
             h = (y1+y2)/2
             # check if the circle is visible
-            if h - np.sqrt(y0**2 + x0**2) > np.sqrt(self.ydim**2 + self.xdim**2):
+            if h - np.sqrt(y0**2 + x0**2) > np.sqrt(self.plo.ydim**2 + self.plo.xdim**2):
                 return False, False, False
             t = np.linspace(0, 2*np.pi, 2*steps)
             x = x0 + h * np.sin(t)
             y = y0 + (y1-y2)/2 + h * np.cos(t)
         elif 0 < abs(ecc) < 1:
             # ellipse
             yd = (y1-y2)/2
@@ -937,16 +872,15 @@
         else:
             label_pos = min(y) if theta < np.pi/2 else max(y)
         
         # return x, y and the label position
         return x, y, label_pos
 
     def show_tooltip(self, widget, event):
-        if not widget.name or not self.cont_ref_hkl:
-            event.ignore()
+        if not widget.name or not self.plo.cont_ref_hkl:
             return False
         pos = QtCore.QPoint(*map(int, event.screenPos()))# - QtCore.QPoint(10,20)
         QtWidgets.QToolTip.showText(pos, str(widget.name))
         event.ignore()
 
     def update_screen(self, val=None):
         if val is not None:
@@ -960,15 +894,15 @@
                 self.geo.yoff = float(val)
             elif self.sender().objectName() == 'xoff':
                 self.geo.xoff = float(val)
             elif self.sender().objectName() == 'ener':
                 self.geo.ener = float(val)
 
         # re-calculate cones and re-draw contours
-        self.draw_conics()
+        self.draw_contours()
         # draw reference contours
         if self.geo.reference != 'None':
             self.get_reference()
             self.draw_reference()
 
     def dragEnterEvent(self, event):
         # Drag-and-Drop cif-file
@@ -986,198 +920,150 @@
             self.get_cif_reference(fpath)
 
     def init_par(self):
         # fetch the geometry, detector, plot specifications and limits
         self.get_defaults()
         # file name to store current settings
         # if file_dump doesn't exists, make a dump
-        if not os.path.exists(self.path_settings):
+        if not os.path.exists(self.file_dump):
             self.save_par()
         # if it exists load parameters
         else:
             self.load_par()
         # reset to default if requested
         if self.plo.reset_settings:
             self.get_defaults()
             self.save_par()
         # update with default if requested
         #  - e.g. to add missing entries
         if self.plo.update_settings:
             self.save_par()
 
-    def reset_to_default(self):
-        # plo: plot details
-        self.plo = self.get_specs_plo()
-        # lmt: geometry limits
-        self.lmt = self.get_specs_lmt()
-        self.save_par()
-        self.change_settings()
-
     def save_par(self):
         # Writing geo as dict to file
-        with open(self.path_settings, 'w') as wf:
+        with open(self.file_dump, 'w') as wf:
             json.dump({'geo':self.geo.__dict__, 'plo':self.plo.__dict__, 'lmt':self.lmt.__dict__}, wf, indent=4)
 
-    def load_par(self, skip=[]):
+    def load_par(self):
         # Opening JSON file as dict
-        with open(self.path_settings, 'r') as of:
+        with open(self.file_dump, 'r') as of:
             pars = json.load(of)
         conv = {'geo':self.geo, 'plo':self.plo, 'lmt':self.lmt}
         for key, vals in pars.items():
-            if key in skip:
-                continue
             for p, x in vals.items():
                 if p in conv[key].__dict__.keys():
                     setattr(conv[key], p, x)
                 else:
                     print(f'WARNING: "{p}" is not a valid key!')
 
 class container(object):
     pass
 
 class SliderWidget(QtWidgets.QFrame):
-    def __init__(self, parent):
+    def __init__(self, parent, geo, plo, lmt):
         super().__init__(parent)
-        self.layout = QtWidgets.QVBoxLayout(self)
-        self.layout.setContentsMargins(0, 0, 0, 0)
-        self.layout.setSpacing(0)
+        layout = QtWidgets.QVBoxLayout(self)
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(0)
+        self.geo = geo
+        self.plo = plo
+        self.lmt = lmt
         self.leaveEvent = self.toggle_panel
         self.enterEvent = self.toggle_panel
-        self.frame = QtWidgets.QFrame()
-        self.frame.setContentsMargins(0, 0, 0, 0)
-        self.frame.setFixedHeight(self.parent().plo.slider_margin)
-        self.layout.addWidget(self.frame)
+        frame = QtWidgets.QFrame()
+        frame.setContentsMargins(0, 0, 0, 0)
+        frame.setFixedHeight(self.plo.slider_margin)
+        layout.addWidget(frame)
+        frame.setStyleSheet(f'''
+            QFrame {{
+                border: {self.plo.slider_border_width}px solid {self.plo.slider_border_color};
+                border-radius: {self.plo.slider_border_radius}px;
+                background: {self.plo.slider_border_color};
+            }}
+        ''')
         self.box = QtWidgets.QFrame()
         self.box.setContentsMargins(0, 5, 0, 5)
-        self.layout.addWidget(self.box)
-        self.box.setHidden(True)
-        self.box_toggle = False
-        self.box_height_show = int(np.ceil(parent.size().height()/3))
-        self.box_height_hide = int(np.ceil(self.frame.size().height()))
-
-        self.grid = QtWidgets.QGridLayout()
-        self.grid.setContentsMargins(0, 0, 0, 0)
-        self.grid.setRowStretch(1,10)
-        self.box.setLayout(self.grid)
-
-        self.apply_style()
-        self.update_sliders()
-        self.center_frame()
-
-    def apply_style(self):
         self.box.setStyleSheet(f'''
             QFrame {{
-                border: {self.parent().plo.slider_border_width}px solid {self.parent().plo.slider_border_color};
-                border-radius: {self.parent().plo.slider_border_radius}px;
-                background: {self.parent().plo.slider_bg_color};
+                border: {self.plo.slider_border_width}px solid {self.plo.slider_border_color};
+                border-radius: {self.plo.slider_border_radius}px;
+                background: {self.plo.slider_bg_color};
             }}
             QFrame:hover {{
-                background: {self.parent().plo.slider_bg_hover};
-            }}
-        ''')
-        self.frame.setStyleSheet(f'''
-            QFrame {{
-                border: {self.parent().plo.slider_border_width}px solid {self.parent().plo.slider_border_color};
-                border-radius: {self.parent().plo.slider_border_radius}px;
-                background: {self.parent().plo.slider_border_color};
+                background: {self.plo.slider_bg_hover};
             }}
         ''')
+        layout.addWidget(self.box)
+        self.box.setHidden(True)
+        self.box_toggle = False
+        self.box_width_dynamic = 0
+        self.box_height_show = int(np.ceil(parent.size().height()/3))
+        self.box_height_hide = int(np.ceil(frame.size().height()))
 
-    def update_sliders(self):
-        # remove sliders and labels
-        for i in reversed(range(self.grid.count())): 
-            self.grid.itemAt(i).widget().deleteLater()
-        # add new set of sliders with updated values
+        grid = QtWidgets.QGridLayout()
+        grid.setContentsMargins(0, 0, 0, 0)
+        grid.setRowStretch(1,10)
+        self.box.setLayout(grid)
+        
         _idx = 0
-        self.box_width_dynamic = 0
-        if self.parent().plo.enable_slider_ener:
-            self.sl_ener = self.add_slider(self.grid,
-                                           'Energy\n[keV]','ener', _idx,
-                                           self.parent().geo.ener,
-                                           self.parent().lmt.ener_min,
-                                           self.parent().lmt.ener_max,
-                                           self.parent().lmt.ener_stp)
-            self.box_width_dynamic += self.parent().plo.slider_column_width
+        if plo.enable_slider_ener:
+            self.add_slider(grid, 'Energy\n[keV]', 'ener', _idx, self.geo.ener, lmt.ener_min, lmt.ener_max, lmt.ener_stp)
+            self.box_width_dynamic += self.plo.slider_column_width
             _idx += 1
-        if self.parent().plo.enable_slider_dist:
-            self.sl_dist = self.add_slider(self.grid,
-                                           'Distance\n[mm]', 'dist', _idx,
-                                           self.parent().geo.dist,
-                                           self.parent().lmt.dist_min,
-                                           self.parent().lmt.dist_max,
-                                           self.parent().lmt.dist_stp)
-            self.box_width_dynamic += self.parent().plo.slider_column_width
+        if plo.enable_slider_dist:
+            self.add_slider(grid, 'Distance\n[mm]', 'dist', _idx, self.geo.dist, lmt.dist_min, lmt.dist_max, lmt.dist_stp)
+            self.box_width_dynamic += self.plo.slider_column_width
             _idx += 1
-        if self.parent().plo.enable_slider_yoff:
-            self.sl_yoff = self.add_slider(self.grid,
-                                           'Y offset\n[mm]', 'yoff', _idx,
-                                           self.parent().geo.yoff,
-                                           self.parent().lmt.yoff_min,
-                                           self.parent().lmt.yoff_max,
-                                           self.parent().lmt.yoff_stp)
-            self.box_width_dynamic += self.parent().plo.slider_column_width
+        if plo.enable_slider_yoff:
+            self.add_slider(grid, 'Y offset\n[mm]', 'yoff', _idx, self.geo.yoff, lmt.yoff_min, lmt.yoff_max, lmt.yoff_stp)
+            self.box_width_dynamic += self.plo.slider_column_width
             _idx += 1
-        if self.parent().plo.enable_slider_xoff:
-            self.sl_xoff = self.add_slider(self.grid,
-                                           'X offset\n[mm]', 'xoff', _idx,
-                                           self.parent().geo.xoff,
-                                           self.parent().lmt.xoff_min,
-                                           self.parent().lmt.xoff_max,
-                                           self.parent().lmt.xoff_stp)
-            self.box_width_dynamic += self.parent().plo.slider_column_width
+        if plo.enable_slider_xoff:
+            self.add_slider(grid, 'X offset\n[mm]', 'xoff', _idx, self.geo.xoff, lmt.xoff_min, lmt.xoff_max, lmt.xoff_stp)
+            self.box_width_dynamic += self.plo.slider_column_width
             _idx += 1
-        if self.parent().plo.enable_slider_tilt:
-            self.sl_tilt = self.add_slider(self.grid,
-                                           'Tilt\n[˚]', 'tilt', _idx,
-                                           self.parent().geo.tilt,
-                                           self.parent().lmt.tilt_min,
-                                           self.parent().lmt.tilt_max,
-                                           self.parent().lmt.tilt_stp)
-            self.box_width_dynamic += self.parent().plo.slider_column_width
+        if plo.enable_slider_tilt:
+            self.add_slider(grid, 'Tilt\n[˚]', 'tilt', _idx, self.geo.tilt, lmt.tilt_min, lmt.tilt_max, lmt.tilt_stp)
+            self.box_width_dynamic += self.plo.slider_column_width
             _idx += 1
-        if self.parent().plo.enable_slider_rota:
-            self.sl_rota = self.add_slider(self.grid,
-                                           'Rotation\n[˚]', 'rota', _idx,
-                                           self.parent().geo.rota,
-                                           self.parent().lmt.rota_min,
-                                           self.parent().lmt.rota_max,
-                                           self.parent().lmt.rota_stp)
-            self.box_width_dynamic += self.parent().plo.slider_column_width
+        if plo.enable_slider_rota:
+            self.add_slider(grid, 'Rotation\n[˚]', 'rota', _idx, self.geo.rota, lmt.rota_min, lmt.rota_max, lmt.rota_stp)
+            self.box_width_dynamic += self.plo.slider_column_width
             _idx += 1
+        
         self.resize(self.box_width_dynamic, self.box_height_hide)
+        self.center_frame()
 
     def center_frame(self):
         self.move(int((self.parent().size().width()-self.box_width_dynamic)/2), self.parent().offset_win32)
 
     def update_slider(self, label, value):
         label.setText(str(int(value)))
 
     def add_slider(self, layout, label, token, idx, lval, lmin, lmax, lstp):
         font = QtGui.QFont()
-        font.setPixelSize(self.parent().plo.slider_label_size)
+        font.setPixelSize(self.plo.slider_label_size)
 
         label_name = QtWidgets.QLabel(label)
         label_name.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         label_name.setFont(font)
         label_name.setStyleSheet(f'''
             QLabel {{
-                color: {self.parent().plo.slider_label_color};
-                border: 0px solid none;
-                background: transparent;
+                color: {self.plo.slider_label_color};
+                border: 0px solid transparent;
             }}
         ''')
         
         label_value = QtWidgets.QLabel()
         label_value.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         label_value.setFont(font)
         label_value.setStyleSheet(f'''
             QLabel {{
-                color: {self.parent().plo.slider_label_color};
+                color: {self.plo.slider_label_color};
                 border: 0px solid transparent;
-                background: transparent;
             }}
         ''')
 
         slider = QtWidgets.QSlider(QtCore.Qt.Orientation.Vertical, objectName=token)
         slider.setValue(999)
         slider.valueChanged.connect(self.parent().update_screen)
         slider.valueChanged.connect(lambda value: self.update_slider(label_value, value))
@@ -1186,15 +1072,15 @@
         slider.setPageStep(int(lstp))
         slider.setValue(int(lval))
         
         layout.addWidget(label_name, 0, idx, QtCore.Qt.AlignmentFlag.AlignCenter)
         layout.addWidget(slider, 1, idx, QtCore.Qt.AlignmentFlag.AlignHCenter)
         layout.addWidget(label_value, 2, idx, QtCore.Qt.AlignmentFlag.AlignCenter)
 
-        return (slider, label_name, label_value)
+        return slider
 
     def toggle_panel(self, event):
         if type(event) == QtGui.QEnterEvent:
             #self.box.setHidden(not self.box.isHidden())
             self.box.setHidden(False)
             self.resize(self.box_width_dynamic, self.box_height_show)
         elif type(event) == QtCore.QEvent and not self.box_toggle:
```

### Comparing `xrdPlanner-1.0.2/xrdPlanner/resources.py` & `xrdPlanner-2023.6.21/xrdPlanner/resources.py`

 * *Files identical despite different names*

### Comparing `xrdPlanner-1.0.2/xrdPlanner.egg-info/PKG-INFO` & `xrdPlanner-2023.6.21/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,28 @@
-Metadata-Version: 2.1
-Name: xrdPlanner
-Version: 1.0.2
-Summary: A tool to project X-ray diffraction cones on a detector screen at different geometries (tilt, rotation, offset) and X-ray energies.
-Home-page: https://github.com/LennardKrause/xrdPlanner/
-Author: Lennard Krause
-Author-email: lkrause@chem.au.dk
-License: GNU GENERAL PUBLIC LICENSE
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # xrdPlanner
 #### A tool to project X-ray diffraction cones on a detector screen at different geometries (tilt, rotation, offset) and X-ray energies
  - Main application is to visualize the maximum achievable resolution at a given geometry.
  - Is able to project diffraction cones for standard samples or directly from cif files.
- - Can turn out valuable when planning beamtimes at synchrotron facilities (e.g. [DanMAX](https://www.maxiv.lu.se/beamlines-accelerators/beamlines/danmax/)).
- - Helps in deciding on the geometry of an experiment.
+ - Can turn out valuable when planning beamtimes and deciding on the geometry of the experiment.
  - The math used is not meant to bring people to the moon but to provide a quick and simple preview.
- - The module building code is designed for [Dectris](https://www.dectris.com) [PILATUS3](https://www.dectris.com/detectors/x-ray-detectors/pilatus3/) / [EIGER2](https://www.dectris.com/detectors/x-ray-detectors/eiger2/) or [SACLA](https://sacla.xfel.jp/?lang=en) MPCCD Detectors (central hole geometry) but one-module systems like the [Bruker](https://www.bruker.com/en.html) [Photon II](https://www.bruker.com/en/products-and-solutions/diffractometers-and-scattering-systems/single-crystal-x-ray-diffractometers/sc-xrd-components/detectors.html) and [Rayonix](https://www.rayonix.com/) [MX-HS](https://www.rayonix.com/rayonix-mx-hs-series/) are possible as well.
+ - The module building code is designed for [Dectris](https://www.dectris.com) [PILATUS3](https://www.dectris.com/detectors/x-ray-detectors/pilatus3/) / [EIGER2](https://www.dectris.com/detectors/x-ray-detectors/eiger2/) and [SACLA](https://sacla.xfel.jp/?lang=en) MPCCD Detectors (central hole geometry) but one-module systems like the [Bruker](https://www.bruker.com/en.html) [Photon II](https://www.bruker.com/en/products-and-solutions/diffractometers-and-scattering-systems/single-crystal-x-ray-diffractometers/sc-xrd-components/detectors.html) are possible as well.
  - It uses [python3](https://www.python.org), [numpy](https://numpy.org), [pyqt6](https://www.riverbankcomputing.com/software/pyqt/), [pyqtgraph](https://pyqtgraph.readthedocs.io/en/latest/), [pyFAI](https://pyfai.readthedocs.io/en/v2023.1/) and [Dans_Diffraction](https://github.com/DanPorter/Dans_Diffraction).
 
 ## Short how-to:
- - pip install xrdPlanner.
  - Type _xrdPlanner_ in a terminal and hit enter.
  - Choose a detector and a model from the _Detector_ menu.
  - Pick a reference from the _Reference_ menu to plot its contours ([pyFAI](https://pyfai.readthedocs.io/en/v2023.1/)).
  - Drop a .cif file onto the window to draw its contours ([Dans_Diffraction](https://github.com/DanPorter/Dans_Diffraction)), click a contour to get a hkl tooltip.
  - Use the units from the _Units_ menu you are the most comfortable with.
  - Hover over the grey line at the top to show the sliders. Click it to make it stay open.
  - Drag the sliders to change energy and geometry.
-
-## Customisation:
-  - Edit the _settings.json_ file and the _detector_db.json_ files.
-  - Use _Settings_ -> _Edit Settings_ or _Edit Detector db_.
-  - A click on _Apply Changes_ lets you see the difference.
-  - _"geo"_ determines the startup defaults.
-  - _"plo"_ customises the general layout and visuals.
-  - _"lmt"_ sets the limiting values of the geometry/energy sliders.
-  - Add all the missing detectors to the _detector_db.json_.
-  - I hope the variable naming is self-explanatory.
-
-## Known Bugs:
-  - Overwriting defaults while in darkmode requires a reset to go back to light mode.
+ - Edit the _settings.json_ file to suit your needs.
+ - Add all the missing detectors to the _detectors.json_ file.
 
 ## Latest updates:
-  - 2023-06-30 Update: Reference hkl intensity determines linewidth (irel).
-  - 2023-06-30 Bugfix: Reference lines stay after settings reload.
-  - 2023-06-23 Bugfix: Fixed several bugs with regard to the reloading of the settings file.
-  - 2023-06-21 Update: Settings files accessible from menu, changes can be applied on the fly.
   - 2023-06-14 Update: Big speed update.
   - 2023-06-01 Update: countourpy was dropped, the conics are now calculated directly instead of being evaluated on a grid.
   - 2023-05-25 Update: Dans_Diffraction is used in favour of gemmi as it allows the direct calculation of intensities from the cif.
   - 2023-04-26 Update: A hkl tooltip is shown on click on a contour (only for cif contours).
   - 2023-04-25 Bugfix: Segmented contours are now drawn properly.
   - 2023-04-20 Bugfix: Confined slider window mobility to main window area.
   - 2023-04-10 Bugfix: Main window aspect ratio on Windows (menu bar within window).
@@ -68,16 +34,10 @@
 ## Older updates
   - 2023-03-23 Update: Settings are saved to (if doesn't exist) or loaded from (if exists) a 'settings.json' file.
   - 2023-03-23 Update: Added horizontal offset support and slider.
   - 2022-06-07 Update: Added functionality to plot Standard (LaB6, CeO2, ...) contours (needs [pyFAI](https://pyfai.readthedocs.io/en/master/)).
   - 2022-04-28 Update: Changed contour line generation to accept a list of 2-theta values as input.
   - 2022-04-27 Update: Added support for [SACLA](https://sacla.xfel.jp/?lang=en) MPCCD Detectors (central hole geometry).
   - 2022-04-25 Bugfix: Calculation of the beamcenter (rotation and tilt).
-
-## Examples
-#### A PILATUS3 2M detector and a Silicon sample.
-![Preview](https://github.com/LennardKrause/xrdPlanner/blob/main/examples/PILATUS3_2M_Si.png)
-
-#### A rotated EIGER2 4M detector and a Aluminium sample (darkmode).
-![Preview](https://github.com/LennardKrause/xrdPlanner/blob/main/examples/EIGER2_4M_Al.png)
+  - 2022-04-25 Bugfix: Unresponsive radio buttons / redrawing the figure.
 
 #### I hope this turns out to be useful for someone!
```

