# Comparing `tmp/nexus3d-0.0.2.tar.gz` & `tmp/nexus3d-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus3d-0.0.2.tar", last modified: Wed Mar 15 07:25:51 2023, max compression
+gzip compressed data, was "nexus3d-0.0.3.tar", last modified: Fri Jun 30 16:51:21 2023, max compression
```

## Comparing `nexus3d-0.0.2.tar` & `nexus3d-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.453452 nexus3d-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.449452 nexus3d-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.449452 nexus3d-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-15 07:25:36.000000 nexus3d-0.0.2/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-15 07:25:36.000000 nexus3d-0.0.2/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-15 07:25:36.000000 nexus3d-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-15 07:25:36.000000 nexus3d-0.0.2/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-15 07:25:36.000000 nexus3d-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-15 07:25:36.000000 nexus3d-0.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-03-15 07:25:36.000000 nexus3d-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-03-15 07:25:51.453452 nexus3d-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-03-15 07:25:36.000000 nexus3d-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-15 07:25:36.000000 nexus3d-0.0.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.449452 nexus3d-0.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.453452 nexus3d-0.0.2/examples/threejs/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-15 07:25:36.000000 nexus3d-0.0.2/examples/threejs/experiment.glb
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-03-15 07:25:36.000000 nexus3d-0.0.2/examples/threejs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-15 07:25:36.000000 nexus3d-0.0.2/examples/threejs/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.453452 nexus3d-0.0.2/nexus3d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/coordinate_systems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.453452 nexus3d-0.0.2/nexus3d/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/formats/cube_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/formats/gltf_cube_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/formats/gltf_test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/formats/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/formats/stl_cube_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/nexus_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-15 07:25:36.000000 nexus3d-0.0.2/nexus3d/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.453452 nexus3d-0.0.2/nexus3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-03-15 07:25:51.000000 nexus3d-0.0.2/nexus3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-15 07:25:51.000000 nexus3d-0.0.2/nexus3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 07:25:51.000000 nexus3d-0.0.2/nexus3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-15 07:25:51.000000 nexus3d-0.0.2/nexus3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-15 07:25:51.000000 nexus3d-0.0.2/nexus3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 07:25:51.000000 nexus3d-0.0.2/nexus3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-15 07:25:36.000000 nexus3d-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.453452 nexus3d-0.0.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-03-15 07:25:36.000000 nexus3d-0.0.2/scripts/create_example_glb.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-03-15 07:25:36.000000 nexus3d-0.0.2/scripts/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 07:25:51.453452 nexus3d-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.453452 nexus3d-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:25:51.453452 nexus3d-0.0.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    58888 2023-03-15 07:25:36.000000 nexus3d-0.0.2/tests/data/transformation_example.h5
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-15 07:25:36.000000 nexus3d-0.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-15 07:25:36.000000 nexus3d-0.0.2/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-03-15 07:25:36.000000 nexus3d-0.0.2/tests/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.980065 nexus3d-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.968065 nexus3d-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.972066 nexus3d-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 16:51:06.000000 nexus3d-0.0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-30 16:51:06.000000 nexus3d-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-06-30 16:51:21.980065 nexus3d-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-30 16:51:06.000000 nexus3d-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-30 16:51:06.000000 nexus3d-0.0.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.972066 nexus3d-0.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-30 16:51:06.000000 nexus3d-0.0.3/examples/gltf_test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.972066 nexus3d-0.0.3/examples/threejs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-30 16:51:06.000000 nexus3d-0.0.3/examples/threejs/experiment.glb
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-30 16:51:06.000000 nexus3d-0.0.3/examples/threejs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-30 16:51:06.000000 nexus3d-0.0.3/examples/threejs/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.976065 nexus3d-0.0.3/nexus3d/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/coordinate_systems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.976065 nexus3d-0.0.3/nexus3d/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/gltf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/formats/stl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/nexus_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 16:51:06.000000 nexus3d-0.0.3/nexus3d/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.976065 nexus3d-0.0.3/nexus3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17997 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 16:51:21.000000 nexus3d-0.0.3/nexus3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-30 16:51:06.000000 nexus3d-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.976065 nexus3d-0.0.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-30 16:51:06.000000 nexus3d-0.0.3/scripts/create_example_glb.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-06-30 16:51:06.000000 nexus3d-0.0.3/scripts/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:51:21.980065 nexus3d-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.980065 nexus3d-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:21.980065 nexus3d-0.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    58888 2023-06-30 16:51:06.000000 nexus3d-0.0.3/tests/data/transformation_example.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-30 16:51:06.000000 nexus3d-0.0.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-30 16:51:06.000000 nexus3d-0.0.3/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-30 16:51:06.000000 nexus3d-0.0.3/tests/test_transformations.py
```

### Comparing `nexus3d-0.0.2/.github/workflows/pylint.yml` & `nexus3d-0.0.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/.github/workflows/pytest.yml` & `nexus3d-0.0.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/.github/workflows/python-publish.yml` & `nexus3d-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/.github/workflows/static.yml` & `nexus3d-0.0.3/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/.gitignore` & `nexus3d-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/LICENSE` & `nexus3d-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/PKG-INFO` & `nexus3d-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus3d
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convert NXtransformation matrices inside a nexus file to 3D file formats
 Author-email: Florian Dobener <florian.dobener@physik.hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,14 +201,18 @@
         
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
+Project-URL: homepage, https://github.com/domna/nexus3d
+Project-URL: repository, https://github.com/domna/nexus3d
+Project-URL: tracker, https://github.com/domna/nexus3d/issues
+Project-URL: download, https://github.com/domna/nexus3d/releases
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -218,16 +222,16 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nexus3d)
 [![PyPI](https://img.shields.io/pypi/v/nexus3d)](https://pypi.org/project/nexus3d/)
 [![Pytest](https://github.com/domna/nexus3d/actions/workflows/pytest.yml/badge.svg)](https://github.com/domna/nexus3d/actions/workflows/pytest.yml)
 
 # Scope
 
-This is a project for reading out NX_TRANSFORMATION matrices from nexus files and
-visualizing them by creating a 3D representation file (e.g. stl or gltf) which may be imported into 3D visualization software.
+This is a project for reading out NX*TRANSFORMATION matrices from nexus files and
+visualizing them by creating a 3D representation file ([stl](<https://en.wikipedia.org/wiki/STL*(file_format)>) or [gltf/glb](https://en.wikipedia.org/wiki/GlTF) - we recommend using `glb`) which may be imported into 3D visualization software (e.g. blender). It is possible to load CAD drawings from stl files to visualize your experiment with it. For glb files you can easily visualize it in the web with three.js (see the [example](https://github.com/domna/nexus3d/tree/main/examples/threejs))
 
 # Install
 
 The easiest way to install is with pip
 
 ```
 pip install nexus3d
@@ -271,21 +275,23 @@
 Usage: nexus3d [OPTIONS] FILE
 
   Create a glb/gltf or stl from a nexus file via the command line. The actual
   file format is chosen from the file ending of the output file (default:
   experiment.glb).
 
 Options:
-  -o, --output TEXT     The filename to write to (default: experiment.glb).
+  -o, --output TEXT     The filename to write to.  [default: experiment.glb]
   -c, --config TEXT     Config file to load stl drawings into the final output
-  -s, --size FLOAT      The side length of a cube in meters. (default: 0.1 m).
+  -s, --size FLOAT      The side length of a cube in meters.  [default: 0.1]
   -f, --force           Force overwriting of output file.
   --include-process     Include transformations inside /entry/process
   --store-intermediate  Store the intermediate matrices in gltf child nodes.
                         Only applicable for gltf or glb files.
+  --shape [cone|cube]   The shape to write into the gltf file. Only applicable
+                        for gltf or glb files.   [default: cone]
   --help                Show this message and exit.
 ```
 
 The optional config file in json format can be used to load stl files for the different objects, it should be according to the following format:
 
 ```json
 {
@@ -320,8 +326,8 @@
 , applied to the vector `v` in the coordinate frame of the entry.
 To account for different units in the stl files a unit field may be provided.
 The unit needs to be [pint](https://pint.readthedocs.io) convertible to meter.
 If the unit field is not given meter is taken as default unit.
 
 # Display in the web
 
-An example for [three.js](https://threejs.org) based rendering is available in `examples/threejs`. It is based on this [example](https://threejs.org/examples/?q=gltf#webgl_loader_gltf) from three.js. The example can be directly viewed in the github pages of this project: [https://domna.github.io/nexus3d/](https://domna.github.io/nexus3d/). To quickly view your model there exists the excellent [gltf viewer](https://gltf-viewer.donmccurdy.com), which also allows to adjust lighting and materials of your model.
+An example for [three.js](https://threejs.org) based rendering is available in [`examples/threejs`](https://github.com/domna/nexus3d/tree/main/examples/threejs). It is based on this [example](https://threejs.org/examples/?q=gltf#webgl_loader_gltf) from three.js. The example can be directly viewed in the github pages of this project: [https://domna.github.io/nexus3d/](https://domna.github.io/nexus3d/). To quickly view your model there exists the excellent [gltf viewer](https://gltf-viewer.donmccurdy.com), which also allows to adjust lighting and materials of your model.
```

### Comparing `nexus3d-0.0.2/README.md` & `nexus3d-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nexus3d)
 [![PyPI](https://img.shields.io/pypi/v/nexus3d)](https://pypi.org/project/nexus3d/)
 [![Pytest](https://github.com/domna/nexus3d/actions/workflows/pytest.yml/badge.svg)](https://github.com/domna/nexus3d/actions/workflows/pytest.yml)
 
 # Scope
 
-This is a project for reading out NX_TRANSFORMATION matrices from nexus files and
-visualizing them by creating a 3D representation file (e.g. stl or gltf) which may be imported into 3D visualization software.
+This is a project for reading out NX*TRANSFORMATION matrices from nexus files and
+visualizing them by creating a 3D representation file ([stl](<https://en.wikipedia.org/wiki/STL*(file_format)>) or [gltf/glb](https://en.wikipedia.org/wiki/GlTF) - we recommend using `glb`) which may be imported into 3D visualization software (e.g. blender). It is possible to load CAD drawings from stl files to visualize your experiment with it. For glb files you can easily visualize it in the web with three.js (see the [example](https://github.com/domna/nexus3d/tree/main/examples/threejs))
 
 # Install
 
 The easiest way to install is with pip
 
 ```
 pip install nexus3d
@@ -53,21 +53,23 @@
 Usage: nexus3d [OPTIONS] FILE
 
   Create a glb/gltf or stl from a nexus file via the command line. The actual
   file format is chosen from the file ending of the output file (default:
   experiment.glb).
 
 Options:
-  -o, --output TEXT     The filename to write to (default: experiment.glb).
+  -o, --output TEXT     The filename to write to.  [default: experiment.glb]
   -c, --config TEXT     Config file to load stl drawings into the final output
-  -s, --size FLOAT      The side length of a cube in meters. (default: 0.1 m).
+  -s, --size FLOAT      The side length of a cube in meters.  [default: 0.1]
   -f, --force           Force overwriting of output file.
   --include-process     Include transformations inside /entry/process
   --store-intermediate  Store the intermediate matrices in gltf child nodes.
                         Only applicable for gltf or glb files.
+  --shape [cone|cube]   The shape to write into the gltf file. Only applicable
+                        for gltf or glb files.   [default: cone]
   --help                Show this message and exit.
 ```
 
 The optional config file in json format can be used to load stl files for the different objects, it should be according to the following format:
 
 ```json
 {
@@ -102,8 +104,8 @@
 , applied to the vector `v` in the coordinate frame of the entry.
 To account for different units in the stl files a unit field may be provided.
 The unit needs to be [pint](https://pint.readthedocs.io) convertible to meter.
 If the unit field is not given meter is taken as default unit.
 
 # Display in the web
 
-An example for [three.js](https://threejs.org) based rendering is available in `examples/threejs`. It is based on this [example](https://threejs.org/examples/?q=gltf#webgl_loader_gltf) from three.js. The example can be directly viewed in the github pages of this project: [https://domna.github.io/nexus3d/](https://domna.github.io/nexus3d/). To quickly view your model there exists the excellent [gltf viewer](https://gltf-viewer.donmccurdy.com), which also allows to adjust lighting and materials of your model.
+An example for [three.js](https://threejs.org) based rendering is available in [`examples/threejs`](https://github.com/domna/nexus3d/tree/main/examples/threejs). It is based on this [example](https://threejs.org/examples/?q=gltf#webgl_loader_gltf) from three.js. The example can be directly viewed in the github pages of this project: [https://domna.github.io/nexus3d/](https://domna.github.io/nexus3d/). To quickly view your model there exists the excellent [gltf viewer](https://gltf-viewer.donmccurdy.com), which also allows to adjust lighting and materials of your model.
```

### Comparing `nexus3d-0.0.2/dev-requirements.txt` & `nexus3d-0.0.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/examples/threejs/experiment.glb` & `nexus3d-0.0.3/examples/threejs/experiment.glb`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/examples/threejs/index.html` & `nexus3d-0.0.3/examples/threejs/index.html`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/examples/threejs/main.css` & `nexus3d-0.0.3/examples/threejs/main.css`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/nexus3d/coordinate_systems.py` & `nexus3d-0.0.3/nexus3d/coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/nexus3d/formats/gltf_cube_mesh.py` & `nexus3d-0.0.3/nexus3d/formats/gltf_writer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """Functions for creating a gltf cube mesh file"""
 from sys import version_info
+import logging
 from typing import Any, Dict, List, Mapping, Union
 import numpy as np
 from numpy.typing import NDArray
 import pygltflib
 
-from nexus3d.formats.cube_mesh import create_cube_arrays, get_mesh_from_stl
+from nexus3d.formats.mesh import (
+    create_cube_arrays,
+    create_cone_arrays,
+    get_mesh_from_stl,
+)
 from nexus3d.formats.interfaces import WriterInput
 from nexus3d.matrix import rotate, translate
 
 TransformationMatrix = Union[Dict[str, NDArray[np.float64]], NDArray[np.float64]]
 TransformationMatrixDict = Mapping[str, TransformationMatrix]
 
+logger = logging.getLogger(__name__)
+
 
 def get_binary_blobs(indices: NDArray[np.uint8], vertices: NDArray[np.float32]):
     """Converts points and triangles arrays to binary blobs.
 
     Args:
         vertices (NDArray[np.float32]): The vertices array
         indices (NDArray[np.uint8]): The indices array
@@ -239,36 +246,43 @@
                         mode=mode,
                     )
                 ]
             ),
         )
 
     def create_meshs():
+        shapes = {"cube": create_cube_arrays, "cone": create_cone_arrays}
         mesh_indices = {}
-        cube_index = None
+        shape_index = None
         for name in cli_input.transformation_matrices:
             if name in cli_input.config_dict and "file" in cli_input.config_dict[name]:
                 stl_indices, stl_vertices = get_mesh_from_stl(
                     cli_input.config_dict[name]["file"],
                     cli_input.config_dict[name].get("unit"),
                 )
 
                 indices.append(stl_indices)
                 vertices.append(stl_vertices)
                 mesh_indices[name] = len(vertices) - 1
                 append_mesh()
                 continue
 
-            if cube_index is None:
-                cube_indices, cube_vertices = create_cube_arrays(cli_input.size / 2)
-                indices.append(cube_indices)
-                vertices.append(cube_vertices)
-                cube_index = len(vertices) - 1
+            if shape_index is None:
+                if cli_input.shape not in shapes:
+                    logger.warning(
+                        "Shape `%s` not valid. Using cones as default.", cli_input.shape
+                    )
+                shape_indices, shape_vertices = shapes.get(
+                    cli_input.shape, create_cone_arrays
+                )(cli_input.size / 2)
+                indices.append(shape_indices)
+                vertices.append(shape_vertices)
+                shape_index = len(vertices) - 1
                 append_mesh()
-            mesh_indices[name] = cube_index
+            mesh_indices[name] = shape_index
 
         return mesh_indices
 
     if cli_input.config_dict is None:
         cli_input.config_dict = {}
 
     gltf = pygltflib.GLTF2(
```

### Comparing `nexus3d-0.0.2/nexus3d/formats/gltf_test_files.py` & `nexus3d-0.0.3/examples/gltf_test_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Creates test files for rotation and translation for reference."""
 import numpy as np
-from nexus3d.formats.gltf_cube_mesh import write_gltf_file
+from nexus3d.formats.gltf_writer import write_gltf_file
 from nexus3d.formats.interfaces import WriterInput
 from nexus3d.matrix import rotate, translate
 
 
 def create_rot_test_file(angle: float = 20, gltf: bool = False):
     """Creates a rotation test file containing rotation around all three coordinate axes."""
     rot_vecs = {
```

### Comparing `nexus3d-0.0.2/nexus3d/formats/interfaces.py` & `nexus3d-0.0.3/nexus3d/formats/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,7 +14,8 @@
     """Inputs for the writer classes"""
 
     output: str
     transformation_matrices: TransformationMatrixDict
     size: float
     show_beam: bool = False
     config_dict: Optional[Dict[str, Dict[str, str]]] = None
+    shape: str = "cone"
```

### Comparing `nexus3d-0.0.2/nexus3d/formats/stl_cube_mesh.py` & `nexus3d-0.0.3/nexus3d/formats/stl_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Functions for creating a stl cube mesh file"""
 from typing import Dict, Mapping, Union
 import numpy as np
 from numpy.typing import NDArray
 from stl import mesh
 
-from nexus3d.formats.cube_mesh import create_cube_arrays
+from nexus3d.formats.mesh import create_cube_arrays
 from nexus3d.formats.interfaces import WriterInput
 
 TransformationMatrixDict = Mapping[
     str, Union[Dict[str, NDArray[np.float64]], NDArray[np.float64]]
 ]
```

### Comparing `nexus3d-0.0.2/nexus3d/matrix.py` & `nexus3d-0.0.3/nexus3d/matrix.py`

 * *Files 26% similar despite different names*

```diff
@@ -46,14 +46,41 @@
             [0, 0, 0, 1],
         ]
     )
 
     return rot_matrix
 
 
+def rotate_z_onto_vec(
+    vec: NDArray[np.float64], offset: Optional[NDArray[np.float64]] = None
+) -> NDArray[np.float64]:
+    """Generates a 4D rotation matrix to transform the z-axis
+    from the reference frame onto the provided vector.
+
+    Args:
+        vec (NDArray[np.float64]): The vector to rotate onto.
+        offset (Optional[NDArray[np.float64]], optional):
+            An additional offset. Setting this to None ignores the offset. Defaults to None.
+
+    Returns:
+        np.ndarray[(4, 4), float]: The 4D rotation matrix
+    """
+    if offset is None:
+        offset = np.zeros(3)
+
+    return np.array(
+        [
+            [0, 0, vec[0], offset[0]],
+            [0, 0, vec[1], offset[1]],
+            [0, 0, vec[2], offset[2]],
+            [0, 0, 0, 1],
+        ]
+    )
+
+
 def translate(
     translation: NDArray[np.float64], offset: Optional[NDArray[np.float64]] = None
 ) -> NDArray[np.float64]:
     """Generates a 4D translation matrix.
 
     Returns:
         np.ndarray[(4, 4), float]: The translation matrix.
```

### Comparing `nexus3d-0.0.2/nexus3d/nexus_transformations.py` & `nexus3d-0.0.3/nexus3d/nexus_transformations.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import numpy as np
 from numpy.typing import NDArray
 import h5py
 import click
 from nexus3d.formats.interfaces import WriterInput
 
 from nexus3d.matrix import rotate, translate
-from nexus3d.formats.stl_cube_mesh import write_stl_file
-from nexus3d.formats.gltf_cube_mesh import write_gltf_file
+from nexus3d.formats.stl_writer import write_stl_file
+from nexus3d.formats.gltf_writer import write_gltf_file
 from nexus3d.units import ureg
 
 TransformationMatrixDict = Mapping[
     str, Union[Dict[str, NDArray[np.float64]], NDArray[np.float64]]
 ]
 
 
@@ -50,16 +50,19 @@
         offset_si = (offset * offset_unit).to_base_units().magnitude
 
         vector = attrs["vector"]
 
         # Always use the first element and ignore the dimension
         # With gltf we probably could also animate it!
         field = h5file[entry][()].flat[0]
-        if not isinstance(field, (int, float)):
-            raise NotImplementedError("Only float fields are supported yet.")
+        if not isinstance(field, (int, float, np.int64, np.float64)):
+            raise NotImplementedError(
+                "Only float fields are supported yet, "
+                f"but {entry}: {field} is {type(field)}"
+            )
         field_si = ureg(f"{field} {attrs['units']}").to_base_units().magnitude  # type: ignore
 
         if attrs["transformation_type"] == "translation":
             matrix = translate(field_si * vector, offset_si)
         elif attrs["transformation_type"] == "rotation":
             matrix = rotate(field_si, vector, offset_si)
         else:
@@ -116,28 +119,30 @@
 
 @click.command()
 @click.argument("file")
 @click.option(
     "-o",
     "--output",
     default="experiment.glb",
-    help="The filename to write to (default: experiment.glb).",
+    help="The filename to write to.",
+    show_default=True,
 )
 @click.option(
     "-c",
     "--config",
     default="",
     help="Config file to load stl drawings into the final output",
 )
 @click.option(
     "-s",
     "--size",
     default=0.1,
     type=float,
-    help="The side length of a cube in meters. (default: 0.1 m).",
+    help="The side length of a cube in meters.",
+    show_default=True,
 )
 @click.option(
     "-f",
     "--force",
     is_flag=True,
     default=False,
     type=bool,
@@ -156,22 +161,32 @@
     default=False,
     type=bool,
     help=(
         "Store the intermediate matrices in gltf child nodes. "
         "Only applicable for gltf or glb files."
     ),
 )
+@click.option(
+    "--shape",
+    default="cone",
+    type=click.Choice(["cone", "cube"]),
+    help=(
+        "The shape to write into the gltf file. Only applicable for gltf or glb files. "
+    ),
+    show_default=True,
+)
 def cli(  # pylint: disable=too-many-arguments
     file: str,
     config: str,
     output: str,
     force: bool,
     size: float,
     include_process: bool,
     store_intermediate: bool,
+    shape: str,
 ):
     """
     Create a glb/gltf or stl from a nexus file via the command line.
     The actual file format is chosen from the
     file ending of the output file (default: experiment.glb).
     """
 
@@ -229,9 +244,10 @@
             output=output,
             transformation_matrices=transformation_matrices_from(
                 file, include_process, store_intermediate
             ),
             size=size,
             show_beam=True,
             config_dict=config_dict,
+            shape=shape,
         )
     )
```

### Comparing `nexus3d-0.0.2/nexus3d.egg-info/PKG-INFO` & `nexus3d-0.0.3/nexus3d.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus3d
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convert NXtransformation matrices inside a nexus file to 3D file formats
 Author-email: Florian Dobener <florian.dobener@physik.hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,14 +201,18 @@
         
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
+Project-URL: homepage, https://github.com/domna/nexus3d
+Project-URL: repository, https://github.com/domna/nexus3d
+Project-URL: tracker, https://github.com/domna/nexus3d/issues
+Project-URL: download, https://github.com/domna/nexus3d/releases
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -218,16 +222,16 @@
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nexus3d)
 [![PyPI](https://img.shields.io/pypi/v/nexus3d)](https://pypi.org/project/nexus3d/)
 [![Pytest](https://github.com/domna/nexus3d/actions/workflows/pytest.yml/badge.svg)](https://github.com/domna/nexus3d/actions/workflows/pytest.yml)
 
 # Scope
 
-This is a project for reading out NX_TRANSFORMATION matrices from nexus files and
-visualizing them by creating a 3D representation file (e.g. stl or gltf) which may be imported into 3D visualization software.
+This is a project for reading out NX*TRANSFORMATION matrices from nexus files and
+visualizing them by creating a 3D representation file ([stl](<https://en.wikipedia.org/wiki/STL*(file_format)>) or [gltf/glb](https://en.wikipedia.org/wiki/GlTF) - we recommend using `glb`) which may be imported into 3D visualization software (e.g. blender). It is possible to load CAD drawings from stl files to visualize your experiment with it. For glb files you can easily visualize it in the web with three.js (see the [example](https://github.com/domna/nexus3d/tree/main/examples/threejs))
 
 # Install
 
 The easiest way to install is with pip
 
 ```
 pip install nexus3d
@@ -271,21 +275,23 @@
 Usage: nexus3d [OPTIONS] FILE
 
   Create a glb/gltf or stl from a nexus file via the command line. The actual
   file format is chosen from the file ending of the output file (default:
   experiment.glb).
 
 Options:
-  -o, --output TEXT     The filename to write to (default: experiment.glb).
+  -o, --output TEXT     The filename to write to.  [default: experiment.glb]
   -c, --config TEXT     Config file to load stl drawings into the final output
-  -s, --size FLOAT      The side length of a cube in meters. (default: 0.1 m).
+  -s, --size FLOAT      The side length of a cube in meters.  [default: 0.1]
   -f, --force           Force overwriting of output file.
   --include-process     Include transformations inside /entry/process
   --store-intermediate  Store the intermediate matrices in gltf child nodes.
                         Only applicable for gltf or glb files.
+  --shape [cone|cube]   The shape to write into the gltf file. Only applicable
+                        for gltf or glb files.   [default: cone]
   --help                Show this message and exit.
 ```
 
 The optional config file in json format can be used to load stl files for the different objects, it should be according to the following format:
 
 ```json
 {
@@ -320,8 +326,8 @@
 , applied to the vector `v` in the coordinate frame of the entry.
 To account for different units in the stl files a unit field may be provided.
 The unit needs to be [pint](https://pint.readthedocs.io) convertible to meter.
 If the unit field is not given meter is taken as default unit.
 
 # Display in the web
 
-An example for [three.js](https://threejs.org) based rendering is available in `examples/threejs`. It is based on this [example](https://threejs.org/examples/?q=gltf#webgl_loader_gltf) from three.js. The example can be directly viewed in the github pages of this project: [https://domna.github.io/nexus3d/](https://domna.github.io/nexus3d/). To quickly view your model there exists the excellent [gltf viewer](https://gltf-viewer.donmccurdy.com), which also allows to adjust lighting and materials of your model.
+An example for [three.js](https://threejs.org) based rendering is available in [`examples/threejs`](https://github.com/domna/nexus3d/tree/main/examples/threejs). It is based on this [example](https://threejs.org/examples/?q=gltf#webgl_loader_gltf) from three.js. The example can be directly viewed in the github pages of this project: [https://domna.github.io/nexus3d/](https://domna.github.io/nexus3d/). To quickly view your model there exists the excellent [gltf viewer](https://gltf-viewer.donmccurdy.com), which also allows to adjust lighting and materials of your model.
```

### Comparing `nexus3d-0.0.2/nexus3d.egg-info/SOURCES.txt` & `nexus3d-0.0.3/nexus3d.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.md
 dev-requirements.txt
 pyproject.toml
 .github/workflows/pylint.yml
 .github/workflows/pytest.yml
 .github/workflows/python-publish.yml
 .github/workflows/static.yml
+examples/gltf_test_files.py
 examples/threejs/experiment.glb
 examples/threejs/index.html
 examples/threejs/main.css
 nexus3d/__init__.py
 nexus3d/coordinate_systems.py
 nexus3d/matrix.py
 nexus3d/nexus_transformations.py
@@ -19,18 +20,17 @@
 nexus3d.egg-info/PKG-INFO
 nexus3d.egg-info/SOURCES.txt
 nexus3d.egg-info/dependency_links.txt
 nexus3d.egg-info/entry_points.txt
 nexus3d.egg-info/requires.txt
 nexus3d.egg-info/top_level.txt
 nexus3d/formats/__init__.py
-nexus3d/formats/cube_mesh.py
-nexus3d/formats/gltf_cube_mesh.py
-nexus3d/formats/gltf_test_files.py
+nexus3d/formats/gltf_writer.py
 nexus3d/formats/interfaces.py
-nexus3d/formats/stl_cube_mesh.py
+nexus3d/formats/mesh.py
+nexus3d/formats/stl_writer.py
 scripts/create_example_glb.sh
 scripts/lint.sh
 tests/test_cli.py
 tests/test_stl.py
 tests/test_transformations.py
 tests/data/transformation_example.h5
```

### Comparing `nexus3d-0.0.2/pyproject.toml` & `nexus3d-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,20 @@
     "numpy",
     "pint",
     "numpy-stl",
     "click",
     "pygltflib",
 ]
 
+[project.urls]
+homepage = "https://github.com/domna/nexus3d"
+repository = "https://github.com/domna/nexus3d"
+tracker = "https://github.com/domna/nexus3d/issues"
+download = "https://github.com/domna/nexus3d/releases"
+
 [project.optional-dependencies]
 dev = [
     "mypy",
     "pylint",
     "pycodestyle",
     "pytest",
     "pytest-cov",
```

### Comparing `nexus3d-0.0.2/tests/data/transformation_example.h5` & `nexus3d-0.0.3/tests/data/transformation_example.h5`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/tests/test_cli.py` & `nexus3d-0.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nexus3d-0.0.2/tests/test_stl.py` & `nexus3d-0.0.3/tests/test_stl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tests for stl file functions"""
 import numpy as np
 from numpy.testing import assert_array_almost_equal
-from nexus3d.formats.cube_mesh import create_cube_arrays, get_mesh_from_stl
+from nexus3d.formats.mesh import create_cube_arrays, get_mesh_from_stl
 from nexus3d.formats.interfaces import WriterInput
-from nexus3d.formats.stl_cube_mesh import write_stl_file
+from nexus3d.formats.stl_writer import write_stl_file
 
 
 def test_cube_mesh_reconstruction(tmp_path):
     """Test whether a cube mesh is correctly reconstructed from a stl file"""
     test_file = tmp_path / "cube.stl"
     write_stl_file(WriterInput(test_file, {"test": np.identity(4)}, 2.0, False, {}))
```

### Comparing `nexus3d-0.0.2/tests/test_transformations.py` & `nexus3d-0.0.3/tests/test_transformations.py`

 * *Files identical despite different names*

