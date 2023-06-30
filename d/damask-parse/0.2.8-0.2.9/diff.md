# Comparing `tmp/damask-parse-0.2.8.tar.gz` & `tmp/damask-parse-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\damask-parse-0.2.8.tar", last modified: Tue Jan 19 21:10:33 2021, max compression
+gzip compressed data, was "dist\damask-parse-0.2.9.tar", last modified: Mon Jan 25 17:52:40 2021, max compression
```

## Comparing `damask-parse-0.2.8.tar` & `damask-parse-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2021-01-19 21:10:33.000000 damask-parse-0.2.8/
--rw-rw-rw-   0        0        0     2215 2021-01-19 21:10:33.000000 damask-parse-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      978 2020-08-25 11:15:06.000000 damask-parse-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2021-01-19 21:10:33.000000 damask-parse-0.2.8/damask_parse/
--rw-rw-rw-   0        0        0      150 2019-11-03 02:38:33.000000 damask-parse-0.2.8/damask_parse/__init__.py
--rw-rw-rw-   0        0        0       22 2021-01-19 21:09:39.000000 damask-parse-0.2.8/damask_parse/_version.py
-drwxrwxrwx   0        0        0        0 2021-01-19 21:10:33.000000 damask-parse-0.2.8/damask_parse/legacy/
--rw-rw-rw-   0        0        0      125 2021-01-09 17:53:51.000000 damask-parse-0.2.8/damask_parse/legacy/__init__.py
--rw-rw-rw-   0        0        0     7873 2021-01-19 21:09:12.000000 damask-parse-0.2.8/damask_parse/legacy/readers.py
--rw-rw-rw-   0        0        0    13192 2021-01-19 21:09:12.000000 damask-parse-0.2.8/damask_parse/legacy/writers.py
--rw-rw-rw-   0        0        0     3668 2021-01-19 21:09:12.000000 damask-parse-0.2.8/damask_parse/quats.py
--rw-rw-rw-   0        0        0    23347 2021-01-19 21:09:12.000000 damask-parse-0.2.8/damask_parse/readers.py
--rw-rw-rw-   0        0        0     6598 2020-08-17 10:35:03.000000 damask-parse-0.2.8/damask_parse/rotation.py
--rw-rw-rw-   0        0        0    43907 2021-01-19 21:09:12.000000 damask-parse-0.2.8/damask_parse/utils.py
--rw-rw-rw-   0        0        0    14365 2021-01-19 21:09:12.000000 damask-parse-0.2.8/damask_parse/writers.py
-drwxrwxrwx   0        0        0        0 2021-01-19 21:10:33.000000 damask-parse-0.2.8/damask_parse.egg-info/
--rw-rw-rw-   0        0        0     2215 2021-01-19 21:10:33.000000 damask-parse-0.2.8/damask_parse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2021-01-19 21:10:33.000000 damask-parse-0.2.8/damask_parse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-19 21:10:33.000000 damask-parse-0.2.8/damask_parse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2021-01-19 21:10:33.000000 damask-parse-0.2.8/damask_parse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-01-19 21:10:33.000000 damask-parse-0.2.8/damask_parse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-01-19 21:10:33.000000 damask-parse-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1764 2021-01-09 17:53:51.000000 damask-parse-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-01-25 17:52:40.000000 damask-parse-0.2.9/
+-rw-rw-rw-   0        0        0     2236 2021-01-25 17:52:40.000000 damask-parse-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      978 2020-08-25 11:15:06.000000 damask-parse-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2021-01-25 17:52:40.000000 damask-parse-0.2.9/damask_parse/
+-rw-rw-rw-   0        0        0      150 2019-11-03 02:38:33.000000 damask-parse-0.2.9/damask_parse/__init__.py
+-rw-rw-rw-   0        0        0       22 2021-01-25 17:51:06.000000 damask-parse-0.2.9/damask_parse/_version.py
+drwxrwxrwx   0        0        0        0 2021-01-25 17:52:40.000000 damask-parse-0.2.9/damask_parse/legacy/
+-rw-rw-rw-   0        0        0      125 2021-01-09 17:53:51.000000 damask-parse-0.2.9/damask_parse/legacy/__init__.py
+-rw-rw-rw-   0        0        0     7873 2021-01-19 21:09:12.000000 damask-parse-0.2.9/damask_parse/legacy/readers.py
+-rw-rw-rw-   0        0        0    13192 2021-01-19 21:09:12.000000 damask-parse-0.2.9/damask_parse/legacy/writers.py
+-rw-rw-rw-   0        0        0     3668 2021-01-19 21:09:12.000000 damask-parse-0.2.9/damask_parse/quats.py
+-rw-rw-rw-   0        0        0    23347 2021-01-19 21:09:12.000000 damask-parse-0.2.9/damask_parse/readers.py
+-rw-rw-rw-   0        0        0     6598 2020-08-17 10:35:03.000000 damask-parse-0.2.9/damask_parse/rotation.py
+-rw-rw-rw-   0        0        0    44293 2021-01-25 17:50:53.000000 damask-parse-0.2.9/damask_parse/utils.py
+-rw-rw-rw-   0        0        0    14365 2021-01-19 21:09:12.000000 damask-parse-0.2.9/damask_parse/writers.py
+drwxrwxrwx   0        0        0        0 2021-01-25 17:52:40.000000 damask-parse-0.2.9/damask_parse.egg-info/
+-rw-rw-rw-   0        0        0     2236 2021-01-25 17:52:40.000000 damask-parse-0.2.9/damask_parse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2021-01-25 17:52:40.000000 damask-parse-0.2.9/damask_parse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-01-25 17:52:40.000000 damask-parse-0.2.9/damask_parse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2021-01-25 17:52:40.000000 damask-parse-0.2.9/damask_parse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2021-01-25 17:52:40.000000 damask-parse-0.2.9/damask_parse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-01-25 17:52:40.000000 damask-parse-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1785 2021-01-25 17:50:53.000000 damask-parse-0.2.9/setup.py
```

### Comparing `damask-parse-0.2.8/PKG-INFO` & `damask-parse-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: damask-parse
-Version: 0.2.8
+Version: 0.2.9
 Summary: Input file writers and output file parsers for the crystal plasticity code DAMASK.
 Home-page: UNKNOWN
-Author: Adam J. Plowman
+Author: Adam J. Plowman, Michael D. Atkinson
 Author-email: adam.plowman@manchester.ac.uk
 License: UNKNOWN
 Project-URL: Github, https://github.com/LightForm-group/damask-parse
 Description: [![PyPI version](https://badge.fury.io/py/damask-parse.svg)](https://badge.fury.io/py/damask-parse)
         
         # damask-parse
         Input file writers and output file readers for the crystal plasticity code DAMASK.
```

### Comparing `damask-parse-0.2.8/README.md` & `damask-parse-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `damask-parse-0.2.8/damask_parse/legacy/readers.py` & `damask-parse-0.2.9/damask_parse/legacy/readers.py`

 * *Files identical despite different names*

### Comparing `damask-parse-0.2.8/damask_parse/legacy/writers.py` & `damask-parse-0.2.9/damask_parse/legacy/writers.py`

 * *Files identical despite different names*

### Comparing `damask-parse-0.2.8/damask_parse/quats.py` & `damask-parse-0.2.9/damask_parse/quats.py`

 * *Files identical despite different names*

### Comparing `damask-parse-0.2.8/damask_parse/readers.py` & `damask-parse-0.2.9/damask_parse/readers.py`

 * *Files identical despite different names*

### Comparing `damask-parse-0.2.8/damask_parse/rotation.py` & `damask-parse-0.2.9/damask_parse/rotation.py`

 * *Files identical despite different names*

### Comparing `damask-parse-0.2.8/damask_parse/utils.py` & `damask-parse-0.2.9/damask_parse/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,15 +528,15 @@
         # flatten structured datatype for orientations
         if dat_path.split('/')[-1] == 'O':
             data = data.view((data.dtype[data.dtype.names[0]], len(data.dtype)))
 
             # cast to orientation dict
             data = {
                 'type': 'quat',
-                'quaternions': data, # P=-1 convention
+                'quaternions': data,  # P=-1 convention
                 'unit_cell_alignment': {'x': 'a'},
                 'P': -1,
             }
 
         # transform options don't really apply to orientations
         elif transforms:
             for i in transforms:
@@ -554,22 +554,24 @@
     Parameters
     ----------
     orientations : dict
         Dict containing the following keys:
             type : str
                 One of "euler", "quat".
             quaternions : (list or ndarray of shape (R, 4)) of float, optional
-                Array of R row four-vectors of unit quaternions. Specify either
-                `quaternions` or `euler_angles`.
+                Array of R row four-vectors of unit quaternions. A single quaternion in an
+                array of shape (4,) is also allowed. Specify either `quaternions` or
+                `euler_angles`.
             P : int, optional
                 The "P" constant, either +1 or -1, as defined within [1]. If not
                 specified, P = +1 will be used.
             euler_angles : (list or ndarray of shape (R, 3)) of float, optional           
                 Array of R row three-vectors of Euler angles in degrees or radians,
-                as determined by `euler_degrees`. Specify either `quaternions` or
+                as determined by `euler_degrees`. A single Euler angle triplet in an
+                array of shape (3,) is also allowed. Specify either `quaternions` or
                 `euler_angles`. Specified as proper Euler angles in the Bunge
                 convention. (Rotations are about Z, new X, new new Z.)
             euler_degrees : bool, optional
                 If True, `euler_angles` are expected in degrees, rather than
                 radians.
             unit_cell_alignment : dict
                 Alignment of the unit cell.
@@ -626,30 +628,40 @@
                    f'with the key "euler_angles".')
             raise ValueError(msg)
         if euler_is_degs is None:
             msg = (f'If orientations are specified as Euler angles, "euler_degrees" must '
                    f'be specified as True or False to indicate the format of the Euler '
                    f'angles.')
             raise ValueError(msg)
+
         euler_angles = np.array(eulers)
-        if euler_angles.shape[1] != 3:
+
+        if euler_angles.shape == (3,):
+            euler_angles.reshape((1, 3))
+
+        elif euler_angles.ndim != 2 or euler_angles.shape[1] != 3:
             msg = (f'Euler angles specified in "euler_angles" should be a nested list or '
                    f'array of shape (R, 3), but shape passed was: {euler_angles.shape}.')
             raise ValueError(msg)
 
         # Convert Euler angles to quaternions:
         quaternions = euler2quat(euler_angles, degrees=euler_is_degs, P=P)
 
     elif ori_type == 'quat':
         if quats is None:
             msg = (f'Specify orientations as an array of row four-vector unit '
                    f'quaternions with the key "quaternions".')
             raise ValueError(msg)
+
         quaternions = np.array(quats)
-        if quaternions.shape[1] != 4:
+
+        if quaternions.shape == (4,):
+            quaternions.reshape((1, 4))
+
+        elif quaternions.ndim != 2 or quaternions.shape[1] != 4:
             msg = (f'Quaternions specified in "quaternions" should be a nested list or '
                    f'array of shape (R, 4), but shape passed was: {quaternions.shape}.')
             raise ValueError(msg)
 
     norm_factor = np.sqrt(np.sum(quaternions ** 2, axis=1))
     if not np.allclose(norm_factor, 1):
         print('Quaternions are not normalised; they will be normalised.')
@@ -1107,15 +1119,15 @@
                 if 'unit_cell_alignment' not in volume_element['orientations']:
                     msg = 'Orientation `unit_cell_alignment` must be specified.'
                     raise ValueError(msg)
 
                 if volume_element['orientations']['unit_cell_alignment'].get('y') == 'b':
                     # Convert from y//b to x//a:
                     hex_transform_quat = axang2quat(
-                        volume_element['orientations']['P'] * np.array([0, 0, 1]), 
+                        volume_element['orientations']['P'] * np.array([0, 0, 1]),
                         np.pi/6
                     )
                     mat_i_const_j_ori = multiply_quaternions(
                         q1=hex_transform_quat,
                         q2=mat_i_const_j_ori,
                         P=volume_element['orientations']['P'],
                     )
```

### Comparing `damask-parse-0.2.8/damask_parse/writers.py` & `damask-parse-0.2.9/damask_parse/writers.py`

 * *Files identical despite different names*

### Comparing `damask-parse-0.2.8/damask_parse.egg-info/PKG-INFO` & `damask-parse-0.2.9/damask_parse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: damask-parse
-Version: 0.2.8
+Version: 0.2.9
 Summary: Input file writers and output file parsers for the crystal plasticity code DAMASK.
 Home-page: UNKNOWN
-Author: Adam J. Plowman
+Author: Adam J. Plowman, Michael D. Atkinson
 Author-email: adam.plowman@manchester.ac.uk
 License: UNKNOWN
 Project-URL: Github, https://github.com/LightForm-group/damask-parse
 Description: [![PyPI version](https://badge.fury.io/py/damask-parse.svg)](https://badge.fury.io/py/damask-parse)
         
         # damask-parse
         Input file writers and output file readers for the crystal plasticity code DAMASK.
```

### Comparing `damask-parse-0.2.8/setup.py` & `damask-parse-0.2.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 setup(
     name='damask-parse',
     version=get_version(),
     description=('Input file writers and output file parsers for the crystal '
                  'plasticity code DAMASK.'),
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
-    author='Adam J. Plowman',
+    author='Adam J. Plowman, Michael D. Atkinson',
     author_email='adam.plowman@manchester.ac.uk',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'h5py',
         'damask',
```

