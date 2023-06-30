# Comparing `tmp/pyvista-0.39.0.tar.gz` & `tmp/pyvista-0.39.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvista-0.39.0.tar", last modified: Fri May  5 18:20:36 2023, max compression
+gzip compressed data, was "pyvista-0.39.1.tar", last modified: Tue May 16 05:32:08 2023, max compression
```

## Comparing `pyvista-0.39.0.tar` & `pyvista-0.39.1.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.109243 pyvista-0.39.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-05-05 18:03:18.000000 pyvista-0.39.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-05-05 18:03:18.000000 pyvista-0.39.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-05-05 18:03:18.000000 pyvista-0.39.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    12345 2023-05-05 18:20:36.109243 pyvista-0.39.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-05-05 18:03:18.000000 pyvista-0.39.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.073243 pyvista-0.39.0/pyvista/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2231 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    14263 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/_vtk.py
--rw-r--r--   0 runner    (1001) docker     (122)      478 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.077243 pyvista-0.39.0/pyvista/core/
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12405 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/cell.py
--rw-r--r--   0 runner    (1001) docker     (122)     4839 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/celltype.py
--rw-r--r--   0 runner    (1001) docker     (122)    40859 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/composite.py
--rw-r--r--   0 runner    (1001) docker     (122)    21363 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/dataobject.py
--rw-r--r--   0 runner    (1001) docker     (122)   105351 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    44236 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/datasetattributes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.077243 pyvista-0.39.0/pyvista/core/filters/
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6450 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/filters/composite.py
--rw-r--r--   0 runner    (1001) docker     (122)   212811 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/filters/data_set.py
--rw-r--r--   0 runner    (1001) docker     (122)   129520 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/filters/poly_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5243 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/filters/rectilinear_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)     7325 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/filters/structured_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)    29568 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/filters/uniform_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)     6054 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/filters/unstructured_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)    27876 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (122)     9984 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)   102128 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/pointset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/pyvista_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (122)    20014 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/core/texture.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.077243 pyvista-0.39.0/pyvista/demos/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15920 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/demos/demos.py
--rw-r--r--   0 runner    (1001) docker     (122)     7063 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/demos/logo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1163 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.085243 pyvista-0.39.0/pyvista/examples/
--rw-r--r--   0 runner    (1001) docker     (122)   463087 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/2k_earth_daymap.jpg
--rwxr-xr-x   0 runner    (1001) docker     (122)      193 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    74547 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/airplane.ply
--rw-r--r--   0 runner    (1001) docker     (122)    17941 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/ant.ply
--rw-r--r--   0 runner    (1001) docker     (122)    21542 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/cells.py
--rw-r--r--   0 runner    (1001) docker     (122)   522284 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/channels.vti
--rw-r--r--   0 runner    (1001) docker     (122)   150844 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/downloads.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11939 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (122)    37447 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/globe.vtk
--rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/gltf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3091 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/hexbeam.vtk
--rw-r--r--   0 runner    (1001) docker     (122)    20128 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/nut.ply
--rw-r--r--   0 runner    (1001) docker     (122)    27413 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/planets.py
--rw-r--r--   0 runner    (1001) docker     (122)   228473 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/rectilinear.vtk
--rw-r--r--   0 runner    (1001) docker     (122)    16237 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/sphere.ply
--rw-r--r--   0 runner    (1001) docker     (122)    14094 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/uniform.vtk
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/examples/vrml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.085243 pyvista-0.39.0/pyvista/ext/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16136 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/ext/coverage.py
--rw-r--r--   0 runner    (1001) docker     (122)    18239 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/ext/plot_directive.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.085243 pyvista-0.39.0/pyvista/jupyter/
--rw-r--r--   0 runner    (1001) docker     (122)     7467 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5195 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/jupyter/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/jupyter/pv_ipygany.py
--rw-r--r--   0 runner    (1001) docker     (122)    22749 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/jupyter/pv_pythreejs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.093243 pyvista-0.39.0/pyvista/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9649 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)    34303 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/_property.py
--rw-r--r--   0 runner    (1001) docker     (122)    12876 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/actor_properties.py
--rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/axes.py
--rw-r--r--   0 runner    (1001) docker     (122)    14679 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/axes_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/background_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)    26737 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/camera.py
--rw-r--r--   0 runner    (1001) docker     (122)   140624 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/charts.py
--rw-r--r--   0 runner    (1001) docker     (122)    38870 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/colors.py
--rw-r--r--   0 runner    (1001) docker     (122)    28747 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/composite_mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)    16607 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/cube_axes_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)    25828 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/export_vtkjs.py
--rw-r--r--   0 runner    (1001) docker     (122)    13398 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    41354 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/lights.py
--rw-r--r--   0 runner    (1001) docker     (122)    35079 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    35227 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/opts.py
--rw-r--r--   0 runner    (1001) docker     (122)    45361 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/picking.py
--rw-r--r--   0 runner    (1001) docker     (122)   251234 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/prop3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     9141 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/render_passes.py
--rw-r--r--   0 runner    (1001) docker     (122)    37300 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/render_window_interactor.py
--rw-r--r--   0 runner    (1001) docker     (122)   122579 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)    21771 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/scalar_bars.py
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/theme.py
--rw-r--r--   0 runner    (1001) docker     (122)    20176 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/volume.py
--rw-r--r--   0 runner    (1001) docker     (122)    12575 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/volume_property.py
--rw-r--r--   0 runner    (1001) docker     (122)    84085 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/plotting/widgets.py
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    88834 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/themes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.093243 pyvista-0.39.0/pyvista/trame/
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/trame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/trame/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (122)    17938 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/trame/ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     7314 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/trame/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.101243 pyvista-0.39.0/pyvista/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11456 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/cell_type_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)     9246 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/cells.py
--rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)    13004 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     9083 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    19032 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)    51230 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/geometric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    49898 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5980 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)    36436 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/parametric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    74473 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     5933 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/sphinx_gallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     9427 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/transformations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-05-05 18:03:18.000000 pyvista-0.39.0/pyvista/utilities/xvfb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.073243 pyvista-0.39.0/pyvista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    12345 2023-05-05 18:20:36.000000 pyvista-0.39.0/pyvista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4429 2023-05-05 18:20:36.000000 pyvista-0.39.0/pyvista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 18:20:36.000000 pyvista-0.39.0/pyvista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-05-05 18:20:36.000000 pyvista-0.39.0/pyvista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-05 18:20:36.000000 pyvista-0.39.0/pyvista.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 18:20:36.109243 pyvista-0.39.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-05 18:03:18.000000 pyvista-0.39.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 18:20:36.109243 pyvista-0.39.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4030 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (122)     9856 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (122)     8947 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (122)    38449 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_charts.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)    27072 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (122)     3774 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_cube_axes_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_dataobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    58497 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    21038 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_datasetattributes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (122)   100179 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    12950 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_geometric_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    49729 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (122)    12703 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_imaging.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)    10294 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_lights.py
--rw-r--r--   0 runner    (1001) docker     (122)     6228 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_meshio.py
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     6051 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     3544 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_parametric_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    13322 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_picking.py
--rw-r--r--   0 runner    (1001) docker     (122)    12840 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (122)     9386 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_pointset.py
--rw-r--r--   0 runner    (1001) docker     (122)    30731 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_polydata.py
--rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     3171 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_pyvista_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_render_pass.py
--rw-r--r--   0 runner    (1001) docker     (122)     6380 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_render_window_interactor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1927 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_scalar_bars.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_scraper.py
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_texture.py
--rw-r--r--   0 runner    (1001) docker     (122)    17989 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_theme.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_tinypages.py
--rw-r--r--   0 runner    (1001) docker     (122)    29185 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-05-05 18:03:18.000000 pyvista-0.39.0/tests/test_volume_property.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.063045 pyvista-0.39.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-05-16 05:17:45.000000 pyvista-0.39.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-05-16 05:17:45.000000 pyvista-0.39.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-05-16 05:17:45.000000 pyvista-0.39.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12345 2023-05-16 05:32:08.063045 pyvista-0.39.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-05-16 05:17:45.000000 pyvista-0.39.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.039043 pyvista-0.39.1/pyvista/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2231 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14263 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.039043 pyvista-0.39.1/pyvista/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12405 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/cell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4811 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/celltype.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40948 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21371 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)   105351 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44236 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/datasetattributes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.043043 pyvista-0.39.1/pyvista/core/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6450 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/filters/composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)   212805 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/filters/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)   130478 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/filters/poly_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6414 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/filters/rectilinear_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7325 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/filters/structured_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29568 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/filters/uniform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6054 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/filters/unstructured_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27876 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9984 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)   101353 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/pointset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/pyvista_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19952 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/core/texture.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.043043 pyvista-0.39.1/pyvista/demos/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15920 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/demos/demos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7063 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/demos/logo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1163 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.047044 pyvista-0.39.1/pyvista/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)   463087 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/2k_earth_daymap.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      193 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74547 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/airplane.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    17941 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/ant.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    21542 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)   522284 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/channels.vti
+-rw-r--r--   0 runner    (1001) docker     (122)   150539 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/downloads.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11939 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37447 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/globe.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3091 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/hexbeam.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)    20128 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/nut.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    27413 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/planets.py
+-rw-r--r--   0 runner    (1001) docker     (122)   228473 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/rectilinear.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)    16237 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/sphere.ply
+-rw-r--r--   0 runner    (1001) docker     (122)    14094 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/uniform.vtk
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/examples/vrml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.047044 pyvista-0.39.1/pyvista/ext/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16136 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/ext/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18239 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/ext/plot_directive.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.047044 pyvista-0.39.1/pyvista/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (122)     7467 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5195 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/jupyter/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/jupyter/pv_ipygany.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22749 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/jupyter/pv_pythreejs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.055044 pyvista-0.39.1/pyvista/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9649 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34303 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/actor_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/axes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14645 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/axes_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/background_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26774 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/camera.py
+-rw-r--r--   0 runner    (1001) docker     (122)   140624 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/charts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38870 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28687 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/composite_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16607 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/cube_axes_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25828 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/export_vtkjs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13398 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41354 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/lights.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34946 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35181 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/opts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45361 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/picking.py
+-rw-r--r--   0 runner    (1001) docker     (122)   251196 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/prop3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9141 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/render_passes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37300 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/render_window_interactor.py
+-rw-r--r--   0 runner    (1001) docker     (122)   122568 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21771 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/scalar_bars.py
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20176 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/volume.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12575 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/volume_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)    84085 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/plotting/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    88834 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.055044 pyvista-0.39.1/pyvista/trame/
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/trame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/trame/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17938 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/trame/ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7314 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/trame/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.059044 pyvista-0.39.1/pyvista/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11456 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/cell_type_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9246 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13004 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9083 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19032 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51230 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/geometric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49855 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5980 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36436 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/parametric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74473 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5933 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2191 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/sphinx_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9427 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-05-16 05:17:45.000000 pyvista-0.39.1/pyvista/utilities/xvfb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.039043 pyvista-0.39.1/pyvista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12345 2023-05-16 05:32:07.000000 pyvista-0.39.1/pyvista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4429 2023-05-16 05:32:08.000000 pyvista-0.39.1/pyvista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 05:32:07.000000 pyvista-0.39.1/pyvista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-05-16 05:32:07.000000 pyvista-0.39.1/pyvista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-16 05:32:07.000000 pyvista-0.39.1/pyvista.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 05:32:08.063045 pyvista-0.39.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-16 05:17:45.000000 pyvista-0.39.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 05:32:08.063045 pyvista-0.39.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4030 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9856 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8947 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38449 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_charts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27072 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3774 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_cube_axes_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58497 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21038 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_datasetattributes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (122)   100179 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12950 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_geometric_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49729 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12703 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10294 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_lights.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6228 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_meshio.py
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6051 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3544 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_parametric_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13322 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_picking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12840 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9386 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_pointset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31128 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_polydata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3171 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_pyvista_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_render_pass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6380 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_render_window_interactor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1927 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_scalar_bars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4543 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_texture.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17989 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_tinypages.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29185 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-05-16 05:17:45.000000 pyvista-0.39.1/tests/test_volume_property.py
```

### Comparing `pyvista-0.39.0/AUTHORS.rst` & `pyvista-0.39.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/LICENSE` & `pyvista-0.39.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/PKG-INFO` & `pyvista-0.39.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista
-Version: 0.39.0
+Version: 0.39.1
 Summary: Easier Pythonic interface to VTK
 Author-email: PyVista Developers <info@pyvista.org>
 License: MIT
 Project-URL: Documentation, https://docs.pyvista.org/
 Project-URL: Bug Tracker, https://github.com/pyvista/pyvista/issues
 Project-URL: Source Code, https://github.com/pyvista/pyvista
 Keywords: vtk,numpy,plotting,mesh
```

### Comparing `pyvista-0.39.0/README.rst` & `pyvista-0.39.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyproject.toml` & `pyvista-0.39.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/__init__.py` & `pyvista-0.39.1/pyvista/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/_typing.py` & `pyvista-0.39.1/pyvista/_typing.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/_vtk.py` & `pyvista-0.39.1/pyvista/_vtk.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/__init__.py` & `pyvista-0.39.1/pyvista/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/cell.py` & `pyvista-0.39.1/pyvista/core/cell.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/celltype.py` & `pyvista-0.39.1/pyvista/core/celltype.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     ...         [1, 0, 1],
     ...         [1, 1, 1],
     ...         [0, 1, 1],
     ...     ],
     ...     dtype=np.float32,
     ... )
     >>> grid = pyvista.UnstructuredGrid(cells, cell_type, points)
-    >>> grid  # doctest:+SKIP
-    UnstructuredGrid (0x7f5b0a55e1a0)
+    >>> grid
+    UnstructuredGrid (...)
       N Cells:    1
       N Points:   8
       X Bounds:   0.000e+00, 1.000e+00
       Y Bounds:   0.000e+00, 1.000e+00
       Z Bounds:   0.000e+00, 1.000e+00
       N Arrays:   0
```

### Comparing `pyvista-0.39.0/pyvista/core/composite.py` & `pyvista-0.39.1/pyvista/core/composite.py`

 * *Files 0% similar despite different names*

```diff
@@ -925,21 +925,22 @@
         return fmt
 
     def __repr__(self) -> str:
         """Define an adequate representation."""
         # return a string that is Python console friendly
         fmt = f"{type(self).__name__} ({hex(id(self))})\n"
         # now make a call on the object to get its attributes as a list of len 2 tuples
-        row = "  {}:\t{}\n"
+        max_len = max(len(attr[0]) for attr in self._get_attrs()) + 4
+        row = "  {:%ds}{}\n" % max_len
         for attr in self._get_attrs():
             try:
                 fmt += row.format(attr[0], attr[2].format(*attr[1]))
             except:
                 fmt += row.format(attr[0], attr[2].format(attr[1]))
-        return fmt
+        return fmt.strip()
 
     def __str__(self) -> str:
         """Return the str representation of the multi block."""
         return MultiBlock.__repr__(self)
 
     def __len__(self) -> int:
         """Return the number of blocks."""
```

### Comparing `pyvista-0.39.0/pyvista/core/dataobject.py` & `pyvista-0.39.1/pyvista/core/dataobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         for attr in self._get_attrs():
             try:
                 fmt += row.format(attr[0] + ':', attr[2].format(*attr[1]))
             except:
                 fmt += row.format(attr[0] + ':', attr[2].format(attr[1]))
         if hasattr(self, 'n_arrays'):
             fmt += row.format('N Arrays:', self.n_arrays)
-        return fmt
+        return fmt.strip()
 
     def _repr_html_(self):  # pragma: no cover
         """Return a pretty representation for Jupyter notebooks.
 
         This includes header details and information about all arrays.
 
         """
```

### Comparing `pyvista-0.39.0/pyvista/core/dataset.py` & `pyvista-0.39.1/pyvista/core/dataset.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/datasetattributes.py` & `pyvista-0.39.1/pyvista/core/datasetattributes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/errors.py` & `pyvista-0.39.1/pyvista/core/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/filters/__init__.py` & `pyvista-0.39.1/pyvista/core/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/filters/composite.py` & `pyvista-0.39.1/pyvista/core/filters/composite.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/filters/data_set.py` & `pyvista-0.39.1/pyvista/core/filters/data_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1151,22 +1151,22 @@
         --------
         >>> import pyvista
         >>> import numpy as np
         >>> volume = np.zeros([10, 10, 10])
         >>> volume[:3] = 1
         >>> vol = pyvista.wrap(volume)
         >>> threshed = vol.threshold(0.1)
-        >>> threshed  # doctest:+SKIP
-        UnstructuredGrid (0x7f00f9983fa0)
-          N Cells:	243
-          N Points:	400
-          X Bounds:	0.000e+00, 3.000e+00
-          Y Bounds:	0.000e+00, 9.000e+00
-          Z Bounds:	0.000e+00, 9.000e+00
-          N Arrays:	1
+        >>> threshed
+        UnstructuredGrid (...)
+          N Cells:    243
+          N Points:   400
+          X Bounds:   0.000e+00, 3.000e+00
+          Y Bounds:   0.000e+00, 9.000e+00
+          Z Bounds:   0.000e+00, 9.000e+00
+          N Arrays:   1
 
         Apply the threshold filter to Perlin noise.  First generate
         the structured grid.
 
         >>> import pyvista
         >>> noise = pyvista.perlin_noise(0.1, (1, 1, 1), (0, 0, 0))
         >>> grid = pyvista.sample_function(
@@ -1472,22 +1472,23 @@
         Examples
         --------
         Extract the surface of a sample unstructured grid.
 
         >>> import pyvista
         >>> from pyvista import examples
         >>> hex_beam = pyvista.read(examples.hexbeamfile)
-        >>> hex_beam.extract_geometry()  # doctest:+SKIP
-        PolyData (0x7f2f8c132040)
-          N Cells:	88
-          N Points:	90
-          X Bounds:	0.000e+00, 1.000e+00
-          Y Bounds:	0.000e+00, 1.000e+00
-          Z Bounds:	0.000e+00, 5.000e+00
-          N Arrays:	3
+        >>> hex_beam.extract_geometry()
+        PolyData (...)
+          N Cells:    88
+          N Points:   90
+          N Strips:   0
+          X Bounds:   0.000e+00, 1.000e+00
+          Y Bounds:   0.000e+00, 1.000e+00
+          Z Bounds:   0.000e+00, 5.000e+00
+          N Arrays:   3
 
         See :ref:`surface_smoothing_example` for more examples using this filter.
 
         """
         alg = _vtk.vtkGeometryFilter()
         alg.SetInputDataObject(self)
         if extent is not None:
```

### Comparing `pyvista-0.39.0/pyvista/core/filters/poly_data.py` & `pyvista-0.39.1/pyvista/core/filters/poly_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,20 @@
         Examples
         --------
         Plot the mask of points that exceed 45 degrees.
 
         >>> import pyvista
         >>> mesh = pyvista.Cube().triangulate().subdivide(4)
         >>> mask = mesh.edge_mask(45)
+        >>> mesh.plot(scalars=mask)
+
+        Show the array of masked points.
+
         >>> mask  # doctest:+SKIP
         array([ True,  True,  True, ..., False, False, False])
-        >>> mesh.plot(scalars=mask)
 
         """
         poly_data = self
         if not isinstance(poly_data, pyvista.PolyData):  # pragma: no cover
             poly_data = pyvista.PolyData(poly_data)
         poly_data.point_data['point_ind'] = np.arange(poly_data.n_points)
         featureEdges = _vtk.vtkFeatureEdges()
@@ -416,38 +419,54 @@
         >>> sphere_b = pyvista.Sphere(center=(0.5, 0, 0))
         >>> merged = sphere_a.merge(sphere_b)
         >>> merged.plot(style='wireframe', color='tan')
 
         """
         # check if dataset or datasets are not polydata
         if isinstance(dataset, (list, tuple, pyvista.MultiBlock)):
-            is_pd = all(isinstance(data, pyvista.PolyData) for data in dataset)
+            is_polydata = all(isinstance(data, pyvista.PolyData) for data in dataset)
         else:
-            is_pd = isinstance(dataset, pyvista.PolyData)
+            is_polydata = isinstance(dataset, pyvista.PolyData)
 
-        if inplace and not is_pd:
+        if inplace and not is_polydata:
             raise TypeError("In-place merge requires both input datasets to be PolyData.")
 
         merged = DataSetFilters.merge(
             self,
             dataset,
             merge_points=merge_points,
             tolerance=tolerance,
             main_has_priority=main_has_priority,
             inplace=False,
             progress_bar=progress_bar,
         )
 
         # convert back to a polydata if both inputs were polydata
-        if is_pd:
-            pd_merged = pyvista.PolyData(merged.points, faces=merged.cells, n_faces=merged.n_cells)
-            pd_merged.point_data.update(merged.point_data)
-            pd_merged.cell_data.update(merged.cell_data)
-            pd_merged.field_data.update(merged.field_data)
-            merged = pd_merged
+        if is_polydata:
+            # if either of the input datasets contained lines or strips, we
+            # must use extract_geometry to ensure they get converted back
+            # correctly. This incurrs a performance penalty, but is needed to
+            # maintain data consistency.
+            if isinstance(dataset, (list, tuple, pyvista.MultiBlock)):
+                dataset_has_lines_strips = any(
+                    [ds.n_lines or ds.n_strips or ds.n_verts for ds in dataset]
+                )
+            else:
+                dataset_has_lines_strips = dataset.n_lines or dataset.n_strips or dataset.n_verts
+
+            if self.n_lines or self.n_strips or self.n_verts or dataset_has_lines_strips:
+                merged = merged.extract_geometry()
+            else:
+                polydata_merged = pyvista.PolyData(
+                    merged.points, faces=merged.cells, n_faces=merged.n_cells, deep=False
+                )
+                polydata_merged.point_data.update(merged.point_data)
+                polydata_merged.cell_data.update(merged.cell_data)
+                polydata_merged.field_data.update(merged.field_data)
+                merged = polydata_merged
 
         if inplace:
             self.deep_copy(merged)
             return self
 
         return merged
 
@@ -548,25 +567,25 @@
         Returns
         -------
         numpy.ndarray
             Array of curvature values.
 
         Examples
         --------
-        Calculate the mean curvature of the hills example mesh.
+        Calculate the mean curvature of the hills example mesh and plot it.
 
         >>> from pyvista import examples
         >>> hills = examples.load_random_hills()
         >>> curv = hills.curvature()
-        >>> curv  # doctest:+SKIP
-        array([0.20587616, 0.06747695, ..., 0.11781171, 0.15988467])
+        >>> hills.plot(scalars=curv)
 
-        Plot it.
+        Show the curvature array.
 
-        >>> hills.plot(scalars=curv)
+        >>> curv  # doctest:+SKIP
+        array([0.20587616, 0.06747695, ..., 0.11781171, 0.15988467])
 
         """
         curv_type = curv_type.lower()
 
         # Create curve filter and compute curvature
         curvefilter = _vtk.vtkCurvatures()
         curvefilter.SetInputData(self)
```

### Comparing `pyvista-0.39.0/pyvista/core/filters/rectilinear_grid.py` & `pyvista-0.39.1/pyvista/core/filters/rectilinear_grid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """Filters module with the class to manage filters/algorithms for rectilinear grid datasets."""
 
 import collections
 from typing import Sequence, Union
+import warnings
 
 import numpy as np
 
 from pyvista import _vtk, abstract_class
 from pyvista.core.filters import _get_output, _update_alg
+from pyvista.utilities import assert_empty_kwargs
+from pyvista.utilities.misc import PyVistaDeprecationWarning
 
 
 @abstract_class
 class RectilinearGridFilters:
     """An internal class to manage filters/algorithms for rectilinear grid datasets."""
 
+    # Note remove kwargs when removing deprecation for pass_cell_data
     def to_tetrahedra(
         self,
         tetra_per_cell: int = 5,
         mixed: Union[Sequence[int], bool] = False,
         pass_cell_ids: bool = True,
-        pass_cell_data: bool = True,
+        pass_data: bool = True,
         progress_bar: bool = False,
+        **kwargs,
     ):
         """Create a tetrahedral mesh structured grid.
 
         Parameters
         ----------
         tetra_per_cell : int, default: 5
             The number of tetrahedrons to divide each cell into. Can be
@@ -42,23 +47,26 @@
 
         pass_cell_ids : bool, default: True
             Set to ``True`` to make the tetrahedra have scalar data indicating
             which cell they came from in the original
             :class:`pyvista.RectilinearGrid`. The name of this array is
             ``'vtkOriginalCellIds'`` within the ``cell_data``.
 
-        pass_cell_data : bool, default: True
+        pass_data : bool, default: True
             Set to ``True`` to make the tetrahedra mesh have the cell data from
             the original :class:`pyvista.RectilinearGrid`.  This uses
             ``pass_cell_ids=True`` internally. If ``True``, ``pass_cell_ids``
             will also be set to ``True``.
 
         progress_bar : bool, default: False
             Display a progress bar to indicate progress.
 
+        **kwargs : dict, optional
+            Deprecated keyword argument ``pass_cell_data``.
+
         Returns
         -------
         pyvista.UnstructuredGrid
             UnstructuredGrid containing the tetrahedral cells.
 
         Examples
         --------
@@ -83,16 +91,25 @@
         Take the same grid but divide the first cell into 5 cells and the other
         cell into 12 tetrahedrons per cell.
 
         >>> tet_grid = grid.to_tetrahedra(mixed=[5, 12])
         >>> tet_grid.explode(factor=0.5).plot(show_edges=True)
 
         """
+        # Note remove this section when deprecation is done
+        pass_cell_data = kwargs.pop("pass_cell_data", None)
+        assert_empty_kwargs(**kwargs)
+        if pass_cell_data is not None:
+            warnings.warn(
+                "pass_cell_data is a deprecated option, use pass_data", PyVistaDeprecationWarning
+            )
+            pass_data = pass_cell_data
+
         alg = _vtk.vtkRectilinearGridToTetrahedra()
-        alg.SetRememberVoxelId(pass_cell_ids or pass_cell_data)
+        alg.SetRememberVoxelId(pass_cell_ids or pass_data)
         if mixed is not False:
             if isinstance(mixed, str):
                 self.cell_data.active_scalars_name = mixed
             elif isinstance(mixed, (np.ndarray, collections.abc.Sequence)):
                 self.cell_data['_MIXED_CELLS_'] = mixed  # type: ignore
             elif not isinstance(mixed, bool):
                 raise TypeError('`mixed` must be either a sequence of ints or bool')
@@ -112,20 +129,31 @@
                 )
 
             alg.SetTetraPerCell(tetra_per_cell)
 
         alg.SetInputData(self)
         _update_alg(alg, progress_bar, 'Converting to tetrahedra')
         out = _get_output(alg)
-        if pass_cell_data:
+
+        if pass_data:
             # algorithm stores original cell ids in active scalars
+            # this does not preserve active scalars, but we need to
+            # keep active scalars until they are renamed
             for name in self.cell_data:  # type: ignore
                 if name != out.cell_data.active_scalars_name:
                     out[name] = self.cell_data[name][out.cell_data.active_scalars]  # type: ignore
 
+            for name in self.point_data:  # type: ignore
+                out[name] = self.point_data[name]  # type: ignore
+
         if alg.GetRememberVoxelId():
             # original cell_ids are not named and are the active scalars
             out.cell_data.set_array(
                 out.cell_data.pop(out.cell_data.active_scalars_name), 'vtkOriginalCellIds'
             )
 
+        if pass_data:
+            # Now reset active scalars in cast the original mesh had data with active scalars
+            association, name = self.active_scalars_info  # type: ignore
+            out.set_active_scalars(name, preference=association)
+
         return out
```

### Comparing `pyvista-0.39.0/pyvista/core/filters/structured_grid.py` & `pyvista-0.39.1/pyvista/core/filters/structured_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/filters/uniform_grid.py` & `pyvista-0.39.1/pyvista/core/filters/uniform_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/filters/unstructured_grid.py` & `pyvista-0.39.1/pyvista/core/filters/unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/grid.py` & `pyvista-0.39.1/pyvista/core/grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/objects.py` & `pyvista-0.39.1/pyvista/core/objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/pointset.py` & `pyvista-0.39.1/pyvista/core/pointset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2001,23 +2001,23 @@
     Create from NumPy arrays.
 
     >>> xrng = np.arange(-10, 10, 2, dtype=np.float32)
     >>> yrng = np.arange(-10, 10, 5, dtype=np.float32)
     >>> zrng = np.arange(-10, 10, 1, dtype=np.float32)
     >>> x, y, z = np.meshgrid(xrng, yrng, zrng, indexing='ij')
     >>> grid = pyvista.StructuredGrid(x, y, z)
-    >>> grid  # doctest:+SKIP
-    StructuredGrid (0x7fb18f2a8580)
-    N Cells:    513
-    N Points:   800
-    X Bounds:   -1.000e+01, 8.000e+00
-    Y Bounds:   -1.000e+01, 5.000e+00
-    Z Bounds:   -1.000e+01, 9.000e+00
-    Dimensions: 10, 4, 20
-    N Arrays:   0
+    >>> grid
+    StructuredGrid (...)
+      N Cells:      513
+      N Points:     800
+      X Bounds:     -1.000e+01, 8.000e+00
+      Y Bounds:     -1.000e+01, 5.000e+00
+      Z Bounds:     -1.000e+01, 9.000e+00
+      Dimensions:   10, 4, 20
+      N Arrays:     0
 
     """
 
     _WRITERS = {'.vtk': _vtk.vtkStructuredGridWriter, '.vts': _vtk.vtkXMLStructuredGridWriter}
 
     def __init__(self, uinput=None, y=None, z=None, *args, deep=False, **kwargs) -> None:
         """Initialize the structured grid."""
@@ -2352,15 +2352,15 @@
     >>>
     >>> # reorder and reshape to VTK order
     >>> corners = grid_ijk.transpose().reshape(-1, 3)
     >>>
     >>> dims = np.array([ni, nj, nk]) + 1
     >>> grid = pv.ExplicitStructuredGrid(dims, corners)
     >>> grid = grid.compute_connectivity()
-    >>> grid.plot(show_edges=True)  # doctest:+SKIP
+    >>> grid.plot(show_edges=True)
 
     """
 
     _WRITERS = {'.vtu': _vtk.vtkXMLUnstructuredGridWriter, '.vtk': _vtk.vtkUnstructuredGridWriter}
 
     def __init__(self, *args, deep=False, **kwargs):
         """Initialize the explicit structured grid."""
@@ -2460,33 +2460,25 @@
         grid from the visible subgrid, use the ``extract_cells``
         filter and the cell indices where the ghost cell array is
         ``0``.
 
         Examples
         --------
         >>> from pyvista import examples
-        >>> grid = examples.load_explicit_structured()  # doctest:+SKIP
-        >>> grid.plot(
-        ...     color='w', show_edges=True, show_bounds=True
-        ... )  # doctest:+SKIP
+        >>> grid = examples.load_explicit_structured()
+        >>> grid.plot(color='w', show_edges=True, show_bounds=True)
 
-        >>> grid = grid.hide_cells(range(80, 120))  # doctest:+SKIP
-        >>> grid.plot(
-        ...     color='w', show_edges=True, show_bounds=True
-        ... )  # doctest:+SKIP
+        >>> grid = grid.hide_cells(range(80, 120))
+        >>> grid.plot(color='w', show_edges=True, show_bounds=True)
 
-        >>> grid = grid.cast_to_unstructured_grid()  # doctest:+SKIP
-        >>> grid.plot(
-        ...     color='w', show_edges=True, show_bounds=True
-        ... )  # doctest:+SKIP
+        >>> grid = grid.cast_to_unstructured_grid()
+        >>> grid.plot(color='w', show_edges=True, show_bounds=True)
 
-        >>> grid = grid.cast_to_explicit_structured_grid()  # doctest:+SKIP
-        >>> grid.plot(
-        ...     color='w', show_edges=True, show_bounds=True
-        ... )  # doctest:+SKIP
+        >>> grid = grid.cast_to_explicit_structured_grid()
+        >>> grid.plot(color='w', show_edges=True, show_bounds=True)
 
         """
         grid = ExplicitStructuredGrid()
         grid.copy_structure(self)
         alg = _vtk.vtkExplicitStructuredGridToUnstructuredGrid()
         alg.SetInputDataObject(grid)
         alg.Update()
@@ -2637,16 +2629,16 @@
         -------
         tuple[int, int, int]
             Number of sampling points in the I, J and Z directions respectively.
 
         Examples
         --------
         >>> from pyvista import examples
-        >>> grid = examples.load_explicit_structured()  # doctest:+SKIP
-        >>> grid.dimensions  # doctest:+SKIP
+        >>> grid = examples.load_explicit_structured()
+        >>> grid.dimensions
         (5, 6, 7)
 
         """
         return self._dimensions()
 
     @property
     def visible_bounds(self) -> BoundsLike:
@@ -2662,21 +2654,21 @@
         tuple[float, float, float]
             The limits of the visible grid in the X, Y and Z
             directions respectively.
 
         Examples
         --------
         >>> from pyvista import examples
-        >>> grid = examples.load_explicit_structured()  # doctest:+SKIP
-        >>> grid = grid.hide_cells(range(80, 120))  # doctest:+SKIP
-        >>> grid.bounds  # doctest:+SKIP
-        [0.0, 80.0, 0.0, 50.0, 0.0, 6.0]
+        >>> grid = examples.load_explicit_structured()
+        >>> grid = grid.hide_cells(range(80, 120))
+        >>> grid.bounds
+        (0.0, 80.0, 0.0, 50.0, 0.0, 6.0)
 
-        >>> grid.visible_bounds  # doctest:+SKIP
-        [0.0, 80.0, 0.0, 50.0, 0.0, 4.0]
+        >>> grid.visible_bounds
+        (0.0, 80.0, 0.0, 50.0, 0.0, 4.0)
 
         """
         name = _vtk.vtkDataSetAttributes.GhostArrayName()
         if name in self.cell_data:
             array = self.cell_data[name]
             grid = self.extract_cells(array == 0)
             return grid.bounds
@@ -2699,20 +2691,20 @@
         See Also
         --------
         pyvista.ExplicitStructuredGrid.cell_coords : Return the cell structured coordinates.
 
         Examples
         --------
         >>> from pyvista import examples
-        >>> grid = examples.load_explicit_structured()  # doctest:+SKIP
-        >>> grid.cell_id((3, 4, 0))  # doctest:+SKIP
+        >>> grid = examples.load_explicit_structured()
+        >>> grid.cell_id((3, 4, 0))
         19
 
         >>> coords = [(3, 4, 0), (3, 2, 1), (1, 0, 2), (2, 3, 2)]
-        >>> grid.cell_id(coords)  # doctest:+SKIP
+        >>> grid.cell_id(coords)
         array([19, 31, 41, 54])
 
         """
         # `vtk.vtkExplicitStructuredGrid.ComputeCellId` is not used
         # here because this method returns invalid cell IDs when
         # `coords` is outside the grid extent.
         if isinstance(coords, list):
@@ -2746,19 +2738,19 @@
         See Also
         --------
         pyvista.ExplicitStructuredGrid.cell_id : Return the cell ID.
 
         Examples
         --------
         >>> from pyvista import examples
-        >>> grid = examples.load_explicit_structured()  # doctest:+SKIP
-        >>> grid.cell_coords(19)  # doctest:+SKIP
+        >>> grid = examples.load_explicit_structured()
+        >>> grid.cell_coords(19)
         (3, 4, 0)
 
-        >>> grid.cell_coords((19, 31, 41, 54))  # doctest:+SKIP
+        >>> grid.cell_coords((19, 31, 41, 54))
         array([[3, 4, 0],
                [3, 2, 1],
                [1, 0, 2],
                [2, 3, 2]])
 
         """
         dims = self._dimensions()
@@ -2795,28 +2787,23 @@
         list(int)
             Indices of neighboring cells.
 
         Examples
         --------
         >>> import pyvista as pv
         >>> from pyvista import examples
-        >>> grid = examples.load_explicit_structured()  # doctest:+SKIP
-        >>> cell = grid.extract_cells(31)  # doctest:+SKIP
-        >>> ind = grid.neighbors(31)  # doctest:+SKIP
-        >>> neighbors = grid.extract_cells(ind)  # doctest:+SKIP
-        >>>
+        >>> grid = examples.load_explicit_structured()
+        >>> cell = grid.extract_cells(31)
+        >>> ind = grid.neighbors(31)
+        >>> neighbors = grid.extract_cells(ind)
         >>> plotter = pv.Plotter()
-        >>> plotter.add_axes()  # doctest:+SKIP
-        >>> plotter.add_mesh(
-        ...     cell, color='r', show_edges=True
-        ... )  # doctest:+SKIP
-        >>> plotter.add_mesh(
-        ...     neighbors, color='w', show_edges=True
-        ... )  # doctest:+SKIP
-        >>> plotter.show()  # doctest:+SKIP
+        >>> _ = plotter.add_axes()
+        >>> _ = plotter.add_mesh(cell, color='r', show_edges=True)
+        >>> _ = plotter.add_mesh(neighbors, color='w', show_edges=True)
+        >>> plotter.show()
 
         """
 
         def connectivity(ind):
             indices = []
             cell_coords = self.cell_coords(ind)
             cell_points = self.get_cell(ind).points
@@ -2934,17 +2921,17 @@
         --------
         ExplicitStructuredGrid.compute_connections : Compute an array with the number of connected cell faces.
 
         Examples
         --------
         >>> from pyvista import examples
         >>>
-        >>> grid = examples.load_explicit_structured()  # doctest:+SKIP
-        >>> grid = grid.compute_connectivity()  # doctest:+SKIP
-        >>> grid.plot(show_edges=True)  # doctest:+SKIP
+        >>> grid = examples.load_explicit_structured()
+        >>> grid = grid.compute_connectivity()
+        >>> grid.plot(show_edges=True)
 
         """
         if inplace:
             self.ComputeFacesConnectivityFlagsArray()
             return self
         else:
             grid = self.copy()
@@ -2973,17 +2960,17 @@
         See Also
         --------
         ExplicitStructuredGrid.compute_connectivity : Compute the faces connectivity flags array.
 
         Examples
         --------
         >>> from pyvista import examples
-        >>> grid = examples.load_explicit_structured()  # doctest:+SKIP
-        >>> grid = grid.compute_connections()  # doctest:+SKIP
-        >>> grid.plot(show_edges=True)  # doctest:+SKIP
+        >>> grid = examples.load_explicit_structured()
+        >>> grid = grid.compute_connections()
+        >>> grid.plot(show_edges=True)
 
         """
         if inplace:
             if 'ConnectivityFlags' in self.cell_data:
                 array = self.cell_data['ConnectivityFlags']
             else:
                 grid = self.compute_connectivity(inplace=False)
```

### Comparing `pyvista-0.39.0/pyvista/core/pyvista_ndarray.py` & `pyvista-0.39.1/pyvista/core/pyvista_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/core/texture.py` & `pyvista-0.39.1/pyvista/core/texture.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     >>> import os
     >>> import pyvista as pv
     >>> from pyvista import examples
     >>> path = examples.download_masonry_texture(load=False)
     >>> os.path.basename(path)
     'masonry.bmp'
     >>> texture = pv.Texture(path)
-    >>> texture  # doctest:+SKIP
+    >>> texture
     Texture (...)
       Components:   3
       Cube Map:     False
       Dimensions:   256, 256
 
     Create a texture from an RGB array. Note how this is colored per "point"
     rather than per "pixel".
@@ -341,15 +341,15 @@
         numpy.ndarray
             Texture as a numpy array.
 
         Examples
         --------
         >>> from pyvista import examples
         >>> texture = examples.download_puppy_texture()
-        >>> texture  # doctest:+SKIP
+        >>> texture
         Texture (...)
           Components:   3
           Cube Map:     False
           Dimensions:   1600, 1200
         >>> texture.to_array().shape
         (1200, 1600, 3)
         >>> texture.to_array().dtype
@@ -632,16 +632,16 @@
         calculation equation of ``Y = 0.299*R + 0.587*G + 0.114*B``.
 
         Examples
         --------
         >>> from pyvista import examples
         >>> texture = examples.download_masonry_texture()
         >>> bw_texture = texture.to_grayscale()
-        >>> bw_texture  # doctest:+SKIP
-        Texture (0x7f711fc6a740)
+        >>> bw_texture
+        Texture (...)
           Components:   1
           Cube Map:     False
           Dimensions:   256, 256
         >>> bw_texture.plot()
 
         """
         if self.n_components == 1:
```

### Comparing `pyvista-0.39.0/pyvista/demos/demos.py` & `pyvista-0.39.1/pyvista/demos/demos.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/demos/logo.py` & `pyvista-0.39.1/pyvista/demos/logo.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/errors.py` & `pyvista-0.39.1/pyvista/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/2k_earth_daymap.jpg` & `pyvista-0.39.1/pyvista/examples/2k_earth_daymap.jpg`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/airplane.ply` & `pyvista-0.39.1/pyvista/examples/airplane.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/ant.ply` & `pyvista-0.39.1/pyvista/examples/ant.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/cells.py` & `pyvista-0.39.1/pyvista/examples/cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/channels.vti` & `pyvista-0.39.1/pyvista/examples/channels.vti`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/downloads.py` & `pyvista-0.39.1/pyvista/examples/downloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -6782,2647 +6782,2628 @@
 0001a7d0: 2070 7976 6973 7461 2061 7320 7076 0a20   pyvista as pv. 
 0001a7e0: 2020 203e 3e3e 2066 726f 6d20 7079 7669     >>> from pyvi
 0001a7f0: 7374 6120 696d 706f 7274 2065 7861 6d70  sta import examp
 0001a800: 6c65 730a 2020 2020 3e3e 3e20 6461 7461  les.    >>> data
 0001a810: 7365 7420 3d20 6578 616d 706c 6573 2e64  set = examples.d
 0001a820: 6f77 6e6c 6f61 645f 7075 6d70 5f62 7261  ownload_pump_bra
 0001a830: 636b 6574 2829 0a20 2020 203e 3e3e 2064  cket().    >>> d
-0001a840: 6174 6173 6574 2020 2320 646f 6374 6573  ataset  # doctes
-0001a850: 743a 2b53 4b49 500a 2020 2020 556e 7374  t:+SKIP.    Unst
-0001a860: 7275 6374 7572 6564 4772 6964 2028 3078  ructuredGrid (0x
-0001a870: 3766 3436 6139 3237 3931 3230 290a 2020  7f46a9279120).  
-0001a880: 2020 2020 4e20 4365 6c6c 733a 2020 2020      N Cells:    
-0001a890: 3132 3438 3036 0a20 2020 2020 204e 2050  124806.      N P
-0001a8a0: 6f69 6e74 733a 2020 2032 3530 3438 370a  oints:   250487.
-0001a8b0: 2020 2020 2020 5820 426f 756e 6473 3a20        X Bounds: 
-0001a8c0: 2020 2d35 2e30 3030 652d 3031 2c20 352e    -5.000e-01, 5.
-0001a8d0: 3030 3065 2d30 310a 2020 2020 2020 5920  000e-01.      Y 
-0001a8e0: 426f 756e 6473 3a20 2020 2d34 2e30 3030  Bounds:   -4.000
-0001a8f0: 652d 3031 2c20 302e 3030 3065 2b30 300a  e-01, 0.000e+00.
-0001a900: 2020 2020 2020 5a20 426f 756e 6473 3a20        Z Bounds: 
-0001a910: 2020 2d32 2e35 3030 652d 3032 2c20 322e    -2.500e-02, 2.
-0001a920: 3530 3065 2d30 320a 2020 2020 2020 4e20  500e-02.      N 
-0001a930: 4172 7261 7973 3a20 2020 3130 0a0a 2020  Arrays:   10..  
-0001a940: 2020 506c 6f74 2074 6865 2064 6973 706c    Plot the displ
-0001a950: 6163 656d 656e 7420 6f66 2074 6865 2034  acement of the 4
-0001a960: 7468 206d 6f64 6520 7368 6170 6520 6173  th mode shape as
-0001a970: 2073 6361 6c61 7273 2e0a 0a20 2020 203e   scalars...    >
-0001a980: 3e3e 2063 706f 7320 3d20 5b0a 2020 2020  >> cpos = [.    
-0001a990: 2e2e 2e20 2020 2020 2830 2e37 3434 2c20  ...     (0.744, 
-0001a9a0: 2d30 2e35 3032 2c20 2d30 2e38 3330 292c  -0.502, -0.830),
-0001a9b0: 0a20 2020 202e 2e2e 2020 2020 2028 302e  .    ...     (0.
-0001a9c0: 3035 3230 2c20 2d30 2e31 3630 2c20 302e  0520, -0.160, 0.
-0001a9d0: 3037 3433 292c 0a20 2020 202e 2e2e 2020  0743),.    ...  
-0001a9e0: 2020 2028 2d30 2e31 3830 2c20 2d30 2e39     (-0.180, -0.9
-0001a9f0: 3538 2c20 302e 3232 3429 2c0a 2020 2020  58, 0.224),.    
-0001aa00: 2e2e 2e20 5d0a 2020 2020 3e3e 3e20 6461  ... ].    >>> da
-0001aa10: 7461 7365 742e 706c 6f74 280a 2020 2020  taset.plot(.    
-0001aa20: 2e2e 2e20 2020 2020 7363 616c 6172 733d  ...     scalars=
-0001aa30: 2764 6973 705f 3327 2c0a 2020 2020 2e2e  'disp_3',.    ..
-0001aa40: 2e20 2020 2020 6370 6f73 3d63 706f 732c  .     cpos=cpos,
-0001aa50: 0a20 2020 202e 2e2e 2020 2020 2073 686f  .    ...     sho
-0001aa60: 775f 7363 616c 6172 5f62 6172 3d46 616c  w_scalar_bar=Fal
-0001aa70: 7365 2c0a 2020 2020 2e2e 2e20 2020 2020  se,.    ...     
-0001aa80: 616d 6269 656e 743d 302e 322c 0a20 2020  ambient=0.2,.   
-0001aa90: 202e 2e2e 2020 2020 2061 6e74 695f 616c   ...     anti_al
-0001aaa0: 6961 7369 6e67 3d27 6678 6161 272c 0a20  iasing='fxaa',. 
-0001aab0: 2020 202e 2e2e 2029 0a0a 2020 2020 5365     ... )..    Se
-0001aac0: 6520 3a72 6566 3a60 7075 6d70 5f62 7261  e :ref:`pump_bra
-0001aad0: 636b 6574 5f65 7861 6d70 6c65 6020 666f  cket_example` fo
-0001aae0: 7220 6120 6675 6c6c 2065 7861 6d70 6c65  r a full example
-0001aaf0: 2075 7369 6e67 2074 6869 7320 6461 7461   using this data
-0001ab00: 7365 742e 0a0a 2020 2020 2222 220a 2020  set...    """.  
-0001ab10: 2020 6669 6c65 6e61 6d65 203d 205f 646f    filename = _do
-0001ab20: 776e 6c6f 6164 5f61 7263 6869 7665 280a  wnload_archive(.
-0001ab30: 2020 2020 2020 2020 2766 6561 2f70 756d          'fea/pum
-0001ab40: 705f 6272 6163 6b65 742f 7075 6d70 5f62  p_bracket/pump_b
-0001ab50: 7261 636b 6574 2e7a 6970 272c 0a20 2020  racket.zip',.   
-0001ab60: 2020 2020 2027 7075 6d70 5f62 7261 636b       'pump_brack
-0001ab70: 6574 2e76 746b 272c 0a20 2020 2029 0a20  et.vtk',.    ). 
-0001ab80: 2020 2069 6620 6c6f 6164 3a0a 2020 2020     if load:.    
-0001ab90: 2020 2020 7265 7475 726e 2070 7976 6973      return pyvis
-0001aba0: 7461 2e72 6561 6428 6669 6c65 6e61 6d65  ta.read(filename
-0001abb0: 290a 2020 2020 7265 7475 726e 2066 696c  ).    return fil
-0001abc0: 656e 616d 650a 0a0a 6465 6620 646f 776e  ename...def down
-0001abd0: 6c6f 6164 5f65 6c65 6374 726f 6e69 6373  load_electronics
-0001abe0: 5f63 6f6f 6c69 6e67 286c 6f61 643d 5472  _cooling(load=Tr
-0001abf0: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
-0001ac00: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
-0001ac10: 446f 776e 6c6f 6164 2074 6865 2065 6c65  Download the ele
-0001ac20: 6374 726f 6e69 6373 2063 6f6f 6c69 6e67  ctronics cooling
-0001ac30: 2065 7861 6d70 6c65 2064 6174 6173 6574   example dataset
-0001ac40: 732e 0a0a 2020 2020 4461 7461 2067 656e  s...    Data gen
-0001ac50: 6572 6174 6564 2066 726f 6d20 7075 626c  erated from publ
-0001ac60: 6963 2053 696d 5363 616c 6520 6578 616d  ic SimScale exam
-0001ac70: 706c 6573 2061 7420 6053 696d 5363 616c  ples at `SimScal
-0001ac80: 6520 5072 6f6a 6563 7420 4c69 6272 6172  e Project Librar
-0001ac90: 7920 2d0a 2020 2020 5475 7262 6f20 3c68  y -.    Turbo <h
-0001aca0: 7474 7073 3a2f 2f77 7777 2e73 696d 7363  ttps://www.simsc
-0001acb0: 616c 652e 636f 6d2f 7072 6f6a 6563 7473  ale.com/projects
-0001acc0: 2f61 7961 726e 6f7a 2f74 7572 626f 2f3e  /ayarnoz/turbo/>
-0001acd0: 605f 2e0a 0a20 2020 204c 6963 656e 7369  `_...    Licensi
-0001ace0: 6e67 2066 6f72 2074 6869 7320 6461 7461  ng for this data
-0001acf0: 7365 7420 6973 2067 7261 6e74 6564 2074  set is granted t
-0001ad00: 6f20 6672 6565 6c79 2061 6e64 2077 6974  o freely and wit
-0001ad10: 686f 7574 2072 6573 7472 6963 7469 6f6e  hout restriction
-0001ad20: 0a20 2020 2072 6570 726f 6475 6365 2c20  .    reproduce, 
-0001ad30: 6469 7374 7269 6275 7465 2c20 7075 626c  distribute, publ
-0001ad40: 6973 6820 6163 636f 7264 696e 6720 746f  ish according to
-0001ad50: 2074 6865 2060 5369 6d53 6361 6c65 2054   the `SimScale T
-0001ad60: 6572 6d73 2061 6e64 0a20 2020 2043 6f6e  erms and.    Con
-0001ad70: 6469 7469 6f6e 7320 3c68 7474 7073 3a2f  ditions <https:/
-0001ad80: 2f77 7777 2e73 696d 7363 616c 652e 636f  /www.simscale.co
-0001ad90: 6d2f 7465 726d 732d 616e 642d 636f 6e64  m/terms-and-cond
-0001ada0: 6974 696f 6e73 2f3e 605f 2e0a 0a20 2020  itions/>`_...   
-0001adb0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0001adc0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c  ----------.    l
-0001add0: 6f61 6420 3a20 626f 6f6c 2c20 6465 6661  oad : bool, defa
-0001ade0: 756c 743a 2054 7275 650a 2020 2020 2020  ult: True.      
-0001adf0: 2020 4c6f 6164 2074 6865 2064 6174 6173    Load the datas
-0001ae00: 6574 2061 6674 6572 2064 6f77 6e6c 6f61  et after downloa
-0001ae10: 6469 6e67 2069 7420 7768 656e 2060 6054  ding it when ``T
-0001ae20: 7275 6560 602e 2020 5365 7420 7468 6973  rue``.  Set this
-0001ae30: 0a20 2020 2020 2020 2074 6f20 6060 4661  .        to ``Fa
-0001ae40: 6c73 6560 6020 616e 6420 6f6e 6c79 2074  lse`` and only t
-0001ae50: 6865 2066 696c 656e 616d 6520 7769 6c6c  he filename will
-0001ae60: 2062 6520 7265 7475 726e 6564 2e0a 0a20   be returned... 
-0001ae70: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-0001ae80: 2d2d 2d2d 2d2d 0a20 2020 2074 7570 6c65  ------.    tuple
-0001ae90: 5b50 6f6c 7944 6174 612c 2055 6e73 7472  [PolyData, Unstr
-0001aea0: 7563 7475 7265 6447 7269 645d 207c 206c  ucturedGrid] | l
-0001aeb0: 6973 745b 7374 725d 0a20 2020 2020 2020  ist[str].       
-0001aec0: 2044 6174 6153 6574 7320 6f72 2066 696c   DataSets or fil
-0001aed0: 656e 616d 6573 2064 6570 656e 6469 6e67  enames depending
-0001aee0: 206f 6e20 6060 6c6f 6164 6060 2e0a 0a20   on ``load``... 
-0001aef0: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-0001af00: 2d2d 2d2d 2d2d 2d2d 0a20 2020 204c 6f61  --------.    Loa
-0001af10: 6420 7468 6520 6461 7461 7365 7473 0a0a  d the datasets..
-0001af20: 2020 2020 3e3e 3e20 696d 706f 7274 2070      >>> import p
-0001af30: 7976 6973 7461 2061 7320 7076 0a20 2020  yvista as pv.   
-0001af40: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-0001af50: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-0001af60: 730a 2020 2020 3e3e 3e20 7374 7275 6374  s.    >>> struct
-0001af70: 7572 652c 2061 6972 203d 2065 7861 6d70  ure, air = examp
-0001af80: 6c65 732e 646f 776e 6c6f 6164 5f65 6c65  les.download_ele
-0001af90: 6374 726f 6e69 6373 5f63 6f6f 6c69 6e67  ctronics_cooling
-0001afa0: 2829 0a20 2020 203e 3e3e 2073 7472 7563  ().    >>> struc
-0001afb0: 7475 7265 2c20 6169 7220 2023 2064 6f63  ture, air  # doc
-0001afc0: 7465 7374 3a2b 534b 4950 0a20 2020 2028  test:+SKIP.    (
-0001afd0: 506f 6c79 4461 7461 2028 3078 3766 6466  PolyData (0x7fdf
-0001afe0: 6534 6562 3234 6130 290a 2020 2020 2020  e4eb24a0).      
-0001aff0: 204e 2043 656c 6c73 3a20 2020 2033 3434   N Cells:    344
-0001b000: 3237 300a 2020 2020 2020 204e 2050 6f69  270.       N Poi
-0001b010: 6e74 733a 2020 2031 3837 3939 320a 2020  nts:   187992.  
-0001b020: 2020 2020 204e 2053 7472 6970 733a 2020       N Strips:  
-0001b030: 2030 0a20 2020 2020 2020 5820 426f 756e   0.       X Boun
-0001b040: 6473 3a20 2020 2d33 2e30 3030 652d 3033  ds:   -3.000e-03
-0001b050: 2c20 312e 3533 3065 2d30 310a 2020 2020  , 1.530e-01.    
-0001b060: 2020 2059 2042 6f75 6e64 733a 2020 202d     Y Bounds:   -
-0001b070: 332e 3030 3065 2d30 332c 2032 2e30 3330  3.000e-03, 2.030
-0001b080: 652d 3031 0a20 2020 2020 2020 5a20 426f  e-01.       Z Bo
-0001b090: 756e 6473 3a20 2020 2d39 2e30 3030 652d  unds:   -9.000e-
-0001b0a0: 3033 2c20 342e 3230 3065 2d30 320a 2020  03, 4.200e-02.  
-0001b0b0: 2020 2020 204e 2041 7272 6179 733a 2020       N Arrays:  
-0001b0c0: 2035 2c0a 2020 2020 2055 6e73 7472 7563   5,.     Unstruc
-0001b0d0: 7475 7265 6447 7269 6420 2830 7837 6664  turedGrid (0x7fd
-0001b0e0: 6664 6534 3437 3865 3029 0a20 2020 2020  fde4478e0).     
-0001b0f0: 2020 4e20 4365 6c6c 733a 2020 2020 3137    N Cells:    17
-0001b100: 3439 3939 320a 2020 2020 2020 204e 2050  49992.       N P
-0001b110: 6f69 6e74 733a 2020 2036 3130 3137 360a  oints:   610176.
-0001b120: 2020 2020 2020 2058 2042 6f75 6e64 733a         X Bounds:
-0001b130: 2020 202d 312e 3338 3865 2d31 382c 2031     -1.388e-18, 1
-0001b140: 2e35 3030 652d 3031 0a20 2020 2020 2020  .500e-01.       
-0001b150: 5920 426f 756e 6473 3a20 2020 2d33 2e30  Y Bounds:   -3.0
-0001b160: 3030 652d 3033 2c20 322e 3033 3065 2d30  00e-03, 2.030e-0
-0001b170: 310a 2020 2020 2020 205a 2042 6f75 6e64  1.       Z Bound
-0001b180: 733a 2020 202d 362e 3030 3065 2d30 332c  s:   -6.000e-03,
-0001b190: 2034 2e34 3030 652d 3032 0a20 2020 2020   4.400e-02.     
-0001b1a0: 2020 4e20 4172 7261 7973 3a20 2020 3130    N Arrays:   10
-0001b1b0: 290a 0a20 2020 2050 6c6f 7420 7468 6520  )..    Plot the 
-0001b1c0: 6169 7220 7665 6c6f 6369 7479 2074 6872  air velocity thr
-0001b1d0: 6f75 6768 2074 6865 2065 6c65 6374 726f  ough the electro
-0001b1e0: 6e69 6373 2e0a 0a20 2020 203e 3e3e 207a  nics...    >>> z
-0001b1f0: 5f73 6c69 6365 203d 2061 6972 2e63 6c69  _slice = air.cli
-0001b200: 7028 277a 272c 2076 616c 7565 3d2d 302e  p('z', value=-0.
-0001b210: 3030 3529 0a20 2020 203e 3e3e 2070 6c20  005).    >>> pl 
-0001b220: 3d20 7076 2e50 6c6f 7474 6572 2829 0a20  = pv.Plotter(). 
-0001b230: 2020 203e 3e3e 2070 6c2e 656e 6162 6c65     >>> pl.enable
-0001b240: 5f73 7361 6f28 7261 6469 7573 3d30 2e30  _ssao(radius=0.0
-0001b250: 3129 0a20 2020 203e 3e3e 205f 203d 2070  1).    >>> _ = p
-0001b260: 6c2e 6164 645f 6d65 7368 280a 2020 2020  l.add_mesh(.    
-0001b270: 2e2e 2e20 2020 2020 7a5f 736c 6963 652c  ...     z_slice,
-0001b280: 0a20 2020 202e 2e2e 2020 2020 2073 6361  .    ...     sca
-0001b290: 6c61 7273 3d27 5527 2c0a 2020 2020 2e2e  lars='U',.    ..
-0001b2a0: 2e20 2020 2020 6c69 6768 7469 6e67 3d46  .     lighting=F
-0001b2b0: 616c 7365 2c0a 2020 2020 2e2e 2e20 2020  alse,.    ...   
-0001b2c0: 2020 7363 616c 6172 5f62 6172 5f61 7267    scalar_bar_arg
-0001b2d0: 733d 7b27 7469 746c 6527 3a20 2756 656c  s={'title': 'Vel
-0001b2e0: 6f63 6974 7927 7d2c 0a20 2020 202e 2e2e  ocity'},.    ...
-0001b2f0: 2029 0a20 2020 203e 3e3e 205f 203d 2070   ).    >>> _ = p
-0001b300: 6c2e 6164 645f 6d65 7368 280a 2020 2020  l.add_mesh(.    
-0001b310: 2e2e 2e20 2020 2020 7374 7275 6374 7572  ...     structur
-0001b320: 652c 0a20 2020 202e 2e2e 2020 2020 2063  e,.    ...     c
-0001b330: 6f6c 6f72 3d27 7727 2c0a 2020 2020 2e2e  olor='w',.    ..
-0001b340: 2e20 2020 2020 736d 6f6f 7468 5f73 6861  .     smooth_sha
-0001b350: 6469 6e67 3d54 7275 652c 0a20 2020 202e  ding=True,.    .
-0001b360: 2e2e 2020 2020 2073 706c 6974 5f73 6861  ..     split_sha
-0001b370: 7270 5f65 6467 6573 3d54 7275 652c 0a20  rp_edges=True,. 
-0001b380: 2020 202e 2e2e 2029 0a20 2020 203e 3e3e     ... ).    >>>
-0001b390: 2070 6c2e 6361 6d65 7261 5f70 6f73 6974   pl.camera_posit
-0001b3a0: 696f 6e20 3d20 2778 7927 0a20 2020 203e  ion = 'xy'.    >
-0001b3b0: 3e3e 2070 6c2e 6361 6d65 7261 2e72 6f6c  >> pl.camera.rol
-0001b3c0: 6c20 3d20 3930 0a20 2020 203e 3e3e 2070  l = 90.    >>> p
-0001b3d0: 6c2e 656e 6162 6c65 5f61 6e74 695f 616c  l.enable_anti_al
-0001b3e0: 6961 7369 6e67 2827 6678 6161 2729 0a20  iasing('fxaa'). 
-0001b3f0: 2020 203e 3e3e 2070 6c2e 7368 6f77 2829     >>> pl.show()
-0001b400: 0a0a 2020 2020 5365 6520 3a72 6566 3a60  ..    See :ref:`
-0001b410: 6f70 656e 666f 616d 5f63 6f6f 6c69 6e67  openfoam_cooling
-0001b420: 5f65 7861 6d70 6c65 6020 666f 7220 6120  _example` for a 
-0001b430: 6675 6c6c 2065 7861 6d70 6c65 2075 7369  full example usi
-0001b440: 6e67 2074 6869 7320 6461 7461 7365 742e  ng this dataset.
-0001b450: 0a0a 2020 2020 2222 220a 2020 2020 666e  ..    """.    fn
-0001b460: 616d 6573 203d 205f 646f 776e 6c6f 6164  ames = _download
-0001b470: 5f61 7263 6869 7665 2827 6676 6d2f 636f  _archive('fvm/co
-0001b480: 6f6c 696e 675f 656c 6563 7472 6f6e 6963  oling_electronic
-0001b490: 732f 6461 7461 7365 7473 2e7a 6970 2729  s/datasets.zip')
-0001b4a0: 0a20 2020 2069 6620 6c6f 6164 3a0a 2020  .    if load:.  
-0001b4b0: 2020 2020 2020 2320 7265 7475 726e 2074        # return t
-0001b4c0: 6865 2073 7472 7563 7475 7265 2064 6174  he structure dat
-0001b4d0: 6173 6574 2066 6972 7374 0a20 2020 2020  aset first.     
-0001b4e0: 2020 2069 6620 666e 616d 6573 5b31 5d2e     if fnames[1].
-0001b4f0: 656e 6473 7769 7468 2827 7374 7275 6374  endswith('struct
-0001b500: 7572 652e 7674 7027 293a 0a20 2020 2020  ure.vtp'):.     
-0001b510: 2020 2020 2020 2066 6e61 6d65 7320 3d20         fnames = 
-0001b520: 666e 616d 6573 5b3a 3a2d 315d 0a20 2020  fnames[::-1].   
-0001b530: 2020 2020 2072 6574 7572 6e20 7079 7669       return pyvi
-0001b540: 7374 612e 7265 6164 2866 6e61 6d65 735b  sta.read(fnames[
-0001b550: 305d 292c 2070 7976 6973 7461 2e72 6561  0]), pyvista.rea
-0001b560: 6428 666e 616d 6573 5b31 5d29 0a20 2020  d(fnames[1]).   
-0001b570: 2072 6574 7572 6e20 666e 616d 6573 0a0a   return fnames..
-0001b580: 0a64 6566 2064 6f77 6e6c 6f61 645f 6361  .def download_ca
-0001b590: 6e28 7061 7274 6961 6c3d 4661 6c73 652c  n(partial=False,
-0001b5a0: 206c 6f61 643d 5472 7565 293a 2020 2320   load=True):  # 
-0001b5b0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
-0001b5c0: 0a20 2020 2022 2222 446f 776e 6c6f 6164  .    """Download
-0001b5d0: 2074 6865 2063 616e 2064 6174 6173 6574   the can dataset
-0001b5e0: 206d 6573 682e 0a0a 2020 2020 4669 6c65   mesh...    File
-0001b5f0: 206f 6274 6169 6e65 6420 6672 6f6d 2060   obtained from `
-0001b600: 4b69 7477 6172 6520 3c68 7474 7073 3a2f  Kitware <https:/
-0001b610: 2f77 7777 2e6b 6974 7761 7265 2e63 6f6d  /www.kitware.com
-0001b620: 2f3e 605f 2e20 5573 6564 0a20 2020 2066  />`_. Used.    f
-0001b630: 6f72 2074 6573 7469 6e67 2068 6466 2066  or testing hdf f
-0001b640: 696c 6573 2e0a 0a20 2020 2050 6172 616d  iles...    Param
-0001b650: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-0001b660: 2d2d 2d2d 0a20 2020 2070 6172 7469 616c  ----.    partial
-0001b670: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-0001b680: 3a20 4661 6c73 650a 2020 2020 2020 2020  : False.        
-0001b690: 4c6f 6164 2070 6172 7420 6f66 2074 6865  Load part of the
-0001b6a0: 2064 6174 6173 6574 2e0a 0a20 2020 206c   dataset...    l
-0001b6b0: 6f61 6420 3a20 626f 6f6c 2c20 6465 6661  oad : bool, defa
-0001b6c0: 756c 743a 2054 7275 650a 2020 2020 2020  ult: True.      
-0001b6d0: 2020 4c6f 6164 2074 6865 2064 6174 6173    Load the datas
-0001b6e0: 6574 2061 6674 6572 2064 6f77 6e6c 6f61  et after downloa
-0001b6f0: 6469 6e67 2069 7420 7768 656e 2060 6054  ding it when ``T
-0001b700: 7275 6560 602e 2020 5365 7420 7468 6973  rue``.  Set this
-0001b710: 0a20 2020 2020 2020 2074 6f20 6060 4661  .        to ``Fa
-0001b720: 6c73 6560 6020 616e 6420 6f6e 6c79 2074  lse`` and only t
-0001b730: 6865 2066 696c 656e 616d 6520 7769 6c6c  he filename will
-0001b740: 2062 6520 7265 7475 726e 6564 2e0a 0a20   be returned... 
-0001b750: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-0001b760: 2d2d 2d2d 2d2d 0a20 2020 2070 7976 6973  ------.    pyvis
-0001b770: 7461 2e50 6f6c 7944 6174 612c 2073 7472  ta.PolyData, str
-0001b780: 2c20 6f72 204c 6973 745b 7374 725d 0a20  , or List[str]. 
-0001b790: 2020 2020 2020 2054 6865 2065 7861 6d70         The examp
-0001b7a0: 6c65 2050 6172 6156 6965 7720 6361 6e20  le ParaView can 
-0001b7b0: 4461 7461 5365 7420 6f72 2066 696c 6520  DataSet or file 
-0001b7c0: 7061 7468 2873 292e 0a0a 2020 2020 4578  path(s)...    Ex
-0001b7d0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-0001b7e0: 2d2d 2d0a 2020 2020 506c 6f74 2074 6865  ---.    Plot the
-0001b7f0: 2063 616e 2064 6174 6173 6574 2e0a 0a20   can dataset... 
-0001b800: 2020 203e 3e3e 2066 726f 6d20 7079 7669     >>> from pyvi
-0001b810: 7374 6120 696d 706f 7274 2065 7861 6d70  sta import examp
-0001b820: 6c65 730a 2020 2020 3e3e 3e20 696d 706f  les.    >>> impo
-0001b830: 7274 2070 7976 6973 7461 0a20 2020 203e  rt pyvista.    >
-0001b840: 3e3e 2064 6174 6173 6574 203d 2065 7861  >> dataset = exa
-0001b850: 6d70 6c65 732e 646f 776e 6c6f 6164 5f63  mples.download_c
-0001b860: 616e 2829 2020 2320 646f 6374 6573 743a  an()  # doctest:
-0001b870: 2b53 4b49 500a 2020 2020 3e3e 3e20 6461  +SKIP.    >>> da
-0001b880: 7461 7365 742e 706c 6f74 2873 6361 6c61  taset.plot(scala
-0001b890: 7273 3d27 5645 4c27 2c20 736d 6f6f 7468  rs='VEL', smooth
-0001b8a0: 5f73 6861 6469 6e67 3d54 7275 6529 2020  _shading=True)  
-0001b8b0: 2320 646f 6374 6573 743a 2b53 4b49 500a  # doctest:+SKIP.
-0001b8c0: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-0001b8d0: 7079 7669 7374 612e 7674 6b5f 7665 7273  pyvista.vtk_vers
-0001b8e0: 696f 6e5f 696e 666f 203e 2028 392c 2031  ion_info > (9, 1
-0001b8f0: 293a 2020 2320 7072 6167 6d61 3a20 6e6f  ):  # pragma: no
-0001b900: 2063 6f76 6572 0a20 2020 2020 2020 2072   cover.        r
-0001b910: 6169 7365 2056 544b 5665 7273 696f 6e45  aise VTKVersionE
-0001b920: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0001b930: 2020 2754 6869 7320 6578 616d 706c 6520    'This example 
-0001b940: 6669 6c65 2069 7320 6465 7072 6563 6174  file is deprecat
-0001b950: 6564 2066 6f72 2056 544b 2076 392e 322e  ed for VTK v9.2.
-0001b960: 3020 616e 6420 6e65 7765 722e 2027 0a20  0 and newer. '. 
-0001b970: 2020 2020 2020 2020 2020 2027 5573 6520             'Use 
-0001b980: 6064 6f77 6e6c 6f61 645f 6361 6e5f 6372  `download_can_cr
-0001b990: 7573 6865 645f 6864 6660 2069 6e73 7465  ushed_hdf` inste
-0001b9a0: 6164 2e27 0a20 2020 2020 2020 2029 0a0a  ad.'.        )..
-0001b9b0: 2020 2020 6361 6e5f 3020 3d20 5f64 6f77      can_0 = _dow
-0001b9c0: 6e6c 6f61 645f 616e 645f 7265 6164 2827  nload_and_read('
-0001b9d0: 6864 662f 6361 6e5f 302e 6864 6627 2c20  hdf/can_0.hdf', 
-0001b9e0: 6c6f 6164 3d6c 6f61 6429 0a20 2020 2069  load=load).    i
-0001b9f0: 6620 7061 7274 6961 6c3a 0a20 2020 2020  f partial:.     
-0001ba00: 2020 2072 6574 7572 6e20 6361 6e5f 300a     return can_0.
-0001ba10: 0a20 2020 2063 616e 7320 3d20 5b0a 2020  .    cans = [.  
-0001ba20: 2020 2020 2020 6361 6e5f 302c 0a20 2020        can_0,.   
-0001ba30: 2020 2020 205f 646f 776e 6c6f 6164 5f61       _download_a
-0001ba40: 6e64 5f72 6561 6428 2768 6466 2f63 616e  nd_read('hdf/can
-0001ba50: 5f31 2e68 6466 272c 206c 6f61 643d 6c6f  _1.hdf', load=lo
-0001ba60: 6164 292c 0a20 2020 2020 2020 205f 646f  ad),.        _do
-0001ba70: 776e 6c6f 6164 5f61 6e64 5f72 6561 6428  wnload_and_read(
-0001ba80: 2768 6466 2f63 616e 5f32 2e68 6466 272c  'hdf/can_2.hdf',
-0001ba90: 206c 6f61 643d 6c6f 6164 292c 0a20 2020   load=load),.   
-0001baa0: 205d 0a0a 2020 2020 6966 206c 6f61 643a   ]..    if load:
-0001bab0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001bac0: 7079 7669 7374 612e 6d65 7267 6528 6361  pyvista.merge(ca
-0001bad0: 6e73 290a 2020 2020 7265 7475 726e 2063  ns).    return c
-0001bae0: 616e 730a 0a0a 6465 6620 646f 776e 6c6f  ans...def downlo
-0001baf0: 6164 5f63 616e 5f63 7275 7368 6564 5f68  ad_can_crushed_h
-0001bb00: 6466 286c 6f61 643d 5472 7565 293a 2020  df(load=True):  
-0001bb10: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-0001bb20: 6572 0a20 2020 2022 2222 446f 776e 6c6f  er.    """Downlo
-0001bb30: 6164 2074 6865 2063 7275 7368 6564 2063  ad the crushed c
-0001bb40: 616e 2064 6174 6173 6574 2e0a 0a20 2020  an dataset...   
-0001bb50: 2046 696c 6520 6f62 7461 696e 6564 2066   File obtained f
-0001bb60: 726f 6d20 604b 6974 7761 7265 203c 6874  rom `Kitware <ht
-0001bb70: 7470 733a 2f2f 7777 772e 6b69 7477 6172  tps://www.kitwar
-0001bb80: 652e 636f 6d2f 3e60 5f2e 2055 7365 640a  e.com/>`_. Used.
-0001bb90: 2020 2020 666f 7220 7465 7374 696e 6720      for testing 
-0001bba0: 6864 6620 6669 6c65 732e 0a0a 2020 2020  hdf files...    
-0001bbb0: 4f72 6967 696e 616c 6c79 2062 7569 6c74  Originally built
-0001bbc0: 2075 7369 6e67 2056 544b 2076 392e 322e   using VTK v9.2.
-0001bbd0: 3072 6320 6672 6f6d 3a0a 0a20 2020 2060  0rc from:..    `
-0001bbe0: 6056 544b 2f62 7569 6c64 2f45 7874 6572  `VTK/build/Exter
-0001bbf0: 6e61 6c54 6573 7469 6e67 2f63 616e 2d76  nalTesting/can-v
-0001bc00: 7475 2e68 6466 6060 0a0a 2020 2020 5061  tu.hdf``..    Pa
-0001bc10: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0001bc20: 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f 6164  -------.    load
-0001bc30: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-0001bc40: 3a20 5472 7565 0a20 2020 2020 2020 204c  : True.        L
-0001bc50: 6f61 6420 7468 6520 6461 7461 7365 7420  oad the dataset 
-0001bc60: 6166 7465 7220 646f 776e 6c6f 6164 696e  after downloadin
-0001bc70: 6720 6974 2077 6865 6e20 6060 5472 7565  g it when ``True
-0001bc80: 6060 2e20 2053 6574 2074 6869 730a 2020  ``.  Set this.  
-0001bc90: 2020 2020 2020 746f 2060 6046 616c 7365        to ``False
-0001bca0: 6060 2061 6e64 206f 6e6c 7920 7468 6520  `` and only the 
-0001bcb0: 6669 6c65 6e61 6d65 2077 696c 6c20 6265  filename will be
-0001bcc0: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
-0001bcd0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0001bce0: 2d2d 2d0a 2020 2020 7079 7669 7374 612e  ---.    pyvista.
-0001bcf0: 556e 7374 7275 6374 7572 6564 4772 6964  UnstructuredGrid
-0001bd00: 207c 2073 7472 0a20 2020 2020 2020 2043   | str.        C
-0001bd10: 7275 7368 6564 2063 616e 2064 6174 6173  rushed can datas
-0001bd20: 6574 206f 7220 7061 7468 2064 6570 656e  et or path depen
-0001bd30: 6469 6e67 206f 6e20 7468 6520 7661 6c75  ding on the valu
-0001bd40: 6520 6f66 2060 606c 6f61 6460 602e 0a0a  e of ``load``...
-0001bd50: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
-0001bd60: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 506c   --------.    Pl
-0001bd70: 6f74 2074 6865 2063 7275 7368 6564 2063  ot the crushed c
-0001bd80: 616e 2064 6174 6173 6574 2e0a 0a20 2020  an dataset...   
-0001bd90: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-0001bda0: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-0001bdb0: 730a 2020 2020 3e3e 3e20 696d 706f 7274  s.    >>> import
-0001bdc0: 2070 7976 6973 7461 0a20 2020 203e 3e3e   pyvista.    >>>
-0001bdd0: 2064 6174 6173 6574 203d 2065 7861 6d70   dataset = examp
-0001bde0: 6c65 732e 646f 776e 6c6f 6164 5f63 616e  les.download_can
-0001bdf0: 5f63 7275 7368 6564 5f68 6466 2829 0a20  _crushed_hdf(). 
-0001be00: 2020 203e 3e3e 2064 6174 6173 6574 2e70     >>> dataset.p
-0001be10: 6c6f 7428 736d 6f6f 7468 5f73 6861 6469  lot(smooth_shadi
-0001be20: 6e67 3d54 7275 6529 0a0a 2020 2020 2222  ng=True)..    ""
-0001be30: 220a 2020 2020 7265 7475 726e 205f 646f  ".    return _do
-0001be40: 776e 6c6f 6164 5f61 6e64 5f72 6561 6428  wnload_and_read(
-0001be50: 2768 6466 2f63 616e 2d76 7475 2e68 6466  'hdf/can-vtu.hdf
-0001be60: 272c 206c 6f61 643d 6c6f 6164 290a 0a0a  ', load=load)...
-0001be70: 6465 6620 646f 776e 6c6f 6164 5f63 676e  def download_cgn
-0001be80: 735f 7374 7275 6374 7572 6564 286c 6f61  s_structured(loa
-0001be90: 643d 5472 7565 293a 2020 2320 7072 6167  d=True):  # prag
-0001bea0: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
-0001beb0: 2022 2222 446f 776e 6c6f 6164 2074 6865   """Download the
-0001bec0: 2073 7472 7563 7475 7265 6420 4347 4e53   structured CGNS
-0001bed0: 2064 6174 6173 6574 206d 6573 682e 0a0a   dataset mesh...
-0001bee0: 2020 2020 4f72 6967 696e 616c 6c79 2064      Originally d
-0001bef0: 6f77 6e6c 6f61 6465 6420 6672 6f6d 2060  ownloaded from `
-0001bf00: 4346 4420 4765 6e65 7261 6c20 4e6f 7461  CFD General Nota
-0001bf10: 7469 6f6e 2053 7973 7465 6d20 4578 616d  tion System Exam
-0001bf20: 706c 6520 4669 6c65 730a 2020 2020 3c68  ple Files.    <h
-0001bf30: 7474 7073 3a2f 2f63 676e 732e 6769 7468  ttps://cgns.gith
-0001bf40: 7562 2e69 6f2f 4347 4e53 4669 6c65 732e  ub.io/CGNSFiles.
-0001bf50: 6874 6d6c 3e60 5f0a 0a20 2020 2050 6172  html>`_..    Par
-0001bf60: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0001bf70: 2d2d 2d2d 2d2d 0a20 2020 206c 6f61 6420  ------.    load 
-0001bf80: 3a20 626f 6f6c 2c20 6465 6661 756c 743a  : bool, default:
-0001bf90: 2054 7275 650a 2020 2020 2020 2020 4c6f   True.        Lo
-0001bfa0: 6164 2074 6865 2064 6174 6173 6574 2061  ad the dataset a
-0001bfb0: 6674 6572 2064 6f77 6e6c 6f61 6469 6e67  fter downloading
-0001bfc0: 2069 7420 7768 656e 2060 6054 7275 6560   it when ``True`
-0001bfd0: 602e 2020 5365 7420 7468 6973 0a20 2020  `.  Set this.   
-0001bfe0: 2020 2020 2074 6f20 6060 4661 6c73 6560       to ``False`
-0001bff0: 6020 616e 6420 6f6e 6c79 2074 6865 2066  ` and only the f
-0001c000: 696c 656e 616d 6520 7769 6c6c 2062 6520  ilename will be 
-0001c010: 7265 7475 726e 6564 2e0a 0a20 2020 2052  returned...    R
-0001c020: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0001c030: 2d2d 0a20 2020 2070 7976 6973 7461 2e4d  --.    pyvista.M
-0001c040: 756c 7469 426c 6f63 6b20 7c20 7374 720a  ultiBlock | str.
-0001c050: 2020 2020 2020 2020 5374 7275 6374 7572          Structur
-0001c060: 6564 2c20 3132 2062 6c6f 636b 2c20 332d  ed, 12 block, 3-
-0001c070: 4420 636f 6e73 7472 6963 7469 6e67 2063  D constricting c
-0001c080: 6861 6e6e 656c 2c20 7769 7468 2065 7861  hannel, with exa
-0001c090: 6d70 6c65 2075 7365 206f 660a 2020 2020  mple use of.    
-0001c0a0: 2020 2020 4661 6d69 6c79 5f74 2066 6f72      Family_t for
-0001c0b0: 2042 4373 2028 4144 4620 7479 7065 292e   BCs (ADF type).
-0001c0c0: 2049 6620 6060 6c6f 6164 6060 2069 7320   If ``load`` is 
-0001c0d0: 6060 4661 6c73 6560 602c 2074 6865 6e20  ``False``, then 
-0001c0e0: 7468 6520 7061 7468 206f 6620 7468 650a  the path of the.
-0001c0f0: 2020 2020 2020 2020 6578 616d 706c 6520          example 
-0001c100: 4347 4e53 2066 696c 6520 6973 2072 6574  CGNS file is ret
-0001c110: 7572 6e65 642e 0a0a 2020 2020 4578 616d  urned...    Exam
-0001c120: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-0001c130: 2d0a 2020 2020 506c 6f74 2074 6865 2065  -.    Plot the e
-0001c140: 7861 6d70 6c65 2043 474e 5320 6461 7461  xample CGNS data
-0001c150: 7365 742e 0a0a 2020 2020 3e3e 3e20 6672  set...    >>> fr
-0001c160: 6f6d 2070 7976 6973 7461 2069 6d70 6f72  om pyvista impor
-0001c170: 7420 6578 616d 706c 6573 0a20 2020 203e  t examples.    >
-0001c180: 3e3e 2069 6d70 6f72 7420 7079 7669 7374  >> import pyvist
-0001c190: 610a 2020 2020 3e3e 3e20 6461 7461 7365  a.    >>> datase
-0001c1a0: 7420 3d20 6578 616d 706c 6573 2e64 6f77  t = examples.dow
-0001c1b0: 6e6c 6f61 645f 6367 6e73 5f73 7472 7563  nload_cgns_struc
-0001c1c0: 7475 7265 6428 290a 2020 2020 3e3e 3e20  tured().    >>> 
-0001c1d0: 6461 7461 7365 745b 305d 2e70 6c6f 7428  dataset[0].plot(
-0001c1e0: 7363 616c 6172 733d 2744 656e 7369 7479  scalars='Density
-0001c1f0: 2729 0a0a 2020 2020 2222 220a 2020 2020  ')..    """.    
-0001c200: 6669 6c65 6e61 6d65 203d 2064 6f77 6e6c  filename = downl
-0001c210: 6f61 645f 6669 6c65 2827 6367 6e73 2f73  oad_file('cgns/s
-0001c220: 716e 7a5f 732e 6164 662e 6367 6e73 2729  qnz_s.adf.cgns')
-0001c230: 0a20 2020 2069 6620 6e6f 7420 6c6f 6164  .    if not load
-0001c240: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001c250: 2066 696c 656e 616d 650a 2020 2020 7265   filename.    re
-0001c260: 7475 726e 2070 7976 6973 7461 2e67 6574  turn pyvista.get
-0001c270: 5f72 6561 6465 7228 6669 6c65 6e61 6d65  _reader(filename
-0001c280: 292e 7265 6164 2829 0a0a 0a64 6566 2064  ).read()...def d
-0001c290: 6f77 6e6c 6f61 645f 7465 6370 6c6f 745f  ownload_tecplot_
-0001c2a0: 6173 6369 6928 6c6f 6164 3d54 7275 6529  ascii(load=True)
-0001c2b0: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-0001c2c0: 636f 7665 720a 2020 2020 2222 2244 6f77  cover.    """Dow
-0001c2d0: 6e6c 6f61 6420 7468 6520 7369 6e67 6c65  nload the single
-0001c2e0: 2062 6c6f 636b 2041 5343 4949 2054 6563   block ASCII Tec
-0001c2f0: 706c 6f74 2064 6174 6173 6574 2e0a 0a20  plot dataset... 
-0001c300: 2020 204f 7269 6769 6e61 6c6c 7920 646f     Originally do
-0001c310: 776e 6c6f 6164 6564 2066 726f 6d20 5061  wnloaded from Pa
-0001c320: 756c 2042 6f75 726b 6527 730a 2020 2020  ul Bourke's.    
-0001c330: 6053 616d 706c 6520 6669 6c65 203c 6874  `Sample file <ht
-0001c340: 7470 3a2f 2f70 6175 6c62 6f75 726b 652e  tp://paulbourke.
-0001c350: 6e65 742f 6461 7461 666f 726d 6174 732f  net/dataformats/
-0001c360: 7470 2f73 616d 706c 652e 7470 3e60 5f0a  tp/sample.tp>`_.
-0001c370: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-0001c380: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0001c390: 2020 206c 6f61 6420 3a20 626f 6f6c 2c20     load : bool, 
-0001c3a0: 6465 6661 756c 743a 2054 7275 650a 2020  default: True.  
-0001c3b0: 2020 2020 2020 4c6f 6164 2074 6865 2064        Load the d
-0001c3c0: 6174 6173 6574 2061 6674 6572 2064 6f77  ataset after dow
-0001c3d0: 6e6c 6f61 6469 6e67 2069 7420 7768 656e  nloading it when
-0001c3e0: 2060 6054 7275 6560 602e 2020 5365 7420   ``True``.  Set 
-0001c3f0: 7468 6973 0a20 2020 2020 2020 2074 6f20  this.        to 
-0001c400: 6060 4661 6c73 6560 6020 616e 6420 6f6e  ``False`` and on
-0001c410: 6c79 2074 6865 2066 696c 656e 616d 6520  ly the filename 
-0001c420: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
-0001c430: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
-0001c440: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2070     -------.    p
-0001c450: 7976 6973 7461 2e4d 756c 7469 426c 6f63  yvista.MultiBloc
-0001c460: 6b20 7c20 7374 720a 2020 2020 2020 2020  k | str.        
-0001c470: 4d75 6c74 6962 6c6f 636b 2066 6f72 6d61  Multiblock forma
-0001c480: 7420 7769 7468 206f 6e6c 7920 3120 6461  t with only 1 da
-0001c490: 7461 2062 6c6f 636b 2c20 7369 6d70 6c65  ta block, simple
-0001c4a0: 2067 656f 6d65 7472 6963 2073 6861 7065   geometric shape
-0001c4b0: 2e0a 2020 2020 2020 2020 4966 2060 606c  ..        If ``l
-0001c4c0: 6f61 6460 6020 6973 2060 6046 616c 7365  oad`` is ``False
-0001c4d0: 6060 2c20 7468 656e 2074 6865 2070 6174  ``, then the pat
-0001c4e0: 6820 6f66 2074 6865 2065 7861 6d70 6c65  h of the example
-0001c4f0: 2054 6563 706c 6f74 2066 696c 650a 2020   Tecplot file.  
-0001c500: 2020 2020 2020 6973 2072 6574 7572 6e65        is returne
-0001c510: 642e 0a0a 2020 2020 4578 616d 706c 6573  d...    Examples
-0001c520: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-0001c530: 2020 506c 6f74 2074 6865 2065 7861 6d70    Plot the examp
-0001c540: 6c65 2054 6563 706c 6f74 2064 6174 6173  le Tecplot datas
-0001c550: 6574 2e0a 0a20 2020 203e 3e3e 2066 726f  et...    >>> fro
-0001c560: 6d20 7079 7669 7374 6120 696d 706f 7274  m pyvista import
-0001c570: 2065 7861 6d70 6c65 730a 2020 2020 3e3e   examples.    >>
-0001c580: 3e20 696d 706f 7274 2070 7976 6973 7461  > import pyvista
-0001c590: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
-0001c5a0: 203d 2065 7861 6d70 6c65 732e 646f 776e   = examples.down
-0001c5b0: 6c6f 6164 5f74 6563 706c 6f74 5f61 7363  load_tecplot_asc
-0001c5c0: 6969 2829 0a20 2020 203e 3e3e 2064 6174  ii().    >>> dat
-0001c5d0: 6173 6574 2e70 6c6f 7428 290a 0a20 2020  aset.plot()..   
-0001c5e0: 2022 2222 0a20 2020 2066 696c 656e 616d   """.    filenam
-0001c5f0: 6520 3d20 646f 776e 6c6f 6164 5f66 696c  e = download_fil
-0001c600: 6528 2774 6563 706c 6f74 5f61 7363 6969  e('tecplot_ascii
-0001c610: 2e64 6174 2729 0a20 2020 2069 6620 6e6f  .dat').    if no
-0001c620: 7420 6c6f 6164 3a0a 2020 2020 2020 2020  t load:.        
-0001c630: 7265 7475 726e 2066 696c 656e 616d 650a  return filename.
-0001c640: 2020 2020 7265 7475 726e 2070 7976 6973      return pyvis
-0001c650: 7461 2e67 6574 5f72 6561 6465 7228 6669  ta.get_reader(fi
-0001c660: 6c65 6e61 6d65 292e 7265 6164 2829 0a0a  lename).read()..
-0001c670: 0a64 6566 2064 6f77 6e6c 6f61 645f 6367  .def download_cg
-0001c680: 6e73 5f6d 756c 7469 286c 6f61 643d 5472  ns_multi(load=Tr
-0001c690: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
-0001c6a0: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
-0001c6b0: 446f 776e 6c6f 6164 2061 206d 756c 7469  Download a multi
-0001c6c0: 656c 656d 656e 7420 6169 7266 6f69 6c20  element airfoil 
-0001c6d0: 7769 7468 2061 2063 656c 6c20 6365 6e74  with a cell cent
-0001c6e0: 6572 6564 2073 6f6c 7574 696f 6e2e 0a0a  ered solution...
-0001c6f0: 2020 2020 4f72 6967 696e 616c 6c79 2064      Originally d
-0001c700: 6f77 6e6c 6f61 6465 6420 6672 6f6d 2060  ownloaded from `
-0001c710: 4346 4420 4765 6e65 7261 6c20 4e6f 7461  CFD General Nota
-0001c720: 7469 6f6e 2053 7973 7465 6d20 4578 616d  tion System Exam
-0001c730: 706c 6520 4669 6c65 730a 2020 2020 3c68  ple Files.    <h
-0001c740: 7474 7073 3a2f 2f63 676e 732e 6769 7468  ttps://cgns.gith
-0001c750: 7562 2e69 6f2f 4347 4e53 4669 6c65 732e  ub.io/CGNSFiles.
-0001c760: 6874 6d6c 3e60 5f0a 0a20 2020 2050 6172  html>`_..    Par
-0001c770: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0001c780: 2d2d 2d2d 2d2d 0a20 2020 206c 6f61 6420  ------.    load 
-0001c790: 3a20 626f 6f6c 2c20 6465 6661 756c 743a  : bool, default:
-0001c7a0: 2054 7275 650a 2020 2020 2020 2020 4c6f   True.        Lo
-0001c7b0: 6164 2074 6865 2064 6174 6173 6574 2061  ad the dataset a
-0001c7c0: 6674 6572 2064 6f77 6e6c 6f61 6469 6e67  fter downloading
-0001c7d0: 2069 7420 7768 656e 2060 6054 7275 6560   it when ``True`
-0001c7e0: 602e 2020 5365 7420 7468 6973 0a20 2020  `.  Set this.   
-0001c7f0: 2020 2020 2074 6f20 6060 4661 6c73 6560       to ``False`
-0001c800: 6020 616e 6420 6f6e 6c79 2074 6865 2066  ` and only the f
-0001c810: 696c 656e 616d 6520 7769 6c6c 2062 6520  ilename will be 
-0001c820: 7265 7475 726e 6564 2e0a 0a20 2020 2052  returned...    R
-0001c830: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0001c840: 2d2d 0a20 2020 2070 7976 6973 7461 2e4d  --.    pyvista.M
-0001c850: 756c 7469 426c 6f63 6b20 7c20 7374 720a  ultiBlock | str.
-0001c860: 2020 2020 2020 2020 5374 7275 6374 7572          Structur
-0001c870: 6564 2c20 3420 626c 6f63 6b73 2c20 3244  ed, 4 blocks, 2D
-0001c880: 2028 3220 706c 616e 6573 2069 6e20 7468   (2 planes in th
-0001c890: 6972 6420 6469 6d65 6e73 696f 6e29 206d  ird dimension) m
-0001c8a0: 756c 7469 656c 656d 656e 740a 2020 2020  ultielement.    
-0001c8b0: 2020 2020 6169 7266 6f69 6c2c 2077 6974      airfoil, wit
-0001c8c0: 6820 6365 6c6c 2063 656e 7465 7265 6420  h cell centered 
-0001c8d0: 736f 6c75 7469 6f6e 2e20 4966 2060 606c  solution. If ``l
-0001c8e0: 6f61 6460 6020 6973 2060 6046 616c 7365  oad`` is ``False
-0001c8f0: 6060 2c20 7468 656e 2074 6865 2070 6174  ``, then the pat
-0001c900: 6820 6f66 2074 6865 0a20 2020 2020 2020  h of the.       
-0001c910: 2065 7861 6d70 6c65 2043 474e 5320 6669   example CGNS fi
-0001c920: 6c65 2069 7320 7265 7475 726e 6564 2e0a  le is returned..
-0001c930: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
-0001c940: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2050    --------.    P
-0001c950: 6c6f 7420 7468 6520 6169 7266 6f69 6c20  lot the airfoil 
-0001c960: 6461 7461 7365 742e 204d 6572 6765 2074  dataset. Merge t
-0001c970: 6865 206d 756c 7469 2d62 6c6f 636b 2061  he multi-block a
-0001c980: 6e64 2074 6865 6e20 706c 6f74 2074 6865  nd then plot the
-0001c990: 2061 6972 666f 696c 2773 0a20 2020 2060   airfoil's.    `
-0001c9a0: 6022 5669 7363 6f73 6974 7945 6464 7922  `"ViscosityEddy"
-0001c9b0: 6060 2e20 436f 6e76 6572 7420 7468 6520  ``. Convert the 
-0001c9c0: 6365 6c6c 2064 6174 6120 746f 2070 6f69  cell data to poi
-0001c9d0: 6e74 2064 6174 6120 6173 2069 6e20 7468  nt data as in th
-0001c9e0: 6973 0a20 2020 2064 6174 6173 6574 2c20  is.    dataset, 
-0001c9f0: 7468 6520 736f 6c75 7469 6f6e 2069 7320  the solution is 
-0001ca00: 7374 6f72 6564 2077 6974 6869 6e20 7468  stored within th
-0001ca10: 6520 6365 6c6c 732e 0a0a 2020 2020 3e3e  e cells...    >>
-0001ca20: 3e20 6672 6f6d 2070 7976 6973 7461 2069  > from pyvista i
-0001ca30: 6d70 6f72 7420 6578 616d 706c 6573 0a20  mport examples. 
-0001ca40: 2020 203e 3e3e 2069 6d70 6f72 7420 7079     >>> import py
-0001ca50: 7669 7374 610a 2020 2020 3e3e 3e20 6461  vista.    >>> da
-0001ca60: 7461 7365 7420 3d20 6578 616d 706c 6573  taset = examples
-0001ca70: 2e64 6f77 6e6c 6f61 645f 6367 6e73 5f6d  .download_cgns_m
-0001ca80: 756c 7469 2829 0a20 2020 203e 3e3e 2075  ulti().    >>> u
-0001ca90: 6772 6964 203d 2064 6174 6173 6574 2e63  grid = dataset.c
-0001caa0: 6f6d 6269 6e65 2829 0a20 2020 203e 3e3e  ombine().    >>>
-0001cab0: 2075 6772 6964 203d 2075 6772 6964 203d   ugrid = ugrid =
-0001cac0: 2075 6772 6964 2e63 656c 6c5f 6461 7461   ugrid.cell_data
-0001cad0: 5f74 6f5f 706f 696e 745f 6461 7461 2829  _to_point_data()
-0001cae0: 0a20 2020 203e 3e3e 2075 6772 6964 2e70  .    >>> ugrid.p
-0001caf0: 6c6f 7428 0a20 2020 202e 2e2e 2020 2020  lot(.    ...    
-0001cb00: 2063 6d61 703d 2762 7772 272c 0a20 2020   cmap='bwr',.   
-0001cb10: 202e 2e2e 2020 2020 2073 6361 6c61 7273   ...     scalars
-0001cb20: 3d27 5669 7363 6f73 6974 7945 6464 7927  ='ViscosityEddy'
-0001cb30: 2c0a 2020 2020 2e2e 2e20 2020 2020 7a6f  ,.    ...     zo
-0001cb40: 6f6d 3d34 2c0a 2020 2020 2e2e 2e20 2020  om=4,.    ...   
-0001cb50: 2020 6370 6f73 3d27 787a 272c 0a20 2020    cpos='xz',.   
-0001cb60: 202e 2e2e 2020 2020 2073 686f 775f 7363   ...     show_sc
-0001cb70: 616c 6172 5f62 6172 3d46 616c 7365 2c0a  alar_bar=False,.
-0001cb80: 2020 2020 2e2e 2e20 290a 0a20 2020 2022      ... )..    "
-0001cb90: 2222 0a20 2020 2066 696c 656e 616d 6520  "".    filename 
-0001cba0: 3d20 646f 776e 6c6f 6164 5f66 696c 6528  = download_file(
-0001cbb0: 2763 676e 732f 6d75 6c74 692e 6367 6e73  'cgns/multi.cgns
-0001cbc0: 2729 0a20 2020 2069 6620 6e6f 7420 6c6f  ').    if not lo
-0001cbd0: 6164 3a0a 2020 2020 2020 2020 7265 7475  ad:.        retu
-0001cbe0: 726e 2066 696c 656e 616d 650a 2020 2020  rn filename.    
-0001cbf0: 7265 6164 6572 203d 2070 7976 6973 7461  reader = pyvista
-0001cc00: 2e67 6574 5f72 6561 6465 7228 6669 6c65  .get_reader(file
-0001cc10: 6e61 6d65 290a 0a20 2020 2023 2064 6973  name)..    # dis
-0001cc20: 6162 6c65 2072 6561 6469 6e67 2074 6865  able reading the
-0001cc30: 2062 6f75 6e64 6172 7920 7061 7463 682e   boundary patch.
-0001cc40: 2041 7320 6f66 2056 544b 2039 2e31 2e30   As of VTK 9.1.0
-0001cc50: 2074 6869 7320 6765 6e65 7261 7465 730a   this generates.
-0001cc60: 2020 2020 2320 6d65 7373 6167 6573 206c      # messages l
-0001cc70: 696b 6520 2253 6b69 7070 696e 6720 4243  ike "Skipping BC
-0001cc80: 5f74 206e 6f64 653a 2042 435f 7420 7479  _t node: BC_t ty
-0001cc90: 7065 2027 4243 4661 7266 6965 6c64 2720  pe 'BCFarfield' 
-0001cca0: 6e6f 7420 7375 7070 6f72 7465 640a 2020  not supported.  
-0001ccb0: 2020 2320 7965 742e 220a 2020 2020 7265    # yet.".    re
-0001ccc0: 6164 6572 2e6c 6f61 645f 626f 756e 6461  ader.load_bounda
-0001ccd0: 7279 5f70 6174 6368 203d 2046 616c 7365  ry_patch = False
-0001cce0: 0a20 2020 2072 6574 7572 6e20 7265 6164  .    return read
-0001ccf0: 6572 2e72 6561 6428 290a 0a0a 6465 6620  er.read()...def 
-0001cd00: 646f 776e 6c6f 6164 5f64 6963 6f6d 5f73  download_dicom_s
-0001cd10: 7461 636b 286c 6f61 643a 2062 6f6f 6c20  tack(load: bool 
-0001cd20: 3d20 5472 7565 2920 2d3e 2055 6e69 6f6e  = True) -> Union
-0001cd30: 5b70 7976 6973 7461 2e55 6e69 666f 726d  [pyvista.Uniform
-0001cd40: 4772 6964 2c20 7374 725d 3a20 2023 2070  Grid, str]:  # p
-0001cd50: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
-0001cd60: 2020 2020 2222 2244 6f77 6e6c 6f61 6420      """Download 
-0001cd70: 5443 4941 2044 4943 4f4d 2073 7461 636b  TCIA DICOM stack
-0001cd80: 2076 6f6c 756d 652e 0a0a 2020 2020 4f72   volume...    Or
-0001cd90: 6967 696e 616c 2064 6f77 6e6c 6f61 6420  iginal download 
-0001cda0: 6672 6f6d 2074 6865 2060 5468 6520 4361  from the `The Ca
-0001cdb0: 6e63 6572 2049 6d61 6769 6e67 2041 7263  ncer Imaging Arc
-0001cdc0: 6869 7665 2028 5443 4941 290a 2020 2020  hive (TCIA).    
-0001cdd0: 3c68 7474 7073 3a2f 2f77 7777 2e63 616e  <https://www.can
-0001cde0: 6365 7269 6d61 6769 6e67 6172 6368 6976  cerimagingarchiv
-0001cdf0: 652e 6e65 742f 3e60 5f2e 2054 6869 7320  e.net/>`_. This 
-0001ce00: 6973 2070 6172 7420 6f66 2074 6865 0a20  is part of the. 
-0001ce10: 2020 2043 6c69 6e69 6361 6c20 5072 6f74     Clinical Prot
-0001ce20: 656f 6d69 6320 5475 6d6f 7220 416e 616c  eomic Tumor Anal
-0001ce30: 7973 6973 2043 6f6e 736f 7274 6975 6d20  ysis Consortium 
-0001ce40: 5361 7263 6f6d 6173 2028 4350 5441 432d  Sarcomas (CPTAC-
-0001ce50: 5341 5229 0a20 2020 2063 6f6c 6c65 6374  SAR).    collect
-0001ce60: 696f 6e2e 0a0a 2020 2020 5061 7261 6d65  ion...    Parame
-0001ce70: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0001ce80: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-0001ce90: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-0001cea0: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-0001ceb0: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-0001cec0: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-0001ced0: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-0001cee0: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-0001cef0: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-0001cf00: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-0001cf10: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-0001cf20: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-0001cf30: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0001cf40: 2020 2020 7079 7669 7374 612e 556e 6966      pyvista.Unif
-0001cf50: 6f72 6d47 7269 6420 7c20 7374 720a 2020  ormGrid | str.  
-0001cf60: 2020 2020 2020 4461 7461 5365 7420 6f72        DataSet or
-0001cf70: 2070 6174 6820 6465 7065 6e64 696e 6720   path depending 
-0001cf80: 6f6e 2060 606c 6f61 6460 602e 0a0a 2020  on ``load``...  
-0001cf90: 2020 5265 6665 7265 6e63 6573 0a20 2020    References.   
-0001cfa0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0001cfb0: 2a20 2a2a 4461 7461 2043 6974 6174 696f  * **Data Citatio
-0001cfc0: 6e2a 2a0a 0a20 2020 2020 2020 204e 6174  n**..        Nat
-0001cfd0: 696f 6e61 6c20 4361 6e63 6572 2049 6e73  ional Cancer Ins
-0001cfe0: 7469 7475 7465 2043 6c69 6e69 6361 6c20  titute Clinical 
-0001cff0: 5072 6f74 656f 6d69 6320 5475 6d6f 7220  Proteomic Tumor 
-0001d000: 416e 616c 7973 6973 2043 6f6e 736f 7274  Analysis Consort
-0001d010: 6975 6d0a 2020 2020 2020 2020 2843 5054  ium.        (CPT
-0001d020: 4143 292e 2028 3230 3138 292e 2020 5261  AC). (2018).  Ra
-0001d030: 6469 6f6c 6f67 7920 4461 7461 2066 726f  diology Data fro
-0001d040: 6d20 7468 6520 436c 696e 6963 616c 2050  m the Clinical P
-0001d050: 726f 7465 6f6d 6963 2054 756d 6f72 0a20  roteomic Tumor. 
-0001d060: 2020 2020 2020 2041 6e61 6c79 7369 7320         Analysis 
-0001d070: 436f 6e73 6f72 7469 756d 2053 6172 636f  Consortium Sarco
-0001d080: 6d61 7320 5b43 5054 4143 2d53 4152 5d20  mas [CPTAC-SAR] 
-0001d090: 636f 6c6c 6563 7469 6f6e 205b 4461 7461  collection [Data
-0001d0a0: 2073 6574 5d2e 2054 6865 0a20 2020 2020   set]. The.     
-0001d0b0: 2020 2043 616e 6365 7220 496d 6167 696e     Cancer Imagin
-0001d0c0: 6720 4172 6368 6976 652e 2020 444f 493a  g Archive.  DOI:
-0001d0d0: 2031 302e 3739 3337 2f54 4349 412e 3230   10.7937/TCIA.20
-0001d0e0: 3139 2e39 6274 3233 7239 350a 0a20 2020  19.9bt23r95..   
-0001d0f0: 202a 202a 2a41 636b 6e6f 776c 6564 6765   * **Acknowledge
-0001d100: 6d65 6e74 2a2a 0a0a 2020 2020 2020 2020  ment**..        
-0001d110: 4461 7461 2075 7365 6420 696e 2074 6869  Data used in thi
-0001d120: 7320 7075 626c 6963 6174 696f 6e20 7765  s publication we
-0001d130: 7265 2067 656e 6572 6174 6564 2062 7920  re generated by 
-0001d140: 7468 6520 4e61 7469 6f6e 616c 2043 616e  the National Can
-0001d150: 6365 7220 496e 7374 6974 7574 6520 436c  cer Institute Cl
-0001d160: 696e 6963 616c 0a20 2020 2020 2020 2050  inical.        P
-0001d170: 726f 7465 6f6d 6963 2054 756d 6f72 2041  roteomic Tumor A
-0001d180: 6e61 6c79 7369 7320 436f 6e73 6f72 7469  nalysis Consorti
-0001d190: 756d 2028 4350 5441 4329 2e0a 0a20 2020  um (CPTAC)...   
-0001d1a0: 202a 202a 2a54 4349 4120 4369 7461 7469   * **TCIA Citati
-0001d1b0: 6f6e 2a2a 0a0a 2020 2020 2020 2020 436c  on**..        Cl
-0001d1c0: 6172 6b20 4b2c 2056 656e 6474 2042 2c20  ark K, Vendt B, 
-0001d1d0: 536d 6974 6820 4b2c 2046 7265 796d 616e  Smith K, Freyman
-0001d1e0: 6e20 4a2c 204b 6972 6279 204a 2c20 4b6f  n J, Kirby J, Ko
-0001d1f0: 7070 656c 2050 2c20 4d6f 6f72 6520 532c  ppel P, Moore S,
-0001d200: 2050 6869 6c6c 6970 7320 532c 0a20 2020   Phillips S,.   
-0001d210: 2020 2020 204d 6166 6669 7474 2044 2c20       Maffitt D, 
-0001d220: 5072 696e 676c 6520 4d2c 2054 6172 626f  Pringle M, Tarbo
-0001d230: 7820 4c2c 2050 7269 6f72 2046 2e20 5468  x L, Prior F. Th
-0001d240: 6520 4361 6e63 6572 2049 6d61 6769 6e67  e Cancer Imaging
-0001d250: 2041 7263 6869 7665 2028 5443 4941 293a   Archive (TCIA):
-0001d260: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
-0001d270: 6f76 6572 0a20 2020 2020 2020 204d 6169  over.        Mai
-0001d280: 6e74 6169 6e69 6e67 2061 6e64 204f 7065  ntaining and Ope
-0001d290: 7261 7469 6e67 2061 2050 7562 6c69 6320  rating a Public 
-0001d2a0: 496e 666f 726d 6174 696f 6e20 5265 706f  Information Repo
-0001d2b0: 7369 746f 7279 2c20 4a6f 7572 6e61 6c20  sitory, Journal 
-0001d2c0: 6f66 2044 6967 6974 616c 2049 6d61 6769  of Digital Imagi
-0001d2d0: 6e67 2c0a 2020 2020 2020 2020 566f 6c75  ng,.        Volu
-0001d2e0: 6d65 2032 362c 204e 756d 6265 7220 362c  me 26, Number 6,
-0001d2f0: 2044 6563 656d 6265 722c 2032 3031 332c   December, 2013,
-0001d300: 2070 7020 3130 3435 2d31 3035 372e 2064   pp 1045-1057. d
-0001d310: 6f69 3a20 3130 2e31 3030 372f 7331 3032  oi: 10.1007/s102
-0001d320: 3738 2d30 3133 2d39 3632 322d 370a 0a20  78-013-9622-7.. 
-0001d330: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-0001d340: 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e  --------.    >>>
-0001d350: 2066 726f 6d20 7079 7669 7374 6120 696d   from pyvista im
-0001d360: 706f 7274 2065 7861 6d70 6c65 730a 2020  port examples.  
-0001d370: 2020 3e3e 3e20 6461 7461 7365 7420 3d20    >>> dataset = 
-0001d380: 6578 616d 706c 6573 2e64 6f77 6e6c 6f61  examples.downloa
-0001d390: 645f 6469 636f 6d5f 7374 6163 6b28 290a  d_dicom_stack().
-0001d3a0: 2020 2020 3e3e 3e20 6461 7461 7365 742e      >>> dataset.
-0001d3b0: 706c 6f74 2876 6f6c 756d 653d 5472 7565  plot(volume=True
-0001d3c0: 2c20 7a6f 6f6d 3d33 2c20 7368 6f77 5f73  , zoom=3, show_s
-0001d3d0: 6361 6c61 725f 6261 723d 4661 6c73 6529  calar_bar=False)
-0001d3e0: 0a0a 2020 2020 2222 220a 2020 2020 666e  ..    """.    fn
-0001d3f0: 616d 6573 203d 205f 646f 776e 6c6f 6164  ames = _download
-0001d400: 5f61 7263 6869 7665 2827 4449 434f 4d5f  _archive('DICOM_
-0001d410: 5374 6163 6b2f 6461 7461 2e7a 6970 2729  Stack/data.zip')
-0001d420: 0a20 2020 2070 6174 6820 3d20 6f73 2e70  .    path = os.p
-0001d430: 6174 682e 6469 726e 616d 6528 666e 616d  ath.dirname(fnam
-0001d440: 6573 5b30 5d29 0a20 2020 2069 6620 6c6f  es[0]).    if lo
-0001d450: 6164 3a0a 2020 2020 2020 2020 7265 6164  ad:.        read
-0001d460: 6572 203d 2070 7976 6973 7461 2e44 4943  er = pyvista.DIC
-0001d470: 4f4d 5265 6164 6572 2870 6174 6829 0a20  OMReader(path). 
-0001d480: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0001d490: 6164 6572 2e72 6561 6428 290a 2020 2020  ader.read().    
-0001d4a0: 7265 7475 726e 2070 6174 680a 0a0a 6465  return path...de
-0001d4b0: 6620 646f 776e 6c6f 6164 5f70 6172 6368  f download_parch
-0001d4c0: 6564 5f63 616e 616c 5f34 6b28 6c6f 6164  ed_canal_4k(load
-0001d4d0: 3d54 7275 6529 3a20 2023 2070 7261 676d  =True):  # pragm
-0001d4e0: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
-0001d4f0: 2222 2244 6f77 6e6c 6f61 6420 7061 7263  """Download parc
-0001d500: 6865 6420 6361 6e61 6c20 346b 2064 6174  hed canal 4k dat
-0001d510: 6173 6574 2e0a 0a20 2020 2050 6172 616d  aset...    Param
-0001d520: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-0001d530: 2d2d 2d2d 0a20 2020 206c 6f61 6420 3a20  ----.    load : 
-0001d540: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
-0001d550: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
-0001d560: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
-0001d570: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
-0001d580: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
-0001d590: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
-0001d5a0: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
-0001d5b0: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
-0001d5c0: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
-0001d5d0: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
-0001d5e0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-0001d5f0: 0a20 2020 2070 7976 6973 7461 2e54 6578  .    pyvista.Tex
-0001d600: 7475 7265 207c 2073 7472 0a20 2020 2020  ture | str.     
-0001d610: 2020 2044 6174 6153 6574 206f 7220 6669     DataSet or fi
-0001d620: 6c65 6e61 6d65 2064 6570 656e 6469 6e67  lename depending
-0001d630: 206f 6e20 6060 6c6f 6164 6060 2e0a 0a20   on ``load``... 
-0001d640: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-0001d650: 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e  --------.    >>>
-0001d660: 2066 726f 6d20 7079 7669 7374 6120 696d   from pyvista im
-0001d670: 706f 7274 2065 7861 6d70 6c65 730a 2020  port examples.  
-0001d680: 2020 3e3e 3e20 6461 7461 7365 7420 3d20    >>> dataset = 
-0001d690: 6578 616d 706c 6573 2e64 6f77 6e6c 6f61  examples.downloa
-0001d6a0: 645f 7061 7263 6865 645f 6361 6e61 6c5f  d_parched_canal_
-0001d6b0: 346b 2829 0a20 2020 203e 3e3e 2064 6174  4k().    >>> dat
-0001d6c0: 6173 6574 2e70 6c6f 7428 6370 6f73 3d22  aset.plot(cpos="
-0001d6d0: 7879 2229 0a0a 2020 2020 2222 220a 2020  xy")..    """.  
-0001d6e0: 2020 7265 7475 726e 205f 646f 776e 6c6f    return _downlo
-0001d6f0: 6164 5f61 6e64 5f72 6561 6428 2270 6172  ad_and_read("par
-0001d700: 6368 6564 5f63 616e 616c 5f34 6b2e 6864  ched_canal_4k.hd
-0001d710: 7222 2c20 7465 7874 7572 653d 5472 7565  r", texture=True
-0001d720: 2c20 6c6f 6164 3d6c 6f61 6429 0a0a 0a64  , load=load)...d
-0001d730: 6566 2064 6f77 6e6c 6f61 645f 6365 6c6c  ef download_cell
-0001d740: 735f 6e64 286c 6f61 643d 5472 7565 293a  s_nd(load=True):
-0001d750: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
-0001d760: 6f76 6572 0a20 2020 2022 2222 446f 776e  over.    """Down
-0001d770: 6c6f 6164 2065 7861 6d70 6c65 2041 5653  load example AVS
-0001d780: 2055 4344 2064 6174 6173 6574 2e0a 0a20   UCD dataset... 
-0001d790: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0001d7a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0001d7b0: 206c 6f61 6420 3a20 626f 6f6c 2c20 6465   load : bool, de
-0001d7c0: 6661 756c 743a 2054 7275 650a 2020 2020  fault: True.    
-0001d7d0: 2020 2020 4c6f 6164 2074 6865 2064 6174      Load the dat
-0001d7e0: 6173 6574 2061 6674 6572 2064 6f77 6e6c  aset after downl
-0001d7f0: 6f61 6469 6e67 2069 7420 7768 656e 2060  oading it when `
-0001d800: 6054 7275 6560 602e 2020 5365 7420 7468  `True``.  Set th
-0001d810: 6973 0a20 2020 2020 2020 2074 6f20 6060  is.        to ``
-0001d820: 4661 6c73 6560 6020 616e 6420 6f6e 6c79  False`` and only
-0001d830: 2074 6865 2066 696c 656e 616d 6520 7769   the filename wi
-0001d840: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
-0001d850: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-0001d860: 202d 2d2d 2d2d 2d2d 0a20 2020 2070 7976   -------.    pyv
-0001d870: 6973 7461 2e55 6e73 7472 7563 7475 7265  ista.Unstructure
-0001d880: 6447 7269 6420 7c20 7374 720a 2020 2020  dGrid | str.    
-0001d890: 2020 2020 4461 7461 5365 7420 6f72 2066      DataSet or f
-0001d8a0: 696c 656e 616d 6520 6465 7065 6e64 696e  ilename dependin
-0001d8b0: 6720 6f6e 2060 606c 6f61 6460 602e 0a0a  g on ``load``...
-0001d8c0: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
-0001d8d0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e   --------.    >>
-0001d8e0: 3e20 6672 6f6d 2070 7976 6973 7461 2069  > from pyvista i
-0001d8f0: 6d70 6f72 7420 6578 616d 706c 6573 0a20  mport examples. 
-0001d900: 2020 203e 3e3e 2064 6174 6173 6574 203d     >>> dataset =
-0001d910: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
-0001d920: 6164 5f63 656c 6c73 5f6e 6428 290a 2020  ad_cells_nd().  
-0001d930: 2020 3e3e 3e20 6461 7461 7365 742e 706c    >>> dataset.pl
-0001d940: 6f74 2863 706f 733d 2278 7922 290a 0a20  ot(cpos="xy").. 
-0001d950: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
-0001d960: 6e20 5f64 6f77 6e6c 6f61 645f 616e 645f  n _download_and_
-0001d970: 7265 6164 2822 6365 6c6c 736e 642e 6173  read("cellsnd.as
-0001d980: 6369 692e 696e 7022 2c20 6c6f 6164 3d6c  cii.inp", load=l
-0001d990: 6f61 6429 0a0a 0a64 6566 2064 6f77 6e6c  oad)...def downl
-0001d9a0: 6f61 645f 6d6f 6f6e 6c61 6e64 696e 675f  oad_moonlanding_
-0001d9b0: 696d 6167 6528 6c6f 6164 3d54 7275 6529  image(load=True)
-0001d9c0: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-0001d9d0: 636f 7665 720a 2020 2020 2222 2244 6f77  cover.    """Dow
-0001d9e0: 6e6c 6f61 6420 7468 6520 4d6f 6f6e 206c  nload the Moon l
-0001d9f0: 616e 6469 6e67 2069 6d61 6765 2e0a 0a20  anding image... 
-0001da00: 2020 2054 6869 7320 6973 2061 206e 6f69     This is a noi
-0001da10: 7379 2069 6d61 6765 206f 7269 6769 6e61  sy image origina
-0001da20: 6c6c 7920 6f62 7461 696e 6564 2066 726f  lly obtained fro
-0001da30: 6d20 6053 6369 7079 204c 6563 7475 7265  m `Scipy Lecture
-0001da40: 204e 6f74 6573 0a20 2020 203c 6874 7470   Notes.    <http
-0001da50: 733a 2f2f 7363 6970 792d 6c65 6374 7572  s://scipy-lectur
-0001da60: 6573 2e6f 7267 2f69 6e64 6578 2e68 746d  es.org/index.htm
-0001da70: 6c3e 605f 2061 6e64 2063 616e 2062 6520  l>`_ and can be 
-0001da80: 7573 6564 2074 6f20 6465 6d6f 6e73 7472  used to demonstr
-0001da90: 6174 6520 610a 2020 2020 6c6f 7720 7061  ate a.    low pa
-0001daa0: 7373 2066 696c 7465 722e 0a0a 2020 2020  ss filter...    
-0001dab0: 5365 6520 7468 6520 6073 6369 7079 2d6c  See the `scipy-l
-0001dac0: 6563 7475 7265 7320 6c69 6365 6e73 650a  ectures license.
-0001dad0: 2020 2020 3c68 7474 703a 2f2f 7363 6970      <http://scip
-0001dae0: 792d 6c65 6374 7572 6573 2e6f 7267 2f70  y-lectures.org/p
-0001daf0: 7265 6661 6365 2e68 746d 6c23 6c69 6365  reface.html#lice
-0001db00: 6e73 653e 605f 2066 6f72 206d 6f72 6520  nse>`_ for more 
-0001db10: 6465 7461 696c 730a 2020 2020 7265 6761  details.    rega
-0001db20: 7264 696e 6720 7468 6973 2069 6d61 6765  rding this image
-0001db30: 2773 2075 7365 2061 6e64 2064 6973 7472  's use and distr
-0001db40: 6962 7574 696f 6e2e 0a0a 2020 2020 5061  ibution...    Pa
-0001db50: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-0001db60: 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f 6164  -------.    load
-0001db70: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-0001db80: 3a20 5472 7565 0a20 2020 2020 2020 204c  : True.        L
-0001db90: 6f61 6420 7468 6520 6461 7461 7365 7420  oad the dataset 
-0001dba0: 6166 7465 7220 646f 776e 6c6f 6164 696e  after downloadin
-0001dbb0: 6720 6974 2077 6865 6e20 6060 5472 7565  g it when ``True
-0001dbc0: 6060 2e20 2053 6574 2074 6869 730a 2020  ``.  Set this.  
-0001dbd0: 2020 2020 2020 746f 2060 6046 616c 7365        to ``False
-0001dbe0: 6060 2061 6e64 206f 6e6c 7920 7468 6520  `` and only the 
-0001dbf0: 6669 6c65 6e61 6d65 2077 696c 6c20 6265  filename will be
-0001dc00: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
-0001dc10: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0001dc20: 2d2d 2d0a 2020 2020 7079 7669 7374 612e  ---.    pyvista.
-0001dc30: 556e 6966 6f72 6d47 7269 6420 7c20 7374  UniformGrid | st
-0001dc40: 720a 2020 2020 2020 2020 6060 4461 7461  r.        ``Data
-0001dc50: 5365 7460 6020 6f72 2066 696c 656e 616d  Set`` or filenam
-0001dc60: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
-0001dc70: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
-0001dc80: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-0001dc90: 2d2d 2d0a 2020 2020 3e3e 3e20 6672 6f6d  ---.    >>> from
-0001dca0: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
-0001dcb0: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
-0001dcc0: 2064 6174 6173 6574 203d 2065 7861 6d70   dataset = examp
-0001dcd0: 6c65 732e 646f 776e 6c6f 6164 5f6d 6f6f  les.download_moo
-0001dce0: 6e6c 616e 6469 6e67 5f69 6d61 6765 2829  nlanding_image()
-0001dcf0: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
-0001dd00: 2e70 6c6f 7428 0a20 2020 202e 2e2e 2020  .plot(.    ...  
-0001dd10: 2020 2063 706f 733d 2778 7927 2c0a 2020     cpos='xy',.  
-0001dd20: 2020 2e2e 2e20 2020 2020 636d 6170 3d27    ...     cmap='
-0001dd30: 6772 6179 272c 0a20 2020 202e 2e2e 2020  gray',.    ...  
-0001dd40: 2020 2062 6163 6b67 726f 756e 643d 2777     background='w
-0001dd50: 272c 0a20 2020 202e 2e2e 2020 2020 2073  ',.    ...     s
-0001dd60: 686f 775f 7363 616c 6172 5f62 6172 3d46  how_scalar_bar=F
-0001dd70: 616c 7365 2c0a 2020 2020 2e2e 2e20 290a  alse,.    ... ).
-0001dd80: 0a20 2020 2053 6565 203a 7265 663a 6069  .    See :ref:`i
-0001dd90: 6d61 6765 5f66 6674 5f65 7861 6d70 6c65  mage_fft_example
-0001dda0: 6020 666f 7220 6120 6675 6c6c 2065 7861  ` for a full exa
-0001ddb0: 6d70 6c65 2075 7369 6e67 2074 6869 7320  mple using this 
-0001ddc0: 6461 7461 7365 742e 0a0a 2020 2020 2222  dataset...    ""
-0001ddd0: 220a 2020 2020 7265 7475 726e 205f 646f  ".    return _do
-0001dde0: 776e 6c6f 6164 5f61 6e64 5f72 6561 6428  wnload_and_read(
-0001ddf0: 276d 6f6f 6e6c 616e 6469 6e67 2e70 6e67  'moonlanding.png
-0001de00: 272c 206c 6f61 643d 6c6f 6164 290a 0a0a  ', load=load)...
-0001de10: 6465 6620 646f 776e 6c6f 6164 5f61 6e67  def download_ang
-0001de20: 756c 6172 5f73 6563 746f 7228 6c6f 6164  ular_sector(load
-0001de30: 3d54 7275 6529 3a20 2023 2070 7261 676d  =True):  # pragm
-0001de40: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
-0001de50: 2222 2244 6f77 6e6c 6f61 6420 7468 6520  """Download the 
-0001de60: 616e 6775 6c61 7220 7365 6374 6f72 2064  angular sector d
-0001de70: 6174 6173 6574 2e0a 0a20 2020 2050 6172  ataset...    Par
-0001de80: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0001de90: 2d2d 2d2d 2d2d 0a20 2020 206c 6f61 6420  ------.    load 
-0001dea0: 3a20 626f 6f6c 2c20 6465 6661 756c 743a  : bool, default:
-0001deb0: 2054 7275 650a 2020 2020 2020 2020 4c6f   True.        Lo
-0001dec0: 6164 2074 6865 2064 6174 6173 6574 2061  ad the dataset a
-0001ded0: 6674 6572 2064 6f77 6e6c 6f61 6469 6e67  fter downloading
-0001dee0: 2069 7420 7768 656e 2060 6054 7275 6560   it when ``True`
-0001def0: 602e 2020 5365 7420 7468 6973 0a20 2020  `.  Set this.   
-0001df00: 2020 2020 2074 6f20 6060 4661 6c73 6560       to ``False`
-0001df10: 6020 616e 6420 6f6e 6c79 2074 6865 2066  ` and only the f
-0001df20: 696c 656e 616d 6520 7769 6c6c 2062 6520  ilename will be 
-0001df30: 7265 7475 726e 6564 2e0a 0a20 2020 2052  returned...    R
-0001df40: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0001df50: 2d2d 0a20 2020 2070 7976 6973 7461 2e55  --.    pyvista.U
-0001df60: 6e73 7472 7563 7475 7265 6447 7269 6420  nstructuredGrid 
-0001df70: 7c20 7374 720a 2020 2020 2020 2020 4461  | str.        Da
-0001df80: 7461 5365 7420 6f72 2066 696c 656e 616d  taSet or filenam
-0001df90: 6520 6465 7065 6e64 696e 6720 6f6e 2060  e depending on `
-0001dfa0: 606c 6f61 6460 602e 0a0a 2020 2020 4578  `load``...    Ex
-0001dfb0: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-0001dfc0: 2d2d 2d0a 2020 2020 3e3e 3e20 6672 6f6d  ---.    >>> from
-0001dfd0: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
-0001dfe0: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
-0001dff0: 2064 6174 6173 6574 203d 2065 7861 6d70   dataset = examp
-0001e000: 6c65 732e 646f 776e 6c6f 6164 5f61 6e67  les.download_ang
-0001e010: 756c 6172 5f73 6563 746f 7228 290a 2020  ular_sector().  
-0001e020: 2020 3e3e 3e20 6461 7461 7365 742e 706c    >>> dataset.pl
-0001e030: 6f74 2873 6361 6c61 7273 3d27 506f 696e  ot(scalars='Poin
-0001e040: 7449 6427 290a 0a20 2020 2022 2222 0a20  tId')..    """. 
-0001e050: 2020 2072 6574 7572 6e20 5f64 6f77 6e6c     return _downl
-0001e060: 6f61 645f 616e 645f 7265 6164 2827 416e  oad_and_read('An
-0001e070: 6775 6c61 7253 6563 746f 722e 7674 6b27  gularSector.vtk'
-0001e080: 2c20 6c6f 6164 3d6c 6f61 6429 0a0a 0a64  , load=load)...d
-0001e090: 6566 2064 6f77 6e6c 6f61 645f 6d6f 756e  ef download_moun
-0001e0a0: 745f 6461 6d61 7661 6e64 286c 6f61 643d  t_damavand(load=
-0001e0b0: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
-0001e0c0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
-0001e0d0: 2222 446f 776e 6c6f 6164 2074 6865 204d  ""Download the M
-0001e0e0: 6f75 6e74 2044 616d 6176 616e 6420 6461  ount Damavand da
-0001e0f0: 7461 7365 742e 0a0a 2020 2020 5669 7375  taset...    Visu
-0001e100: 616c 697a 6520 3344 206d 6f64 656c 7320  alize 3D models 
-0001e110: 6f66 2044 616d 6176 616e 6420 566f 6c63  of Damavand Volc
-0001e120: 616e 6f2c 2041 6c62 6f72 7a2c 2049 7261  ano, Alborz, Ira
-0001e130: 6e2e 2054 6869 7320 6973 2061 2032 4420  n. This is a 2D 
-0001e140: 6d61 700a 2020 2020 7769 7468 2074 6865  map.    with the
-0001e150: 2061 6c74 6974 7564 6520 656d 6265 6464   altitude embedd
-0001e160: 6564 2061 7320 6060 277a 2760 6020 6365  ed as ``'z'`` ce
-0001e170: 6c6c 2064 6174 6120 7769 7468 696e 2074  ll data within t
-0001e180: 6865 0a20 2020 203a 636c 6173 733a 6070  he.    :class:`p
-0001e190: 7976 6973 7461 2e50 6f6c 7944 6174 6160  yvista.PolyData`
-0001e1a0: 2e0a 0a20 2020 204f 7269 6769 6e61 6c6c  ...    Originall
-0001e1b0: 7920 706f 7374 6564 2061 7420 6062 616e  y posted at `ban
-0001e1c0: 6573 756c 6c69 7661 6e2f 6461 6d61 7661  esullivan/damava
-0001e1d0: 6e64 2d76 6f6c 6361 6e6f 0a20 2020 203c  nd-volcano.    <
-0001e1e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0001e1f0: 6f6d 2f62 616e 6573 756c 6c69 7661 6e2f  om/banesullivan/
-0001e200: 6461 6d61 7661 6e64 2d76 6f6c 6361 6e6f  damavand-volcano
-0001e210: 3e60 5f2e 0a0a 2020 2020 5061 7261 6d65  >`_...    Parame
-0001e220: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0001e230: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-0001e240: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-0001e250: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-0001e260: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-0001e270: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-0001e280: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-0001e290: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-0001e2a0: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-0001e2b0: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-0001e2c0: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-0001e2d0: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-0001e2e0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0001e2f0: 2020 2020 7079 7669 7374 612e 506f 6c79      pyvista.Poly
-0001e300: 4461 7461 207c 2073 7472 0a20 2020 2020  Data | str.     
-0001e310: 2020 2044 6174 6153 6574 206f 7220 6669     DataSet or fi
-0001e320: 6c65 6e61 6d65 2064 6570 656e 6469 6e67  lename depending
-0001e330: 206f 6e20 6060 6c6f 6164 6060 2e0a 0a20   on ``load``... 
-0001e340: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-0001e350: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6f77  --------.    Dow
-0001e360: 6e6c 6f61 6420 7468 6520 4461 6d61 7661  nload the Damava
-0001e370: 6e64 2064 6174 6173 6574 2061 6e64 2070  nd dataset and p
-0001e380: 6c6f 7420 6974 2061 6674 6572 2077 6172  lot it after war
-0001e390: 7069 6e67 2069 7420 6279 2069 7473 2061  ping it by its a
-0001e3a0: 6c74 6974 7564 652e 0a0a 2020 2020 3e3e  ltitude...    >>
-0001e3b0: 3e20 6672 6f6d 2070 7976 6973 7461 2069  > from pyvista i
-0001e3c0: 6d70 6f72 7420 6578 616d 706c 6573 0a20  mport examples. 
-0001e3d0: 2020 203e 3e3e 2064 6174 6173 6574 203d     >>> dataset =
-0001e3e0: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
-0001e3f0: 6164 5f6d 6f75 6e74 5f64 616d 6176 616e  ad_mount_damavan
-0001e400: 6428 290a 2020 2020 3e3e 3e20 6461 7461  d().    >>> data
-0001e410: 7365 7420 3d20 6461 7461 7365 742e 6365  set = dataset.ce
-0001e420: 6c6c 5f64 6174 615f 746f 5f70 6f69 6e74  ll_data_to_point
-0001e430: 5f64 6174 6128 290a 2020 2020 3e3e 3e20  _data().    >>> 
-0001e440: 6461 7461 7365 7420 3d20 6461 7461 7365  dataset = datase
-0001e450: 742e 7761 7270 5f62 795f 7363 616c 6172  t.warp_by_scalar
-0001e460: 2827 7a27 2c20 6661 6374 6f72 3d32 290a  ('z', factor=2).
-0001e470: 2020 2020 3e3e 3e20 6461 7461 7365 742e      >>> dataset.
-0001e480: 706c 6f74 2863 6d61 703d 2767 6973 745f  plot(cmap='gist_
-0001e490: 6561 7274 6827 2c20 7368 6f77 5f73 6361  earth', show_sca
-0001e4a0: 6c61 725f 6261 723d 4661 6c73 6529 0a0a  lar_bar=False)..
-0001e4b0: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
-0001e4c0: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
-0001e4d0: 5f72 6561 6428 2741 4f49 2e44 616d 6176  _read('AOI.Damav
-0001e4e0: 616e 642e 3332 3633 392e 7674 7027 2c20  and.32639.vtp', 
-0001e4f0: 6c6f 6164 3d6c 6f61 6429 0a0a 0a64 6566  load=load)...def
-0001e500: 2064 6f77 6e6c 6f61 645f 7061 7274 6963   download_partic
-0001e510: 6c65 735f 6c65 7468 6528 6c6f 6164 3d54  les_lethe(load=T
-0001e520: 7275 6529 3a20 2023 2070 7261 676d 613a  rue):  # pragma:
-0001e530: 206e 6f20 636f 7665 720a 2020 2020 2222   no cover.    ""
-0001e540: 2244 6f77 6e6c 6f61 6420 6120 7061 7274  "Download a part
-0001e550: 6963 6c65 7320 6461 7461 7365 7420 6765  icles dataset ge
-0001e560: 6e65 7261 7465 6420 6279 2060 6c65 7468  nerated by `leth
-0001e570: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
-0001e580: 622e 636f 6d2f 6c65 7468 652d 6366 642f  b.com/lethe-cfd/
-0001e590: 6c65 7468 653e 605f 202e 0a0a 2020 2020  lethe>`_ ...    
-0001e5a0: 5365 6520 6050 7956 6973 7461 2064 6973  See `PyVista dis
-0001e5b0: 6375 7373 696f 6e73 2023 3139 3834 0a20  cussions #1984. 
-0001e5c0: 2020 203c 6874 7470 733a 2f2f 6769 7468     <https://gith
-0001e5d0: 7562 2e63 6f6d 2f70 7976 6973 7461 2f70  ub.com/pyvista/p
-0001e5e0: 7976 6973 7461 2f64 6973 6375 7373 696f  yvista/discussio
-0001e5f0: 6e73 2f31 3938 343e 605f 0a0a 2020 2020  ns/1984>`_..    
-0001e600: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-0001e610: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
-0001e620: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
-0001e630: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
-0001e640: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
-0001e650: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
-0001e660: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
-0001e670: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
-0001e680: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
-0001e690: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
-0001e6a0: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
-0001e6b0: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
-0001e6c0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-0001e6d0: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
-0001e6e0: 612e 556e 7374 7275 6374 7572 6564 4772  a.UnstructuredGr
-0001e6f0: 6964 207c 2073 7472 0a20 2020 2020 2020  id | str.       
-0001e700: 2044 6174 6153 6574 206f 7220 6669 6c65   DataSet or file
-0001e710: 6e61 6d65 2064 6570 656e 6469 6e67 206f  name depending o
-0001e720: 6e20 6060 6c6f 6164 6060 2e0a 0a20 2020  n ``load``...   
-0001e730: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
-0001e740: 2d2d 2d2d 2d2d 0a20 2020 2044 6f77 6e6c  ------.    Downl
-0001e750: 6f61 6420 7468 6520 7061 7274 6963 6c65  oad the particle
-0001e760: 7320 6461 7461 7365 7420 616e 6420 706c  s dataset and pl
-0001e770: 6f74 2069 7420 6166 7465 7220 6765 6e65  ot it after gene
-0001e780: 7261 7469 6e67 2067 6c79 7068 732e 0a0a  rating glyphs...
-0001e790: 2020 2020 3e3e 3e20 6672 6f6d 2070 7976      >>> from pyv
-0001e7a0: 6973 7461 2069 6d70 6f72 7420 6578 616d  ista import exam
-0001e7b0: 706c 6573 0a20 2020 203e 3e3e 2070 6172  ples.    >>> par
-0001e7c0: 7469 636c 6573 203d 2065 7861 6d70 6c65  ticles = example
-0001e7d0: 732e 646f 776e 6c6f 6164 5f70 6172 7469  s.download_parti
-0001e7e0: 636c 6573 5f6c 6574 6865 2829 0a20 2020  cles_lethe().   
-0001e7f0: 203e 3e3e 2070 6172 7469 636c 6573 2e70   >>> particles.p
-0001e800: 6c6f 7428 0a20 2020 202e 2e2e 2020 2020  lot(.    ...    
-0001e810: 2072 656e 6465 725f 706f 696e 7473 5f61   render_points_a
-0001e820: 735f 7370 6865 7265 733d 5472 7565 2c0a  s_spheres=True,.
-0001e830: 2020 2020 2e2e 2e20 2020 2020 7374 796c      ...     styl
-0001e840: 653d 2770 6f69 6e74 7327 2c0a 2020 2020  e='points',.    
-0001e850: 2e2e 2e20 2020 2020 7363 616c 6172 733d  ...     scalars=
-0001e860: 2756 656c 6f63 6974 7927 2c0a 2020 2020  'Velocity',.    
-0001e870: 2e2e 2e20 2020 2020 6261 636b 6772 6f75  ...     backgrou
-0001e880: 6e64 3d27 7727 2c0a 2020 2020 2e2e 2e20  nd='w',.    ... 
-0001e890: 2020 2020 7363 616c 6172 5f62 6172 5f61      scalar_bar_a
-0001e8a0: 7267 733d 7b27 636f 6c6f 7227 3a20 276b  rgs={'color': 'k
-0001e8b0: 277d 2c0a 2020 2020 2e2e 2e20 2020 2020  '},.    ...     
-0001e8c0: 636d 6170 3d27 6277 7227 2c0a 2020 2020  cmap='bwr',.    
-0001e8d0: 2e2e 2e20 290a 0a20 2020 2022 2222 0a20  ... )..    """. 
-0001e8e0: 2020 2072 6574 7572 6e20 5f64 6f77 6e6c     return _downl
-0001e8f0: 6f61 645f 616e 645f 7265 6164 2827 6c65  oad_and_read('le
-0001e900: 7468 652f 7265 7375 6c74 5f70 6172 7469  the/result_parti
-0001e910: 636c 6573 2e32 3030 3030 2e30 3030 302e  cles.20000.0000.
-0001e920: 7674 7527 2c20 6c6f 6164 3d6c 6f61 6429  vtu', load=load)
-0001e930: 0a0a 0a64 6566 2064 6f77 6e6c 6f61 645f  ...def download_
-0001e940: 6769 665f 7369 6d70 6c65 286c 6f61 643d  gif_simple(load=
-0001e950: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
-0001e960: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
-0001e970: 2222 446f 776e 6c6f 6164 2061 2073 696d  ""Download a sim
-0001e980: 706c 6520 7468 7265 6520 6672 616d 6520  ple three frame 
-0001e990: 4749 462e 0a0a 2020 2020 5061 7261 6d65  GIF...    Parame
-0001e9a0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0001e9b0: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-0001e9c0: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-0001e9d0: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-0001e9e0: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-0001e9f0: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-0001ea00: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-0001ea10: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-0001ea20: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-0001ea30: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-0001ea40: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-0001ea50: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-0001ea60: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0001ea70: 2020 2020 7079 7669 7374 612e 556e 6966      pyvista.Unif
-0001ea80: 6f72 6d47 7269 6420 7c20 7374 720a 2020  ormGrid | str.  
-0001ea90: 2020 2020 2020 4461 7461 5365 7420 6f72        DataSet or
-0001eaa0: 2066 696c 656e 616d 6520 6465 7065 6e64   filename depend
-0001eab0: 696e 6720 6f6e 2060 606c 6f61 6460 602e  ing on ``load``.
-0001eac0: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
-0001ead0: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-0001eae0: 446f 776e 6c6f 6164 2061 6e64 2070 6c6f  Download and plo
-0001eaf0: 7420 7468 6520 6669 7273 7420 6672 616d  t the first fram
-0001eb00: 6520 6f66 2061 2073 696d 706c 6520 4749  e of a simple GI
-0001eb10: 462e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  F...    >>> from
-0001eb20: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
-0001eb30: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
-0001eb40: 2067 7269 6420 3d20 6578 616d 706c 6573   grid = examples
-0001eb50: 2e64 6f77 6e6c 6f61 645f 6769 665f 7369  .download_gif_si
-0001eb60: 6d70 6c65 2829 0a20 2020 203e 3e3e 2067  mple().    >>> g
-0001eb70: 7269 642e 706c 6f74 280a 2020 2020 2e2e  rid.plot(.    ..
-0001eb80: 2e20 2020 2020 7363 616c 6172 733d 2766  .     scalars='f
-0001eb90: 7261 6d65 3027 2c0a 2020 2020 2e2e 2e20  rame0',.    ... 
-0001eba0: 2020 2020 7267 623d 5472 7565 2c0a 2020      rgb=True,.  
-0001ebb0: 2020 2e2e 2e20 2020 2020 6261 636b 6772    ...     backgr
-0001ebc0: 6f75 6e64 3d27 7727 2c0a 2020 2020 2e2e  ound='w',.    ..
-0001ebd0: 2e20 2020 2020 7368 6f77 5f73 6361 6c61  .     show_scala
-0001ebe0: 725f 6261 723d 4661 6c73 652c 0a20 2020  r_bar=False,.   
-0001ebf0: 202e 2e2e 2020 2020 2063 706f 733d 2778   ...     cpos='x
-0001ec00: 7927 2c0a 2020 2020 2e2e 2e20 290a 0a20  y',.    ... ).. 
-0001ec10: 2020 2050 6c6f 7420 7468 6520 7365 636f     Plot the seco
-0001ec20: 6e64 2066 7261 6d65 2e0a 0a20 2020 203e  nd frame...    >
-0001ec30: 3e3e 2067 7269 642e 706c 6f74 280a 2020  >> grid.plot(.  
-0001ec40: 2020 2e2e 2e20 2020 2020 7363 616c 6172    ...     scalar
-0001ec50: 733d 2766 7261 6d65 3127 2c0a 2020 2020  s='frame1',.    
-0001ec60: 2e2e 2e20 2020 2020 7267 623d 5472 7565  ...     rgb=True
-0001ec70: 2c0a 2020 2020 2e2e 2e20 2020 2020 6261  ,.    ...     ba
-0001ec80: 636b 6772 6f75 6e64 3d27 7727 2c0a 2020  ckground='w',.  
-0001ec90: 2020 2e2e 2e20 2020 2020 7368 6f77 5f73    ...     show_s
-0001eca0: 6361 6c61 725f 6261 723d 4661 6c73 652c  calar_bar=False,
-0001ecb0: 0a20 2020 202e 2e2e 2020 2020 2063 706f  .    ...     cpo
-0001ecc0: 733d 2778 7927 2c0a 2020 2020 2e2e 2e20  s='xy',.    ... 
-0001ecd0: 290a 0a20 2020 2022 2222 0a20 2020 2072  )..    """.    r
-0001ece0: 6574 7572 6e20 5f64 6f77 6e6c 6f61 645f  eturn _download_
-0001ecf0: 616e 645f 7265 6164 2827 6769 6673 2f73  and_read('gifs/s
-0001ed00: 616d 706c 652e 6769 6627 2c20 6c6f 6164  ample.gif', load
-0001ed10: 3d6c 6f61 6429 0a0a 0a64 6566 2064 6f77  =load)...def dow
-0001ed20: 6e6c 6f61 645f 636c 6f75 645f 6461 726b  nload_cloud_dark
-0001ed30: 5f6d 6174 7465 7228 6c6f 6164 3d54 7275  _matter(load=Tru
-0001ed40: 6529 3a20 2023 2070 7261 676d 613a 206e  e):  # pragma: n
-0001ed50: 6f20 636f 7665 720a 2020 2020 2222 2244  o cover.    """D
-0001ed60: 6f77 6e6c 6f61 6420 7061 7274 6963 6c65  ownload particle
-0001ed70: 7320 6672 6f6d 2061 2073 696d 756c 6174  s from a simulat
-0001ed80: 6564 2064 6172 6b20 6d61 7474 6572 2068  ed dark matter h
-0001ed90: 616c 6f2e 0a0a 2020 2020 5468 6973 2064  alo...    This d
-0001eda0: 6174 6173 6574 2063 6f6e 7461 696e 7320  ataset contains 
-0001edb0: 3332 2c33 3134 2070 6172 7469 636c 6573  32,314 particles
-0001edc0: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-0001edd0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-0001ede0: 0a20 2020 206c 6f61 6420 3a20 626f 6f6c  .    load : bool
-0001edf0: 2c20 6465 6661 756c 743a 2054 7275 650a  , default: True.
-0001ee00: 2020 2020 2020 2020 4c6f 6164 2074 6865          Load the
-0001ee10: 2064 6174 6173 6574 2061 6674 6572 2064   dataset after d
-0001ee20: 6f77 6e6c 6f61 6469 6e67 2069 7420 7768  ownloading it wh
-0001ee30: 656e 2060 6054 7275 6560 602e 2020 5365  en ``True``.  Se
-0001ee40: 7420 7468 6973 0a20 2020 2020 2020 2074  t this.        t
-0001ee50: 6f20 6060 4661 6c73 6560 6020 616e 6420  o ``False`` and 
-0001ee60: 6f6e 6c79 2074 6865 2066 696c 656e 616d  only the filenam
-0001ee70: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
-0001ee80: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
-0001ee90: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-0001eea0: 2070 7976 6973 7461 2e50 6f69 6e74 5365   pyvista.PointSe
-0001eeb0: 7420 7c20 7374 720a 2020 2020 2020 2020  t | str.        
-0001eec0: 4461 7461 5365 7420 6f72 2066 696c 656e  DataSet or filen
-0001eed0: 616d 6520 6465 7065 6e64 696e 6720 6f6e  ame depending on
-0001eee0: 2060 606c 6f61 6460 602e 0a0a 2020 2020   ``load``...    
-0001eef0: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
-0001ef00: 2d2d 2d2d 2d0a 2020 2020 446f 776e 6c6f  -----.    Downlo
-0001ef10: 6164 2074 6865 2064 6172 6b20 6d61 7474  ad the dark matt
-0001ef20: 6572 2063 6c6f 7564 2061 6e64 2064 6973  er cloud and dis
-0001ef30: 706c 6179 2069 7473 2072 6570 7265 7365  play its represe
-0001ef40: 6e74 6174 696f 6e2e 0a0a 2020 2020 3e3e  ntation...    >>
-0001ef50: 3e20 696d 706f 7274 206e 756d 7079 2061  > import numpy a
-0001ef60: 7320 6e70 0a20 2020 203e 3e3e 2066 726f  s np.    >>> fro
-0001ef70: 6d20 7079 7669 7374 6120 696d 706f 7274  m pyvista import
-0001ef80: 2065 7861 6d70 6c65 730a 2020 2020 3e3e   examples.    >>
-0001ef90: 3e20 7063 203d 2065 7861 6d70 6c65 732e  > pc = examples.
-0001efa0: 646f 776e 6c6f 6164 5f63 6c6f 7564 5f64  download_cloud_d
-0001efb0: 6172 6b5f 6d61 7474 6572 2829 0a20 2020  ark_matter().   
-0001efc0: 203e 3e3e 2070 6320 2023 2064 6f63 7465   >>> pc  # docte
-0001efd0: 7374 3a2b 534b 4950 0a20 2020 2050 6f69  st:+SKIP.    Poi
-0001efe0: 6e74 5365 7420 2830 7837 6639 3766 3731  ntSet (0x7f97f71
-0001eff0: 3864 3436 3029 0a20 2020 2020 204e 2043  8d460).      N C
-0001f000: 656c 6c73 3a20 2020 2020 2030 0a20 2020  ells:      0.   
-0001f010: 2020 204e 2050 6f69 6e74 733a 2020 2020     N Points:    
-0001f020: 2033 3233 3134 0a20 2020 2020 2058 2042   32314.      X B
-0001f030: 6f75 6e64 733a 2020 2020 2037 2e34 3531  ounds:     7.451
-0001f040: 652b 3031 2c20 372e 3839 3265 2b30 310a  e+01, 7.892e+01.
-0001f050: 2020 2020 2020 5920 426f 756e 6473 3a20        Y Bounds: 
-0001f060: 2020 2020 312e 3631 3665 2b30 312c 2032      1.616e+01, 2
-0001f070: 2e32 3735 652b 3031 0a20 2020 2020 205a  .275e+01.      Z
-0001f080: 2042 6f75 6e64 733a 2020 2020 2038 2e39   Bounds:     8.9
-0001f090: 3030 652b 3031 2c20 392e 3331 3965 2b30  00e+01, 9.319e+0
-0001f0a0: 310a 2020 2020 2020 4e20 4172 7261 7973  1.      N Arrays
-0001f0b0: 3a20 2020 2020 300a 0a20 2020 2050 6c6f  :     0..    Plo
-0001f0c0: 7420 7468 6520 706f 696e 7420 636c 6f75  t the point clou
-0001f0d0: 642e 2043 6f6c 6f72 2062 6173 6564 206f  d. Color based o
-0001f0e0: 6e20 7468 6520 6469 7374 616e 6365 2066  n the distance f
-0001f0f0: 726f 6d20 7468 6520 6365 6e74 6572 206f  rom the center o
-0001f100: 6620 7468 650a 2020 2020 636c 6f75 642e  f the.    cloud.
-0001f110: 0a0a 2020 2020 3e3e 3e20 7063 2e70 6c6f  ..    >>> pc.plo
-0001f120: 7428 0a20 2020 202e 2e2e 2020 2020 2073  t(.    ...     s
-0001f130: 6361 6c61 7273 3d6e 702e 6c69 6e61 6c67  calars=np.linalg
-0001f140: 2e6e 6f72 6d28 7063 2e70 6f69 6e74 7320  .norm(pc.points 
-0001f150: 2d20 7063 2e63 656e 7465 722c 2061 7869  - pc.center, axi
-0001f160: 733d 3129 2c0a 2020 2020 2e2e 2e20 2020  s=1),.    ...   
-0001f170: 2020 7374 796c 653d 2770 6f69 6e74 735f    style='points_
-0001f180: 6761 7573 7369 616e 272c 0a20 2020 202e  gaussian',.    .
-0001f190: 2e2e 2020 2020 206f 7061 6369 7479 3d30  ..     opacity=0
-0001f1a0: 2e35 2c0a 2020 2020 2e2e 2e20 2020 2020  .5,.    ...     
-0001f1b0: 706f 696e 745f 7369 7a65 3d31 2e35 2c0a  point_size=1.5,.
-0001f1c0: 2020 2020 2e2e 2e20 2020 2020 7368 6f77      ...     show
-0001f1d0: 5f73 6361 6c61 725f 6261 723d 4661 6c73  _scalar_bar=Fals
-0001f1e0: 652c 0a20 2020 202e 2e2e 2020 2020 207a  e,.    ...     z
-0001f1f0: 6f6f 6d3d 322c 0a20 2020 202e 2e2e 2029  oom=2,.    ... )
-0001f200: 0a0a 2020 2020 5365 6520 7468 6520 3a72  ..    See the :r
-0001f210: 6566 3a60 706c 6f74 7469 6e67 5f70 6f69  ef:`plotting_poi
-0001f220: 6e74 5f63 6c6f 7564 7360 2066 6f72 2061  nt_clouds` for a
-0001f230: 2066 756c 6c20 6578 616d 706c 6520 7573   full example us
-0001f240: 696e 6720 7468 6973 2064 6174 6173 6574  ing this dataset
-0001f250: 2e0a 0a20 2020 2022 2222 0a20 2020 2066  ...    """.    f
-0001f260: 696c 656e 616d 6520 3d20 646f 776e 6c6f  ilename = downlo
-0001f270: 6164 5f66 696c 6528 2770 6f69 6e74 2d63  ad_file('point-c
-0001f280: 6c6f 7564 732f 6669 6e64 7573 3233 2f68  louds/findus23/h
-0001f290: 616c 6f5f 6c6f 775f 7265 732e 6e70 7927  alo_low_res.npy'
-0001f2a0: 290a 0a20 2020 2069 6620 6c6f 6164 3a0a  )..    if load:.
-0001f2b0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-0001f2c0: 7976 6973 7461 2e50 6f69 6e74 5365 7428  yvista.PointSet(
-0001f2d0: 6e70 2e6c 6f61 6428 6669 6c65 6e61 6d65  np.load(filename
-0001f2e0: 2929 0a20 2020 2072 6574 7572 6e20 6669  )).    return fi
-0001f2f0: 6c65 6e61 6d65 0a0a 0a64 6566 2064 6f77  lename...def dow
-0001f300: 6e6c 6f61 645f 636c 6f75 645f 6461 726b  nload_cloud_dark
-0001f310: 5f6d 6174 7465 725f 6465 6e73 6528 6c6f  _matter_dense(lo
-0001f320: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
-0001f330: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-0001f340: 2020 2222 2244 6f77 6e6c 6f61 6420 6120    """Download a 
-0001f350: 7061 7274 6963 6c65 7320 6672 6f6d 2061  particles from a
-0001f360: 2073 696d 756c 6174 6564 2064 6172 6b20   simulated dark 
-0001f370: 6d61 7474 6572 2068 616c 6f2e 0a0a 2020  matter halo...  
-0001f380: 2020 5468 6973 2064 6174 6173 6574 2063    This dataset c
-0001f390: 6f6e 7461 696e 7320 322c 3036 322c 3235  ontains 2,062,25
-0001f3a0: 3620 7061 7274 6963 6c65 732e 0a0a 2020  6 particles...  
-0001f3b0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0001f3c0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0001f3d0: 6c6f 6164 203a 2062 6f6f 6c2c 2064 6566  load : bool, def
-0001f3e0: 6175 6c74 3a20 5472 7565 0a20 2020 2020  ault: True.     
-0001f3f0: 2020 204c 6f61 6420 7468 6520 6461 7461     Load the data
-0001f400: 7365 7420 6166 7465 7220 646f 776e 6c6f  set after downlo
-0001f410: 6164 696e 6720 6974 2077 6865 6e20 6060  ading it when ``
-0001f420: 5472 7565 6060 2e20 2053 6574 2074 6869  True``.  Set thi
-0001f430: 730a 2020 2020 2020 2020 746f 2060 6046  s.        to ``F
-0001f440: 616c 7365 6060 2061 6e64 206f 6e6c 7920  alse`` and only 
-0001f450: 7468 6520 6669 6c65 6e61 6d65 2077 696c  the filename wil
-0001f460: 6c20 6265 2072 6574 7572 6e65 642e 0a0a  l be returned...
-0001f470: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0001f480: 2d2d 2d2d 2d2d 2d0a 2020 2020 7079 7669  -------.    pyvi
-0001f490: 7374 612e 506f 696e 7453 6574 207c 2073  sta.PointSet | s
-0001f4a0: 7472 0a20 2020 2020 2020 2044 6174 6153  tr.        DataS
-0001f4b0: 6574 206f 7220 6669 6c65 6e61 6d65 2064  et or filename d
-0001f4c0: 6570 656e 6469 6e67 206f 6e20 6060 6c6f  epending on ``lo
-0001f4d0: 6164 6060 2e0a 0a20 2020 2045 7861 6d70  ad``...    Examp
-0001f4e0: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-0001f4f0: 0a20 2020 2044 6f77 6e6c 6f61 6420 7468  .    Download th
-0001f500: 6520 6461 726b 206d 6174 7465 7220 636c  e dark matter cl
-0001f510: 6f75 6420 616e 6420 6469 7370 6c61 7920  oud and display 
-0001f520: 6974 7320 7265 7072 6573 656e 7461 7469  its representati
-0001f530: 6f6e 2e0a 0a20 2020 203e 3e3e 2069 6d70  on...    >>> imp
-0001f540: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-0001f550: 2020 2020 3e3e 3e20 6672 6f6d 2070 7976      >>> from pyv
-0001f560: 6973 7461 2069 6d70 6f72 7420 6578 616d  ista import exam
-0001f570: 706c 6573 0a20 2020 203e 3e3e 2070 6320  ples.    >>> pc 
-0001f580: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
-0001f590: 6f61 645f 636c 6f75 645f 6461 726b 5f6d  oad_cloud_dark_m
-0001f5a0: 6174 7465 725f 6465 6e73 6528 290a 2020  atter_dense().  
-0001f5b0: 2020 3e3e 3e20 7063 2020 2320 646f 6374    >>> pc  # doct
-0001f5c0: 6573 743a 2b53 4b49 500a 2020 2020 506f  est:+SKIP.    Po
-0001f5d0: 696e 7453 6574 2028 3078 3766 6437 3934  intSet (0x7fd794
-0001f5e0: 3933 6133 3430 290a 2020 2020 4e20 4365  93a340).    N Ce
-0001f5f0: 6c6c 733a 2020 2020 2020 300a 2020 2020  lls:      0.    
-0001f600: 4e20 506f 696e 7473 3a20 2020 2020 3230  N Points:     20
-0001f610: 3632 3235 360a 2020 2020 5820 426f 756e  62256.    X Boun
-0001f620: 6473 3a20 2020 2020 372e 3436 3265 2b30  ds:     7.462e+0
-0001f630: 312c 2037 2e38 3633 652b 3031 0a20 2020  1, 7.863e+01.   
-0001f640: 2059 2042 6f75 6e64 733a 2020 2020 2031   Y Bounds:     1
-0001f650: 2e36 3034 652b 3031 2c20 322e 3234 3465  .604e+01, 2.244e
-0001f660: 2b30 310a 2020 2020 5a20 426f 756e 6473  +01.    Z Bounds
-0001f670: 3a20 2020 2020 382e 3839 3365 2b30 312c  :     8.893e+01,
-0001f680: 2039 2e33 3337 652b 3031 0a20 2020 204e   9.337e+01.    N
-0001f690: 2041 7272 6179 733a 2020 2020 2030 0a0a   Arrays:     0..
-0001f6a0: 2020 2020 506c 6f74 2074 6865 2070 6f69      Plot the poi
-0001f6b0: 6e74 2063 6c6f 7564 2e20 436f 6c6f 7220  nt cloud. Color 
-0001f6c0: 6261 7365 6420 6f6e 2074 6865 2064 6973  based on the dis
-0001f6d0: 7461 6e63 6520 6672 6f6d 2074 6865 2063  tance from the c
-0001f6e0: 656e 7465 7220 6f66 2074 6865 0a20 2020  enter of the.   
-0001f6f0: 2063 6c6f 7564 2e0a 0a20 2020 203e 3e3e   cloud...    >>>
-0001f700: 2070 632e 706c 6f74 280a 2020 2020 2e2e   pc.plot(.    ..
-0001f710: 2e20 2020 2020 7363 616c 6172 733d 6e70  .     scalars=np
-0001f720: 2e6c 696e 616c 672e 6e6f 726d 2870 632e  .linalg.norm(pc.
-0001f730: 706f 696e 7473 202d 2070 632e 6365 6e74  points - pc.cent
-0001f740: 6572 2c20 6178 6973 3d31 292c 0a20 2020  er, axis=1),.   
-0001f750: 202e 2e2e 2020 2020 2073 7479 6c65 3d27   ...     style='
-0001f760: 706f 696e 7473 5f67 6175 7373 6961 6e27  points_gaussian'
-0001f770: 2c0a 2020 2020 2e2e 2e20 2020 2020 6f70  ,.    ...     op
-0001f780: 6163 6974 793d 302e 3033 302c 0a20 2020  acity=0.030,.   
-0001f790: 202e 2e2e 2020 2020 2070 6f69 6e74 5f73   ...     point_s
-0001f7a0: 697a 653d 322e 302c 0a20 2020 202e 2e2e  ize=2.0,.    ...
-0001f7b0: 2020 2020 2073 686f 775f 7363 616c 6172       show_scalar
-0001f7c0: 5f62 6172 3d46 616c 7365 2c0a 2020 2020  _bar=False,.    
-0001f7d0: 2e2e 2e20 2020 2020 7a6f 6f6d 3d32 2c0a  ...     zoom=2,.
-0001f7e0: 2020 2020 2e2e 2e20 290a 0a20 2020 2053      ... )..    S
-0001f7f0: 6565 2074 6865 203a 7265 663a 6070 6c6f  ee the :ref:`plo
-0001f800: 7474 696e 675f 706f 696e 745f 636c 6f75  tting_point_clou
-0001f810: 6473 6020 666f 7220 6d6f 7265 2064 6574  ds` for more det
-0001f820: 6169 6c73 206f 6e20 686f 7720 746f 2070  ails on how to p
-0001f830: 6c6f 7420 706f 696e 740a 2020 2020 636c  lot point.    cl
-0001f840: 6f75 6473 2e0a 0a20 2020 2022 2222 0a20  ouds...    """. 
-0001f850: 2020 2066 696c 656e 616d 6520 3d20 646f     filename = do
-0001f860: 776e 6c6f 6164 5f66 696c 6528 2770 6f69  wnload_file('poi
-0001f870: 6e74 2d63 6c6f 7564 732f 6669 6e64 7573  nt-clouds/findus
-0001f880: 3233 2f68 616c 6f5f 6869 6768 5f72 6573  23/halo_high_res
-0001f890: 2e6e 7079 2729 0a0a 2020 2020 6966 206c  .npy')..    if l
-0001f8a0: 6f61 643a 0a20 2020 2020 2020 2072 6574  oad:.        ret
-0001f8b0: 7572 6e20 7079 7669 7374 612e 506f 696e  urn pyvista.Poin
-0001f8c0: 7453 6574 286e 702e 6c6f 6164 2866 696c  tSet(np.load(fil
-0001f8d0: 656e 616d 6529 290a 2020 2020 7265 7475  ename)).    retu
-0001f8e0: 726e 2066 696c 656e 616d 650a 0a0a 6465  rn filename...de
-0001f8f0: 6620 646f 776e 6c6f 6164 5f73 7461 7273  f download_stars
-0001f900: 5f63 6c6f 7564 5f68 7967 286c 6f61 643d  _cloud_hyg(load=
-0001f910: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
-0001f920: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
-0001f930: 2222 446f 776e 6c6f 6164 2061 2070 6f69  ""Download a poi
-0001f940: 6e74 2063 6c6f 7564 206f 6620 7374 6172  nt cloud of star
-0001f950: 7320 6173 2063 6f6d 7075 7465 6420 6279  s as computed by
-0001f960: 2074 6865 2048 5947 2044 6174 6162 6173   the HYG Databas
-0001f970: 652e 0a0a 2020 2020 5365 6520 6048 5947  e...    See `HYG
-0001f980: 2d44 6174 6162 6173 6520 3c68 7474 7073  -Database <https
-0001f990: 3a2f 2f67 6974 6875 622e 636f 6d2f 6173  ://github.com/as
-0001f9a0: 7472 6f6e 6578 7573 2f48 5947 2d44 6174  tronexus/HYG-Dat
-0001f9b0: 6162 6173 653e 605f 2066 6f72 206d 6f72  abase>`_ for mor
-0001f9c0: 650a 2020 2020 6465 7461 696c 732e 0a0a  e.    details...
-0001f9d0: 2020 2020 5468 6973 2064 6174 6120 7365      This data se
-0001f9e0: 7420 6973 206c 6963 656e 7365 6420 6279  t is licensed by
-0001f9f0: 2061 2043 7265 6174 6976 6520 436f 6d6d   a Creative Comm
-0001fa00: 6f6e 7320 4174 7472 6962 7574 696f 6e2d  ons Attribution-
-0001fa10: 5368 6172 6541 6c69 6b65 0a20 2020 206c  ShareAlike.    l
-0001fa20: 6963 656e 7365 2e20 466f 7220 6d6f 7265  icense. For more
-0001fa30: 2064 6574 6169 6c73 2c20 7265 6164 2074   details, read t
-0001fa40: 6865 2060 4372 6561 7469 7665 2043 6f6d  he `Creative Com
-0001fa50: 6d6f 6e73 2070 6167 650a 2020 2020 3c68  mons page.    <h
-0001fa60: 7474 7073 3a2f 2f63 7265 6174 6976 6563  ttps://creativec
-0001fa70: 6f6d 6d6f 6e73 2e6f 7267 2f6c 6963 656e  ommons.org/licen
-0001fa80: 7365 732f 6279 2d73 612f 322e 352f 3e60  ses/by-sa/2.5/>`
-0001fa90: 5f0a 0a20 2020 2053 6565 2074 6865 2060  _..    See the `
-0001faa0: 5245 4144 4d45 2e6d 640a 2020 2020 3c68  README.md.    <h
-0001fab0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0001fac0: 6d2f 7079 7669 7374 612f 7674 6b2d 6461  m/pyvista/vtk-da
-0001fad0: 7461 2f62 6c6f 622f 6d61 7374 6572 2f44  ta/blob/master/D
-0001fae0: 6174 612f 706f 696e 742d 636c 6f75 6473  ata/point-clouds
-0001faf0: 2f68 7967 2d64 6174 6162 6173 652f 5245  /hyg-database/RE
-0001fb00: 4144 4d45 2e6d 643e 605f 0a20 2020 2066  ADME.md>`_.    f
-0001fb10: 6f72 206d 6f72 6520 6465 7461 696c 7320  or more details 
-0001fb20: 666f 7220 686f 7720 7468 6520 7374 6172  for how the star
-0001fb30: 2063 6f6c 6f72 7320 7765 7265 2063 6f6d   colors were com
-0001fb40: 7075 7465 642e 0a0a 2020 2020 4469 7374  puted...    Dist
-0001fb50: 616e 6365 7320 6172 6520 696e 2070 6172  ances are in par
-0001fb60: 7365 6373 2066 726f 6d20 4561 7274 682e  secs from Earth.
-0001fb70: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-0001fb80: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0001fb90: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
-0001fba0: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
-0001fbb0: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
-0001fbc0: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
-0001fbd0: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
-0001fbe0: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
-0001fbf0: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
-0001fc00: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
-0001fc10: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
-0001fc20: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
-0001fc30: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
-0001fc40: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0001fc50: 7079 7669 7374 612e 506f 6c79 4461 7461  pyvista.PolyData
-0001fc60: 207c 2073 7472 0a20 2020 2020 2020 2044   | str.        D
-0001fc70: 6174 6153 6574 206f 7220 6669 6c65 6e61  ataSet or filena
-0001fc80: 6d65 2064 6570 656e 6469 6e67 206f 6e20  me depending on 
-0001fc90: 6060 6c6f 6164 6060 2e0a 0a20 2020 2045  ``load``...    E
-0001fca0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-0001fcb0: 2d2d 2d2d 0a20 2020 2044 6f77 6e6c 6f61  ----.    Downloa
-0001fcc0: 6420 616e 6420 706c 6f74 2061 2070 6f69  d and plot a poi
-0001fcd0: 6e74 2063 6c6f 7564 206f 6620 7374 6172  nt cloud of star
-0001fce0: 7320 7769 7468 696e 2033 2c30 3030 206c  s within 3,000 l
-0001fcf0: 6967 6874 2079 6561 7273 2e20 5374 6172  ight years. Star
-0001fd00: 730a 2020 2020 6172 6520 636f 6c6f 7265  s.    are colore
-0001fd10: 6420 6163 636f 7264 696e 6720 746f 2074  d according to t
-0001fd20: 6865 6972 2052 4742 4120 636f 6c6f 7273  heir RGBA colors
-0001fd30: 2e0a 0a20 2020 203e 3e3e 2069 6d70 6f72  ...    >>> impor
-0001fd40: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
-0001fd50: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
-0001fd60: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
-0001fd70: 6573 0a20 2020 203e 3e3e 2073 7461 7273  es.    >>> stars
-0001fd80: 203d 2065 7861 6d70 6c65 732e 646f 776e   = examples.down
-0001fd90: 6c6f 6164 5f73 7461 7273 5f63 6c6f 7564  load_stars_cloud
-0001fda0: 5f68 7967 2829 0a20 2020 203e 3e3e 2073  _hyg().    >>> s
-0001fdb0: 7461 7273 2e70 6c6f 7428 0a20 2020 202e  tars.plot(.    .
-0001fdc0: 2e2e 2020 2020 2073 7479 6c65 3d27 706f  ..     style='po
-0001fdd0: 696e 7473 5f67 6175 7373 6961 6e27 2c0a  ints_gaussian',.
-0001fde0: 2020 2020 2e2e 2e20 2020 2020 6261 636b      ...     back
-0001fdf0: 6772 6f75 6e64 3d27 6b27 2c0a 2020 2020  ground='k',.    
-0001fe00: 2e2e 2e20 2020 2020 706f 696e 745f 7369  ...     point_si
-0001fe10: 7a65 3d30 2e35 2c0a 2020 2020 2e2e 2e20  ze=0.5,.    ... 
-0001fe20: 2020 2020 7363 616c 6172 733d 275f 7267      scalars='_rg
-0001fe30: 6261 272c 0a20 2020 202e 2e2e 2020 2020  ba',.    ...    
-0001fe40: 2072 656e 6465 725f 706f 696e 7473 5f61   render_points_a
-0001fe50: 735f 7370 6865 7265 733d 4661 6c73 652c  s_spheres=False,
-0001fe60: 0a20 2020 202e 2e2e 2020 2020 207a 6f6f  .    ...     zoo
-0001fe70: 6d3d 332e 302c 0a20 2020 202e 2e2e 2029  m=3.0,.    ... )
-0001fe80: 0a0a 2020 2020 3e3e 3e20 7374 6172 7320  ..    >>> stars 
-0001fe90: 2023 2064 6f63 7465 7374 3a2b 534b 4950   # doctest:+SKIP
-0001fea0: 0a20 2020 2050 6f6c 7944 6174 6120 2830  .    PolyData (0
-0001feb0: 7837 6665 3538 3531 6163 3061 3029 0a20  x7fe5851ac0a0). 
-0001fec0: 2020 2020 204e 2043 656c 6c73 3a20 2020       N Cells:   
-0001fed0: 2020 2031 3037 3835 370a 2020 2020 2020     107857.      
-0001fee0: 4e20 506f 696e 7473 3a20 2020 2020 3130  N Points:     10
-0001fef0: 3738 3537 0a20 2020 2020 204e 2053 7472  7857.      N Str
-0001ff00: 6970 733a 2020 2020 2030 0a20 2020 2020  ips:     0.     
-0001ff10: 2058 2042 6f75 6e64 733a 2020 2020 202d   X Bounds:     -
-0001ff20: 392e 3735 3565 2b30 322c 2039 2e37 3734  9.755e+02, 9.774
-0001ff30: 652b 3032 0a20 2020 2020 2059 2042 6f75  e+02.      Y Bou
-0001ff40: 6e64 733a 2020 2020 202d 392e 3632 3065  nds:     -9.620e
-0001ff50: 2b30 322c 2039 2e36 3632 652b 3032 0a20  +02, 9.662e+02. 
-0001ff60: 2020 2020 205a 2042 6f75 6e64 733a 2020       Z Bounds:  
-0001ff70: 2020 202d 392e 3738 3865 2b30 322c 2039     -9.788e+02, 9
-0001ff80: 2e37 3032 652b 3032 0a20 2020 2020 204e  .702e+02.      N
-0001ff90: 2041 7272 6179 733a 2020 2020 2034 0a0a   Arrays:     4..
-0001ffa0: 2020 2020 5365 6520 7468 6520 3a72 6566      See the :ref
-0001ffb0: 3a60 706c 6f74 7469 6e67 5f70 6f69 6e74  :`plotting_point
-0001ffc0: 5f63 6c6f 7564 7360 2066 6f72 206d 6f72  _clouds` for mor
-0001ffd0: 6520 6465 7461 696c 7320 6f6e 2068 6f77  e details on how
-0001ffe0: 2074 6f20 706c 6f74 2070 6f69 6e74 0a20   to plot point. 
-0001fff0: 2020 2063 6c6f 7564 732e 0a0a 2020 2020     clouds...    
-00020000: 2222 220a 2020 2020 7265 7475 726e 205f  """.    return _
-00020010: 646f 776e 6c6f 6164 5f61 6e64 5f72 6561  download_and_rea
-00020020: 6428 2770 6f69 6e74 2d63 6c6f 7564 732f  d('point-clouds/
-00020030: 6879 672d 6461 7461 6261 7365 2f73 7461  hyg-database/sta
-00020040: 7273 2e76 7470 272c 206c 6f61 643d 6c6f  rs.vtp', load=lo
-00020050: 6164 290a 0a0a 6465 6620 646f 776e 6c6f  ad)...def downlo
-00020060: 6164 5f66 6561 5f62 7261 636b 6574 286c  ad_fea_bracket(l
-00020070: 6f61 643d 5472 7565 293a 2020 2320 7072  oad=True):  # pr
-00020080: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
-00020090: 2020 2022 2222 446f 776e 6c6f 6164 2074     """Download t
-000200a0: 6865 2066 696e 6974 6520 656c 656d 656e  he finite elemen
-000200b0: 7420 736f 6c75 7469 6f6e 206f 6620 6120  t solution of a 
-000200c0: 6272 6163 6b65 742e 0a0a 2020 2020 436f  bracket...    Co
-000200d0: 6e74 6169 6e73 2076 6f6e 2d6d 6973 6573  ntains von-mises
-000200e0: 2065 7175 6976 616c 656e 7420 6365 6c6c   equivalent cell
-000200f0: 2073 7472 6573 7320 6173 7375 6d69 6e67   stress assuming
-00020100: 2061 2076 6572 7469 6361 6c20 2879 2d61   a vertical (y-a
-00020110: 7869 7329 206c 6f61 642e 0a0a 2020 2020  xis) load...    
-00020120: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00020130: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
-00020140: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
-00020150: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
-00020160: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
-00020170: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
-00020180: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
-00020190: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
-000201a0: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
-000201b0: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
-000201c0: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
-000201d0: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
-000201e0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-000201f0: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
-00020200: 612e 556e 7374 7275 6374 7572 6564 4772  a.UnstructuredGr
-00020210: 6964 207c 2073 7472 0a20 2020 2020 2020  id | str.       
-00020220: 2044 6174 6153 6574 206f 7220 6669 6c65   DataSet or file
-00020230: 6e61 6d65 2064 6570 656e 6469 6e67 206f  name depending o
-00020240: 6e20 6060 6c6f 6164 6060 2e0a 0a20 2020  n ``load``...   
-00020250: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
-00020260: 2d2d 2d2d 2d2d 0a20 2020 2044 6f77 6e6c  ------.    Downl
-00020270: 6f61 6420 616e 6420 706c 6f74 2065 7175  oad and plot equ
-00020280: 6976 616c 656e 7420 6365 6c6c 2073 7472  ivalent cell str
-00020290: 6573 732e 0a0a 2020 2020 3e3e 3e20 6672  ess...    >>> fr
-000202a0: 6f6d 2070 7976 6973 7461 2069 6d70 6f72  om pyvista impor
-000202b0: 7420 6578 616d 706c 6573 0a20 2020 203e  t examples.    >
-000202c0: 3e3e 2067 7269 6420 3d20 6578 616d 706c  >> grid = exampl
-000202d0: 6573 2e64 6f77 6e6c 6f61 645f 6665 615f  es.download_fea_
-000202e0: 6272 6163 6b65 7428 290a 2020 2020 3e3e  bracket().    >>
-000202f0: 3e20 6772 6964 2e70 6c6f 7428 290a 0a20  > grid.plot().. 
-00020300: 2020 2050 6c6f 7420 7468 6520 706f 696e     Plot the poin
-00020310: 7420 7374 7265 7373 2075 7369 6e67 2074  t stress using t
-00020320: 6865 2060 6027 6a65 7427 6060 2063 6f6c  he ``'jet'`` col
-00020330: 6f72 206d 6170 2e20 436f 6e76 6572 7420  or map. Convert 
-00020340: 7468 6520 6365 6c6c 2064 6174 610a 2020  the cell data.  
-00020350: 2020 746f 2070 6f69 6e74 2064 6174 612e    to point data.
-00020360: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2070  ..    >>> from p
-00020370: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
-00020380: 616d 706c 6573 0a20 2020 203e 3e3e 2067  amples.    >>> g
-00020390: 7269 6420 3d20 6578 616d 706c 6573 2e64  rid = examples.d
-000203a0: 6f77 6e6c 6f61 645f 6665 615f 6272 6163  ownload_fea_brac
-000203b0: 6b65 7428 290a 2020 2020 3e3e 3e20 6772  ket().    >>> gr
-000203c0: 6964 203d 2067 7269 642e 6365 6c6c 5f64  id = grid.cell_d
-000203d0: 6174 615f 746f 5f70 6f69 6e74 5f64 6174  ata_to_point_dat
-000203e0: 6128 290a 2020 2020 3e3e 3e20 6772 6964  a().    >>> grid
-000203f0: 2e70 6c6f 7428 736d 6f6f 7468 5f73 6861  .plot(smooth_sha
-00020400: 6469 6e67 3d54 7275 652c 2073 706c 6974  ding=True, split
-00020410: 5f73 6861 7270 5f65 6467 6573 3d54 7275  _sharp_edges=Tru
-00020420: 652c 2063 6d61 703d 276a 6574 2729 0a0a  e, cmap='jet')..
-00020430: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
-00020440: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
-00020450: 5f72 6561 6428 2766 6561 2f6b 6965 6665  _read('fea/kiefe
-00020460: 722f 6461 7461 7365 742e 7674 7527 2c20  r/dataset.vtu', 
-00020470: 6c6f 6164 3d6c 6f61 6429 0a0a 0a64 6566  load=load)...def
-00020480: 2064 6f77 6e6c 6f61 645f 6665 615f 6865   download_fea_he
-00020490: 7274 7a69 616e 5f63 6f6e 7461 6374 5f63  rtzian_contact_c
-000204a0: 796c 696e 6465 7228 6c6f 6164 3d54 7275  ylinder(load=Tru
-000204b0: 6529 3a20 2023 2070 7261 676d 613a 206e  e):  # pragma: n
-000204c0: 6f20 636f 7665 720a 2020 2020 2222 2244  o cover.    """D
-000204d0: 6f77 6e6c 6f61 6420 6120 6865 7274 7a69  ownload a hertzi
-000204e0: 616e 2063 6f6e 7461 6374 2066 696e 6974  an contact finit
-000204f0: 6520 656c 656d 656e 7420 736f 6c75 7469  e element soluti
-00020500: 6f6e 2e0a 0a20 2020 2048 6572 747a 6961  on...    Hertzia
-00020510: 6e20 636f 6e74 6163 7420 6973 2072 6566  n contact is ref
-00020520: 6572 7265 6420 746f 2074 6865 2066 7269  erred to the fri
-00020530: 6374 696f 6e6c 6573 7320 636f 6e74 6163  ctionless contac
-00020540: 7420 6265 7477 6565 6e20 7477 6f0a 2020  t between two.  
-00020550: 2020 626f 6469 6573 2e20 5370 6865 7269    bodies. Spheri
-00020560: 6361 6c20 636f 6e74 6163 7420 6973 2061  cal contact is a
-00020570: 2073 7065 6369 616c 2063 6173 6520 6f66   special case of
-00020580: 2074 6865 2048 6572 747a 2063 6f6e 7461   the Hertz conta
-00020590: 6374 2c20 7768 6963 6820 6973 0a20 2020  ct, which is.   
-000205a0: 2062 6574 7765 656e 2074 776f 2073 7068   between two sph
-000205b0: 6572 6573 2c20 6f72 2061 7320 696e 2074  eres, or as in t
-000205c0: 6865 2063 6173 6520 6f66 2074 6869 7320  he case of this 
-000205d0: 6461 7461 7365 742c 2062 6574 7765 656e  dataset, between
-000205e0: 2061 2073 7068 6572 650a 2020 2020 616e   a sphere.    an
-000205f0: 6420 7468 6520 7375 7266 6163 6520 6f66  d the surface of
-00020600: 2061 2068 616c 6620 7370 6163 6520 2866   a half space (f
-00020610: 6c61 7420 706c 616e 6529 2e0a 0a20 2020  lat plane)...   
-00020620: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00020630: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c  ----------.    l
-00020640: 6f61 6420 3a20 626f 6f6c 2c20 6465 6661  oad : bool, defa
-00020650: 756c 743a 2054 7275 650a 2020 2020 2020  ult: True.      
-00020660: 2020 4c6f 6164 2074 6865 2064 6174 6173    Load the datas
-00020670: 6574 2061 6674 6572 2064 6f77 6e6c 6f61  et after downloa
-00020680: 6469 6e67 2069 7420 7768 656e 2060 6054  ding it when ``T
-00020690: 7275 6560 602e 2020 5365 7420 7468 6973  rue``.  Set this
-000206a0: 0a20 2020 2020 2020 2074 6f20 6060 4661  .        to ``Fa
-000206b0: 6c73 6560 6020 616e 6420 6f6e 6c79 2074  lse`` and only t
-000206c0: 6865 2066 696c 656e 616d 6520 7769 6c6c  he filename will
-000206d0: 2062 6520 7265 7475 726e 6564 2e0a 0a20   be returned... 
-000206e0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-000206f0: 2d2d 2d2d 2d2d 0a20 2020 2070 7976 6973  ------.    pyvis
-00020700: 7461 2e55 6e73 7472 7563 7475 7265 6447  ta.UnstructuredG
-00020710: 7269 6420 7c20 7374 720a 2020 2020 2020  rid | str.      
-00020720: 2020 4461 7461 5365 7420 6f72 2066 696c    DataSet or fil
-00020730: 656e 616d 6520 6465 7065 6e64 696e 6720  ename depending 
-00020740: 6f6e 2060 606c 6f61 6460 602e 0a0a 2020  on ``load``...  
-00020750: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
-00020760: 2d2d 2d2d 2d2d 2d0a 2020 2020 506c 6f74  -------.    Plot
-00020770: 2062 7920 7061 7274 2049 442e 0a0a 2020   by part ID...  
-00020780: 2020 3e3e 3e20 696d 706f 7274 206e 756d    >>> import num
-00020790: 7079 2061 7320 6e70 0a20 2020 203e 3e3e  py as np.    >>>
-000207a0: 2069 6d70 6f72 7420 7079 7669 7374 6120   import pyvista 
-000207b0: 6173 2070 760a 2020 2020 3e3e 3e20 6672  as pv.    >>> fr
-000207c0: 6f6d 2070 7976 6973 7461 2069 6d70 6f72  om pyvista impor
-000207d0: 7420 6578 616d 706c 6573 0a20 2020 203e  t examples.    >
-000207e0: 3e3e 2067 7269 6420 3d20 6578 616d 706c  >> grid = exampl
-000207f0: 6573 2e64 6f77 6e6c 6f61 645f 6665 615f  es.download_fea_
-00020800: 6865 7274 7a69 616e 5f63 6f6e 7461 6374  hertzian_contact
-00020810: 5f63 796c 696e 6465 7228 290a 2020 2020  _cylinder().    
-00020820: 3e3e 3e20 6772 6964 2e70 6c6f 7428 0a20  >>> grid.plot(. 
-00020830: 2020 202e 2e2e 2020 2020 2073 6361 6c61     ...     scala
-00020840: 7273 3d27 5061 7274 4944 272c 2063 6d61  rs='PartID', cma
-00020850: 703d 5b27 6772 6565 6e27 2c20 2762 6c75  p=['green', 'blu
-00020860: 6527 5d2c 2073 686f 775f 7363 616c 6172  e'], show_scalar
-00020870: 5f62 6172 3d46 616c 7365 0a20 2020 202e  _bar=False.    .
-00020880: 2e2e 2029 0a0a 2020 2020 506c 6f74 2074  .. )..    Plot t
-00020890: 6865 2061 6273 6f6c 7574 6520 7661 6c75  he absolute valu
-000208a0: 6520 6f66 2074 6865 2063 6f6d 706f 6e65  e of the compone
-000208b0: 6e74 2073 7472 6573 7320 696e 2074 6865  nt stress in the
-000208c0: 205a 2064 6972 6563 7469 6f6e 2e0a 0a20   Z direction... 
-000208d0: 2020 203e 3e3e 2070 6c20 3d20 7076 2e50     >>> pl = pv.P
-000208e0: 6c6f 7474 6572 2829 0a20 2020 203e 3e3e  lotter().    >>>
-000208f0: 207a 5f73 7472 6573 7320 3d20 6e70 2e61   z_stress = np.a
-00020900: 6273 2867 7269 645b 2753 7472 6573 7327  bs(grid['Stress'
-00020910: 5d5b 3a2c 2032 5d29 0a20 2020 203e 3e3e  ][:, 2]).    >>>
-00020920: 205f 203d 2070 6c2e 6164 645f 6d65 7368   _ = pl.add_mesh
-00020930: 280a 2020 2020 2e2e 2e20 2020 2020 6772  (.    ...     gr
-00020940: 6964 2c0a 2020 2020 2e2e 2e20 2020 2020  id,.    ...     
-00020950: 7363 616c 6172 733d 7a5f 7374 7265 7373  scalars=z_stress
-00020960: 2c0a 2020 2020 2e2e 2e20 2020 2020 636c  ,.    ...     cl
-00020970: 696d 3d5b 302c 2031 2e32 6539 5d2c 0a20  im=[0, 1.2e9],. 
-00020980: 2020 202e 2e2e 2020 2020 2063 6d61 703d     ...     cmap=
-00020990: 276a 6574 272c 0a20 2020 202e 2e2e 2020  'jet',.    ...  
-000209a0: 2020 206c 6967 6874 696e 673d 5472 7565     lighting=True
-000209b0: 2c0a 2020 2020 2e2e 2e20 2020 2020 7368  ,.    ...     sh
-000209c0: 6f77 5f65 6467 6573 3d46 616c 7365 2c0a  ow_edges=False,.
-000209d0: 2020 2020 2e2e 2e20 2020 2020 616d 6269      ...     ambi
-000209e0: 656e 743d 302e 322c 0a20 2020 202e 2e2e  ent=0.2,.    ...
-000209f0: 2029 0a20 2020 203e 3e3e 2070 6c2e 6361   ).    >>> pl.ca
-00020a00: 6d65 7261 5f70 6f73 6974 696f 6e20 3d20  mera_position = 
-00020a10: 2778 7a27 0a20 2020 203e 3e3e 2070 6c2e  'xz'.    >>> pl.
-00020a20: 6361 6d65 7261 2e7a 6f6f 6d28 312e 3429  camera.zoom(1.4)
-00020a30: 0a20 2020 203e 3e3e 2070 6c2e 7368 6f77  .    >>> pl.show
-00020a40: 2829 0a0a 2020 2020 2222 220a 2020 2020  ()..    """.    
-00020a50: 6669 6c65 6e61 6d65 203d 205f 646f 776e  filename = _down
-00020a60: 6c6f 6164 5f61 7263 6869 7665 280a 2020  load_archive(.  
-00020a70: 2020 2020 2020 2766 6561 2f68 6572 747a        'fea/hertz
-00020a80: 6961 6e5f 636f 6e74 6163 745f 6379 6c69  ian_contact_cyli
-00020a90: 6e64 6572 2f48 6572 747a 6961 6e5f 6379  nder/Hertzian_cy
-00020aa0: 6c69 6e64 6572 5f6f 6e5f 706c 6174 652e  linder_on_plate.
-00020ab0: 7a69 7027 2c0a 2020 2020 2020 2020 7461  zip',.        ta
-00020ac0: 7267 6574 5f66 696c 653d 2762 6661 6339  rget_file='bfac9
-00020ad0: 6664 312d 6539 3832 2d34 3832 352d 3961  fd1-e982-4825-9a
-00020ae0: 3935 2d39 6535 6438 6335 6234 6433 655f  95-9e5d8c5b4d3e_
-00020af0: 7265 7375 6c74 5f31 2e70 7674 7527 2c0a  result_1.pvtu',.
-00020b00: 2020 2020 290a 2020 2020 6966 206c 6f61      ).    if loa
-00020b10: 643a 0a20 2020 2020 2020 2072 6574 7572  d:.        retur
-00020b20: 6e20 7079 7669 7374 612e 7265 6164 2866  n pyvista.read(f
-00020b30: 696c 656e 616d 6529 0a20 2020 2072 6574  ilename).    ret
-00020b40: 7572 6e20 6669 6c65 6e61 6d65 0a0a 0a64  urn filename...d
-00020b50: 6566 2064 6f77 6e6c 6f61 645f 626c 6163  ef download_blac
-00020b60: 6b5f 7661 7365 286c 6f61 643d 5472 7565  k_vase(load=True
-00020b70: 293a 2020 2320 7072 6167 6d61 3a20 6e6f  ):  # pragma: no
-00020b80: 2063 6f76 6572 0a20 2020 2022 2222 446f   cover.    """Do
-00020b90: 776e 6c6f 6164 2061 2062 6c61 636b 2076  wnload a black v
-00020ba0: 6173 6520 7363 616e 2063 7265 6174 6564  ase scan created
-00020bb0: 2062 7920 4976 616e 204e 696b 6f6c 6f76   by Ivan Nikolov
-00020bc0: 2e0a 0a20 2020 2054 6865 2064 6174 6173  ...    The datas
-00020bd0: 6574 2077 6173 2064 6f77 6e6c 6f61 6465  et was downloade
-00020be0: 6420 6672 6f6d 2060 4747 472d 4265 6e63  d from `GGG-Benc
-00020bf0: 686d 6172 6b53 664d 3a20 4461 7461 7365  hmarkSfM: Datase
-00020c00: 7420 666f 7220 4265 6e63 686d 6172 6b69  t for Benchmarki
-00020c10: 6e67 0a20 2020 2043 6c6f 7365 2d72 616e  ng.    Close-ran
-00020c20: 6765 2053 664d 2053 6f66 7477 6172 6520  ge SfM Software 
-00020c30: 5065 7266 6f72 6d61 6e63 6520 756e 6465  Performance unde
-00020c40: 7220 5661 7279 696e 6720 4361 7074 7572  r Varying Captur
-00020c50: 696e 6720 436f 6e64 6974 696f 6e73 0a20  ing Conditions. 
-00020c60: 2020 203c 6874 7470 733a 2f2f 6461 7461     <https://data
-00020c70: 2e6d 656e 6465 6c65 792e 636f 6d2f 6461  .mendeley.com/da
-00020c80: 7461 7365 7473 2f62 7a78 6b32 6e37 3873  tasets/bzxk2n78s
-00020c90: 392f 343e 605f 0a0a 2020 2020 4f72 6967  9/4>`_..    Orig
-00020ca0: 696e 616c 2064 6174 6173 6574 7320 6172  inal datasets ar
-00020cb0: 6520 756e 6465 7220 7468 6520 4343 2042  e under the CC B
-00020cc0: 5920 342e 3020 6c69 6365 6e73 652e 0a0a  Y 4.0 license...
-00020cd0: 2020 2020 466f 7220 6d6f 7265 2064 6574      For more det
-00020ce0: 6169 6c73 2c20 7365 6520 6049 7661 6e20  ails, see `Ivan 
-00020cf0: 4e69 6b6f 6c6f 7620 4461 7461 7365 7473  Nikolov Datasets
-00020d00: 0a20 2020 203c 6874 7470 733a 2f2f 6769  .    <https://gi
-00020d10: 7468 7562 2e63 6f6d 2f70 7976 6973 7461  thub.com/pyvista
-00020d20: 2f76 746b 2d64 6174 612f 7472 6565 2f6d  /vtk-data/tree/m
-00020d30: 6173 7465 722f 4461 7461 2f69 7661 6e2d  aster/Data/ivan-
-00020d40: 6e69 6b6f 6c6f 763e 605f 0a0a 2020 2020  nikolov>`_..    
-00020d50: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00020d60: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
-00020d70: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
-00020d80: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
-00020d90: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
-00020da0: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
-00020db0: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
-00020dc0: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
-00020dd0: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
-00020de0: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
-00020df0: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
-00020e00: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
-00020e10: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-00020e20: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
-00020e30: 612e 506f 6c79 4461 7461 207c 2073 7472  a.PolyData | str
-00020e40: 0a20 2020 2020 2020 2044 6174 6153 6574  .        DataSet
-00020e50: 206f 7220 6669 6c65 6e61 6d65 2064 6570   or filename dep
-00020e60: 656e 6469 6e67 206f 6e20 6060 6c6f 6164  ending on ``load
-00020e70: 6060 2e0a 0a20 2020 2045 7861 6d70 6c65  ``...    Example
-00020e80: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
-00020e90: 2020 2044 6f77 6e6c 6f61 6420 616e 6420     Download and 
-00020ea0: 706c 6f74 2074 6865 2064 6174 6173 6574  plot the dataset
-00020eb0: 2e0a 0a20 2020 203e 3e3e 2066 726f 6d20  ...    >>> from 
-00020ec0: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
-00020ed0: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
-00020ee0: 6d65 7368 203d 2065 7861 6d70 6c65 732e  mesh = examples.
-00020ef0: 646f 776e 6c6f 6164 5f62 6c61 636b 5f76  download_black_v
-00020f00: 6173 6528 290a 2020 2020 3e3e 3e20 6d65  ase().    >>> me
-00020f10: 7368 2e70 6c6f 7428 290a 0a20 2020 2052  sh.plot()..    R
-00020f20: 6574 7572 6e20 7468 6520 7374 6174 6973  eturn the statis
-00020f30: 7469 6373 206f 6620 7468 6520 6461 7461  tics of the data
-00020f40: 7365 742e 0a0a 2020 2020 3e3e 3e20 6d65  set...    >>> me
-00020f50: 7368 2020 2320 646f 6374 6573 743a 2b53  sh  # doctest:+S
-00020f60: 4b49 500a 2020 2020 506f 6c79 4461 7461  KIP.    PolyData
-00020f70: 2028 3078 3766 6534 3839 3439 3335 3230   (0x7fe489493520
-00020f80: 290a 2020 2020 2020 4e20 4365 6c6c 733a  ).      N Cells:
-00020f90: 2020 2020 2020 3331 3336 3635 320a 2020        3136652.  
-00020fa0: 2020 2020 4e20 506f 696e 7473 3a20 2020      N Points:   
-00020fb0: 2020 3136 3131 3738 390a 2020 2020 2020    1611789.      
-00020fc0: 5820 426f 756e 6473 3a20 2020 2020 2d31  X Bounds:     -1
-00020fd0: 2e30 3932 652b 3032 2c20 312e 3533 3365  .092e+02, 1.533e
-00020fe0: 2b30 320a 2020 2020 2020 5920 426f 756e  +02.      Y Boun
-00020ff0: 6473 3a20 2020 2020 2d31 2e32 3030 652b  ds:     -1.200e+
-00021000: 3032 2c20 312e 3431 3565 2b30 320a 2020  02, 1.415e+02.  
-00021010: 2020 2020 5a20 426f 756e 6473 3a20 2020      Z Bounds:   
-00021020: 2020 312e 3636 3665 2b30 312c 2034 2e30    1.666e+01, 4.0
-00021030: 3737 652b 3032 0a20 2020 2020 204e 2041  77e+02.      N A
-00021040: 7272 6179 733a 2020 2020 2030 0a0a 2020  rrays:     0..  
-00021050: 2020 2222 220a 2020 2020 6669 6c65 6e61    """.    filena
-00021060: 6d65 203d 205f 646f 776e 6c6f 6164 5f61  me = _download_a
-00021070: 7263 6869 7665 280a 2020 2020 2020 2020  rchive(.        
-00021080: 2769 7661 6e2d 6e69 6b6f 6c6f 762f 626c  'ivan-nikolov/bl
-00021090: 6163 6b56 6173 652e 7a69 7027 2c0a 2020  ackVase.zip',.  
-000210a0: 2020 2020 2020 2762 6c61 636b 5661 7365        'blackVase
-000210b0: 2e76 7470 272c 0a20 2020 2029 0a20 2020  .vtp',.    ).   
-000210c0: 2069 6620 6c6f 6164 3a0a 2020 2020 2020   if load:.      
-000210d0: 2020 7265 7475 726e 2070 7976 6973 7461    return pyvista
-000210e0: 2e72 6561 6428 6669 6c65 6e61 6d65 290a  .read(filename).
-000210f0: 2020 2020 7265 7475 726e 2066 696c 656e      return filen
-00021100: 616d 650a 0a0a 6465 6620 646f 776e 6c6f  ame...def downlo
-00021110: 6164 5f69 7661 6e5f 616e 6765 6c28 6c6f  ad_ivan_angel(lo
-00021120: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
-00021130: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-00021140: 2020 2222 2244 6f77 6e6c 6f61 6420 6120    """Download a 
-00021150: 7363 616e 206f 6620 616e 2061 6e67 656c  scan of an angel
-00021160: 2073 7461 7475 6520 6372 6561 7465 6420   statue created 
-00021170: 6279 2049 7661 6e20 4e69 6b6f 6c6f 762e  by Ivan Nikolov.
-00021180: 0a0a 2020 2020 5468 6520 6461 7461 7365  ..    The datase
-00021190: 7420 7761 7320 646f 776e 6c6f 6164 6564  t was downloaded
-000211a0: 2066 726f 6d20 6047 4747 2d42 656e 6368   from `GGG-Bench
-000211b0: 6d61 726b 5366 4d3a 2044 6174 6173 6574  markSfM: Dataset
-000211c0: 2066 6f72 2042 656e 6368 6d61 726b 696e   for Benchmarkin
-000211d0: 670a 2020 2020 436c 6f73 652d 7261 6e67  g.    Close-rang
-000211e0: 6520 5366 4d20 536f 6674 7761 7265 2050  e SfM Software P
-000211f0: 6572 666f 726d 616e 6365 2075 6e64 6572  erformance under
-00021200: 2056 6172 7969 6e67 2043 6170 7475 7269   Varying Capturi
-00021210: 6e67 2043 6f6e 6469 7469 6f6e 730a 2020  ng Conditions.  
-00021220: 2020 3c68 7474 7073 3a2f 2f64 6174 612e    <https://data.
-00021230: 6d65 6e64 656c 6579 2e63 6f6d 2f64 6174  mendeley.com/dat
-00021240: 6173 6574 732f 627a 786b 326e 3738 7339  asets/bzxk2n78s9
-00021250: 2f34 3e60 5f0a 0a20 2020 204f 7269 6769  /4>`_..    Origi
-00021260: 6e61 6c20 6461 7461 7365 7473 2061 7265  nal datasets are
-00021270: 2075 6e64 6572 2074 6865 2043 4320 4259   under the CC BY
-00021280: 2034 2e30 206c 6963 656e 7365 2e0a 0a20   4.0 license... 
-00021290: 2020 2046 6f72 206d 6f72 6520 6465 7461     For more deta
-000212a0: 696c 732c 2073 6565 2060 4976 616e 204e  ils, see `Ivan N
-000212b0: 696b 6f6c 6f76 2044 6174 6173 6574 730a  ikolov Datasets.
-000212c0: 2020 2020 3c68 7474 7073 3a2f 2f67 6974      <https://git
-000212d0: 6875 622e 636f 6d2f 7079 7669 7374 612f  hub.com/pyvista/
-000212e0: 7674 6b2d 6461 7461 2f74 7265 652f 6d61  vtk-data/tree/ma
-000212f0: 7374 6572 2f44 6174 612f 6976 616e 2d6e  ster/Data/ivan-n
-00021300: 696b 6f6c 6f76 3e60 5f0a 0a20 2020 2050  ikolov>`_..    P
-00021310: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00021320: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c 6f61  --------.    loa
-00021330: 6420 3a20 626f 6f6c 2c20 6465 6661 756c  d : bool, defaul
-00021340: 743a 2054 7275 650a 2020 2020 2020 2020  t: True.        
-00021350: 4c6f 6164 2074 6865 2064 6174 6173 6574  Load the dataset
-00021360: 2061 6674 6572 2064 6f77 6e6c 6f61 6469   after downloadi
-00021370: 6e67 2069 7420 7768 656e 2060 6054 7275  ng it when ``Tru
-00021380: 6560 602e 2020 5365 7420 7468 6973 0a20  e``.  Set this. 
-00021390: 2020 2020 2020 2074 6f20 6060 4661 6c73         to ``Fals
-000213a0: 6560 6020 616e 6420 6f6e 6c79 2074 6865  e`` and only the
-000213b0: 2066 696c 656e 616d 6520 7769 6c6c 2062   filename will b
-000213c0: 6520 7265 7475 726e 6564 2e0a 0a20 2020  e returned...   
-000213d0: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
-000213e0: 2d2d 2d2d 0a20 2020 2070 7976 6973 7461  ----.    pyvista
-000213f0: 2e50 6f6c 7944 6174 6120 7c20 7374 720a  .PolyData | str.
-00021400: 2020 2020 2020 2020 4461 7461 5365 7420          DataSet 
-00021410: 6f72 2066 696c 656e 616d 6520 6465 7065  or filename depe
-00021420: 6e64 696e 6720 6f6e 2060 606c 6f61 6460  nding on ``load`
-00021430: 602e 0a0a 2020 2020 4578 616d 706c 6573  `...    Examples
-00021440: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-00021450: 2020 446f 776e 6c6f 6164 2061 6e64 2070    Download and p
-00021460: 6c6f 7420 7468 6520 6461 7461 7365 742e  lot the dataset.
-00021470: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2070  ..    >>> from p
-00021480: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
-00021490: 616d 706c 6573 0a20 2020 203e 3e3e 206d  amples.    >>> m
-000214a0: 6573 6820 3d20 6578 616d 706c 6573 2e64  esh = examples.d
-000214b0: 6f77 6e6c 6f61 645f 6976 616e 5f61 6e67  ownload_ivan_ang
-000214c0: 656c 2829 0a20 2020 203e 3e3e 2063 706f  el().    >>> cpo
-000214d0: 7320 3d20 5b0a 2020 2020 2e2e 2e20 2020  s = [.    ...   
-000214e0: 2020 282d 3437 362e 3134 2c20 2d33 3933    (-476.14, -393
-000214f0: 2e37 332c 2032 3832 2e31 3429 2c0a 2020  .73, 282.14),.  
-00021500: 2020 2e2e 2e20 2020 2020 282d 3135 2e30    ...     (-15.0
-00021510: 302c 2031 312e 3235 2c20 3434 2e30 3829  0, 11.25, 44.08)
-00021520: 2c0a 2020 2020 2e2e 2e20 2020 2020 2830  ,.    ...     (0
-00021530: 2e32 362c 2030 2e32 342c 2030 2e39 3329  .26, 0.24, 0.93)
-00021540: 2c0a 2020 2020 2e2e 2e20 5d0a 2020 2020  ,.    ... ].    
-00021550: 3e3e 3e20 6d65 7368 2e70 6c6f 7428 6370  >>> mesh.plot(cp
-00021560: 6f73 3d63 706f 7329 0a0a 2020 2020 5265  os=cpos)..    Re
-00021570: 7475 726e 2074 6865 2073 7461 7469 7374  turn the statist
-00021580: 6963 7320 6f66 2074 6865 2064 6174 6173  ics of the datas
-00021590: 6574 2e0a 0a20 2020 203e 3e3e 206d 6573  et...    >>> mes
-000215a0: 6820 2023 2064 6f63 7465 7374 3a2b 534b  h  # doctest:+SK
-000215b0: 4950 0a20 2020 2050 6f6c 7944 6174 6120  IP.    PolyData 
-000215c0: 2830 7837 6636 6564 3133 3435 3532 3029  (0x7f6ed1345520)
-000215d0: 0a20 2020 2020 204e 2043 656c 6c73 3a20  .      N Cells: 
-000215e0: 2020 2020 2034 3534 3737 3136 0a20 2020       4547716.   
-000215f0: 2020 204e 2050 6f69 6e74 733a 2020 2020     N Points:    
-00021600: 2032 3239 3730 3839 0a20 2020 2020 2058   2297089.      X
-00021610: 2042 6f75 6e64 733a 2020 2020 202d 312e   Bounds:     -1.
-00021620: 3134 3765 2b30 322c 2038 2e34 3638 652b  147e+02, 8.468e+
-00021630: 3031 0a20 2020 2020 2059 2042 6f75 6e64  01.      Y Bound
-00021640: 733a 2020 2020 202d 372e 3130 3365 2b30  s:     -7.103e+0
-00021650: 312c 2039 2e32 3437 652b 3031 0a20 2020  1, 9.247e+01.   
-00021660: 2020 205a 2042 6f75 6e64 733a 2020 2020     Z Bounds:    
-00021670: 202d 312e 3139 3865 2b30 322c 2032 2e30   -1.198e+02, 2.0
-00021680: 3532 652b 3032 0a20 2020 2020 204e 2041  52e+02.      N A
-00021690: 7272 6179 733a 2020 2020 2030 0a0a 2020  rrays:     0..  
-000216a0: 2020 2222 220a 2020 2020 6669 6c65 6e61    """.    filena
-000216b0: 6d65 203d 205f 646f 776e 6c6f 6164 5f61  me = _download_a
-000216c0: 7263 6869 7665 280a 2020 2020 2020 2020  rchive(.        
-000216d0: 2769 7661 6e2d 6e69 6b6f 6c6f 762f 416e  'ivan-nikolov/An
-000216e0: 6765 6c2e 7a69 7027 2c0a 2020 2020 2020  gel.zip',.      
-000216f0: 2020 2741 6e67 656c 2e76 7470 272c 0a20    'Angel.vtp',. 
-00021700: 2020 2029 0a20 2020 2069 6620 6c6f 6164     ).    if load
-00021710: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00021720: 2070 7976 6973 7461 2e72 6561 6428 6669   pyvista.read(fi
-00021730: 6c65 6e61 6d65 290a 2020 2020 7265 7475  lename).    retu
-00021740: 726e 2066 696c 656e 616d 650a 0a0a 6465  rn filename...de
-00021750: 6620 646f 776e 6c6f 6164 5f62 6972 645f  f download_bird_
-00021760: 6261 7468 286c 6f61 643d 5472 7565 293a  bath(load=True):
-00021770: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
-00021780: 6f76 6572 0a20 2020 2022 2222 446f 776e  over.    """Down
-00021790: 6c6f 6164 2061 2073 6361 6e20 6f66 2061  load a scan of a
-000217a0: 2062 6972 6420 6261 7468 2063 7265 6174   bird bath creat
-000217b0: 6564 2062 7920 4976 616e 204e 696b 6f6c  ed by Ivan Nikol
-000217c0: 6f76 2e0a 0a20 2020 2054 6865 2064 6174  ov...    The dat
-000217d0: 6173 6574 2077 6173 2064 6f77 6e6c 6f61  aset was downloa
-000217e0: 6465 6420 6672 6f6d 2060 4747 472d 4265  ded from `GGG-Be
-000217f0: 6e63 686d 6172 6b53 664d 3a20 4461 7461  nchmarkSfM: Data
-00021800: 7365 7420 666f 7220 4265 6e63 686d 6172  set for Benchmar
-00021810: 6b69 6e67 0a20 2020 2043 6c6f 7365 2d72  king.    Close-r
-00021820: 616e 6765 2053 664d 2053 6f66 7477 6172  ange SfM Softwar
-00021830: 6520 5065 7266 6f72 6d61 6e63 6520 756e  e Performance un
-00021840: 6465 7220 5661 7279 696e 6720 4361 7074  der Varying Capt
-00021850: 7572 696e 6720 436f 6e64 6974 696f 6e73  uring Conditions
-00021860: 0a20 2020 203c 6874 7470 733a 2f2f 6461  .    <https://da
-00021870: 7461 2e6d 656e 6465 6c65 792e 636f 6d2f  ta.mendeley.com/
-00021880: 6461 7461 7365 7473 2f62 7a78 6b32 6e37  datasets/bzxk2n7
-00021890: 3873 392f 343e 605f 0a0a 2020 2020 4f72  8s9/4>`_..    Or
-000218a0: 6967 696e 616c 2064 6174 6173 6574 7320  iginal datasets 
-000218b0: 6172 6520 756e 6465 7220 7468 6520 4343  are under the CC
-000218c0: 2042 5920 342e 3020 6c69 6365 6e73 652e   BY 4.0 license.
-000218d0: 0a0a 2020 2020 466f 7220 6d6f 7265 2064  ..    For more d
-000218e0: 6574 6169 6c73 2c20 7365 6520 6049 7661  etails, see `Iva
-000218f0: 6e20 4e69 6b6f 6c6f 7620 4461 7461 7365  n Nikolov Datase
-00021900: 7473 0a20 2020 203c 6874 7470 733a 2f2f  ts.    <https://
-00021910: 6769 7468 7562 2e63 6f6d 2f70 7976 6973  github.com/pyvis
-00021920: 7461 2f76 746b 2d64 6174 612f 7472 6565  ta/vtk-data/tree
-00021930: 2f6d 6173 7465 722f 4461 7461 2f69 7661  /master/Data/iva
-00021940: 6e2d 6e69 6b6f 6c6f 763e 605f 0a0a 2020  n-nikolov>`_..  
-00021950: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00021960: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00021970: 6c6f 6164 203a 2062 6f6f 6c2c 2064 6566  load : bool, def
-00021980: 6175 6c74 3a20 5472 7565 0a20 2020 2020  ault: True.     
-00021990: 2020 204c 6f61 6420 7468 6520 6461 7461     Load the data
-000219a0: 7365 7420 6166 7465 7220 646f 776e 6c6f  set after downlo
-000219b0: 6164 696e 6720 6974 2077 6865 6e20 6060  ading it when ``
-000219c0: 5472 7565 6060 2e20 2053 6574 2074 6869  True``.  Set thi
-000219d0: 730a 2020 2020 2020 2020 746f 2060 6046  s.        to ``F
-000219e0: 616c 7365 6060 2061 6e64 206f 6e6c 7920  alse`` and only 
-000219f0: 7468 6520 6669 6c65 6e61 6d65 2077 696c  the filename wil
-00021a00: 6c20 6265 2072 6574 7572 6e65 642e 0a0a  l be returned...
-00021a10: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00021a20: 2d2d 2d2d 2d2d 2d0a 2020 2020 7079 7669  -------.    pyvi
-00021a30: 7374 612e 506f 6c79 4461 7461 207c 2073  sta.PolyData | s
-00021a40: 7472 0a20 2020 2020 2020 2044 6174 6153  tr.        DataS
-00021a50: 6574 206f 7220 6669 6c65 6e61 6d65 2064  et or filename d
-00021a60: 6570 656e 6469 6e67 206f 6e20 6060 6c6f  epending on ``lo
-00021a70: 6164 6060 2e0a 0a20 2020 2045 7861 6d70  ad``...    Examp
-00021a80: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-00021a90: 0a20 2020 2044 6f77 6e6c 6f61 6420 616e  .    Download an
-00021aa0: 6420 706c 6f74 2074 6865 2064 6174 6173  d plot the datas
-00021ab0: 6574 2e0a 0a20 2020 203e 3e3e 2066 726f  et...    >>> fro
-00021ac0: 6d20 7079 7669 7374 6120 696d 706f 7274  m pyvista import
-00021ad0: 2065 7861 6d70 6c65 730a 2020 2020 3e3e   examples.    >>
-00021ae0: 3e20 6d65 7368 203d 2065 7861 6d70 6c65  > mesh = example
-00021af0: 732e 646f 776e 6c6f 6164 5f62 6972 645f  s.download_bird_
-00021b00: 6261 7468 2829 0a20 2020 203e 3e3e 206d  bath().    >>> m
-00021b10: 6573 682e 706c 6f74 2829 0a0a 2020 2020  esh.plot()..    
-00021b20: 5265 7475 726e 2074 6865 2073 7461 7469  Return the stati
-00021b30: 7374 6963 7320 6f66 2074 6865 2064 6174  stics of the dat
-00021b40: 6173 6574 2e0a 0a20 2020 203e 3e3e 206d  aset...    >>> m
-00021b50: 6573 6820 2023 2064 6f63 7465 7374 3a2b  esh  # doctest:+
-00021b60: 534b 4950 0a20 2020 2050 6f6c 7944 6174  SKIP.    PolyDat
-00021b70: 6120 2830 7837 6665 3863 6166 3262 6130  a (0x7fe8caf2ba0
-00021b80: 3029 0a20 2020 204e 2043 656c 6c73 3a20  0).    N Cells: 
-00021b90: 2020 2020 2033 3530 3739 3335 0a20 2020       3507935.   
-00021ba0: 204e 2050 6f69 6e74 733a 2020 2020 2031   N Points:     1
-00021bb0: 3833 3133 3833 0a20 2020 2058 2042 6f75  831383.    X Bou
-00021bc0: 6e64 733a 2020 2020 202d 312e 3630 3165  nds:     -1.601e
-00021bd0: 2b30 322c 2031 2e34 3833 652b 3032 0a20  +02, 1.483e+02. 
-00021be0: 2020 2059 2042 6f75 6e64 733a 2020 2020     Y Bounds:    
-00021bf0: 202d 312e 3532 3165 2b30 322c 2031 2e35   -1.521e+02, 1.5
-00021c00: 3437 652b 3032 0a20 2020 205a 2042 6f75  47e+02.    Z Bou
-00021c10: 6e64 733a 2020 2020 202d 342e 3234 3165  nds:     -4.241e
-00021c20: 2b30 302c 2031 2e34 3039 652b 3032 0a20  +00, 1.409e+02. 
-00021c30: 2020 204e 2041 7272 6179 733a 2020 2020     N Arrays:    
-00021c40: 2030 0a0a 2020 2020 2222 220a 2020 2020   0..    """.    
-00021c50: 6669 6c65 6e61 6d65 203d 205f 646f 776e  filename = _down
-00021c60: 6c6f 6164 5f61 7263 6869 7665 280a 2020  load_archive(.  
-00021c70: 2020 2020 2020 2769 7661 6e2d 6e69 6b6f        'ivan-niko
-00021c80: 6c6f 762f 6269 7264 4261 7468 2e7a 6970  lov/birdBath.zip
-00021c90: 272c 0a20 2020 2020 2020 2027 6269 7264  ',.        'bird
-00021ca0: 4261 7468 2e76 7470 272c 0a20 2020 2029  Bath.vtp',.    )
-00021cb0: 0a20 2020 2069 6620 6c6f 6164 3a0a 2020  .    if load:.  
-00021cc0: 2020 2020 2020 7265 7475 726e 2070 7976        return pyv
-00021cd0: 6973 7461 2e72 6561 6428 6669 6c65 6e61  ista.read(filena
-00021ce0: 6d65 290a 2020 2020 7265 7475 726e 2066  me).    return f
-00021cf0: 696c 656e 616d 650a 0a0a 6465 6620 646f  ilename...def do
-00021d00: 776e 6c6f 6164 5f6f 776c 286c 6f61 643d  wnload_owl(load=
-00021d10: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
-00021d20: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
-00021d30: 2222 446f 776e 6c6f 6164 2061 2073 6361  ""Download a sca
-00021d40: 6e20 6f66 2061 6e20 6f77 6c20 7374 6174  n of an owl stat
-00021d50: 7565 2063 7265 6174 6564 2062 7920 4976  ue created by Iv
-00021d60: 616e 204e 696b 6f6c 6f76 2e0a 0a20 2020  an Nikolov...   
-00021d70: 2054 6865 2064 6174 6173 6574 2077 6173   The dataset was
-00021d80: 2064 6f77 6e6c 6f61 6465 6420 6672 6f6d   downloaded from
-00021d90: 2060 4747 472d 4265 6e63 686d 6172 6b53   `GGG-BenchmarkS
-00021da0: 664d 3a20 4461 7461 7365 7420 666f 7220  fM: Dataset for 
-00021db0: 4265 6e63 686d 6172 6b69 6e67 0a20 2020  Benchmarking.   
-00021dc0: 2043 6c6f 7365 2d72 616e 6765 2053 664d   Close-range SfM
-00021dd0: 2053 6f66 7477 6172 6520 5065 7266 6f72   Software Perfor
-00021de0: 6d61 6e63 6520 756e 6465 7220 5661 7279  mance under Vary
-00021df0: 696e 6720 4361 7074 7572 696e 6720 436f  ing Capturing Co
-00021e00: 6e64 6974 696f 6e73 0a20 2020 203c 6874  nditions.    <ht
-00021e10: 7470 733a 2f2f 6461 7461 2e6d 656e 6465  tps://data.mende
-00021e20: 6c65 792e 636f 6d2f 6461 7461 7365 7473  ley.com/datasets
-00021e30: 2f62 7a78 6b32 6e37 3873 392f 343e 605f  /bzxk2n78s9/4>`_
-00021e40: 0a0a 2020 2020 4f72 6967 696e 616c 2064  ..    Original d
-00021e50: 6174 6173 6574 7320 6172 6520 756e 6465  atasets are unde
-00021e60: 7220 7468 6520 4343 2042 5920 342e 3020  r the CC BY 4.0 
-00021e70: 6c69 6365 6e73 652e 0a0a 2020 2020 466f  license...    Fo
-00021e80: 7220 6d6f 7265 2064 6574 6169 6c73 2c20  r more details, 
-00021e90: 7365 6520 6049 7661 6e20 4e69 6b6f 6c6f  see `Ivan Nikolo
-00021ea0: 7620 4461 7461 7365 7473 0a20 2020 203c  v Datasets.    <
-00021eb0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00021ec0: 6f6d 2f70 7976 6973 7461 2f76 746b 2d64  om/pyvista/vtk-d
-00021ed0: 6174 612f 7472 6565 2f6d 6173 7465 722f  ata/tree/master/
-00021ee0: 4461 7461 2f69 7661 6e2d 6e69 6b6f 6c6f  Data/ivan-nikolo
-00021ef0: 763e 605f 0a0a 2020 2020 5061 7261 6d65  v>`_..    Parame
-00021f00: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00021f10: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-00021f20: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-00021f30: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-00021f40: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-00021f50: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-00021f60: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-00021f70: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-00021f80: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-00021f90: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-00021fa0: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-00021fb0: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-00021fc0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00021fd0: 2020 2020 7079 7669 7374 612e 506f 6c79      pyvista.Poly
-00021fe0: 4461 7461 207c 2073 7472 0a20 2020 2020  Data | str.     
-00021ff0: 2020 2044 6174 6153 6574 206f 7220 6669     DataSet or fi
-00022000: 6c65 6e61 6d65 2064 6570 656e 6469 6e67  lename depending
-00022010: 206f 6e20 6060 6c6f 6164 6060 2e0a 0a20   on ``load``... 
-00022020: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-00022030: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6f77  --------.    Dow
-00022040: 6e6c 6f61 6420 616e 6420 706c 6f74 2074  nload and plot t
-00022050: 6865 2064 6174 6173 6574 2e0a 0a20 2020  he dataset...   
-00022060: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
-00022070: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
-00022080: 730a 2020 2020 3e3e 3e20 6d65 7368 203d  s.    >>> mesh =
-00022090: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
-000220a0: 6164 5f6f 776c 2829 0a20 2020 203e 3e3e  ad_owl().    >>>
-000220b0: 2063 706f 7320 3d20 5b0a 2020 2020 2e2e   cpos = [.    ..
-000220c0: 2e20 2020 2020 282d 3331 352e 3138 2c20  .     (-315.18, 
-000220d0: 2d34 3032 2e32 312c 2032 3330 2e37 3129  -402.21, 230.71)
-000220e0: 2c0a 2020 2020 2e2e 2e20 2020 2020 2836  ,.    ...     (6
-000220f0: 2e30 362c 202d 312e 3734 2c20 3130 312e  .06, -1.74, 101.
-00022100: 3438 292c 0a20 2020 202e 2e2e 2020 2020  48),.    ...    
-00022110: 2028 302e 3130 382c 2030 2e32 3236 2c20   (0.108, 0.226, 
-00022120: 302e 3936 3829 2c0a 2020 2020 2e2e 2e20  0.968),.    ... 
-00022130: 5d0a 2020 2020 3e3e 3e20 6d65 7368 2e70  ].    >>> mesh.p
-00022140: 6c6f 7428 6370 6f73 3d63 706f 7329 0a0a  lot(cpos=cpos)..
-00022150: 2020 2020 5265 7475 726e 2074 6865 2073      Return the s
-00022160: 7461 7469 7374 6963 7320 6f66 2074 6865  tatistics of the
-00022170: 2064 6174 6173 6574 2e0a 0a20 2020 203e   dataset...    >
-00022180: 3e3e 206d 6573 6820 2023 2064 6f63 7465  >> mesh  # docte
-00022190: 7374 3a2b 534b 4950 0a20 2020 2050 6f6c  st:+SKIP.    Pol
-000221a0: 7944 6174 6120 2830 7837 6665 3863 6165  yData (0x7fe8cae
-000221b0: 6561 6565 3029 0a20 2020 2020 204e 2043  eaee0).      N C
-000221c0: 656c 6c73 3a20 2020 2020 2032 3434 3037  ells:      24407
-000221d0: 3037 0a20 2020 2020 204e 2050 6f69 6e74  07.      N Point
-000221e0: 733a 2020 2020 2031 3232 3137 3536 0a20  s:     1221756. 
-000221f0: 2020 2020 2058 2042 6f75 6e64 733a 2020       X Bounds:  
-00022200: 2020 202d 352e 3833 3465 2b30 312c 2037     -5.834e+01, 7
-00022210: 2e30 3437 652b 3031 0a20 2020 2020 2059  .047e+01.      Y
-00022220: 2042 6f75 6e64 733a 2020 2020 202d 372e   Bounds:     -7.
-00022230: 3030 3665 2b30 312c 2036 2e36 3538 652b  006e+01, 6.658e+
-00022240: 3031 0a20 2020 2020 205a 2042 6f75 6e64  01.      Z Bound
-00022250: 733a 2020 2020 2031 2e36 3736 652b 3030  s:     1.676e+00
-00022260: 2c20 322e 3031 3365 2b30 320a 2020 2020  , 2.013e+02.    
-00022270: 2020 4e20 4172 7261 7973 3a20 2020 2020    N Arrays:     
-00022280: 300a 0a20 2020 2022 2222 0a20 2020 2066  0..    """.    f
-00022290: 696c 656e 616d 6520 3d20 5f64 6f77 6e6c  ilename = _downl
-000222a0: 6f61 645f 6172 6368 6976 6528 0a20 2020  oad_archive(.   
-000222b0: 2020 2020 2027 6976 616e 2d6e 696b 6f6c       'ivan-nikol
-000222c0: 6f76 2f6f 776c 2e7a 6970 272c 0a20 2020  ov/owl.zip',.   
-000222d0: 2020 2020 2027 6f77 6c2e 7674 7027 2c0a       'owl.vtp',.
-000222e0: 2020 2020 290a 2020 2020 6966 206c 6f61      ).    if loa
-000222f0: 643a 0a20 2020 2020 2020 2072 6574 7572  d:.        retur
-00022300: 6e20 7079 7669 7374 612e 7265 6164 2866  n pyvista.read(f
-00022310: 696c 656e 616d 6529 0a20 2020 2072 6574  ilename).    ret
-00022320: 7572 6e20 6669 6c65 6e61 6d65 0a0a 0a64  urn filename...d
-00022330: 6566 2064 6f77 6e6c 6f61 645f 706c 6173  ef download_plas
-00022340: 7469 635f 7661 7365 286c 6f61 643d 5472  tic_vase(load=Tr
-00022350: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
-00022360: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
-00022370: 446f 776e 6c6f 6164 2061 2073 6361 6e20  Download a scan 
-00022380: 6f66 2061 2070 6c61 7374 6963 2076 6173  of a plastic vas
-00022390: 6520 6372 6561 7465 6420 6279 2049 7661  e created by Iva
-000223a0: 6e20 4e69 6b6f 6c6f 762e 0a0a 2020 2020  n Nikolov...    
-000223b0: 5468 6520 6461 7461 7365 7420 7761 7320  The dataset was 
-000223c0: 646f 776e 6c6f 6164 6564 2066 726f 6d20  downloaded from 
-000223d0: 6047 4747 2d42 656e 6368 6d61 726b 5366  `GGG-BenchmarkSf
-000223e0: 4d3a 2044 6174 6173 6574 2066 6f72 2042  M: Dataset for B
-000223f0: 656e 6368 6d61 726b 696e 670a 2020 2020  enchmarking.    
-00022400: 436c 6f73 652d 7261 6e67 6520 5366 4d20  Close-range SfM 
-00022410: 536f 6674 7761 7265 2050 6572 666f 726d  Software Perform
-00022420: 616e 6365 2075 6e64 6572 2056 6172 7969  ance under Varyi
-00022430: 6e67 2043 6170 7475 7269 6e67 2043 6f6e  ng Capturing Con
-00022440: 6469 7469 6f6e 730a 2020 2020 3c68 7474  ditions.    <htt
-00022450: 7073 3a2f 2f64 6174 612e 6d65 6e64 656c  ps://data.mendel
-00022460: 6579 2e63 6f6d 2f64 6174 6173 6574 732f  ey.com/datasets/
-00022470: 627a 786b 326e 3738 7339 2f34 3e60 5f0a  bzxk2n78s9/4>`_.
-00022480: 0a20 2020 204f 7269 6769 6e61 6c20 6461  .    Original da
-00022490: 7461 7365 7473 2061 7265 2075 6e64 6572  tasets are under
-000224a0: 2074 6865 2043 4320 4259 2034 2e30 206c   the CC BY 4.0 l
-000224b0: 6963 656e 7365 2e0a 0a20 2020 2046 6f72  icense...    For
-000224c0: 206d 6f72 6520 6465 7461 696c 732c 2073   more details, s
-000224d0: 6565 2060 4976 616e 204e 696b 6f6c 6f76  ee `Ivan Nikolov
-000224e0: 2044 6174 6173 6574 730a 2020 2020 3c68   Datasets.    <h
-000224f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00022500: 6d2f 7079 7669 7374 612f 7674 6b2d 6461  m/pyvista/vtk-da
-00022510: 7461 2f74 7265 652f 6d61 7374 6572 2f44  ta/tree/master/D
-00022520: 6174 612f 6976 616e 2d6e 696b 6f6c 6f76  ata/ivan-nikolov
-00022530: 3e60 5f0a 0a20 2020 2050 6172 616d 6574  >`_..    Paramet
-00022540: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00022550: 2d2d 0a20 2020 206c 6f61 6420 3a20 626f  --.    load : bo
-00022560: 6f6c 2c20 6465 6661 756c 743a 2054 7275  ol, default: Tru
-00022570: 650a 2020 2020 2020 2020 4c6f 6164 2074  e.        Load t
-00022580: 6865 2064 6174 6173 6574 2061 6674 6572  he dataset after
-00022590: 2064 6f77 6e6c 6f61 6469 6e67 2069 7420   downloading it 
-000225a0: 7768 656e 2060 6054 7275 6560 602e 2020  when ``True``.  
-000225b0: 5365 7420 7468 6973 0a20 2020 2020 2020  Set this.       
-000225c0: 2074 6f20 6060 4661 6c73 6560 6020 616e   to ``False`` an
-000225d0: 6420 6f6e 6c79 2074 6865 2066 696c 656e  d only the filen
-000225e0: 616d 6520 7769 6c6c 2062 6520 7265 7475  ame will be retu
-000225f0: 726e 6564 2e0a 0a20 2020 2052 6574 7572  rned...    Retur
-00022600: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-00022610: 2020 2070 7976 6973 7461 2e50 6f6c 7944     pyvista.PolyD
-00022620: 6174 6120 7c20 7374 720a 2020 2020 2020  ata | str.      
-00022630: 2020 4461 7461 5365 7420 6f72 2066 696c    DataSet or fil
-00022640: 656e 616d 6520 6465 7065 6e64 696e 6720  ename depending 
-00022650: 6f6e 2060 606c 6f61 6460 602e 0a0a 2020  on ``load``...  
-00022660: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
-00022670: 2d2d 2d2d 2d2d 2d0a 2020 2020 446f 776e  -------.    Down
-00022680: 6c6f 6164 2061 6e64 2070 6c6f 7420 7468  load and plot th
-00022690: 6520 6461 7461 7365 742e 0a0a 2020 2020  e dataset...    
-000226a0: 3e3e 3e20 6672 6f6d 2070 7976 6973 7461  >>> from pyvista
-000226b0: 2069 6d70 6f72 7420 6578 616d 706c 6573   import examples
-000226c0: 0a20 2020 203e 3e3e 206d 6573 6820 3d20  .    >>> mesh = 
-000226d0: 6578 616d 706c 6573 2e64 6f77 6e6c 6f61  examples.downloa
-000226e0: 645f 706c 6173 7469 635f 7661 7365 2829  d_plastic_vase()
-000226f0: 0a20 2020 203e 3e3e 206d 6573 682e 706c  .    >>> mesh.pl
-00022700: 6f74 2829 0a0a 2020 2020 5265 7475 726e  ot()..    Return
-00022710: 2074 6865 2073 7461 7469 7374 6963 7320   the statistics 
-00022720: 6f66 2074 6865 2064 6174 6173 6574 2e0a  of the dataset..
-00022730: 0a20 2020 203e 3e3e 206d 6573 6820 2023  .    >>> mesh  #
-00022740: 2064 6f63 7465 7374 3a2b 534b 4950 0a20   doctest:+SKIP. 
-00022750: 2020 2050 6f6c 7944 6174 6120 2830 7837     PolyData (0x7
-00022760: 6665 3863 6164 6331 3463 3029 0a20 2020  fe8cadc14c0).   
-00022770: 2020 204e 2043 656c 6c73 3a20 2020 2020     N Cells:     
-00022780: 2033 3537 3039 3637 0a20 2020 2020 204e   3570967.      N
-00022790: 2050 6f69 6e74 733a 2020 2020 2031 3739   Points:     179
-000227a0: 3638 3035 0a20 2020 2020 2058 2042 6f75  6805.      X Bou
-000227b0: 6e64 733a 2020 2020 202d 312e 3336 3465  nds:     -1.364e
-000227c0: 2b30 322c 2031 2e39 3239 652b 3032 0a20  +02, 1.929e+02. 
-000227d0: 2020 2020 2059 2042 6f75 6e64 733a 2020       Y Bounds:  
-000227e0: 2020 202d 312e 3637 3765 2b30 322c 2031     -1.677e+02, 1
-000227f0: 2e36 3033 652b 3032 0a20 2020 2020 205a  .603e+02.      Z
-00022800: 2042 6f75 6e64 733a 2020 2020 2031 2e32   Bounds:     1.2
-00022810: 3039 652b 3032 2c20 342e 3039 3065 2b30  09e+02, 4.090e+0
-00022820: 320a 2020 2020 2020 4e20 4172 7261 7973  2.      N Arrays
-00022830: 3a20 2020 2020 300a 0a20 2020 2022 2222  :     0..    """
-00022840: 0a20 2020 2066 696c 656e 616d 6520 3d20  .    filename = 
-00022850: 5f64 6f77 6e6c 6f61 645f 6172 6368 6976  _download_archiv
-00022860: 6528 0a20 2020 2020 2020 2027 6976 616e  e(.        'ivan
-00022870: 2d6e 696b 6f6c 6f76 2f70 6c61 7374 6963  -nikolov/plastic
-00022880: 5661 7365 2e7a 6970 272c 0a20 2020 2020  Vase.zip',.     
-00022890: 2020 2027 706c 6173 7469 6356 6173 652e     'plasticVase.
-000228a0: 7674 7027 2c0a 2020 2020 290a 2020 2020  vtp',.    ).    
-000228b0: 6966 206c 6f61 643a 0a20 2020 2020 2020  if load:.       
-000228c0: 2072 6574 7572 6e20 7079 7669 7374 612e   return pyvista.
-000228d0: 7265 6164 2866 696c 656e 616d 6529 0a20  read(filename). 
-000228e0: 2020 2072 6574 7572 6e20 6669 6c65 6e61     return filena
-000228f0: 6d65 0a0a 0a64 6566 2064 6f77 6e6c 6f61  me...def downloa
-00022900: 645f 7365 615f 7661 7365 286c 6f61 643d  d_sea_vase(load=
-00022910: 5472 7565 293a 2020 2320 7072 6167 6d61  True):  # pragma
-00022920: 3a20 6e6f 2063 6f76 6572 0a20 2020 2022  : no cover.    "
-00022930: 2222 446f 776e 6c6f 6164 2061 2073 6361  ""Download a sca
-00022940: 6e20 6f66 2061 2073 6561 2076 6173 6520  n of a sea vase 
-00022950: 6372 6561 7465 6420 6279 2049 7661 6e20  created by Ivan 
-00022960: 4e69 6b6f 6c6f 762e 0a0a 2020 2020 5468  Nikolov...    Th
-00022970: 6520 6461 7461 7365 7420 7761 7320 646f  e dataset was do
-00022980: 776e 6c6f 6164 6564 2066 726f 6d20 6047  wnloaded from `G
-00022990: 4747 2d42 656e 6368 6d61 726b 5366 4d3a  GG-BenchmarkSfM:
-000229a0: 2044 6174 6173 6574 2066 6f72 2042 656e   Dataset for Ben
-000229b0: 6368 6d61 726b 696e 670a 2020 2020 436c  chmarking.    Cl
-000229c0: 6f73 652d 7261 6e67 6520 5366 4d20 536f  ose-range SfM So
-000229d0: 6674 7761 7265 2050 6572 666f 726d 616e  ftware Performan
-000229e0: 6365 2075 6e64 6572 2056 6172 7969 6e67  ce under Varying
-000229f0: 2043 6170 7475 7269 6e67 2043 6f6e 6469   Capturing Condi
-00022a00: 7469 6f6e 730a 2020 2020 3c68 7474 7073  tions.    <https
-00022a10: 3a2f 2f64 6174 612e 6d65 6e64 656c 6579  ://data.mendeley
-00022a20: 2e63 6f6d 2f64 6174 6173 6574 732f 627a  .com/datasets/bz
-00022a30: 786b 326e 3738 7339 2f34 3e60 5f0a 0a20  xk2n78s9/4>`_.. 
-00022a40: 2020 204f 7269 6769 6e61 6c20 6461 7461     Original data
-00022a50: 7365 7473 2061 7265 2075 6e64 6572 2074  sets are under t
-00022a60: 6865 2043 4320 4259 2034 2e30 206c 6963  he CC BY 4.0 lic
-00022a70: 656e 7365 2e0a 0a20 2020 2046 6f72 206d  ense...    For m
-00022a80: 6f72 6520 6465 7461 696c 732c 2073 6565  ore details, see
-00022a90: 2060 4976 616e 204e 696b 6f6c 6f76 2044   `Ivan Nikolov D
-00022aa0: 6174 6173 6574 730a 2020 2020 3c68 7474  atasets.    <htt
-00022ab0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00022ac0: 7079 7669 7374 612f 7674 6b2d 6461 7461  pyvista/vtk-data
-00022ad0: 2f74 7265 652f 6d61 7374 6572 2f44 6174  /tree/master/Dat
-00022ae0: 612f 6976 616e 2d6e 696b 6f6c 6f76 3e60  a/ivan-nikolov>`
-00022af0: 5f0a 0a20 2020 2050 6172 616d 6574 6572  _..    Parameter
-00022b00: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00022b10: 0a20 2020 206c 6f61 6420 3a20 626f 6f6c  .    load : bool
-00022b20: 2c20 6465 6661 756c 743a 2054 7275 650a  , default: True.
-00022b30: 2020 2020 2020 2020 4c6f 6164 2074 6865          Load the
-00022b40: 2064 6174 6173 6574 2061 6674 6572 2064   dataset after d
-00022b50: 6f77 6e6c 6f61 6469 6e67 2069 7420 7768  ownloading it wh
-00022b60: 656e 2060 6054 7275 6560 602e 2020 5365  en ``True``.  Se
-00022b70: 7420 7468 6973 0a20 2020 2020 2020 2074  t this.        t
-00022b80: 6f20 6060 4661 6c73 6560 6020 616e 6420  o ``False`` and 
-00022b90: 6f6e 6c79 2074 6865 2066 696c 656e 616d  only the filenam
-00022ba0: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
-00022bb0: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
-00022bc0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00022bd0: 2070 7976 6973 7461 2e50 6f6c 7944 6174   pyvista.PolyDat
-00022be0: 6120 7c20 7374 720a 2020 2020 2020 2020  a | str.        
-00022bf0: 4461 7461 5365 7420 6f72 2066 696c 656e  DataSet or filen
-00022c00: 616d 6520 6465 7065 6e64 696e 6720 6f6e  ame depending on
-00022c10: 2060 606c 6f61 6460 602e 0a0a 2020 2020   ``load``...    
-00022c20: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
-00022c30: 2d2d 2d2d 2d0a 2020 2020 446f 776e 6c6f  -----.    Downlo
-00022c40: 6164 2061 6e64 2070 6c6f 7420 7468 6520  ad and plot the 
-00022c50: 6461 7461 7365 742e 0a0a 2020 2020 3e3e  dataset...    >>
-00022c60: 3e20 6672 6f6d 2070 7976 6973 7461 2069  > from pyvista i
-00022c70: 6d70 6f72 7420 6578 616d 706c 6573 0a20  mport examples. 
-00022c80: 2020 203e 3e3e 206d 6573 6820 3d20 6578     >>> mesh = ex
-00022c90: 616d 706c 6573 2e64 6f77 6e6c 6f61 645f  amples.download_
-00022ca0: 7365 615f 7661 7365 2829 0a20 2020 203e  sea_vase().    >
-00022cb0: 3e3e 206d 6573 682e 706c 6f74 2829 0a0a  >> mesh.plot()..
-00022cc0: 2020 2020 5265 7475 726e 2074 6865 2073      Return the s
-00022cd0: 7461 7469 7374 6963 7320 6f66 2074 6865  tatistics of the
-00022ce0: 2064 6174 6173 6574 2e0a 0a20 2020 203e   dataset...    >
-00022cf0: 3e3e 206d 6573 6820 2023 2064 6f63 7465  >> mesh  # docte
-00022d00: 7374 3a2b 534b 4950 0a20 2020 2050 6f6c  st:+SKIP.    Pol
-00022d10: 7944 6174 6120 2830 7837 6665 3862 3338  yData (0x7fe8b38
-00022d20: 3632 3436 3029 0a20 2020 2020 204e 2043  62460).      N C
-00022d30: 656c 6c73 3a20 2020 2020 2033 3534 3834  ells:      35484
-00022d40: 3733 0a20 2020 2020 204e 2050 6f69 6e74  73.      N Point
-00022d50: 733a 2020 2020 2031 3831 3030 3132 0a20  s:     1810012. 
-00022d60: 2020 2020 2058 2042 6f75 6e64 733a 2020       X Bounds:  
-00022d70: 2020 202d 312e 3636 3665 2b30 322c 2031     -1.666e+02, 1
-00022d80: 2e34 3635 652b 3032 0a20 2020 2020 2059  .465e+02.      Y
-00022d90: 2042 6f75 6e64 733a 2020 2020 202d 312e   Bounds:     -1.
-00022da0: 3734 3265 2b30 322c 2031 2e33 3834 652b  742e+02, 1.384e+
-00022db0: 3032 0a20 2020 2020 205a 2042 6f75 6e64  02.      Z Bound
-00022dc0: 733a 2020 2020 202d 312e 3530 3065 2b30  s:     -1.500e+0
-00022dd0: 322c 2032 2e39 3932 652b 3032 0a20 2020  2, 2.992e+02.   
-00022de0: 2020 204e 2041 7272 6179 733a 2020 2020     N Arrays:    
-00022df0: 2030 0a0a 2020 2020 2222 220a 2020 2020   0..    """.    
-00022e00: 6669 6c65 6e61 6d65 203d 205f 646f 776e  filename = _down
-00022e10: 6c6f 6164 5f61 7263 6869 7665 280a 2020  load_archive(.  
-00022e20: 2020 2020 2020 2769 7661 6e2d 6e69 6b6f        'ivan-niko
-00022e30: 6c6f 762f 7365 6156 6173 652e 7a69 7027  lov/seaVase.zip'
-00022e40: 2c0a 2020 2020 2020 2020 2773 6561 5661  ,.        'seaVa
-00022e50: 7365 2e76 7470 272c 0a20 2020 2029 0a20  se.vtp',.    ). 
-00022e60: 2020 2069 6620 6c6f 6164 3a0a 2020 2020     if load:.    
-00022e70: 2020 2020 7265 7475 726e 2070 7976 6973      return pyvis
-00022e80: 7461 2e72 6561 6428 6669 6c65 6e61 6d65  ta.read(filename
-00022e90: 290a 2020 2020 7265 7475 726e 2066 696c  ).    return fil
-00022ea0: 656e 616d 650a 0a0a 6465 6620 646f 776e  ename...def down
-00022eb0: 6c6f 6164 5f64 696b 686f 6c6f 6c6f 5f6e  load_dikhololo_n
-00022ec0: 6967 6874 2829 3a20 2023 2070 7261 676d  ight():  # pragm
-00022ed0: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
-00022ee0: 2222 2244 6f77 6e6c 6f61 6420 616e 6420  """Download and 
-00022ef0: 7265 6164 2074 6865 2064 696b 686f 6c6f  read the dikholo
-00022f00: 206e 6967 6874 2068 6472 2074 6578 7475   night hdr textu
-00022f10: 7265 2065 7861 6d70 6c65 2e0a 0a20 2020  re example...   
-00022f20: 2046 696c 6573 2068 6f73 7465 6420 6174   Files hosted at
-00022f30: 2068 7474 7073 3a2f 2f70 6f6c 7968 6176   https://polyhav
-00022f40: 656e 2e63 6f6d 2f0a 0a20 2020 2052 6574  en.com/..    Ret
-00022f50: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-00022f60: 0a20 2020 2070 7976 6973 7461 2e54 6578  .    pyvista.Tex
-00022f70: 7475 7265 0a20 2020 2020 2020 2048 4452  ture.        HDR
-00022f80: 2054 6578 7475 7265 2e0a 0a20 2020 2045   Texture...    E
-00022f90: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
-00022fa0: 2d2d 2d2d 0a20 2020 203e 3e3e 2069 6d70  ----.    >>> imp
-00022fb0: 6f72 7420 7079 7669 7374 610a 2020 2020  ort pyvista.    
-00022fc0: 3e3e 3e20 6672 6f6d 2070 7976 6973 7461  >>> from pyvista
-00022fd0: 2069 6d70 6f72 7420 6578 616d 706c 6573   import examples
-00022fe0: 0a20 2020 203e 3e3e 2067 6c74 665f 6669  .    >>> gltf_fi
-00022ff0: 6c65 203d 2065 7861 6d70 6c65 732e 676c  le = examples.gl
-00023000: 7466 2e64 6f77 6e6c 6f61 645f 6461 6d61  tf.download_dama
-00023010: 6765 645f 6865 6c6d 6574 2829 0a20 2020  ged_helmet().   
-00023020: 203e 3e3e 2074 6578 7475 7265 203d 2065   >>> texture = e
-00023030: 7861 6d70 6c65 732e 646f 776e 6c6f 6164  xamples.download
-00023040: 5f64 696b 686f 6c6f 6c6f 5f6e 6967 6874  _dikhololo_night
-00023050: 2829 0a20 2020 203e 3e3e 2070 6c20 3d20  ().    >>> pl = 
-00023060: 7079 7669 7374 612e 506c 6f74 7465 7228  pyvista.Plotter(
-00023070: 290a 2020 2020 3e3e 3e20 706c 2e69 6d70  ).    >>> pl.imp
-00023080: 6f72 745f 676c 7466 2867 6c74 665f 6669  ort_gltf(gltf_fi
-00023090: 6c65 290a 2020 2020 3e3e 3e20 706c 2e73  le).    >>> pl.s
-000230a0: 6574 5f65 6e76 6972 6f6e 6d65 6e74 5f74  et_environment_t
-000230b0: 6578 7475 7265 2874 6578 7475 7265 290a  exture(texture).
-000230c0: 2020 2020 3e3e 3e20 706c 2e73 686f 7728      >>> pl.show(
-000230d0: 290a 0a20 2020 2022 2222 0a20 2020 2074  )..    """.    t
-000230e0: 6578 7475 7265 203d 205f 646f 776e 6c6f  exture = _downlo
-000230f0: 6164 5f61 6e64 5f72 6561 6428 2764 696b  ad_and_read('dik
-00023100: 686f 6c6f 6c6f 5f6e 6967 6874 5f34 6b2e  hololo_night_4k.
-00023110: 6864 7227 2c20 7465 7874 7572 653d 5472  hdr', texture=Tr
-00023120: 7565 290a 2020 2020 7465 7874 7572 652e  ue).    texture.
-00023130: 5365 7443 6f6c 6f72 4d6f 6465 546f 4469  SetColorModeToDi
-00023140: 7265 6374 5363 616c 6172 7328 290a 2020  rectScalars().  
-00023150: 2020 7465 7874 7572 652e 5365 744d 6970    texture.SetMip
-00023160: 6d61 7028 5472 7565 290a 2020 2020 7465  map(True).    te
-00023170: 7874 7572 652e 5365 7449 6e74 6572 706f  xture.SetInterpo
-00023180: 6c61 7465 2854 7275 6529 0a20 2020 2072  late(True).    r
-00023190: 6574 7572 6e20 7465 7874 7572 650a 0a0a  eturn texture...
-000231a0: 6465 6620 646f 776e 6c6f 6164 5f63 6164  def download_cad
-000231b0: 5f6d 6f64 656c 5f63 6173 6528 6c6f 6164  _model_case(load
-000231c0: 3d54 7275 6529 3a20 2023 2070 7261 676d  =True):  # pragm
-000231d0: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
-000231e0: 2222 2244 6f77 6e6c 6f61 6420 6120 4341  """Download a CA
-000231f0: 4420 6d6f 6465 6c20 6f66 2061 2052 6173  D model of a Ras
-00023200: 7062 6572 7279 2050 4920 3420 6361 7365  pberry PI 4 case
-00023210: 2e0a 0a20 2020 2054 6865 2064 6174 6173  ...    The datas
-00023220: 6574 2077 6173 2064 6f77 6e6c 6f61 6465  et was downloade
-00023230: 6420 6672 6f6d 2060 5468 696e 6769 7665  d from `Thingive
-00023240: 7273 650a 2020 2020 3c68 7474 7073 3a2f  rse.    <https:/
-00023250: 2f77 7777 2e74 6869 6e67 6976 6572 7365  /www.thingiverse
-00023260: 2e63 6f6d 2f74 6869 6e67 3a34 3934 3737  .com/thing:49477
-00023270: 3436 3e60 5f0a 0a20 2020 204f 7269 6769  46>`_..    Origi
-00023280: 6e61 6c20 6461 7461 7365 7473 2061 7265  nal datasets are
-00023290: 2075 6e64 6572 2074 6865 2060 4372 6561   under the `Crea
-000232a0: 7469 7665 2043 6f6d 6d6f 6e73 202d 2041  tive Commons - A
-000232b0: 7474 7269 6275 7469 6f6e 0a20 2020 203c  ttribution.    <
-000232c0: 6874 7470 733a 2f2f 6372 6561 7469 7665  https://creative
-000232d0: 636f 6d6d 6f6e 732e 6f72 672f 6c69 6365  commons.org/lice
-000232e0: 6e73 6573 2f62 792f 342e 302f 3e60 5f20  nses/by/4.0/>`_ 
-000232f0: 6c69 6365 6e73 652e 0a0a 2020 2020 5061  license...    Pa
-00023300: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00023310: 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f 6164  -------.    load
-00023320: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-00023330: 3a20 5472 7565 0a20 2020 2020 2020 204c  : True.        L
-00023340: 6f61 6420 7468 6520 6461 7461 7365 7420  oad the dataset 
-00023350: 6166 7465 7220 646f 776e 6c6f 6164 696e  after downloadin
-00023360: 6720 6974 2077 6865 6e20 6060 5472 7565  g it when ``True
-00023370: 6060 2e20 2053 6574 2074 6869 730a 2020  ``.  Set this.  
-00023380: 2020 2020 2020 746f 2060 6046 616c 7365        to ``False
-00023390: 6060 2061 6e64 206f 6e6c 7920 7468 6520  `` and only the 
-000233a0: 6669 6c65 6e61 6d65 2077 696c 6c20 6265  filename will be
-000233b0: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
-000233c0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-000233d0: 2d2d 2d0a 2020 2020 7079 7669 7374 612e  ---.    pyvista.
-000233e0: 506f 6c79 4461 7461 207c 2073 7472 0a20  PolyData | str. 
-000233f0: 2020 2020 2020 2044 6174 6153 6574 206f         DataSet o
-00023400: 7220 6669 6c65 6e61 6d65 2064 6570 656e  r filename depen
-00023410: 6469 6e67 206f 6e20 6060 6c6f 6164 6060  ding on ``load``
-00023420: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
-00023430: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-00023440: 2044 6f77 6e6c 6f61 6420 616e 6420 706c   Download and pl
-00023450: 6f74 2074 6865 2064 6174 6173 6574 2e0a  ot the dataset..
-00023460: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
-00023470: 7669 7374 6120 696d 706f 7274 2065 7861  vista import exa
-00023480: 6d70 6c65 730a 2020 2020 3e3e 3e20 6d65  mples.    >>> me
-00023490: 7368 203d 2065 7861 6d70 6c65 732e 646f  sh = examples.do
-000234a0: 776e 6c6f 6164 5f63 6164 5f6d 6f64 656c  wnload_cad_model
-000234b0: 5f63 6173 6528 290a 2020 2020 3e3e 3e20  _case().    >>> 
-000234c0: 6d65 7368 2e70 6c6f 7428 290a 0a20 2020  mesh.plot()..   
-000234d0: 2052 6574 7572 6e20 7468 6520 7374 6174   Return the stat
-000234e0: 6973 7469 6373 206f 6620 7468 6520 6461  istics of the da
-000234f0: 7461 7365 742e 0a0a 2020 2020 3e3e 3e20  taset...    >>> 
-00023500: 6d65 7368 2020 2320 646f 6374 6573 743a  mesh  # doctest:
-00023510: 2b53 4b49 500a 2020 2020 506f 6c79 4461  +SKIP.    PolyDa
-00023520: 7461 2028 3078 3766 6430 3866 3166 6166  ta (0x7fd08f1faf
-00023530: 3430 290a 2020 2020 2020 4e20 4365 6c6c  40).      N Cell
-00023540: 733a 2020 2020 2020 3133 3730 320a 2020  s:      13702.  
-00023550: 2020 2020 4e20 506f 696e 7473 3a20 2020      N Points:   
-00023560: 2020 3638 3031 0a20 2020 2020 2058 2042    6801.      X B
-00023570: 6f75 6e64 733a 2020 2020 202d 362e 3436  ounds:     -6.46
-00023580: 3065 2d33 312c 2039 2e30 3030 652b 3031  0e-31, 9.000e+01
-00023590: 0a20 2020 2020 2059 2042 6f75 6e64 733a  .      Y Bounds:
-000235a0: 2020 2020 202d 332e 3533 3565 2d33 322c       -3.535e-32,
-000235b0: 2031 2e34 3830 652b 3032 0a20 2020 2020   1.480e+02.     
-000235c0: 205a 2042 6f75 6e64 733a 2020 2020 202d   Z Bounds:     -
-000235d0: 372e 3238 3765 2d31 332c 2032 2e30 3030  7.287e-13, 2.000
-000235e0: 652b 3031 0a20 2020 2020 204e 2041 7272  e+01.      N Arr
-000235f0: 6179 733a 2020 2020 2031 0a0a 2020 2020  ays:     1..    
-00023600: 2222 220a 2020 2020 7265 7475 726e 205f  """.    return _
-00023610: 646f 776e 6c6f 6164 5f61 6e64 5f72 6561  download_and_rea
-00023620: 6428 2763 6164 2f34 3934 3737 3436 2f56  d('cad/4947746/V
-00023630: 656e 7465 645f 5265 6172 5f43 6173 655f  ented_Rear_Case_
-00023640: 5769 7468 5f50 695f 5375 7070 6f72 7473  With_Pi_Supports
-00023650: 2e76 7470 272c 206c 6f61 643d 6c6f 6164  .vtp', load=load
-00023660: 290a 0a0a 6465 6620 646f 776e 6c6f 6164  )...def download
-00023670: 5f61 6572 6f5f 6272 6163 6b65 7428 6c6f  _aero_bracket(lo
-00023680: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
-00023690: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-000236a0: 2020 2222 2244 6f77 6e6c 6f61 6420 7468    """Download th
-000236b0: 6520 6669 6e69 7465 2065 6c65 6d65 6e74  e finite element
-000236c0: 2073 6f6c 7574 696f 6e20 6f66 2061 6e20   solution of an 
-000236d0: 6165 726f 2062 7261 636b 6574 2e0a 0a20  aero bracket... 
-000236e0: 2020 2044 6174 6120 6765 6e65 7261 7465     Data generate
-000236f0: 6420 6672 6f6d 2070 7562 6c69 6320 5369  d from public Si
-00023700: 6d53 6361 6c65 2065 7861 6d70 6c65 7320  mScale examples 
-00023710: 6174 2060 5369 6d53 6361 6c65 2050 726f  at `SimScale Pro
-00023720: 6a65 6374 204c 6962 7261 7279 202d 0a20  ject Library -. 
-00023730: 2020 2054 7572 626f 203c 6874 7470 733a     Turbo <https:
-00023740: 2f2f 7777 772e 7369 6d73 6361 6c65 2e63  //www.simscale.c
-00023750: 6f6d 2f70 726f 6a65 6374 732f 6179 6172  om/projects/ayar
-00023760: 6e6f 7a2f 7475 7262 6f2f 3e60 5f2e 0a0a  noz/turbo/>`_...
-00023770: 2020 2020 4c69 6365 6e73 696e 6720 666f      Licensing fo
-00023780: 7220 7468 6973 2064 6174 6173 6574 2069  r this dataset i
-00023790: 7320 6772 616e 7465 6420 746f 2066 7265  s granted to fre
-000237a0: 656c 7920 616e 6420 7769 7468 6f75 7420  ely and without 
-000237b0: 7265 7374 7269 6374 696f 6e0a 2020 2020  restriction.    
-000237c0: 7265 7072 6f64 7563 652c 2064 6973 7472  reproduce, distr
-000237d0: 6962 7574 652c 2070 7562 6c69 7368 2061  ibute, publish a
-000237e0: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-000237f0: 6053 696d 5363 616c 6520 5465 726d 7320  `SimScale Terms 
-00023800: 616e 640a 2020 2020 436f 6e64 6974 696f  and.    Conditio
-00023810: 6e73 203c 6874 7470 733a 2f2f 7777 772e  ns <https://www.
-00023820: 7369 6d73 6361 6c65 2e63 6f6d 2f74 6572  simscale.com/ter
-00023830: 6d73 2d61 6e64 2d63 6f6e 6469 7469 6f6e  ms-and-condition
-00023840: 732f 3e60 5f2e 0a0a 2020 2020 5468 6973  s/>`_...    This
-00023850: 2070 726f 6a65 6374 2064 656d 6f6e 7374   project demonst
-00023860: 7261 7465 7320 7468 6520 7374 6174 6963  rates the static
-00023870: 2073 7472 6573 7320 616e 616c 7973 6973   stress analysis
-00023880: 206f 6620 7468 7265 6520 6169 7263 7261   of three aircra
-00023890: 6674 0a20 2020 2065 6e67 696e 6520 6265  ft.    engine be
-000238a0: 6172 696e 6720 6272 6163 6b65 7420 6d6f  aring bracket mo
-000238b0: 6465 6c73 2063 6f6e 7369 6465 7269 6e67  dels considering
-000238c0: 2062 6f74 6820 6c69 6e65 6172 2061 6e64   both linear and
-000238d0: 206e 6f6e 6c69 6e65 6172 0a20 2020 206d   nonlinear.    m
-000238e0: 6174 6572 6961 6c20 6465 6669 6e69 7469  aterial definiti
-000238f0: 6f6e 2e20 5468 6520 6d6f 6465 6c73 2061  on. The models a
-00023900: 7265 2074 6573 7465 6420 7769 7468 2068  re tested with h
-00023910: 6f72 697a 6f6e 7461 6c20 616e 6420 7665  orizontal and ve
-00023920: 7274 6963 616c 0a20 2020 206c 6f61 6469  rtical.    loadi
-00023930: 6e67 2063 6f6e 6469 7469 6f6e 7320 6173  ng conditions as
-00023940: 2070 726f 7669 6465 6420 6f6e 2074 6865   provided on the
-00023950: 2060 4772 6162 4341 4420 2d20 4169 7270   `GrabCAD - Airp
-00023960: 6c61 6e65 2042 6561 7269 6e67 2042 7261  lane Bearing Bra
-00023970: 636b 6574 0a20 2020 2043 6861 6c6c 656e  cket.    Challen
-00023980: 6765 0a20 2020 203c 6874 7470 733a 2f2f  ge.    <https://
-00023990: 6772 6162 6361 642e 636f 6d2f 6368 616c  grabcad.com/chal
-000239a0: 6c65 6e67 6573 2f61 6972 706c 616e 652d  lenges/airplane-
-000239b0: 6265 6172 696e 672d 6272 6163 6b65 742d  bearing-bracket-
-000239c0: 6368 616c 6c65 6e67 652f 656e 7472 6965  challenge/entrie
-000239d0: 733e 605f 2e0a 0a20 2020 2050 6172 616d  s>`_...    Param
-000239e0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-000239f0: 2d2d 2d2d 0a20 2020 206c 6f61 6420 3a20  ----.    load : 
-00023a00: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
-00023a10: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
-00023a20: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
-00023a30: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
-00023a40: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
-00023a50: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
-00023a60: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
-00023a70: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
-00023a80: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
-00023a90: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
-00023aa0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-00023ab0: 0a20 2020 2070 7976 6973 7461 2e55 6e73  .    pyvista.Uns
-00023ac0: 7472 7563 7475 7265 6447 7269 6420 7c20  tructuredGrid | 
-00023ad0: 7374 720a 2020 2020 2020 2020 4461 7461  str.        Data
-00023ae0: 5365 7420 6f72 2066 696c 656e 616d 6520  Set or filename 
-00023af0: 6465 7065 6e64 696e 6720 6f6e 2060 606c  depending on ``l
-00023b00: 6f61 6460 602e 0a0a 2020 2020 4578 616d  oad``...    Exam
-00023b10: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-00023b20: 2d0a 2020 2020 446f 776e 6c6f 6164 2074  -.    Download t
-00023b30: 6865 2061 6572 6f20 6272 6163 6b65 742e  he aero bracket.
-00023b40: 0a0a 2020 2020 3e3e 3e20 6672 6f6d 2070  ..    >>> from p
-00023b50: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
-00023b60: 616d 706c 6573 0a20 2020 203e 3e3e 2064  amples.    >>> d
-00023b70: 6174 6173 6574 203d 2065 7861 6d70 6c65  ataset = example
-00023b80: 732e 646f 776e 6c6f 6164 5f61 6572 6f5f  s.download_aero_
-00023b90: 6272 6163 6b65 7428 290a 2020 2020 3e3e  bracket().    >>
-00023ba0: 3e20 6461 7461 7365 7420 2023 2064 6f63  > dataset  # doc
-00023bb0: 7465 7374 3a2b 534b 4950 0a20 2020 2055  test:+SKIP.    U
-00023bc0: 6e73 7472 7563 7475 7265 6447 7269 6420  nstructuredGrid 
-00023bd0: 2830 7837 6634 3339 6161 3263 6163 3029  (0x7f439aa2cac0)
-00023be0: 0a20 2020 2020 204e 2043 656c 6c73 3a20  .      N Cells: 
-00023bf0: 2020 2031 3137 3239 320a 2020 2020 2020     117292.      
-00023c00: 4e20 506f 696e 7473 3a20 2020 3138 3730  N Points:   1870
-00023c10: 3337 0a20 2020 2020 2058 2042 6f75 6e64  37.      X Bound
-00023c20: 733a 2020 202d 362e 3835 3865 2d30 332c  s:   -6.858e-03,
-00023c30: 2031 2e31 3138 652d 3031 0a20 2020 2020   1.118e-01.     
-00023c40: 2059 2042 6f75 6e64 733a 2020 202d 312e   Y Bounds:   -1.
-00023c50: 3233 3765 2d30 322c 2036 2e36 3334 652d  237e-02, 6.634e-
-00023c60: 3032 0a20 2020 2020 205a 2042 6f75 6e64  02.      Z Bound
-00023c70: 733a 2020 202d 312e 3633 3865 2d30 322c  s:   -1.638e-02,
-00023c80: 2031 2e36 3338 652d 3032 0a20 2020 2020   1.638e-02.     
-00023c90: 204e 2041 7272 6179 733a 2020 2033 0a0a   N Arrays:   3..
-00023ca0: 2020 2020 5368 6f77 2074 6865 2061 7661      Show the ava
-00023cb0: 696c 6162 6c65 2070 6f69 6e74 2064 6174  ilable point dat
-00023cc0: 6120 6172 7261 7973 2e0a 0a20 2020 203e  a arrays...    >
-00023cd0: 3e3e 2064 6174 6173 6574 2e70 6f69 6e74  >> dataset.point
-00023ce0: 5f64 6174 610a 2020 2020 7079 7669 7374  _data.    pyvist
-00023cf0: 6120 4461 7461 5365 7441 7474 7269 6275  a DataSetAttribu
-00023d00: 7465 730a 2020 2020 4173 736f 6369 6174  tes.    Associat
-00023d10: 696f 6e20 2020 2020 3a20 504f 494e 540a  ion     : POINT.
-00023d20: 2020 2020 4163 7469 7665 2053 6361 6c61      Active Scala
-00023d30: 7273 2020 3a20 4e6f 6e65 0a20 2020 2041  rs  : None.    A
-00023d40: 6374 6976 6520 5665 6374 6f72 7320 203a  ctive Vectors  :
-00023d50: 204e 6f6e 650a 2020 2020 4163 7469 7665   None.    Active
-00023d60: 2054 6578 7475 7265 2020 3a20 4e6f 6e65   Texture  : None
-00023d70: 0a20 2020 2041 6374 6976 6520 4e6f 726d  .    Active Norm
-00023d80: 616c 7320 203a 204e 6f6e 650a 2020 2020  als  : None.    
-00023d90: 436f 6e74 6169 6e73 2061 7272 6179 7320  Contains arrays 
-00023da0: 3a0a 2020 2020 2020 2020 6469 7370 6c61  :.        displa
-00023db0: 6365 6d65 6e74 2020 2020 2020 2020 2020  cement          
-00023dc0: 2020 666c 6f61 7433 3220 2020 2028 3138    float32    (18
-00023dd0: 3730 3337 2c20 3329 0a20 2020 2020 2020  7037, 3).       
-00023de0: 2074 6f74 616c 206e 6f6e 6c69 6e65 6172   total nonlinear
-00023df0: 2073 7472 6169 6e20 2066 6c6f 6174 3332   strain  float32
-00023e00: 2020 2020 2831 3837 3033 372c 2036 290a      (187037, 6).
-00023e10: 2020 2020 2020 2020 766f 6e20 4d69 7365          von Mise
-00023e20: 7320 7374 7265 7373 2020 2020 2020 2020  s stress        
-00023e30: 666c 6f61 7433 3220 2020 2028 3138 3730  float32    (1870
-00023e40: 3337 2c29 0a0a 2020 2020 506c 6f74 2074  37,)..    Plot t
-00023e50: 6865 2076 6f6e 204d 6973 6573 2073 7472  he von Mises str
-00023e60: 6573 732e 0a0a 2020 2020 3e3e 3e20 6370  ess...    >>> cp
-00023e70: 6f73 203d 205b 0a20 2020 202e 2e2e 2020  os = [.    ...  
-00023e80: 2020 2028 2d30 2e30 3530 332c 2030 2e31     (-0.0503, 0.1
-00023e90: 3332 2c20 2d30 2e31 3739 292c 0a20 2020  32, -0.179),.   
-00023ea0: 202e 2e2e 2020 2020 2028 302e 3035 3035   ...     (0.0505
-00023eb0: 2c20 302e 3031 3835 2c20 2d30 2e30 3032  , 0.0185, -0.002
-00023ec0: 3031 292c 0a20 2020 202e 2e2e 2020 2020  01),.    ...    
-00023ed0: 2028 302e 3237 352c 2030 2e38 3732 2c20   (0.275, 0.872, 
-00023ee0: 302e 3430 3529 2c0a 2020 2020 2e2e 2e20  0.405),.    ... 
-00023ef0: 5d0a 2020 2020 3e3e 3e20 6461 7461 7365  ].    >>> datase
-00023f00: 742e 706c 6f74 280a 2020 2020 2e2e 2e20  t.plot(.    ... 
-00023f10: 2020 2020 736d 6f6f 7468 5f73 6861 6469      smooth_shadi
-00023f20: 6e67 3d54 7275 652c 0a20 2020 202e 2e2e  ng=True,.    ...
-00023f30: 2020 2020 2073 706c 6974 5f73 6861 7270       split_sharp
-00023f40: 5f65 6467 6573 3d54 7275 652c 0a20 2020  _edges=True,.   
-00023f50: 202e 2e2e 2020 2020 2073 6361 6c61 7273   ...     scalars
-00023f60: 3d27 766f 6e20 4d69 7365 7320 7374 7265  ='von Mises stre
-00023f70: 7373 272c 0a20 2020 202e 2e2e 2020 2020  ss',.    ...    
-00023f80: 2063 6d61 703d 2762 7772 272c 0a20 2020   cmap='bwr',.   
-00023f90: 202e 2e2e 2020 2020 2063 706f 733d 6370   ...     cpos=cp
-00023fa0: 6f73 2c0a 2020 2020 2e2e 2e20 2020 2020  os,.    ...     
-00023fb0: 616e 7469 5f61 6c69 6173 696e 673d 2766  anti_aliasing='f
-00023fc0: 7861 6127 2c0a 2020 2020 2e2e 2e20 290a  xaa',.    ... ).
-00023fd0: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
-00023fe0: 7572 6e20 5f64 6f77 6e6c 6f61 645f 616e  urn _download_an
-00023ff0: 645f 7265 6164 2827 6665 612f 6165 726f  d_read('fea/aero
-00024000: 5f62 7261 636b 6574 2f61 6572 6f5f 6272  _bracket/aero_br
-00024010: 6163 6b65 742e 7674 7527 2c20 6c6f 6164  acket.vtu', load
-00024020: 3d6c 6f61 6429 0a0a 0a64 6566 2064 6f77  =load)...def dow
-00024030: 6e6c 6f61 645f 636f 696c 5f6d 6167 6e65  nload_coil_magne
-00024040: 7469 635f 6669 656c 6428 6c6f 6164 3d54  tic_field(load=T
-00024050: 7275 6529 3a20 2023 2070 7261 676d 613a  rue):  # pragma:
-00024060: 206e 6f20 636f 7665 720a 2020 2020 2222   no cover.    ""
-00024070: 2244 6f77 6e6c 6f61 6420 7468 6520 6d61  "Download the ma
-00024080: 676e 6574 6963 2066 6965 6c64 206f 6620  gnetic field of 
-00024090: 6120 636f 696c 2e0a 0a20 2020 2054 6865  a coil...    The
-000240a0: 7365 2065 7861 6d70 6c65 7320 7765 7265  se examples were
-000240b0: 2067 656e 6572 6174 6564 2066 726f 6d20   generated from 
-000240c0: 7468 6520 666f 6c6c 6f77 696e 6720 6073  the following `s
-000240d0: 6372 6970 740a 2020 2020 3c68 7474 7073  cript.    <https
-000240e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-000240f0: 7669 7374 612f 7674 6b2d 6461 7461 2f74  vista/vtk-data/t
-00024100: 7265 652f 6d61 7374 6572 2f44 6174 612f  ree/master/Data/
-00024110: 6d61 6770 796c 6962 2f3e 605f 2e0a 0a20  magpylib/>`_... 
-00024120: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00024130: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00024140: 206c 6f61 6420 3a20 626f 6f6c 2c20 6465   load : bool, de
-00024150: 6661 756c 743a 2054 7275 650a 2020 2020  fault: True.    
-00024160: 2020 2020 4c6f 6164 2074 6865 2064 6174      Load the dat
-00024170: 6173 6574 2061 6674 6572 2064 6f77 6e6c  aset after downl
-00024180: 6f61 6469 6e67 2069 7420 7768 656e 2060  oading it when `
-00024190: 6054 7275 6560 602e 2020 5365 7420 7468  `True``.  Set th
-000241a0: 6973 0a20 2020 2020 2020 2074 6f20 6060  is.        to ``
-000241b0: 4661 6c73 6560 6020 616e 6420 6f6e 6c79  False`` and only
-000241c0: 2074 6865 2066 696c 656e 616d 6520 7769   the filename wi
-000241d0: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
-000241e0: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-000241f0: 202d 2d2d 2d2d 2d2d 0a20 2020 2070 7976   -------.    pyv
-00024200: 6973 7461 2e55 6e69 666f 726d 4772 6964  ista.UniformGrid
-00024210: 206f 7220 7374 720a 2020 2020 2020 2020   or str.        
-00024220: 4461 7461 5365 7420 6f72 2066 696c 656e  DataSet or filen
-00024230: 616d 6520 6465 7065 6e64 696e 6720 6f6e  ame depending on
-00024240: 2060 606c 6f61 6460 602e 0a0a 2020 2020   ``load``...    
-00024250: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
-00024260: 2d2d 2d2d 2d0a 2020 2020 446f 776e 6c6f  -----.    Downlo
-00024270: 6164 2074 6865 206d 6167 6e65 7469 6320  ad the magnetic 
-00024280: 6669 656c 6420 6461 7461 7365 7420 616e  field dataset an
-00024290: 6420 6765 6e65 7261 7465 2073 7472 6561  d generate strea
-000242a0: 6d6c 696e 6573 2066 726f 6d20 7468 6520  mlines from the 
-000242b0: 6669 656c 642e 0a0a 2020 2020 3e3e 3e20  field...    >>> 
-000242c0: 696d 706f 7274 2070 7976 6973 7461 2061  import pyvista a
-000242d0: 7320 7076 0a20 2020 203e 3e3e 2066 726f  s pv.    >>> fro
-000242e0: 6d20 7079 7669 7374 6120 696d 706f 7274  m pyvista import
-000242f0: 2065 7861 6d70 6c65 730a 2020 2020 3e3e   examples.    >>
-00024300: 3e20 6772 6964 203d 2065 7861 6d70 6c65  > grid = example
-00024310: 732e 646f 776e 6c6f 6164 5f63 6f69 6c5f  s.download_coil_
-00024320: 6d61 676e 6574 6963 5f66 6965 6c64 2829  magnetic_field()
-00024330: 0a20 2020 203e 3e3e 2073 6565 6420 3d20  .    >>> seed = 
-00024340: 7076 2e44 6973 6328 696e 6e65 723d 312c  pv.Disc(inner=1,
-00024350: 206f 7574 6572 3d35 2e32 2c20 725f 7265   outer=5.2, r_re
-00024360: 733d 332c 2063 5f72 6573 3d31 3229 0a20  s=3, c_res=12). 
-00024370: 2020 203e 3e3e 2073 7472 6c20 3d20 6772     >>> strl = gr
-00024380: 6964 2e73 7472 6561 6d6c 696e 6573 5f66  id.streamlines_f
-00024390: 726f 6d5f 736f 7572 6365 280a 2020 2020  rom_source(.    
-000243a0: 2e2e 2e20 2020 2020 7365 6564 2c0a 2020  ...     seed,.  
-000243b0: 2020 2e2e 2e20 2020 2020 7665 6374 6f72    ...     vector
-000243c0: 733d 2742 272c 0a20 2020 202e 2e2e 2020  s='B',.    ...  
-000243d0: 2020 206d 6178 5f74 696d 653d 3138 302c     max_time=180,
-000243e0: 0a20 2020 202e 2e2e 2020 2020 2069 6e69  .    ...     ini
-000243f0: 7469 616c 5f73 7465 705f 6c65 6e67 7468  tial_step_length
-00024400: 3d30 2e31 2c0a 2020 2020 2e2e 2e20 2020  =0.1,.    ...   
-00024410: 2020 696e 7465 6772 6174 696f 6e5f 6469    integration_di
-00024420: 7265 6374 696f 6e3d 2762 6f74 6827 2c0a  rection='both',.
-00024430: 2020 2020 2e2e 2e20 290a 2020 2020 3e3e      ... ).    >>
-00024440: 3e20 7374 726c 2e70 6c6f 7428 0a20 2020  > strl.plot(.   
-00024450: 202e 2e2e 2020 2020 2063 6d61 703d 2770   ...     cmap='p
-00024460: 6c61 736d 6127 2c0a 2020 2020 2e2e 2e20  lasma',.    ... 
-00024470: 2020 2020 7265 6e64 6572 5f6c 696e 6573      render_lines
-00024480: 5f61 735f 7475 6265 733d 5472 7565 2c0a  _as_tubes=True,.
-00024490: 2020 2020 2e2e 2e20 2020 2020 6c69 6e65      ...     line
-000244a0: 5f77 6964 7468 3d32 2c0a 2020 2020 2e2e  _width=2,.    ..
-000244b0: 2e20 2020 2020 6c69 6768 7469 6e67 3d46  .     lighting=F
-000244c0: 616c 7365 2c0a 2020 2020 2e2e 2e20 2020  alse,.    ...   
-000244d0: 2020 7a6f 6f6d 3d32 2c0a 2020 2020 2e2e    zoom=2,.    ..
-000244e0: 2e20 290a 0a20 2020 2050 6c6f 7420 7468  . )..    Plot th
-000244f0: 6520 6d61 676e 6574 2066 6965 6c64 2073  e magnet field s
-00024500: 7472 656e 6774 6820 696e 2074 6865 205a  trength in the Z
-00024510: 2064 6972 6563 7469 6f6e 2e0a 0a20 2020   direction...   
-00024520: 203e 3e3e 2069 6d70 6f72 7420 6e75 6d70   >>> import nump
-00024530: 7920 6173 206e 700a 2020 2020 3e3e 3e20  y as np.    >>> 
-00024540: 696d 706f 7274 2070 7976 6973 7461 2061  import pyvista a
-00024550: 7320 7076 0a20 2020 203e 3e3e 2066 726f  s pv.    >>> fro
-00024560: 6d20 7079 7669 7374 6120 696d 706f 7274  m pyvista import
-00024570: 2065 7861 6d70 6c65 730a 2020 2020 3e3e   examples.    >>
-00024580: 3e20 6772 6964 203d 2065 7861 6d70 6c65  > grid = example
-00024590: 732e 646f 776e 6c6f 6164 5f63 6f69 6c5f  s.download_coil_
-000245a0: 6d61 676e 6574 6963 5f66 6965 6c64 2829  magnetic_field()
-000245b0: 0a20 2020 203e 3e3e 2023 2063 7265 6174  .    >>> # creat
-000245c0: 6520 636f 696c 730a 2020 2020 3e3e 3e20  e coils.    >>> 
-000245d0: 636f 696c 7320 3d20 5b5d 0a20 2020 203e  coils = [].    >
-000245e0: 3e3e 2066 6f72 207a 2069 6e20 6e70 2e6c  >> for z in np.l
-000245f0: 696e 7370 6163 6528 2d38 2c20 382c 2031  inspace(-8, 8, 1
-00024600: 3629 3a0a 2020 2020 2e2e 2e20 2020 2020  6):.    ...     
-00024610: 636f 696c 732e 6170 7065 6e64 280a 2020  coils.append(.  
-00024620: 2020 2e2e 2e20 2020 2020 2020 2020 7076    ...         pv
-00024630: 2e50 6f6c 7967 6f6e 2828 302c 2030 2c20  .Polygon((0, 0, 
-00024640: 7a29 2c20 7261 6469 7573 3d35 2c20 6e5f  z), radius=5, n_
-00024650: 7369 6465 733d 3130 302c 2066 696c 6c3d  sides=100, fill=
-00024660: 4661 6c73 6529 0a20 2020 202e 2e2e 2020  False).    ...  
-00024670: 2020 2029 0a20 2020 202e 2e2e 0a20 2020     ).    ....   
-00024680: 203e 3e3e 2063 6f69 6c73 203d 2070 762e   >>> coils = pv.
-00024690: 4d75 6c74 6942 6c6f 636b 2863 6f69 6c73  MultiBlock(coils
-000246a0: 290a 2020 2020 3e3e 3e20 2320 706c 6f74  ).    >>> # plot
-000246b0: 2074 6865 206d 6167 6e65 7420 6669 656c   the magnet fiel
-000246c0: 6420 7374 7265 6e67 7468 2069 6e20 7468  d strength in th
-000246d0: 6520 5a20 6469 7265 6374 696f 6e0a 2020  e Z direction.  
-000246e0: 2020 3e3e 3e20 7363 616c 6172 7320 3d20    >>> scalars = 
-000246f0: 6e70 2e61 6273 2867 7269 645b 2742 275d  np.abs(grid['B']
-00024700: 5b3a 2c20 325d 290a 2020 2020 3e3e 3e20  [:, 2]).    >>> 
-00024710: 706c 203d 2070 762e 506c 6f74 7465 7228  pl = pv.Plotter(
-00024720: 290a 2020 2020 3e3e 3e20 5f20 3d20 706c  ).    >>> _ = pl
-00024730: 2e61 6464 5f6d 6573 6828 0a20 2020 202e  .add_mesh(.    .
-00024740: 2e2e 2020 2020 2063 6f69 6c73 2c20 7265  ..     coils, re
-00024750: 6e64 6572 5f6c 696e 6573 5f61 735f 7475  nder_lines_as_tu
-00024760: 6265 733d 5472 7565 2c20 6c69 6e65 5f77  bes=True, line_w
-00024770: 6964 7468 3d35 2c20 636f 6c6f 723d 2777  idth=5, color='w
-00024780: 270a 2020 2020 2e2e 2e20 290a 2020 2020  '.    ... ).    
-00024790: 3e3e 3e20 766f 6c20 3d20 706c 2e61 6464  >>> vol = pl.add
-000247a0: 5f76 6f6c 756d 6528 0a20 2020 202e 2e2e  _volume(.    ...
-000247b0: 2020 2020 2067 7269 642c 0a20 2020 202e       grid,.    .
-000247c0: 2e2e 2020 2020 2073 6361 6c61 7273 3d73  ..     scalars=s
-000247d0: 6361 6c61 7273 2c0a 2020 2020 2e2e 2e20  calars,.    ... 
-000247e0: 2020 2020 636d 6170 3d27 706c 6173 6d61      cmap='plasma
-000247f0: 272c 0a20 2020 202e 2e2e 2020 2020 2073  ',.    ...     s
-00024800: 686f 775f 7363 616c 6172 5f62 6172 3d46  how_scalar_bar=F
-00024810: 616c 7365 2c0a 2020 2020 2e2e 2e20 2020  alse,.    ...   
-00024820: 2020 6c6f 675f 7363 616c 653d 5472 7565    log_scale=True
-00024830: 2c0a 2020 2020 2e2e 2e20 2020 2020 6f70  ,.    ...     op
-00024840: 6163 6974 793d 2773 6967 6d6f 6964 5f32  acity='sigmoid_2
-00024850: 272c 0a20 2020 202e 2e2e 2029 0a20 2020  ',.    ... ).   
-00024860: 203e 3e3e 2076 6f6c 2e70 726f 702e 696e   >>> vol.prop.in
-00024870: 7465 7270 6f6c 6174 696f 6e5f 7479 7065  terpolation_type
-00024880: 203d 2027 6c69 6e65 6172 270a 2020 2020   = 'linear'.    
-00024890: 3e3e 3e20 5f20 3d20 706c 2e61 6464 5f76  >>> _ = pl.add_v
-000248a0: 6f6c 756d 655f 636c 6970 5f70 6c61 6e65  olume_clip_plane
-000248b0: 280a 2020 2020 2e2e 2e20 2020 2020 766f  (.    ...     vo
-000248c0: 6c2c 0a20 2020 202e 2e2e 2020 2020 206e  l,.    ...     n
-000248d0: 6f72 6d61 6c3d 272d 7827 2c0a 2020 2020  ormal='-x',.    
-000248e0: 2e2e 2e20 2020 2020 6e6f 726d 616c 5f72  ...     normal_r
-000248f0: 6f74 6174 696f 6e3d 4661 6c73 652c 0a20  otation=False,. 
-00024900: 2020 202e 2e2e 2020 2020 2069 6e74 6572     ...     inter
-00024910: 6163 7469 6f6e 5f65 7665 6e74 3d27 616c  action_event='al
-00024920: 7761 7973 272c 0a20 2020 202e 2e2e 2020  ways',.    ...  
-00024930: 2020 2077 6964 6765 745f 636f 6c6f 723d     widget_color=
-00024940: 7076 2e43 6f6c 6f72 286f 7061 6369 7479  pv.Color(opacity
-00024950: 3d30 2e30 292c 0a20 2020 202e 2e2e 2029  =0.0),.    ... )
-00024960: 0a20 2020 203e 3e3e 2070 6c2e 656e 6162  .    >>> pl.enab
-00024970: 6c65 5f61 6e74 695f 616c 6961 7369 6e67  le_anti_aliasing
-00024980: 2829 0a20 2020 203e 3e3e 2070 6c2e 6361  ().    >>> pl.ca
-00024990: 6d65 7261 2e7a 6f6f 6d28 3229 0a20 2020  mera.zoom(2).   
-000249a0: 203e 3e3e 2070 6c2e 7368 6f77 2829 0a0a   >>> pl.show()..
-000249b0: 2020 2020 5365 6520 7468 6520 3a72 6566      See the :ref
-000249c0: 3a60 6d61 676e 6574 6963 5f66 6965 6c64  :`magnetic_field
-000249d0: 735f 6578 616d 706c 6560 2066 6f72 206d  s_example` for m
-000249e0: 6f72 6520 6465 7461 696c 7320 6f6e 2068  ore details on h
-000249f0: 6f77 2074 6f20 706c 6f74 2077 6974 680a  ow to plot with.
-00024a00: 2020 2020 7468 6973 2064 6174 6173 6574      this dataset
-00024a10: 2e0a 0a20 2020 2022 2222 0a20 2020 2072  ...    """.    r
-00024a20: 6574 7572 6e20 5f64 6f77 6e6c 6f61 645f  eturn _download_
-00024a30: 616e 645f 7265 6164 2827 6d61 6770 796c  and_read('magpyl
-00024a40: 6962 2f63 6f69 6c5f 6669 656c 642e 7674  ib/coil_field.vt
-00024a50: 6927 2c20 6c6f 6164 3d6c 6f61 6429 0a0a  i', load=load)..
-00024a60: 0a64 6566 2064 6f77 6e6c 6f61 645f 6d65  .def download_me
-00024a70: 7368 696f 5f78 646d 6628 6c6f 6164 3d54  shio_xdmf(load=T
-00024a80: 7275 6529 3a20 2023 2070 7261 676d 613a  rue):  # pragma:
-00024a90: 206e 6f20 636f 7665 720a 2020 2020 2222   no cover.    ""
-00024aa0: 2244 6f77 6e6c 6f61 6420 7864 6d66 2066  "Download xdmf f
-00024ab0: 696c 6520 6372 6561 7465 6420 6279 206d  ile created by m
-00024ac0: 6573 6869 6f2e 0a0a 2020 2020 5468 6520  eshio...    The 
-00024ad0: 6461 7461 7365 7420 7761 7320 6372 6561  dataset was crea
-00024ae0: 7465 6420 6279 2060 6074 6573 745f 7469  ted by ``test_ti
-00024af0: 6d65 5f73 6572 6965 7360 6020 7465 7374  me_series`` test
-00024b00: 2066 756e 6374 696f 6e20 696e 206d 6573   function in mes
-00024b10: 6869 6f2e 0a0a 2020 2020 5061 7261 6d65  hio...    Parame
-00024b20: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00024b30: 2d2d 2d0a 2020 2020 6c6f 6164 203a 2062  ---.    load : b
-00024b40: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
-00024b50: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
-00024b60: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
-00024b70: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
-00024b80: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
-00024b90: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
-00024ba0: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
-00024bb0: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
-00024bc0: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
-00024bd0: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
-00024be0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-00024bf0: 2020 2020 7079 7669 7374 612e 556e 7374      pyvista.Unst
-00024c00: 7275 6374 7572 6564 4772 6964 206f 7220  ructuredGrid or 
-00024c10: 7374 720a 2020 2020 2020 2020 4461 7461  str.        Data
-00024c20: 5365 7420 6f72 2066 696c 656e 616d 6520  Set or filename 
-00024c30: 6465 7065 6e64 696e 6720 6f6e 2060 606c  depending on ``l
-00024c40: 6f61 6460 602e 0a0a 2020 2020 4578 616d  oad``...    Exam
-00024c50: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
-00024c60: 2d0a 2020 2020 3e3e 3e20 6672 6f6d 2070  -.    >>> from p
-00024c70: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
-00024c80: 616d 706c 6573 0a20 2020 203e 3e3e 2064  amples.    >>> d
-00024c90: 6174 6173 6574 203d 2065 7861 6d70 6c65  ataset = example
-00024ca0: 732e 646f 776e 6c6f 6164 5f6d 6573 6869  s.download_meshi
-00024cb0: 6f5f 7864 6d66 2829 0a20 2020 203e 3e3e  o_xdmf().    >>>
-00024cc0: 2064 6174 6173 6574 2e70 6c6f 7428 290a   dataset.plot().
-00024cd0: 0a20 2020 2022 2222 0a20 2020 205f 203d  .    """.    _ =
-00024ce0: 2064 6f77 6e6c 6f61 645f 6669 6c65 2822   download_file("
-00024cf0: 6d65 7368 696f 2f6f 7574 2e68 3522 290a  meshio/out.h5").
-00024d00: 2020 2020 7265 7475 726e 205f 646f 776e      return _down
-00024d10: 6c6f 6164 5f61 6e64 5f72 6561 6428 226d  load_and_read("m
-00024d20: 6573 6869 6f2f 6f75 742e 7864 6d66 222c  eshio/out.xdmf",
-00024d30: 206c 6f61 643d 6c6f 6164 290a             load=load).
+0001a840: 6174 6173 6574 0a20 2020 2055 6e73 7472  ataset.    Unstr
+0001a850: 7563 7475 7265 6447 7269 6420 282e 2e2e  ucturedGrid (...
+0001a860: 290a 2020 2020 2020 4e20 4365 6c6c 733a  ).      N Cells:
+0001a870: 2020 2020 3132 3438 3036 0a20 2020 2020      124806.     
+0001a880: 204e 2050 6f69 6e74 733a 2020 2032 3530   N Points:   250
+0001a890: 3438 370a 2020 2020 2020 5820 426f 756e  487.      X Boun
+0001a8a0: 6473 3a20 2020 2d35 2e30 3030 652d 3031  ds:   -5.000e-01
+0001a8b0: 2c20 352e 3030 3065 2d30 310a 2020 2020  , 5.000e-01.    
+0001a8c0: 2020 5920 426f 756e 6473 3a20 2020 2d34    Y Bounds:   -4
+0001a8d0: 2e30 3030 652d 3031 2c20 302e 3030 3065  .000e-01, 0.000e
+0001a8e0: 2b30 300a 2020 2020 2020 5a20 426f 756e  +00.      Z Boun
+0001a8f0: 6473 3a20 2020 2d32 2e35 3030 652d 3032  ds:   -2.500e-02
+0001a900: 2c20 322e 3530 3065 2d30 320a 2020 2020  , 2.500e-02.    
+0001a910: 2020 4e20 4172 7261 7973 3a20 2020 3130    N Arrays:   10
+0001a920: 0a0a 2020 2020 506c 6f74 2074 6865 2064  ..    Plot the d
+0001a930: 6973 706c 6163 656d 656e 7420 6f66 2074  isplacement of t
+0001a940: 6865 2034 7468 206d 6f64 6520 7368 6170  he 4th mode shap
+0001a950: 6520 6173 2073 6361 6c61 7273 2e0a 0a20  e as scalars... 
+0001a960: 2020 203e 3e3e 2063 706f 7320 3d20 5b0a     >>> cpos = [.
+0001a970: 2020 2020 2e2e 2e20 2020 2020 2830 2e37      ...     (0.7
+0001a980: 3434 2c20 2d30 2e35 3032 2c20 2d30 2e38  44, -0.502, -0.8
+0001a990: 3330 292c 0a20 2020 202e 2e2e 2020 2020  30),.    ...    
+0001a9a0: 2028 302e 3035 3230 2c20 2d30 2e31 3630   (0.0520, -0.160
+0001a9b0: 2c20 302e 3037 3433 292c 0a20 2020 202e  , 0.0743),.    .
+0001a9c0: 2e2e 2020 2020 2028 2d30 2e31 3830 2c20  ..     (-0.180, 
+0001a9d0: 2d30 2e39 3538 2c20 302e 3232 3429 2c0a  -0.958, 0.224),.
+0001a9e0: 2020 2020 2e2e 2e20 5d0a 2020 2020 3e3e      ... ].    >>
+0001a9f0: 3e20 6461 7461 7365 742e 706c 6f74 280a  > dataset.plot(.
+0001aa00: 2020 2020 2e2e 2e20 2020 2020 7363 616c      ...     scal
+0001aa10: 6172 733d 2764 6973 705f 3327 2c0a 2020  ars='disp_3',.  
+0001aa20: 2020 2e2e 2e20 2020 2020 6370 6f73 3d63    ...     cpos=c
+0001aa30: 706f 732c 0a20 2020 202e 2e2e 2020 2020  pos,.    ...    
+0001aa40: 2073 686f 775f 7363 616c 6172 5f62 6172   show_scalar_bar
+0001aa50: 3d46 616c 7365 2c0a 2020 2020 2e2e 2e20  =False,.    ... 
+0001aa60: 2020 2020 616d 6269 656e 743d 302e 322c      ambient=0.2,
+0001aa70: 0a20 2020 202e 2e2e 2020 2020 2061 6e74  .    ...     ant
+0001aa80: 695f 616c 6961 7369 6e67 3d27 6678 6161  i_aliasing='fxaa
+0001aa90: 272c 0a20 2020 202e 2e2e 2029 0a0a 2020  ',.    ... )..  
+0001aaa0: 2020 5365 6520 3a72 6566 3a60 7075 6d70    See :ref:`pump
+0001aab0: 5f62 7261 636b 6574 5f65 7861 6d70 6c65  _bracket_example
+0001aac0: 6020 666f 7220 6120 6675 6c6c 2065 7861  ` for a full exa
+0001aad0: 6d70 6c65 2075 7369 6e67 2074 6869 7320  mple using this 
+0001aae0: 6461 7461 7365 742e 0a0a 2020 2020 2222  dataset...    ""
+0001aaf0: 220a 2020 2020 6669 6c65 6e61 6d65 203d  ".    filename =
+0001ab00: 205f 646f 776e 6c6f 6164 5f61 7263 6869   _download_archi
+0001ab10: 7665 280a 2020 2020 2020 2020 2766 6561  ve(.        'fea
+0001ab20: 2f70 756d 705f 6272 6163 6b65 742f 7075  /pump_bracket/pu
+0001ab30: 6d70 5f62 7261 636b 6574 2e7a 6970 272c  mp_bracket.zip',
+0001ab40: 0a20 2020 2020 2020 2027 7075 6d70 5f62  .        'pump_b
+0001ab50: 7261 636b 6574 2e76 746b 272c 0a20 2020  racket.vtk',.   
+0001ab60: 2029 0a20 2020 2069 6620 6c6f 6164 3a0a   ).    if load:.
+0001ab70: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+0001ab80: 7976 6973 7461 2e72 6561 6428 6669 6c65  yvista.read(file
+0001ab90: 6e61 6d65 290a 2020 2020 7265 7475 726e  name).    return
+0001aba0: 2066 696c 656e 616d 650a 0a0a 6465 6620   filename...def 
+0001abb0: 646f 776e 6c6f 6164 5f65 6c65 6374 726f  download_electro
+0001abc0: 6e69 6373 5f63 6f6f 6c69 6e67 286c 6f61  nics_cooling(loa
+0001abd0: 643d 5472 7565 293a 2020 2320 7072 6167  d=True):  # prag
+0001abe0: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
+0001abf0: 2022 2222 446f 776e 6c6f 6164 2074 6865   """Download the
+0001ac00: 2065 6c65 6374 726f 6e69 6373 2063 6f6f   electronics coo
+0001ac10: 6c69 6e67 2065 7861 6d70 6c65 2064 6174  ling example dat
+0001ac20: 6173 6574 732e 0a0a 2020 2020 4461 7461  asets...    Data
+0001ac30: 2067 656e 6572 6174 6564 2066 726f 6d20   generated from 
+0001ac40: 7075 626c 6963 2053 696d 5363 616c 6520  public SimScale 
+0001ac50: 6578 616d 706c 6573 2061 7420 6053 696d  examples at `Sim
+0001ac60: 5363 616c 6520 5072 6f6a 6563 7420 4c69  Scale Project Li
+0001ac70: 6272 6172 7920 2d0a 2020 2020 5475 7262  brary -.    Turb
+0001ac80: 6f20 3c68 7474 7073 3a2f 2f77 7777 2e73  o <https://www.s
+0001ac90: 696d 7363 616c 652e 636f 6d2f 7072 6f6a  imscale.com/proj
+0001aca0: 6563 7473 2f61 7961 726e 6f7a 2f74 7572  ects/ayarnoz/tur
+0001acb0: 626f 2f3e 605f 2e0a 0a20 2020 204c 6963  bo/>`_...    Lic
+0001acc0: 656e 7369 6e67 2066 6f72 2074 6869 7320  ensing for this 
+0001acd0: 6461 7461 7365 7420 6973 2067 7261 6e74  dataset is grant
+0001ace0: 6564 2074 6f20 6672 6565 6c79 2061 6e64  ed to freely and
+0001acf0: 2077 6974 686f 7574 2072 6573 7472 6963   without restric
+0001ad00: 7469 6f6e 0a20 2020 2072 6570 726f 6475  tion.    reprodu
+0001ad10: 6365 2c20 6469 7374 7269 6275 7465 2c20  ce, distribute, 
+0001ad20: 7075 626c 6973 6820 6163 636f 7264 696e  publish accordin
+0001ad30: 6720 746f 2074 6865 2060 5369 6d53 6361  g to the `SimSca
+0001ad40: 6c65 2054 6572 6d73 2061 6e64 0a20 2020  le Terms and.   
+0001ad50: 2043 6f6e 6469 7469 6f6e 7320 3c68 7474   Conditions <htt
+0001ad60: 7073 3a2f 2f77 7777 2e73 696d 7363 616c  ps://www.simscal
+0001ad70: 652e 636f 6d2f 7465 726d 732d 616e 642d  e.com/terms-and-
+0001ad80: 636f 6e64 6974 696f 6e73 2f3e 605f 2e0a  conditions/>`_..
+0001ad90: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+0001ada0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001adb0: 2020 206c 6f61 6420 3a20 626f 6f6c 2c20     load : bool, 
+0001adc0: 6465 6661 756c 743a 2054 7275 650a 2020  default: True.  
+0001add0: 2020 2020 2020 4c6f 6164 2074 6865 2064        Load the d
+0001ade0: 6174 6173 6574 2061 6674 6572 2064 6f77  ataset after dow
+0001adf0: 6e6c 6f61 6469 6e67 2069 7420 7768 656e  nloading it when
+0001ae00: 2060 6054 7275 6560 602e 2020 5365 7420   ``True``.  Set 
+0001ae10: 7468 6973 0a20 2020 2020 2020 2074 6f20  this.        to 
+0001ae20: 6060 4661 6c73 6560 6020 616e 6420 6f6e  ``False`` and on
+0001ae30: 6c79 2074 6865 2066 696c 656e 616d 6520  ly the filename 
+0001ae40: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
+0001ae50: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+0001ae60: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2074     -------.    t
+0001ae70: 7570 6c65 5b50 6f6c 7944 6174 612c 2055  uple[PolyData, U
+0001ae80: 6e73 7472 7563 7475 7265 6447 7269 645d  nstructuredGrid]
+0001ae90: 207c 206c 6973 745b 7374 725d 0a20 2020   | list[str].   
+0001aea0: 2020 2020 2044 6174 6153 6574 7320 6f72       DataSets or
+0001aeb0: 2066 696c 656e 616d 6573 2064 6570 656e   filenames depen
+0001aec0: 6469 6e67 206f 6e20 6060 6c6f 6164 6060  ding on ``load``
+0001aed0: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
+0001aee0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001aef0: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
+0001af00: 7473 2061 6e64 2070 6c6f 7420 7468 6520  ts and plot the 
+0001af10: 6169 7220 7665 6c6f 6369 7479 2074 6872  air velocity thr
+0001af20: 6f75 6768 2074 6865 2065 6c65 6374 726f  ough the electro
+0001af30: 6e69 6373 2e0a 0a20 2020 203e 3e3e 2069  nics...    >>> i
+0001af40: 6d70 6f72 7420 7079 7669 7374 6120 6173  mport pyvista as
+0001af50: 2070 760a 2020 2020 3e3e 3e20 6672 6f6d   pv.    >>> from
+0001af60: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
+0001af70: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
+0001af80: 2073 7472 7563 7475 7265 2c20 6169 7220   structure, air 
+0001af90: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
+0001afa0: 6f61 645f 656c 6563 7472 6f6e 6963 735f  oad_electronics_
+0001afb0: 636f 6f6c 696e 6728 290a 2020 2020 3e3e  cooling().    >>
+0001afc0: 3e20 7374 7275 6374 7572 652c 2061 6972  > structure, air
+0001afd0: 0a20 2020 2028 506f 6c79 4461 7461 2028  .    (PolyData (
+0001afe0: 2e2e 2e29 0a20 2020 2020 204e 2043 656c  ...).      N Cel
+0001aff0: 6c73 3a20 2020 2033 3434 3237 300a 2020  ls:    344270.  
+0001b000: 2020 2020 4e20 506f 696e 7473 3a20 2020      N Points:   
+0001b010: 3138 3739 3932 0a20 2020 2020 204e 2053  187992.      N S
+0001b020: 7472 6970 733a 2020 2030 0a20 2020 2020  trips:   0.     
+0001b030: 2058 2042 6f75 6e64 733a 2020 202d 332e   X Bounds:   -3.
+0001b040: 3030 3065 2d30 332c 2031 2e35 3330 652d  000e-03, 1.530e-
+0001b050: 3031 0a20 2020 2020 2059 2042 6f75 6e64  01.      Y Bound
+0001b060: 733a 2020 202d 332e 3030 3065 2d30 332c  s:   -3.000e-03,
+0001b070: 2032 2e30 3330 652d 3031 0a20 2020 2020   2.030e-01.     
+0001b080: 205a 2042 6f75 6e64 733a 2020 202d 392e   Z Bounds:   -9.
+0001b090: 3030 3065 2d30 332c 2034 2e32 3030 652d  000e-03, 4.200e-
+0001b0a0: 3032 0a20 2020 2020 204e 2041 7272 6179  02.      N Array
+0001b0b0: 733a 2020 2034 2c20 556e 7374 7275 6374  s:   4, Unstruct
+0001b0c0: 7572 6564 4772 6964 2028 2e2e 2e29 0a20  uredGrid (...). 
+0001b0d0: 2020 2020 204e 2043 656c 6c73 3a20 2020       N Cells:   
+0001b0e0: 2031 3734 3939 3932 0a20 2020 2020 204e   1749992.      N
+0001b0f0: 2050 6f69 6e74 733a 2020 2036 3130 3137   Points:   61017
+0001b100: 360a 2020 2020 2020 5820 426f 756e 6473  6.      X Bounds
+0001b110: 3a20 2020 2d31 2e33 3838 652d 3138 2c20  :   -1.388e-18, 
+0001b120: 312e 3530 3065 2d30 310a 2020 2020 2020  1.500e-01.      
+0001b130: 5920 426f 756e 6473 3a20 2020 2d33 2e30  Y Bounds:   -3.0
+0001b140: 3030 652d 3033 2c20 322e 3033 3065 2d30  00e-03, 2.030e-0
+0001b150: 310a 2020 2020 2020 5a20 426f 756e 6473  1.      Z Bounds
+0001b160: 3a20 2020 2d36 2e30 3030 652d 3033 2c20  :   -6.000e-03, 
+0001b170: 342e 3430 3065 2d30 320a 2020 2020 2020  4.400e-02.      
+0001b180: 4e20 4172 7261 7973 3a20 2020 3130 290a  N Arrays:   10).
+0001b190: 0a20 2020 203e 3e3e 207a 5f73 6c69 6365  .    >>> z_slice
+0001b1a0: 203d 2061 6972 2e63 6c69 7028 277a 272c   = air.clip('z',
+0001b1b0: 2076 616c 7565 3d2d 302e 3030 3529 0a20   value=-0.005). 
+0001b1c0: 2020 203e 3e3e 2070 6c20 3d20 7076 2e50     >>> pl = pv.P
+0001b1d0: 6c6f 7474 6572 2829 0a20 2020 203e 3e3e  lotter().    >>>
+0001b1e0: 2070 6c2e 656e 6162 6c65 5f73 7361 6f28   pl.enable_ssao(
+0001b1f0: 7261 6469 7573 3d30 2e30 3129 0a20 2020  radius=0.01).   
+0001b200: 203e 3e3e 205f 203d 2070 6c2e 6164 645f   >>> _ = pl.add_
+0001b210: 6d65 7368 280a 2020 2020 2e2e 2e20 2020  mesh(.    ...   
+0001b220: 2020 7a5f 736c 6963 652c 0a20 2020 202e    z_slice,.    .
+0001b230: 2e2e 2020 2020 2073 6361 6c61 7273 3d27  ..     scalars='
+0001b240: 5527 2c0a 2020 2020 2e2e 2e20 2020 2020  U',.    ...     
+0001b250: 6c69 6768 7469 6e67 3d46 616c 7365 2c0a  lighting=False,.
+0001b260: 2020 2020 2e2e 2e20 2020 2020 7363 616c      ...     scal
+0001b270: 6172 5f62 6172 5f61 7267 733d 7b27 7469  ar_bar_args={'ti
+0001b280: 746c 6527 3a20 2756 656c 6f63 6974 7927  tle': 'Velocity'
+0001b290: 7d2c 0a20 2020 202e 2e2e 2029 0a20 2020  },.    ... ).   
+0001b2a0: 203e 3e3e 205f 203d 2070 6c2e 6164 645f   >>> _ = pl.add_
+0001b2b0: 6d65 7368 280a 2020 2020 2e2e 2e20 2020  mesh(.    ...   
+0001b2c0: 2020 7374 7275 6374 7572 652c 0a20 2020    structure,.   
+0001b2d0: 202e 2e2e 2020 2020 2063 6f6c 6f72 3d27   ...     color='
+0001b2e0: 7727 2c0a 2020 2020 2e2e 2e20 2020 2020  w',.    ...     
+0001b2f0: 736d 6f6f 7468 5f73 6861 6469 6e67 3d54  smooth_shading=T
+0001b300: 7275 652c 0a20 2020 202e 2e2e 2020 2020  rue,.    ...    
+0001b310: 2073 706c 6974 5f73 6861 7270 5f65 6467   split_sharp_edg
+0001b320: 6573 3d54 7275 652c 0a20 2020 202e 2e2e  es=True,.    ...
+0001b330: 2029 0a20 2020 203e 3e3e 2070 6c2e 6361   ).    >>> pl.ca
+0001b340: 6d65 7261 5f70 6f73 6974 696f 6e20 3d20  mera_position = 
+0001b350: 2778 7927 0a20 2020 203e 3e3e 2070 6c2e  'xy'.    >>> pl.
+0001b360: 6361 6d65 7261 2e72 6f6c 6c20 3d20 3930  camera.roll = 90
+0001b370: 0a20 2020 203e 3e3e 2070 6c2e 656e 6162  .    >>> pl.enab
+0001b380: 6c65 5f61 6e74 695f 616c 6961 7369 6e67  le_anti_aliasing
+0001b390: 2827 6678 6161 2729 0a20 2020 203e 3e3e  ('fxaa').    >>>
+0001b3a0: 2070 6c2e 7368 6f77 2829 0a0a 2020 2020   pl.show()..    
+0001b3b0: 5368 6f77 2074 6865 2074 7970 6520 616e  Show the type an
+0001b3c0: 6420 626f 756e 6473 206f 6620 7468 6520  d bounds of the 
+0001b3d0: 6461 7461 7365 7473 2e0a 0a20 2020 2053  datasets...    S
+0001b3e0: 6565 203a 7265 663a 606f 7065 6e66 6f61  ee :ref:`openfoa
+0001b3f0: 6d5f 636f 6f6c 696e 675f 6578 616d 706c  m_cooling_exampl
+0001b400: 6560 2066 6f72 2061 2066 756c 6c20 6578  e` for a full ex
+0001b410: 616d 706c 6520 7573 696e 6720 7468 6973  ample using this
+0001b420: 2064 6174 6173 6574 2e0a 0a20 2020 2022   dataset...    "
+0001b430: 2222 0a20 2020 2066 6e61 6d65 7320 3d20  "".    fnames = 
+0001b440: 5f64 6f77 6e6c 6f61 645f 6172 6368 6976  _download_archiv
+0001b450: 6528 2766 766d 2f63 6f6f 6c69 6e67 5f65  e('fvm/cooling_e
+0001b460: 6c65 6374 726f 6e69 6373 2f64 6174 6173  lectronics/datas
+0001b470: 6574 732e 7a69 7027 290a 2020 2020 6966  ets.zip').    if
+0001b480: 206c 6f61 643a 0a20 2020 2020 2020 2023   load:.        #
+0001b490: 2072 6574 7572 6e20 7468 6520 7374 7275   return the stru
+0001b4a0: 6374 7572 6520 6461 7461 7365 7420 6669  cture dataset fi
+0001b4b0: 7273 740a 2020 2020 2020 2020 6966 2066  rst.        if f
+0001b4c0: 6e61 6d65 735b 315d 2e65 6e64 7377 6974  names[1].endswit
+0001b4d0: 6828 2773 7472 7563 7475 7265 2e76 7470  h('structure.vtp
+0001b4e0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0001b4f0: 666e 616d 6573 203d 2066 6e61 6d65 735b  fnames = fnames[
+0001b500: 3a3a 2d31 5d0a 2020 2020 2020 2020 7265  ::-1].        re
+0001b510: 7475 726e 2070 7976 6973 7461 2e72 6561  turn pyvista.rea
+0001b520: 6428 666e 616d 6573 5b30 5d29 2c20 7079  d(fnames[0]), py
+0001b530: 7669 7374 612e 7265 6164 2866 6e61 6d65  vista.read(fname
+0001b540: 735b 315d 290a 2020 2020 7265 7475 726e  s[1]).    return
+0001b550: 2066 6e61 6d65 730a 0a0a 6465 6620 646f   fnames...def do
+0001b560: 776e 6c6f 6164 5f63 616e 2870 6172 7469  wnload_can(parti
+0001b570: 616c 3d46 616c 7365 2c20 6c6f 6164 3d54  al=False, load=T
+0001b580: 7275 6529 3a20 2023 2070 7261 676d 613a  rue):  # pragma:
+0001b590: 206e 6f20 636f 7665 720a 2020 2020 2222   no cover.    ""
+0001b5a0: 2244 6f77 6e6c 6f61 6420 7468 6520 6361  "Download the ca
+0001b5b0: 6e20 6461 7461 7365 7420 6d65 7368 2e0a  n dataset mesh..
+0001b5c0: 0a20 2020 2046 696c 6520 6f62 7461 696e  .    File obtain
+0001b5d0: 6564 2066 726f 6d20 604b 6974 7761 7265  ed from `Kitware
+0001b5e0: 203c 6874 7470 733a 2f2f 7777 772e 6b69   <https://www.ki
+0001b5f0: 7477 6172 652e 636f 6d2f 3e60 5f2e 2055  tware.com/>`_. U
+0001b600: 7365 640a 2020 2020 666f 7220 7465 7374  sed.    for test
+0001b610: 696e 6720 6864 6620 6669 6c65 732e 0a0a  ing hdf files...
+0001b620: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0001b630: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001b640: 2020 7061 7274 6961 6c20 3a20 626f 6f6c    partial : bool
+0001b650: 2c20 6465 6661 756c 743a 2046 616c 7365  , default: False
+0001b660: 0a20 2020 2020 2020 204c 6f61 6420 7061  .        Load pa
+0001b670: 7274 206f 6620 7468 6520 6461 7461 7365  rt of the datase
+0001b680: 742e 0a0a 2020 2020 6c6f 6164 203a 2062  t...    load : b
+0001b690: 6f6f 6c2c 2064 6566 6175 6c74 3a20 5472  ool, default: Tr
+0001b6a0: 7565 0a20 2020 2020 2020 204c 6f61 6420  ue.        Load 
+0001b6b0: 7468 6520 6461 7461 7365 7420 6166 7465  the dataset afte
+0001b6c0: 7220 646f 776e 6c6f 6164 696e 6720 6974  r downloading it
+0001b6d0: 2077 6865 6e20 6060 5472 7565 6060 2e20   when ``True``. 
+0001b6e0: 2053 6574 2074 6869 730a 2020 2020 2020   Set this.      
+0001b6f0: 2020 746f 2060 6046 616c 7365 6060 2061    to ``False`` a
+0001b700: 6e64 206f 6e6c 7920 7468 6520 6669 6c65  nd only the file
+0001b710: 6e61 6d65 2077 696c 6c20 6265 2072 6574  name will be ret
+0001b720: 7572 6e65 642e 0a0a 2020 2020 5265 7475  urned...    Retu
+0001b730: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+0001b740: 2020 2020 7079 7669 7374 612e 506f 6c79      pyvista.Poly
+0001b750: 4461 7461 2c20 7374 722c 206f 7220 4c69  Data, str, or Li
+0001b760: 7374 5b73 7472 5d0a 2020 2020 2020 2020  st[str].        
+0001b770: 5468 6520 6578 616d 706c 6520 5061 7261  The example Para
+0001b780: 5669 6577 2063 616e 2044 6174 6153 6574  View can DataSet
+0001b790: 206f 7220 6669 6c65 2070 6174 6828 7329   or file path(s)
+0001b7a0: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
+0001b7b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001b7c0: 2050 6c6f 7420 7468 6520 6361 6e20 6461   Plot the can da
+0001b7d0: 7461 7365 742e 0a0a 2020 2020 3e3e 3e20  taset...    >>> 
+0001b7e0: 6672 6f6d 2070 7976 6973 7461 2069 6d70  from pyvista imp
+0001b7f0: 6f72 7420 6578 616d 706c 6573 0a20 2020  ort examples.   
+0001b800: 203e 3e3e 2069 6d70 6f72 7420 7079 7669   >>> import pyvi
+0001b810: 7374 610a 2020 2020 3e3e 3e20 6461 7461  sta.    >>> data
+0001b820: 7365 7420 3d20 6578 616d 706c 6573 2e64  set = examples.d
+0001b830: 6f77 6e6c 6f61 645f 6361 6e28 2920 2023  ownload_can()  #
+0001b840: 2064 6f63 7465 7374 3a2b 534b 4950 0a20   doctest:+SKIP. 
+0001b850: 2020 203e 3e3e 2064 6174 6173 6574 2e70     >>> dataset.p
+0001b860: 6c6f 7428 7363 616c 6172 733d 2756 454c  lot(scalars='VEL
+0001b870: 272c 2073 6d6f 6f74 685f 7368 6164 696e  ', smooth_shadin
+0001b880: 673d 5472 7565 2920 2023 2064 6f63 7465  g=True)  # docte
+0001b890: 7374 3a2b 534b 4950 0a0a 2020 2020 2222  st:+SKIP..    ""
+0001b8a0: 220a 2020 2020 6966 2070 7976 6973 7461  ".    if pyvista
+0001b8b0: 2e76 746b 5f76 6572 7369 6f6e 5f69 6e66  .vtk_version_inf
+0001b8c0: 6f20 3e20 2839 2c20 3129 3a20 2023 2070  o > (9, 1):  # p
+0001b8d0: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
+0001b8e0: 2020 2020 2020 2020 7261 6973 6520 5654          raise VT
+0001b8f0: 4b56 6572 7369 6f6e 4572 726f 7228 0a20  KVersionError(. 
+0001b900: 2020 2020 2020 2020 2020 2027 5468 6973             'This
+0001b910: 2065 7861 6d70 6c65 2066 696c 6520 6973   example file is
+0001b920: 2064 6570 7265 6361 7465 6420 666f 7220   deprecated for 
+0001b930: 5654 4b20 7639 2e32 2e30 2061 6e64 206e  VTK v9.2.0 and n
+0001b940: 6577 6572 2e20 270a 2020 2020 2020 2020  ewer. '.        
+0001b950: 2020 2020 2755 7365 2060 646f 776e 6c6f      'Use `downlo
+0001b960: 6164 5f63 616e 5f63 7275 7368 6564 5f68  ad_can_crushed_h
+0001b970: 6466 6020 696e 7374 6561 642e 270a 2020  df` instead.'.  
+0001b980: 2020 2020 2020 290a 0a20 2020 2063 616e        )..    can
+0001b990: 5f30 203d 205f 646f 776e 6c6f 6164 5f61  _0 = _download_a
+0001b9a0: 6e64 5f72 6561 6428 2768 6466 2f63 616e  nd_read('hdf/can
+0001b9b0: 5f30 2e68 6466 272c 206c 6f61 643d 6c6f  _0.hdf', load=lo
+0001b9c0: 6164 290a 2020 2020 6966 2070 6172 7469  ad).    if parti
+0001b9d0: 616c 3a0a 2020 2020 2020 2020 7265 7475  al:.        retu
+0001b9e0: 726e 2063 616e 5f30 0a0a 2020 2020 6361  rn can_0..    ca
+0001b9f0: 6e73 203d 205b 0a20 2020 2020 2020 2063  ns = [.        c
+0001ba00: 616e 5f30 2c0a 2020 2020 2020 2020 5f64  an_0,.        _d
+0001ba10: 6f77 6e6c 6f61 645f 616e 645f 7265 6164  ownload_and_read
+0001ba20: 2827 6864 662f 6361 6e5f 312e 6864 6627  ('hdf/can_1.hdf'
+0001ba30: 2c20 6c6f 6164 3d6c 6f61 6429 2c0a 2020  , load=load),.  
+0001ba40: 2020 2020 2020 5f64 6f77 6e6c 6f61 645f        _download_
+0001ba50: 616e 645f 7265 6164 2827 6864 662f 6361  and_read('hdf/ca
+0001ba60: 6e5f 322e 6864 6627 2c20 6c6f 6164 3d6c  n_2.hdf', load=l
+0001ba70: 6f61 6429 2c0a 2020 2020 5d0a 0a20 2020  oad),.    ]..   
+0001ba80: 2069 6620 6c6f 6164 3a0a 2020 2020 2020   if load:.      
+0001ba90: 2020 7265 7475 726e 2070 7976 6973 7461    return pyvista
+0001baa0: 2e6d 6572 6765 2863 616e 7329 0a20 2020  .merge(cans).   
+0001bab0: 2072 6574 7572 6e20 6361 6e73 0a0a 0a64   return cans...d
+0001bac0: 6566 2064 6f77 6e6c 6f61 645f 6361 6e5f  ef download_can_
+0001bad0: 6372 7573 6865 645f 6864 6628 6c6f 6164  crushed_hdf(load
+0001bae0: 3d54 7275 6529 3a20 2023 2070 7261 676d  =True):  # pragm
+0001baf0: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
+0001bb00: 2222 2244 6f77 6e6c 6f61 6420 7468 6520  """Download the 
+0001bb10: 6372 7573 6865 6420 6361 6e20 6461 7461  crushed can data
+0001bb20: 7365 742e 0a0a 2020 2020 4669 6c65 206f  set...    File o
+0001bb30: 6274 6169 6e65 6420 6672 6f6d 2060 4b69  btained from `Ki
+0001bb40: 7477 6172 6520 3c68 7474 7073 3a2f 2f77  tware <https://w
+0001bb50: 7777 2e6b 6974 7761 7265 2e63 6f6d 2f3e  ww.kitware.com/>
+0001bb60: 605f 2e20 5573 6564 0a20 2020 2066 6f72  `_. Used.    for
+0001bb70: 2074 6573 7469 6e67 2068 6466 2066 696c   testing hdf fil
+0001bb80: 6573 2e0a 0a20 2020 204f 7269 6769 6e61  es...    Origina
+0001bb90: 6c6c 7920 6275 696c 7420 7573 696e 6720  lly built using 
+0001bba0: 5654 4b20 7639 2e32 2e30 7263 2066 726f  VTK v9.2.0rc fro
+0001bbb0: 6d3a 0a0a 2020 2020 6060 5654 4b2f 6275  m:..    ``VTK/bu
+0001bbc0: 696c 642f 4578 7465 726e 616c 5465 7374  ild/ExternalTest
+0001bbd0: 696e 672f 6361 6e2d 7674 752e 6864 6660  ing/can-vtu.hdf`
+0001bbe0: 600a 0a20 2020 2050 6172 616d 6574 6572  `..    Parameter
+0001bbf0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0001bc00: 0a20 2020 206c 6f61 6420 3a20 626f 6f6c  .    load : bool
+0001bc10: 2c20 6465 6661 756c 743a 2054 7275 650a  , default: True.
+0001bc20: 2020 2020 2020 2020 4c6f 6164 2074 6865          Load the
+0001bc30: 2064 6174 6173 6574 2061 6674 6572 2064   dataset after d
+0001bc40: 6f77 6e6c 6f61 6469 6e67 2069 7420 7768  ownloading it wh
+0001bc50: 656e 2060 6054 7275 6560 602e 2020 5365  en ``True``.  Se
+0001bc60: 7420 7468 6973 0a20 2020 2020 2020 2074  t this.        t
+0001bc70: 6f20 6060 4661 6c73 6560 6020 616e 6420  o ``False`` and 
+0001bc80: 6f6e 6c79 2074 6865 2066 696c 656e 616d  only the filenam
+0001bc90: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
+0001bca0: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
+0001bcb0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+0001bcc0: 2070 7976 6973 7461 2e55 6e73 7472 7563   pyvista.Unstruc
+0001bcd0: 7475 7265 6447 7269 6420 7c20 7374 720a  turedGrid | str.
+0001bce0: 2020 2020 2020 2020 4372 7573 6865 6420          Crushed 
+0001bcf0: 6361 6e20 6461 7461 7365 7420 6f72 2070  can dataset or p
+0001bd00: 6174 6820 6465 7065 6e64 696e 6720 6f6e  ath depending on
+0001bd10: 2074 6865 2076 616c 7565 206f 6620 6060   the value of ``
+0001bd20: 6c6f 6164 6060 2e0a 0a20 2020 2045 7861  load``...    Exa
+0001bd30: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+0001bd40: 2d2d 0a20 2020 2050 6c6f 7420 7468 6520  --.    Plot the 
+0001bd50: 6372 7573 6865 6420 6361 6e20 6461 7461  crushed can data
+0001bd60: 7365 742e 0a0a 2020 2020 3e3e 3e20 6672  set...    >>> fr
+0001bd70: 6f6d 2070 7976 6973 7461 2069 6d70 6f72  om pyvista impor
+0001bd80: 7420 6578 616d 706c 6573 0a20 2020 203e  t examples.    >
+0001bd90: 3e3e 2069 6d70 6f72 7420 7079 7669 7374  >> import pyvist
+0001bda0: 610a 2020 2020 3e3e 3e20 6461 7461 7365  a.    >>> datase
+0001bdb0: 7420 3d20 6578 616d 706c 6573 2e64 6f77  t = examples.dow
+0001bdc0: 6e6c 6f61 645f 6361 6e5f 6372 7573 6865  nload_can_crushe
+0001bdd0: 645f 6864 6628 290a 2020 2020 3e3e 3e20  d_hdf().    >>> 
+0001bde0: 6461 7461 7365 742e 706c 6f74 2873 6d6f  dataset.plot(smo
+0001bdf0: 6f74 685f 7368 6164 696e 673d 5472 7565  oth_shading=True
+0001be00: 290a 0a20 2020 2022 2222 0a20 2020 2072  )..    """.    r
+0001be10: 6574 7572 6e20 5f64 6f77 6e6c 6f61 645f  eturn _download_
+0001be20: 616e 645f 7265 6164 2827 6864 662f 6361  and_read('hdf/ca
+0001be30: 6e2d 7674 752e 6864 6627 2c20 6c6f 6164  n-vtu.hdf', load
+0001be40: 3d6c 6f61 6429 0a0a 0a64 6566 2064 6f77  =load)...def dow
+0001be50: 6e6c 6f61 645f 6367 6e73 5f73 7472 7563  nload_cgns_struc
+0001be60: 7475 7265 6428 6c6f 6164 3d54 7275 6529  tured(load=True)
+0001be70: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+0001be80: 636f 7665 720a 2020 2020 2222 2244 6f77  cover.    """Dow
+0001be90: 6e6c 6f61 6420 7468 6520 7374 7275 6374  nload the struct
+0001bea0: 7572 6564 2043 474e 5320 6461 7461 7365  ured CGNS datase
+0001beb0: 7420 6d65 7368 2e0a 0a20 2020 204f 7269  t mesh...    Ori
+0001bec0: 6769 6e61 6c6c 7920 646f 776e 6c6f 6164  ginally download
+0001bed0: 6564 2066 726f 6d20 6043 4644 2047 656e  ed from `CFD Gen
+0001bee0: 6572 616c 204e 6f74 6174 696f 6e20 5379  eral Notation Sy
+0001bef0: 7374 656d 2045 7861 6d70 6c65 2046 696c  stem Example Fil
+0001bf00: 6573 0a20 2020 203c 6874 7470 733a 2f2f  es.    <https://
+0001bf10: 6367 6e73 2e67 6974 6875 622e 696f 2f43  cgns.github.io/C
+0001bf20: 474e 5346 696c 6573 2e68 746d 6c3e 605f  GNSFiles.html>`_
+0001bf30: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+0001bf40: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0001bf50: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
+0001bf60: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
+0001bf70: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
+0001bf80: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
+0001bf90: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
+0001bfa0: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
+0001bfb0: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
+0001bfc0: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
+0001bfd0: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
+0001bfe0: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+0001bff0: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
+0001c000: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0001c010: 7079 7669 7374 612e 4d75 6c74 6942 6c6f  pyvista.MultiBlo
+0001c020: 636b 207c 2073 7472 0a20 2020 2020 2020  ck | str.       
+0001c030: 2053 7472 7563 7475 7265 642c 2031 3220   Structured, 12 
+0001c040: 626c 6f63 6b2c 2033 2d44 2063 6f6e 7374  block, 3-D const
+0001c050: 7269 6374 696e 6720 6368 616e 6e65 6c2c  ricting channel,
+0001c060: 2077 6974 6820 6578 616d 706c 6520 7573   with example us
+0001c070: 6520 6f66 0a20 2020 2020 2020 2046 616d  e of.        Fam
+0001c080: 696c 795f 7420 666f 7220 4243 7320 2841  ily_t for BCs (A
+0001c090: 4446 2074 7970 6529 2e20 4966 2060 606c  DF type). If ``l
+0001c0a0: 6f61 6460 6020 6973 2060 6046 616c 7365  oad`` is ``False
+0001c0b0: 6060 2c20 7468 656e 2074 6865 2070 6174  ``, then the pat
+0001c0c0: 6820 6f66 2074 6865 0a20 2020 2020 2020  h of the.       
+0001c0d0: 2065 7861 6d70 6c65 2043 474e 5320 6669   example CGNS fi
+0001c0e0: 6c65 2069 7320 7265 7475 726e 6564 2e0a  le is returned..
+0001c0f0: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
+0001c100: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2050    --------.    P
+0001c110: 6c6f 7420 7468 6520 6578 616d 706c 6520  lot the example 
+0001c120: 4347 4e53 2064 6174 6173 6574 2e0a 0a20  CGNS dataset... 
+0001c130: 2020 203e 3e3e 2066 726f 6d20 7079 7669     >>> from pyvi
+0001c140: 7374 6120 696d 706f 7274 2065 7861 6d70  sta import examp
+0001c150: 6c65 730a 2020 2020 3e3e 3e20 696d 706f  les.    >>> impo
+0001c160: 7274 2070 7976 6973 7461 0a20 2020 203e  rt pyvista.    >
+0001c170: 3e3e 2064 6174 6173 6574 203d 2065 7861  >> dataset = exa
+0001c180: 6d70 6c65 732e 646f 776e 6c6f 6164 5f63  mples.download_c
+0001c190: 676e 735f 7374 7275 6374 7572 6564 2829  gns_structured()
+0001c1a0: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
+0001c1b0: 5b30 5d2e 706c 6f74 2873 6361 6c61 7273  [0].plot(scalars
+0001c1c0: 3d27 4465 6e73 6974 7927 290a 0a20 2020  ='Density')..   
+0001c1d0: 2022 2222 0a20 2020 2066 696c 656e 616d   """.    filenam
+0001c1e0: 6520 3d20 646f 776e 6c6f 6164 5f66 696c  e = download_fil
+0001c1f0: 6528 2763 676e 732f 7371 6e7a 5f73 2e61  e('cgns/sqnz_s.a
+0001c200: 6466 2e63 676e 7327 290a 2020 2020 6966  df.cgns').    if
+0001c210: 206e 6f74 206c 6f61 643a 0a20 2020 2020   not load:.     
+0001c220: 2020 2072 6574 7572 6e20 6669 6c65 6e61     return filena
+0001c230: 6d65 0a20 2020 2072 6574 7572 6e20 7079  me.    return py
+0001c240: 7669 7374 612e 6765 745f 7265 6164 6572  vista.get_reader
+0001c250: 2866 696c 656e 616d 6529 2e72 6561 6428  (filename).read(
+0001c260: 290a 0a0a 6465 6620 646f 776e 6c6f 6164  )...def download
+0001c270: 5f74 6563 706c 6f74 5f61 7363 6969 286c  _tecplot_ascii(l
+0001c280: 6f61 643d 5472 7565 293a 2020 2320 7072  oad=True):  # pr
+0001c290: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+0001c2a0: 2020 2022 2222 446f 776e 6c6f 6164 2074     """Download t
+0001c2b0: 6865 2073 696e 676c 6520 626c 6f63 6b20  he single block 
+0001c2c0: 4153 4349 4920 5465 6370 6c6f 7420 6461  ASCII Tecplot da
+0001c2d0: 7461 7365 742e 0a0a 2020 2020 4f72 6967  taset...    Orig
+0001c2e0: 696e 616c 6c79 2064 6f77 6e6c 6f61 6465  inally downloade
+0001c2f0: 6420 6672 6f6d 2050 6175 6c20 426f 7572  d from Paul Bour
+0001c300: 6b65 2773 0a20 2020 2060 5361 6d70 6c65  ke's.    `Sample
+0001c310: 2066 696c 6520 3c68 7474 703a 2f2f 7061   file <http://pa
+0001c320: 756c 626f 7572 6b65 2e6e 6574 2f64 6174  ulbourke.net/dat
+0001c330: 6166 6f72 6d61 7473 2f74 702f 7361 6d70  aformats/tp/samp
+0001c340: 6c65 2e74 703e 605f 0a0a 2020 2020 5061  le.tp>`_..    Pa
+0001c350: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+0001c360: 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f 6164  -------.    load
+0001c370: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+0001c380: 3a20 5472 7565 0a20 2020 2020 2020 204c  : True.        L
+0001c390: 6f61 6420 7468 6520 6461 7461 7365 7420  oad the dataset 
+0001c3a0: 6166 7465 7220 646f 776e 6c6f 6164 696e  after downloadin
+0001c3b0: 6720 6974 2077 6865 6e20 6060 5472 7565  g it when ``True
+0001c3c0: 6060 2e20 2053 6574 2074 6869 730a 2020  ``.  Set this.  
+0001c3d0: 2020 2020 2020 746f 2060 6046 616c 7365        to ``False
+0001c3e0: 6060 2061 6e64 206f 6e6c 7920 7468 6520  `` and only the 
+0001c3f0: 6669 6c65 6e61 6d65 2077 696c 6c20 6265  filename will be
+0001c400: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
+0001c410: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+0001c420: 2d2d 2d0a 2020 2020 7079 7669 7374 612e  ---.    pyvista.
+0001c430: 4d75 6c74 6942 6c6f 636b 207c 2073 7472  MultiBlock | str
+0001c440: 0a20 2020 2020 2020 204d 756c 7469 626c  .        Multibl
+0001c450: 6f63 6b20 666f 726d 6174 2077 6974 6820  ock format with 
+0001c460: 6f6e 6c79 2031 2064 6174 6120 626c 6f63  only 1 data bloc
+0001c470: 6b2c 2073 696d 706c 6520 6765 6f6d 6574  k, simple geomet
+0001c480: 7269 6320 7368 6170 652e 0a20 2020 2020  ric shape..     
+0001c490: 2020 2049 6620 6060 6c6f 6164 6060 2069     If ``load`` i
+0001c4a0: 7320 6060 4661 6c73 6560 602c 2074 6865  s ``False``, the
+0001c4b0: 6e20 7468 6520 7061 7468 206f 6620 7468  n the path of th
+0001c4c0: 6520 6578 616d 706c 6520 5465 6370 6c6f  e example Tecplo
+0001c4d0: 7420 6669 6c65 0a20 2020 2020 2020 2069  t file.        i
+0001c4e0: 7320 7265 7475 726e 6564 2e0a 0a20 2020  s returned...   
+0001c4f0: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
+0001c500: 2d2d 2d2d 2d2d 0a20 2020 2050 6c6f 7420  ------.    Plot 
+0001c510: 7468 6520 6578 616d 706c 6520 5465 6370  the example Tecp
+0001c520: 6c6f 7420 6461 7461 7365 742e 0a0a 2020  lot dataset...  
+0001c530: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
+0001c540: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
+0001c550: 6573 0a20 2020 203e 3e3e 2069 6d70 6f72  es.    >>> impor
+0001c560: 7420 7079 7669 7374 610a 2020 2020 3e3e  t pyvista.    >>
+0001c570: 3e20 6461 7461 7365 7420 3d20 6578 616d  > dataset = exam
+0001c580: 706c 6573 2e64 6f77 6e6c 6f61 645f 7465  ples.download_te
+0001c590: 6370 6c6f 745f 6173 6369 6928 290a 2020  cplot_ascii().  
+0001c5a0: 2020 3e3e 3e20 6461 7461 7365 742e 706c    >>> dataset.pl
+0001c5b0: 6f74 2829 0a0a 2020 2020 2222 220a 2020  ot()..    """.  
+0001c5c0: 2020 6669 6c65 6e61 6d65 203d 2064 6f77    filename = dow
+0001c5d0: 6e6c 6f61 645f 6669 6c65 2827 7465 6370  nload_file('tecp
+0001c5e0: 6c6f 745f 6173 6369 692e 6461 7427 290a  lot_ascii.dat').
+0001c5f0: 2020 2020 6966 206e 6f74 206c 6f61 643a      if not load:
+0001c600: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001c610: 6669 6c65 6e61 6d65 0a20 2020 2072 6574  filename.    ret
+0001c620: 7572 6e20 7079 7669 7374 612e 6765 745f  urn pyvista.get_
+0001c630: 7265 6164 6572 2866 696c 656e 616d 6529  reader(filename)
+0001c640: 2e72 6561 6428 290a 0a0a 6465 6620 646f  .read()...def do
+0001c650: 776e 6c6f 6164 5f63 676e 735f 6d75 6c74  wnload_cgns_mult
+0001c660: 6928 6c6f 6164 3d54 7275 6529 3a20 2023  i(load=True):  #
+0001c670: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+0001c680: 720a 2020 2020 2222 2244 6f77 6e6c 6f61  r.    """Downloa
+0001c690: 6420 6120 6d75 6c74 6965 6c65 6d65 6e74  d a multielement
+0001c6a0: 2061 6972 666f 696c 2077 6974 6820 6120   airfoil with a 
+0001c6b0: 6365 6c6c 2063 656e 7465 7265 6420 736f  cell centered so
+0001c6c0: 6c75 7469 6f6e 2e0a 0a20 2020 204f 7269  lution...    Ori
+0001c6d0: 6769 6e61 6c6c 7920 646f 776e 6c6f 6164  ginally download
+0001c6e0: 6564 2066 726f 6d20 6043 4644 2047 656e  ed from `CFD Gen
+0001c6f0: 6572 616c 204e 6f74 6174 696f 6e20 5379  eral Notation Sy
+0001c700: 7374 656d 2045 7861 6d70 6c65 2046 696c  stem Example Fil
+0001c710: 6573 0a20 2020 203c 6874 7470 733a 2f2f  es.    <https://
+0001c720: 6367 6e73 2e67 6974 6875 622e 696f 2f43  cgns.github.io/C
+0001c730: 474e 5346 696c 6573 2e68 746d 6c3e 605f  GNSFiles.html>`_
+0001c740: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+0001c750: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0001c760: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
+0001c770: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
+0001c780: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
+0001c790: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
+0001c7a0: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
+0001c7b0: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
+0001c7c0: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
+0001c7d0: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
+0001c7e0: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
+0001c7f0: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+0001c800: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
+0001c810: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0001c820: 7079 7669 7374 612e 4d75 6c74 6942 6c6f  pyvista.MultiBlo
+0001c830: 636b 207c 2073 7472 0a20 2020 2020 2020  ck | str.       
+0001c840: 2053 7472 7563 7475 7265 642c 2034 2062   Structured, 4 b
+0001c850: 6c6f 636b 732c 2032 4420 2832 2070 6c61  locks, 2D (2 pla
+0001c860: 6e65 7320 696e 2074 6869 7264 2064 696d  nes in third dim
+0001c870: 656e 7369 6f6e 2920 6d75 6c74 6965 6c65  ension) multiele
+0001c880: 6d65 6e74 0a20 2020 2020 2020 2061 6972  ment.        air
+0001c890: 666f 696c 2c20 7769 7468 2063 656c 6c20  foil, with cell 
+0001c8a0: 6365 6e74 6572 6564 2073 6f6c 7574 696f  centered solutio
+0001c8b0: 6e2e 2049 6620 6060 6c6f 6164 6060 2069  n. If ``load`` i
+0001c8c0: 7320 6060 4661 6c73 6560 602c 2074 6865  s ``False``, the
+0001c8d0: 6e20 7468 6520 7061 7468 206f 6620 7468  n the path of th
+0001c8e0: 650a 2020 2020 2020 2020 6578 616d 706c  e.        exampl
+0001c8f0: 6520 4347 4e53 2066 696c 6520 6973 2072  e CGNS file is r
+0001c900: 6574 7572 6e65 642e 0a0a 2020 2020 4578  eturned...    Ex
+0001c910: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+0001c920: 2d2d 2d0a 2020 2020 506c 6f74 2074 6865  ---.    Plot the
+0001c930: 2061 6972 666f 696c 2064 6174 6173 6574   airfoil dataset
+0001c940: 2e20 4d65 7267 6520 7468 6520 6d75 6c74  . Merge the mult
+0001c950: 692d 626c 6f63 6b20 616e 6420 7468 656e  i-block and then
+0001c960: 2070 6c6f 7420 7468 6520 6169 7266 6f69   plot the airfoi
+0001c970: 6c27 730a 2020 2020 6060 2256 6973 636f  l's.    ``"Visco
+0001c980: 7369 7479 4564 6479 2260 602e 2043 6f6e  sityEddy"``. Con
+0001c990: 7665 7274 2074 6865 2063 656c 6c20 6461  vert the cell da
+0001c9a0: 7461 2074 6f20 706f 696e 7420 6461 7461  ta to point data
+0001c9b0: 2061 7320 696e 2074 6869 730a 2020 2020   as in this.    
+0001c9c0: 6461 7461 7365 742c 2074 6865 2073 6f6c  dataset, the sol
+0001c9d0: 7574 696f 6e20 6973 2073 746f 7265 6420  ution is stored 
+0001c9e0: 7769 7468 696e 2074 6865 2063 656c 6c73  within the cells
+0001c9f0: 2e0a 0a20 2020 203e 3e3e 2066 726f 6d20  ...    >>> from 
+0001ca00: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+0001ca10: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+0001ca20: 696d 706f 7274 2070 7976 6973 7461 0a20  import pyvista. 
+0001ca30: 2020 203e 3e3e 2064 6174 6173 6574 203d     >>> dataset =
+0001ca40: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
+0001ca50: 6164 5f63 676e 735f 6d75 6c74 6928 290a  ad_cgns_multi().
+0001ca60: 2020 2020 3e3e 3e20 7567 7269 6420 3d20      >>> ugrid = 
+0001ca70: 6461 7461 7365 742e 636f 6d62 696e 6528  dataset.combine(
+0001ca80: 290a 2020 2020 3e3e 3e20 7567 7269 6420  ).    >>> ugrid 
+0001ca90: 3d20 7567 7269 6420 3d20 7567 7269 642e  = ugrid = ugrid.
+0001caa0: 6365 6c6c 5f64 6174 615f 746f 5f70 6f69  cell_data_to_poi
+0001cab0: 6e74 5f64 6174 6128 290a 2020 2020 3e3e  nt_data().    >>
+0001cac0: 3e20 7567 7269 642e 706c 6f74 280a 2020  > ugrid.plot(.  
+0001cad0: 2020 2e2e 2e20 2020 2020 636d 6170 3d27    ...     cmap='
+0001cae0: 6277 7227 2c0a 2020 2020 2e2e 2e20 2020  bwr',.    ...   
+0001caf0: 2020 7363 616c 6172 733d 2756 6973 636f    scalars='Visco
+0001cb00: 7369 7479 4564 6479 272c 0a20 2020 202e  sityEddy',.    .
+0001cb10: 2e2e 2020 2020 207a 6f6f 6d3d 342c 0a20  ..     zoom=4,. 
+0001cb20: 2020 202e 2e2e 2020 2020 2063 706f 733d     ...     cpos=
+0001cb30: 2778 7a27 2c0a 2020 2020 2e2e 2e20 2020  'xz',.    ...   
+0001cb40: 2020 7368 6f77 5f73 6361 6c61 725f 6261    show_scalar_ba
+0001cb50: 723d 4661 6c73 652c 0a20 2020 202e 2e2e  r=False,.    ...
+0001cb60: 2029 0a0a 2020 2020 2222 220a 2020 2020   )..    """.    
+0001cb70: 6669 6c65 6e61 6d65 203d 2064 6f77 6e6c  filename = downl
+0001cb80: 6f61 645f 6669 6c65 2827 6367 6e73 2f6d  oad_file('cgns/m
+0001cb90: 756c 7469 2e63 676e 7327 290a 2020 2020  ulti.cgns').    
+0001cba0: 6966 206e 6f74 206c 6f61 643a 0a20 2020  if not load:.   
+0001cbb0: 2020 2020 2072 6574 7572 6e20 6669 6c65       return file
+0001cbc0: 6e61 6d65 0a20 2020 2072 6561 6465 7220  name.    reader 
+0001cbd0: 3d20 7079 7669 7374 612e 6765 745f 7265  = pyvista.get_re
+0001cbe0: 6164 6572 2866 696c 656e 616d 6529 0a0a  ader(filename)..
+0001cbf0: 2020 2020 2320 6469 7361 626c 6520 7265      # disable re
+0001cc00: 6164 696e 6720 7468 6520 626f 756e 6461  ading the bounda
+0001cc10: 7279 2070 6174 6368 2e20 4173 206f 6620  ry patch. As of 
+0001cc20: 5654 4b20 392e 312e 3020 7468 6973 2067  VTK 9.1.0 this g
+0001cc30: 656e 6572 6174 6573 0a20 2020 2023 206d  enerates.    # m
+0001cc40: 6573 7361 6765 7320 6c69 6b65 2022 536b  essages like "Sk
+0001cc50: 6970 7069 6e67 2042 435f 7420 6e6f 6465  ipping BC_t node
+0001cc60: 3a20 4243 5f74 2074 7970 6520 2742 4346  : BC_t type 'BCF
+0001cc70: 6172 6669 656c 6427 206e 6f74 2073 7570  arfield' not sup
+0001cc80: 706f 7274 6564 0a20 2020 2023 2079 6574  ported.    # yet
+0001cc90: 2e22 0a20 2020 2072 6561 6465 722e 6c6f  .".    reader.lo
+0001cca0: 6164 5f62 6f75 6e64 6172 795f 7061 7463  ad_boundary_patc
+0001ccb0: 6820 3d20 4661 6c73 650a 2020 2020 7265  h = False.    re
+0001ccc0: 7475 726e 2072 6561 6465 722e 7265 6164  turn reader.read
+0001ccd0: 2829 0a0a 0a64 6566 2064 6f77 6e6c 6f61  ()...def downloa
+0001cce0: 645f 6469 636f 6d5f 7374 6163 6b28 6c6f  d_dicom_stack(lo
+0001ccf0: 6164 3a20 626f 6f6c 203d 2054 7275 6529  ad: bool = True)
+0001cd00: 202d 3e20 556e 696f 6e5b 7079 7669 7374   -> Union[pyvist
+0001cd10: 612e 556e 6966 6f72 6d47 7269 642c 2073  a.UniformGrid, s
+0001cd20: 7472 5d3a 2020 2320 7072 6167 6d61 3a20  tr]:  # pragma: 
+0001cd30: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
+0001cd40: 446f 776e 6c6f 6164 2054 4349 4120 4449  Download TCIA DI
+0001cd50: 434f 4d20 7374 6163 6b20 766f 6c75 6d65  COM stack volume
+0001cd60: 2e0a 0a20 2020 204f 7269 6769 6e61 6c20  ...    Original 
+0001cd70: 646f 776e 6c6f 6164 2066 726f 6d20 7468  download from th
+0001cd80: 6520 6054 6865 2043 616e 6365 7220 496d  e `The Cancer Im
+0001cd90: 6167 696e 6720 4172 6368 6976 6520 2854  aging Archive (T
+0001cda0: 4349 4129 0a20 2020 203c 6874 7470 733a  CIA).    <https:
+0001cdb0: 2f2f 7777 772e 6361 6e63 6572 696d 6167  //www.cancerimag
+0001cdc0: 696e 6761 7263 6869 7665 2e6e 6574 2f3e  ingarchive.net/>
+0001cdd0: 605f 2e20 5468 6973 2069 7320 7061 7274  `_. This is part
+0001cde0: 206f 6620 7468 650a 2020 2020 436c 696e   of the.    Clin
+0001cdf0: 6963 616c 2050 726f 7465 6f6d 6963 2054  ical Proteomic T
+0001ce00: 756d 6f72 2041 6e61 6c79 7369 7320 436f  umor Analysis Co
+0001ce10: 6e73 6f72 7469 756d 2053 6172 636f 6d61  nsortium Sarcoma
+0001ce20: 7320 2843 5054 4143 2d53 4152 290a 2020  s (CPTAC-SAR).  
+0001ce30: 2020 636f 6c6c 6563 7469 6f6e 2e0a 0a20    collection... 
+0001ce40: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0001ce50: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001ce60: 206c 6f61 6420 3a20 626f 6f6c 2c20 6465   load : bool, de
+0001ce70: 6661 756c 743a 2054 7275 650a 2020 2020  fault: True.    
+0001ce80: 2020 2020 4c6f 6164 2074 6865 2064 6174      Load the dat
+0001ce90: 6173 6574 2061 6674 6572 2064 6f77 6e6c  aset after downl
+0001cea0: 6f61 6469 6e67 2069 7420 7768 656e 2060  oading it when `
+0001ceb0: 6054 7275 6560 602e 2020 5365 7420 7468  `True``.  Set th
+0001cec0: 6973 0a20 2020 2020 2020 2074 6f20 6060  is.        to ``
+0001ced0: 4661 6c73 6560 6020 616e 6420 6f6e 6c79  False`` and only
+0001cee0: 2074 6865 2066 696c 656e 616d 6520 7769   the filename wi
+0001cef0: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
+0001cf00: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+0001cf10: 202d 2d2d 2d2d 2d2d 0a20 2020 2070 7976   -------.    pyv
+0001cf20: 6973 7461 2e55 6e69 666f 726d 4772 6964  ista.UniformGrid
+0001cf30: 207c 2073 7472 0a20 2020 2020 2020 2044   | str.        D
+0001cf40: 6174 6153 6574 206f 7220 7061 7468 2064  ataSet or path d
+0001cf50: 6570 656e 6469 6e67 206f 6e20 6060 6c6f  epending on ``lo
+0001cf60: 6164 6060 2e0a 0a20 2020 2052 6566 6572  ad``...    Refer
+0001cf70: 656e 6365 730a 2020 2020 2d2d 2d2d 2d2d  ences.    ------
+0001cf80: 2d2d 2d2d 0a20 2020 202a 202a 2a44 6174  ----.    * **Dat
+0001cf90: 6120 4369 7461 7469 6f6e 2a2a 0a0a 2020  a Citation**..  
+0001cfa0: 2020 2020 2020 4e61 7469 6f6e 616c 2043        National C
+0001cfb0: 616e 6365 7220 496e 7374 6974 7574 6520  ancer Institute 
+0001cfc0: 436c 696e 6963 616c 2050 726f 7465 6f6d  Clinical Proteom
+0001cfd0: 6963 2054 756d 6f72 2041 6e61 6c79 7369  ic Tumor Analysi
+0001cfe0: 7320 436f 6e73 6f72 7469 756d 0a20 2020  s Consortium.   
+0001cff0: 2020 2020 2028 4350 5441 4329 2e20 2832       (CPTAC). (2
+0001d000: 3031 3829 2e20 2052 6164 696f 6c6f 6779  018).  Radiology
+0001d010: 2044 6174 6120 6672 6f6d 2074 6865 2043   Data from the C
+0001d020: 6c69 6e69 6361 6c20 5072 6f74 656f 6d69  linical Proteomi
+0001d030: 6320 5475 6d6f 720a 2020 2020 2020 2020  c Tumor.        
+0001d040: 416e 616c 7973 6973 2043 6f6e 736f 7274  Analysis Consort
+0001d050: 6975 6d20 5361 7263 6f6d 6173 205b 4350  ium Sarcomas [CP
+0001d060: 5441 432d 5341 525d 2063 6f6c 6c65 6374  TAC-SAR] collect
+0001d070: 696f 6e20 5b44 6174 6120 7365 745d 2e20  ion [Data set]. 
+0001d080: 5468 650a 2020 2020 2020 2020 4361 6e63  The.        Canc
+0001d090: 6572 2049 6d61 6769 6e67 2041 7263 6869  er Imaging Archi
+0001d0a0: 7665 2e20 2044 4f49 3a20 3130 2e37 3933  ve.  DOI: 10.793
+0001d0b0: 372f 5443 4941 2e32 3031 392e 3962 7432  7/TCIA.2019.9bt2
+0001d0c0: 3372 3935 0a0a 2020 2020 2a20 2a2a 4163  3r95..    * **Ac
+0001d0d0: 6b6e 6f77 6c65 6467 656d 656e 742a 2a0a  knowledgement**.
+0001d0e0: 0a20 2020 2020 2020 2044 6174 6120 7573  .        Data us
+0001d0f0: 6564 2069 6e20 7468 6973 2070 7562 6c69  ed in this publi
+0001d100: 6361 7469 6f6e 2077 6572 6520 6765 6e65  cation were gene
+0001d110: 7261 7465 6420 6279 2074 6865 204e 6174  rated by the Nat
+0001d120: 696f 6e61 6c20 4361 6e63 6572 2049 6e73  ional Cancer Ins
+0001d130: 7469 7475 7465 2043 6c69 6e69 6361 6c0a  titute Clinical.
+0001d140: 2020 2020 2020 2020 5072 6f74 656f 6d69          Proteomi
+0001d150: 6320 5475 6d6f 7220 416e 616c 7973 6973  c Tumor Analysis
+0001d160: 2043 6f6e 736f 7274 6975 6d20 2843 5054   Consortium (CPT
+0001d170: 4143 292e 0a0a 2020 2020 2a20 2a2a 5443  AC)...    * **TC
+0001d180: 4941 2043 6974 6174 696f 6e2a 2a0a 0a20  IA Citation**.. 
+0001d190: 2020 2020 2020 2043 6c61 726b 204b 2c20         Clark K, 
+0001d1a0: 5665 6e64 7420 422c 2053 6d69 7468 204b  Vendt B, Smith K
+0001d1b0: 2c20 4672 6579 6d61 6e6e 204a 2c20 4b69  , Freymann J, Ki
+0001d1c0: 7262 7920 4a2c 204b 6f70 7065 6c20 502c  rby J, Koppel P,
+0001d1d0: 204d 6f6f 7265 2053 2c20 5068 696c 6c69   Moore S, Philli
+0001d1e0: 7073 2053 2c0a 2020 2020 2020 2020 4d61  ps S,.        Ma
+0001d1f0: 6666 6974 7420 442c 2050 7269 6e67 6c65  ffitt D, Pringle
+0001d200: 204d 2c20 5461 7262 6f78 204c 2c20 5072   M, Tarbox L, Pr
+0001d210: 696f 7220 462e 2054 6865 2043 616e 6365  ior F. The Cance
+0001d220: 7220 496d 6167 696e 6720 4172 6368 6976  r Imaging Archiv
+0001d230: 6520 2854 4349 4129 3a20 2023 2070 7261  e (TCIA):  # pra
+0001d240: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+0001d250: 2020 2020 2020 4d61 696e 7461 696e 696e        Maintainin
+0001d260: 6720 616e 6420 4f70 6572 6174 696e 6720  g and Operating 
+0001d270: 6120 5075 626c 6963 2049 6e66 6f72 6d61  a Public Informa
+0001d280: 7469 6f6e 2052 6570 6f73 6974 6f72 792c  tion Repository,
+0001d290: 204a 6f75 726e 616c 206f 6620 4469 6769   Journal of Digi
+0001d2a0: 7461 6c20 496d 6167 696e 672c 0a20 2020  tal Imaging,.   
+0001d2b0: 2020 2020 2056 6f6c 756d 6520 3236 2c20       Volume 26, 
+0001d2c0: 4e75 6d62 6572 2036 2c20 4465 6365 6d62  Number 6, Decemb
+0001d2d0: 6572 2c20 3230 3133 2c20 7070 2031 3034  er, 2013, pp 104
+0001d2e0: 352d 3130 3537 2e20 646f 693a 2031 302e  5-1057. doi: 10.
+0001d2f0: 3130 3037 2f73 3130 3237 382d 3031 332d  1007/s10278-013-
+0001d300: 3936 3232 2d37 0a0a 2020 2020 4578 616d  9622-7..    Exam
+0001d310: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+0001d320: 2d0a 2020 2020 3e3e 3e20 6672 6f6d 2070  -.    >>> from p
+0001d330: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
+0001d340: 616d 706c 6573 0a20 2020 203e 3e3e 2064  amples.    >>> d
+0001d350: 6174 6173 6574 203d 2065 7861 6d70 6c65  ataset = example
+0001d360: 732e 646f 776e 6c6f 6164 5f64 6963 6f6d  s.download_dicom
+0001d370: 5f73 7461 636b 2829 0a20 2020 203e 3e3e  _stack().    >>>
+0001d380: 2064 6174 6173 6574 2e70 6c6f 7428 766f   dataset.plot(vo
+0001d390: 6c75 6d65 3d54 7275 652c 207a 6f6f 6d3d  lume=True, zoom=
+0001d3a0: 332c 2073 686f 775f 7363 616c 6172 5f62  3, show_scalar_b
+0001d3b0: 6172 3d46 616c 7365 290a 0a20 2020 2022  ar=False)..    "
+0001d3c0: 2222 0a20 2020 2066 6e61 6d65 7320 3d20  "".    fnames = 
+0001d3d0: 5f64 6f77 6e6c 6f61 645f 6172 6368 6976  _download_archiv
+0001d3e0: 6528 2744 4943 4f4d 5f53 7461 636b 2f64  e('DICOM_Stack/d
+0001d3f0: 6174 612e 7a69 7027 290a 2020 2020 7061  ata.zip').    pa
+0001d400: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
+0001d410: 6e61 6d65 2866 6e61 6d65 735b 305d 290a  name(fnames[0]).
+0001d420: 2020 2020 6966 206c 6f61 643a 0a20 2020      if load:.   
+0001d430: 2020 2020 2072 6561 6465 7220 3d20 7079       reader = py
+0001d440: 7669 7374 612e 4449 434f 4d52 6561 6465  vista.DICOMReade
+0001d450: 7228 7061 7468 290a 2020 2020 2020 2020  r(path).        
+0001d460: 7265 7475 726e 2072 6561 6465 722e 7265  return reader.re
+0001d470: 6164 2829 0a20 2020 2072 6574 7572 6e20  ad().    return 
+0001d480: 7061 7468 0a0a 0a64 6566 2064 6f77 6e6c  path...def downl
+0001d490: 6f61 645f 7061 7263 6865 645f 6361 6e61  oad_parched_cana
+0001d4a0: 6c5f 346b 286c 6f61 643d 5472 7565 293a  l_4k(load=True):
+0001d4b0: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
+0001d4c0: 6f76 6572 0a20 2020 2022 2222 446f 776e  over.    """Down
+0001d4d0: 6c6f 6164 2070 6172 6368 6564 2063 616e  load parched can
+0001d4e0: 616c 2034 6b20 6461 7461 7365 742e 0a0a  al 4k dataset...
+0001d4f0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0001d500: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001d510: 2020 6c6f 6164 203a 2062 6f6f 6c2c 2064    load : bool, d
+0001d520: 6566 6175 6c74 3a20 5472 7565 0a20 2020  efault: True.   
+0001d530: 2020 2020 204c 6f61 6420 7468 6520 6461       Load the da
+0001d540: 7461 7365 7420 6166 7465 7220 646f 776e  taset after down
+0001d550: 6c6f 6164 696e 6720 6974 2077 6865 6e20  loading it when 
+0001d560: 6060 5472 7565 6060 2e20 2053 6574 2074  ``True``.  Set t
+0001d570: 6869 730a 2020 2020 2020 2020 746f 2060  his.        to `
+0001d580: 6046 616c 7365 6060 2061 6e64 206f 6e6c  `False`` and onl
+0001d590: 7920 7468 6520 6669 6c65 6e61 6d65 2077  y the filename w
+0001d5a0: 696c 6c20 6265 2072 6574 7572 6e65 642e  ill be returned.
+0001d5b0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+0001d5c0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 7079    -------.    py
+0001d5d0: 7669 7374 612e 5465 7874 7572 6520 7c20  vista.Texture | 
+0001d5e0: 7374 720a 2020 2020 2020 2020 4461 7461  str.        Data
+0001d5f0: 5365 7420 6f72 2066 696c 656e 616d 6520  Set or filename 
+0001d600: 6465 7065 6e64 696e 6720 6f6e 2060 606c  depending on ``l
+0001d610: 6f61 6460 602e 0a0a 2020 2020 4578 616d  oad``...    Exam
+0001d620: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+0001d630: 2d0a 2020 2020 3e3e 3e20 6672 6f6d 2070  -.    >>> from p
+0001d640: 7976 6973 7461 2069 6d70 6f72 7420 6578  yvista import ex
+0001d650: 616d 706c 6573 0a20 2020 203e 3e3e 2064  amples.    >>> d
+0001d660: 6174 6173 6574 203d 2065 7861 6d70 6c65  ataset = example
+0001d670: 732e 646f 776e 6c6f 6164 5f70 6172 6368  s.download_parch
+0001d680: 6564 5f63 616e 616c 5f34 6b28 290a 2020  ed_canal_4k().  
+0001d690: 2020 3e3e 3e20 6461 7461 7365 742e 706c    >>> dataset.pl
+0001d6a0: 6f74 2863 706f 733d 2278 7922 290a 0a20  ot(cpos="xy").. 
+0001d6b0: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
+0001d6c0: 6e20 5f64 6f77 6e6c 6f61 645f 616e 645f  n _download_and_
+0001d6d0: 7265 6164 2822 7061 7263 6865 645f 6361  read("parched_ca
+0001d6e0: 6e61 6c5f 346b 2e68 6472 222c 2074 6578  nal_4k.hdr", tex
+0001d6f0: 7475 7265 3d54 7275 652c 206c 6f61 643d  ture=True, load=
+0001d700: 6c6f 6164 290a 0a0a 6465 6620 646f 776e  load)...def down
+0001d710: 6c6f 6164 5f63 656c 6c73 5f6e 6428 6c6f  load_cells_nd(lo
+0001d720: 6164 3d54 7275 6529 3a20 2023 2070 7261  ad=True):  # pra
+0001d730: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+0001d740: 2020 2222 2244 6f77 6e6c 6f61 6420 6578    """Download ex
+0001d750: 616d 706c 6520 4156 5320 5543 4420 6461  ample AVS UCD da
+0001d760: 7461 7365 742e 0a0a 2020 2020 5061 7261  taset...    Para
+0001d770: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+0001d780: 2d2d 2d2d 2d0a 2020 2020 6c6f 6164 203a  -----.    load :
+0001d790: 2062 6f6f 6c2c 2064 6566 6175 6c74 3a20   bool, default: 
+0001d7a0: 5472 7565 0a20 2020 2020 2020 204c 6f61  True.        Loa
+0001d7b0: 6420 7468 6520 6461 7461 7365 7420 6166  d the dataset af
+0001d7c0: 7465 7220 646f 776e 6c6f 6164 696e 6720  ter downloading 
+0001d7d0: 6974 2077 6865 6e20 6060 5472 7565 6060  it when ``True``
+0001d7e0: 2e20 2053 6574 2074 6869 730a 2020 2020  .  Set this.    
+0001d7f0: 2020 2020 746f 2060 6046 616c 7365 6060      to ``False``
+0001d800: 2061 6e64 206f 6e6c 7920 7468 6520 6669   and only the fi
+0001d810: 6c65 6e61 6d65 2077 696c 6c20 6265 2072  lename will be r
+0001d820: 6574 7572 6e65 642e 0a0a 2020 2020 5265  eturned...    Re
+0001d830: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+0001d840: 2d0a 2020 2020 7079 7669 7374 612e 556e  -.    pyvista.Un
+0001d850: 7374 7275 6374 7572 6564 4772 6964 207c  structuredGrid |
+0001d860: 2073 7472 0a20 2020 2020 2020 2044 6174   str.        Dat
+0001d870: 6153 6574 206f 7220 6669 6c65 6e61 6d65  aSet or filename
+0001d880: 2064 6570 656e 6469 6e67 206f 6e20 6060   depending on ``
+0001d890: 6c6f 6164 6060 2e0a 0a20 2020 2045 7861  load``...    Exa
+0001d8a0: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+0001d8b0: 2d2d 0a20 2020 203e 3e3e 2066 726f 6d20  --.    >>> from 
+0001d8c0: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+0001d8d0: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+0001d8e0: 6461 7461 7365 7420 3d20 6578 616d 706c  dataset = exampl
+0001d8f0: 6573 2e64 6f77 6e6c 6f61 645f 6365 6c6c  es.download_cell
+0001d900: 735f 6e64 2829 0a20 2020 203e 3e3e 2064  s_nd().    >>> d
+0001d910: 6174 6173 6574 2e70 6c6f 7428 6370 6f73  ataset.plot(cpos
+0001d920: 3d22 7879 2229 0a0a 2020 2020 2222 220a  ="xy")..    """.
+0001d930: 2020 2020 7265 7475 726e 205f 646f 776e      return _down
+0001d940: 6c6f 6164 5f61 6e64 5f72 6561 6428 2263  load_and_read("c
+0001d950: 656c 6c73 6e64 2e61 7363 6969 2e69 6e70  ellsnd.ascii.inp
+0001d960: 222c 206c 6f61 643d 6c6f 6164 290a 0a0a  ", load=load)...
+0001d970: 6465 6620 646f 776e 6c6f 6164 5f6d 6f6f  def download_moo
+0001d980: 6e6c 616e 6469 6e67 5f69 6d61 6765 286c  nlanding_image(l
+0001d990: 6f61 643d 5472 7565 293a 2020 2320 7072  oad=True):  # pr
+0001d9a0: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+0001d9b0: 2020 2022 2222 446f 776e 6c6f 6164 2074     """Download t
+0001d9c0: 6865 204d 6f6f 6e20 6c61 6e64 696e 6720  he Moon landing 
+0001d9d0: 696d 6167 652e 0a0a 2020 2020 5468 6973  image...    This
+0001d9e0: 2069 7320 6120 6e6f 6973 7920 696d 6167   is a noisy imag
+0001d9f0: 6520 6f72 6967 696e 616c 6c79 206f 6274  e originally obt
+0001da00: 6169 6e65 6420 6672 6f6d 2060 5363 6970  ained from `Scip
+0001da10: 7920 4c65 6374 7572 6520 4e6f 7465 730a  y Lecture Notes.
+0001da20: 2020 2020 3c68 7474 7073 3a2f 2f73 6369      <https://sci
+0001da30: 7079 2d6c 6563 7475 7265 732e 6f72 672f  py-lectures.org/
+0001da40: 696e 6465 782e 6874 6d6c 3e60 5f20 616e  index.html>`_ an
+0001da50: 6420 6361 6e20 6265 2075 7365 6420 746f  d can be used to
+0001da60: 2064 656d 6f6e 7374 7261 7465 2061 0a20   demonstrate a. 
+0001da70: 2020 206c 6f77 2070 6173 7320 6669 6c74     low pass filt
+0001da80: 6572 2e0a 0a20 2020 2053 6565 2074 6865  er...    See the
+0001da90: 2060 7363 6970 792d 6c65 6374 7572 6573   `scipy-lectures
+0001daa0: 206c 6963 656e 7365 0a20 2020 203c 6874   license.    <ht
+0001dab0: 7470 3a2f 2f73 6369 7079 2d6c 6563 7475  tp://scipy-lectu
+0001dac0: 7265 732e 6f72 672f 7072 6566 6163 652e  res.org/preface.
+0001dad0: 6874 6d6c 236c 6963 656e 7365 3e60 5f20  html#license>`_ 
+0001dae0: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
+0001daf0: 0a20 2020 2072 6567 6172 6469 6e67 2074  .    regarding t
+0001db00: 6869 7320 696d 6167 6527 7320 7573 6520  his image's use 
+0001db10: 616e 6420 6469 7374 7269 6275 7469 6f6e  and distribution
+0001db20: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
+0001db30: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+0001db40: 0a20 2020 206c 6f61 6420 3a20 626f 6f6c  .    load : bool
+0001db50: 2c20 6465 6661 756c 743a 2054 7275 650a  , default: True.
+0001db60: 2020 2020 2020 2020 4c6f 6164 2074 6865          Load the
+0001db70: 2064 6174 6173 6574 2061 6674 6572 2064   dataset after d
+0001db80: 6f77 6e6c 6f61 6469 6e67 2069 7420 7768  ownloading it wh
+0001db90: 656e 2060 6054 7275 6560 602e 2020 5365  en ``True``.  Se
+0001dba0: 7420 7468 6973 0a20 2020 2020 2020 2074  t this.        t
+0001dbb0: 6f20 6060 4661 6c73 6560 6020 616e 6420  o ``False`` and 
+0001dbc0: 6f6e 6c79 2074 6865 2066 696c 656e 616d  only the filenam
+0001dbd0: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
+0001dbe0: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
+0001dbf0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+0001dc00: 2070 7976 6973 7461 2e55 6e69 666f 726d   pyvista.Uniform
+0001dc10: 4772 6964 207c 2073 7472 0a20 2020 2020  Grid | str.     
+0001dc20: 2020 2060 6044 6174 6153 6574 6060 206f     ``DataSet`` o
+0001dc30: 7220 6669 6c65 6e61 6d65 2064 6570 656e  r filename depen
+0001dc40: 6469 6e67 206f 6e20 6060 6c6f 6164 6060  ding on ``load``
+0001dc50: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
+0001dc60: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001dc70: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
+0001dc80: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
+0001dc90: 730a 2020 2020 3e3e 3e20 6461 7461 7365  s.    >>> datase
+0001dca0: 7420 3d20 6578 616d 706c 6573 2e64 6f77  t = examples.dow
+0001dcb0: 6e6c 6f61 645f 6d6f 6f6e 6c61 6e64 696e  nload_moonlandin
+0001dcc0: 675f 696d 6167 6528 290a 2020 2020 3e3e  g_image().    >>
+0001dcd0: 3e20 6461 7461 7365 742e 706c 6f74 280a  > dataset.plot(.
+0001dce0: 2020 2020 2e2e 2e20 2020 2020 6370 6f73      ...     cpos
+0001dcf0: 3d27 7879 272c 0a20 2020 202e 2e2e 2020  ='xy',.    ...  
+0001dd00: 2020 2063 6d61 703d 2767 7261 7927 2c0a     cmap='gray',.
+0001dd10: 2020 2020 2e2e 2e20 2020 2020 6261 636b      ...     back
+0001dd20: 6772 6f75 6e64 3d27 7727 2c0a 2020 2020  ground='w',.    
+0001dd30: 2e2e 2e20 2020 2020 7368 6f77 5f73 6361  ...     show_sca
+0001dd40: 6c61 725f 6261 723d 4661 6c73 652c 0a20  lar_bar=False,. 
+0001dd50: 2020 202e 2e2e 2029 0a0a 2020 2020 5365     ... )..    Se
+0001dd60: 6520 3a72 6566 3a60 696d 6167 655f 6666  e :ref:`image_ff
+0001dd70: 745f 6578 616d 706c 6560 2066 6f72 2061  t_example` for a
+0001dd80: 2066 756c 6c20 6578 616d 706c 6520 7573   full example us
+0001dd90: 696e 6720 7468 6973 2064 6174 6173 6574  ing this dataset
+0001dda0: 2e0a 0a20 2020 2022 2222 0a20 2020 2072  ...    """.    r
+0001ddb0: 6574 7572 6e20 5f64 6f77 6e6c 6f61 645f  eturn _download_
+0001ddc0: 616e 645f 7265 6164 2827 6d6f 6f6e 6c61  and_read('moonla
+0001ddd0: 6e64 696e 672e 706e 6727 2c20 6c6f 6164  nding.png', load
+0001dde0: 3d6c 6f61 6429 0a0a 0a64 6566 2064 6f77  =load)...def dow
+0001ddf0: 6e6c 6f61 645f 616e 6775 6c61 725f 7365  nload_angular_se
+0001de00: 6374 6f72 286c 6f61 643d 5472 7565 293a  ctor(load=True):
+0001de10: 2020 2320 7072 6167 6d61 3a20 6e6f 2063    # pragma: no c
+0001de20: 6f76 6572 0a20 2020 2022 2222 446f 776e  over.    """Down
+0001de30: 6c6f 6164 2074 6865 2061 6e67 756c 6172  load the angular
+0001de40: 2073 6563 746f 7220 6461 7461 7365 742e   sector dataset.
+0001de50: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+0001de60: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0001de70: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
+0001de80: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
+0001de90: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
+0001dea0: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
+0001deb0: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
+0001dec0: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
+0001ded0: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
+0001dee0: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
+0001def0: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
+0001df00: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+0001df10: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
+0001df20: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0001df30: 7079 7669 7374 612e 556e 7374 7275 6374  pyvista.Unstruct
+0001df40: 7572 6564 4772 6964 207c 2073 7472 0a20  uredGrid | str. 
+0001df50: 2020 2020 2020 2044 6174 6153 6574 206f         DataSet o
+0001df60: 7220 6669 6c65 6e61 6d65 2064 6570 656e  r filename depen
+0001df70: 6469 6e67 206f 6e20 6060 6c6f 6164 6060  ding on ``load``
+0001df80: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
+0001df90: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001dfa0: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
+0001dfb0: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
+0001dfc0: 730a 2020 2020 3e3e 3e20 6461 7461 7365  s.    >>> datase
+0001dfd0: 7420 3d20 6578 616d 706c 6573 2e64 6f77  t = examples.dow
+0001dfe0: 6e6c 6f61 645f 616e 6775 6c61 725f 7365  nload_angular_se
+0001dff0: 6374 6f72 2829 0a20 2020 203e 3e3e 2064  ctor().    >>> d
+0001e000: 6174 6173 6574 2e70 6c6f 7428 7363 616c  ataset.plot(scal
+0001e010: 6172 733d 2750 6f69 6e74 4964 2729 0a0a  ars='PointId')..
+0001e020: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
+0001e030: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
+0001e040: 5f72 6561 6428 2741 6e67 756c 6172 5365  _read('AngularSe
+0001e050: 6374 6f72 2e76 746b 272c 206c 6f61 643d  ctor.vtk', load=
+0001e060: 6c6f 6164 290a 0a0a 6465 6620 646f 776e  load)...def down
+0001e070: 6c6f 6164 5f6d 6f75 6e74 5f64 616d 6176  load_mount_damav
+0001e080: 616e 6428 6c6f 6164 3d54 7275 6529 3a20  and(load=True): 
+0001e090: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+0001e0a0: 7665 720a 2020 2020 2222 2244 6f77 6e6c  ver.    """Downl
+0001e0b0: 6f61 6420 7468 6520 4d6f 756e 7420 4461  oad the Mount Da
+0001e0c0: 6d61 7661 6e64 2064 6174 6173 6574 2e0a  mavand dataset..
+0001e0d0: 0a20 2020 2056 6973 7561 6c69 7a65 2033  .    Visualize 3
+0001e0e0: 4420 6d6f 6465 6c73 206f 6620 4461 6d61  D models of Dama
+0001e0f0: 7661 6e64 2056 6f6c 6361 6e6f 2c20 416c  vand Volcano, Al
+0001e100: 626f 727a 2c20 4972 616e 2e20 5468 6973  borz, Iran. This
+0001e110: 2069 7320 6120 3244 206d 6170 0a20 2020   is a 2D map.   
+0001e120: 2077 6974 6820 7468 6520 616c 7469 7475   with the altitu
+0001e130: 6465 2065 6d62 6564 6465 6420 6173 2060  de embedded as `
+0001e140: 6027 7a27 6060 2063 656c 6c20 6461 7461  `'z'`` cell data
+0001e150: 2077 6974 6869 6e20 7468 650a 2020 2020   within the.    
+0001e160: 3a63 6c61 7373 3a60 7079 7669 7374 612e  :class:`pyvista.
+0001e170: 506f 6c79 4461 7461 602e 0a0a 2020 2020  PolyData`...    
+0001e180: 4f72 6967 696e 616c 6c79 2070 6f73 7465  Originally poste
+0001e190: 6420 6174 2060 6261 6e65 7375 6c6c 6976  d at `banesulliv
+0001e1a0: 616e 2f64 616d 6176 616e 642d 766f 6c63  an/damavand-volc
+0001e1b0: 616e 6f0a 2020 2020 3c68 7474 7073 3a2f  ano.    <https:/
+0001e1c0: 2f67 6974 6875 622e 636f 6d2f 6261 6e65  /github.com/bane
+0001e1d0: 7375 6c6c 6976 616e 2f64 616d 6176 616e  sullivan/damavan
+0001e1e0: 642d 766f 6c63 616e 6f3e 605f 2e0a 0a20  d-volcano>`_... 
+0001e1f0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0001e200: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001e210: 206c 6f61 6420 3a20 626f 6f6c 2c20 6465   load : bool, de
+0001e220: 6661 756c 743a 2054 7275 650a 2020 2020  fault: True.    
+0001e230: 2020 2020 4c6f 6164 2074 6865 2064 6174      Load the dat
+0001e240: 6173 6574 2061 6674 6572 2064 6f77 6e6c  aset after downl
+0001e250: 6f61 6469 6e67 2069 7420 7768 656e 2060  oading it when `
+0001e260: 6054 7275 6560 602e 2020 5365 7420 7468  `True``.  Set th
+0001e270: 6973 0a20 2020 2020 2020 2074 6f20 6060  is.        to ``
+0001e280: 4661 6c73 6560 6020 616e 6420 6f6e 6c79  False`` and only
+0001e290: 2074 6865 2066 696c 656e 616d 6520 7769   the filename wi
+0001e2a0: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
+0001e2b0: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+0001e2c0: 202d 2d2d 2d2d 2d2d 0a20 2020 2070 7976   -------.    pyv
+0001e2d0: 6973 7461 2e50 6f6c 7944 6174 6120 7c20  ista.PolyData | 
+0001e2e0: 7374 720a 2020 2020 2020 2020 4461 7461  str.        Data
+0001e2f0: 5365 7420 6f72 2066 696c 656e 616d 6520  Set or filename 
+0001e300: 6465 7065 6e64 696e 6720 6f6e 2060 606c  depending on ``l
+0001e310: 6f61 6460 602e 0a0a 2020 2020 4578 616d  oad``...    Exam
+0001e320: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+0001e330: 2d0a 2020 2020 446f 776e 6c6f 6164 2074  -.    Download t
+0001e340: 6865 2044 616d 6176 616e 6420 6461 7461  he Damavand data
+0001e350: 7365 7420 616e 6420 706c 6f74 2069 7420  set and plot it 
+0001e360: 6166 7465 7220 7761 7270 696e 6720 6974  after warping it
+0001e370: 2062 7920 6974 7320 616c 7469 7475 6465   by its altitude
+0001e380: 2e0a 0a20 2020 203e 3e3e 2066 726f 6d20  ...    >>> from 
+0001e390: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+0001e3a0: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+0001e3b0: 6461 7461 7365 7420 3d20 6578 616d 706c  dataset = exampl
+0001e3c0: 6573 2e64 6f77 6e6c 6f61 645f 6d6f 756e  es.download_moun
+0001e3d0: 745f 6461 6d61 7661 6e64 2829 0a20 2020  t_damavand().   
+0001e3e0: 203e 3e3e 2064 6174 6173 6574 203d 2064   >>> dataset = d
+0001e3f0: 6174 6173 6574 2e63 656c 6c5f 6461 7461  ataset.cell_data
+0001e400: 5f74 6f5f 706f 696e 745f 6461 7461 2829  _to_point_data()
+0001e410: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
+0001e420: 203d 2064 6174 6173 6574 2e77 6172 705f   = dataset.warp_
+0001e430: 6279 5f73 6361 6c61 7228 277a 272c 2066  by_scalar('z', f
+0001e440: 6163 746f 723d 3229 0a20 2020 203e 3e3e  actor=2).    >>>
+0001e450: 2064 6174 6173 6574 2e70 6c6f 7428 636d   dataset.plot(cm
+0001e460: 6170 3d27 6769 7374 5f65 6172 7468 272c  ap='gist_earth',
+0001e470: 2073 686f 775f 7363 616c 6172 5f62 6172   show_scalar_bar
+0001e480: 3d46 616c 7365 290a 0a20 2020 2022 2222  =False)..    """
+0001e490: 0a20 2020 2072 6574 7572 6e20 5f64 6f77  .    return _dow
+0001e4a0: 6e6c 6f61 645f 616e 645f 7265 6164 2827  nload_and_read('
+0001e4b0: 414f 492e 4461 6d61 7661 6e64 2e33 3236  AOI.Damavand.326
+0001e4c0: 3339 2e76 7470 272c 206c 6f61 643d 6c6f  39.vtp', load=lo
+0001e4d0: 6164 290a 0a0a 6465 6620 646f 776e 6c6f  ad)...def downlo
+0001e4e0: 6164 5f70 6172 7469 636c 6573 5f6c 6574  ad_particles_let
+0001e4f0: 6865 286c 6f61 643d 5472 7565 293a 2020  he(load=True):  
+0001e500: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+0001e510: 6572 0a20 2020 2022 2222 446f 776e 6c6f  er.    """Downlo
+0001e520: 6164 2061 2070 6172 7469 636c 6573 2064  ad a particles d
+0001e530: 6174 6173 6574 2067 656e 6572 6174 6564  ataset generated
+0001e540: 2062 7920 606c 6574 6865 203c 6874 7470   by `lethe <http
+0001e550: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
+0001e560: 6574 6865 2d63 6664 2f6c 6574 6865 3e60  ethe-cfd/lethe>`
+0001e570: 5f20 2e0a 0a20 2020 2053 6565 2060 5079  _ ...    See `Py
+0001e580: 5669 7374 6120 6469 7363 7573 7369 6f6e  Vista discussion
+0001e590: 7320 2331 3938 340a 2020 2020 3c68 7474  s #1984.    <htt
+0001e5a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0001e5b0: 7079 7669 7374 612f 7079 7669 7374 612f  pyvista/pyvista/
+0001e5c0: 6469 7363 7573 7369 6f6e 732f 3139 3834  discussions/1984
+0001e5d0: 3e60 5f0a 0a20 2020 2050 6172 616d 6574  >`_..    Paramet
+0001e5e0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+0001e5f0: 2d2d 0a20 2020 206c 6f61 6420 3a20 626f  --.    load : bo
+0001e600: 6f6c 2c20 6465 6661 756c 743a 2054 7275  ol, default: Tru
+0001e610: 650a 2020 2020 2020 2020 4c6f 6164 2074  e.        Load t
+0001e620: 6865 2064 6174 6173 6574 2061 6674 6572  he dataset after
+0001e630: 2064 6f77 6e6c 6f61 6469 6e67 2069 7420   downloading it 
+0001e640: 7768 656e 2060 6054 7275 6560 602e 2020  when ``True``.  
+0001e650: 5365 7420 7468 6973 0a20 2020 2020 2020  Set this.       
+0001e660: 2074 6f20 6060 4661 6c73 6560 6020 616e   to ``False`` an
+0001e670: 6420 6f6e 6c79 2074 6865 2066 696c 656e  d only the filen
+0001e680: 616d 6520 7769 6c6c 2062 6520 7265 7475  ame will be retu
+0001e690: 726e 6564 2e0a 0a20 2020 2052 6574 7572  rned...    Retur
+0001e6a0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+0001e6b0: 2020 2070 7976 6973 7461 2e55 6e73 7472     pyvista.Unstr
+0001e6c0: 7563 7475 7265 6447 7269 6420 7c20 7374  ucturedGrid | st
+0001e6d0: 720a 2020 2020 2020 2020 4461 7461 5365  r.        DataSe
+0001e6e0: 7420 6f72 2066 696c 656e 616d 6520 6465  t or filename de
+0001e6f0: 7065 6e64 696e 6720 6f6e 2060 606c 6f61  pending on ``loa
+0001e700: 6460 602e 0a0a 2020 2020 4578 616d 706c  d``...    Exampl
+0001e710: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
+0001e720: 2020 2020 446f 776e 6c6f 6164 2074 6865      Download the
+0001e730: 2070 6172 7469 636c 6573 2064 6174 6173   particles datas
+0001e740: 6574 2061 6e64 2070 6c6f 7420 6974 2061  et and plot it a
+0001e750: 6674 6572 2067 656e 6572 6174 696e 6720  fter generating 
+0001e760: 676c 7970 6873 2e0a 0a20 2020 203e 3e3e  glyphs...    >>>
+0001e770: 2066 726f 6d20 7079 7669 7374 6120 696d   from pyvista im
+0001e780: 706f 7274 2065 7861 6d70 6c65 730a 2020  port examples.  
+0001e790: 2020 3e3e 3e20 7061 7274 6963 6c65 7320    >>> particles 
+0001e7a0: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
+0001e7b0: 6f61 645f 7061 7274 6963 6c65 735f 6c65  oad_particles_le
+0001e7c0: 7468 6528 290a 2020 2020 3e3e 3e20 7061  the().    >>> pa
+0001e7d0: 7274 6963 6c65 732e 706c 6f74 280a 2020  rticles.plot(.  
+0001e7e0: 2020 2e2e 2e20 2020 2020 7265 6e64 6572    ...     render
+0001e7f0: 5f70 6f69 6e74 735f 6173 5f73 7068 6572  _points_as_spher
+0001e800: 6573 3d54 7275 652c 0a20 2020 202e 2e2e  es=True,.    ...
+0001e810: 2020 2020 2073 7479 6c65 3d27 706f 696e       style='poin
+0001e820: 7473 272c 0a20 2020 202e 2e2e 2020 2020  ts',.    ...    
+0001e830: 2073 6361 6c61 7273 3d27 5665 6c6f 6369   scalars='Veloci
+0001e840: 7479 272c 0a20 2020 202e 2e2e 2020 2020  ty',.    ...    
+0001e850: 2062 6163 6b67 726f 756e 643d 2777 272c   background='w',
+0001e860: 0a20 2020 202e 2e2e 2020 2020 2073 6361  .    ...     sca
+0001e870: 6c61 725f 6261 725f 6172 6773 3d7b 2763  lar_bar_args={'c
+0001e880: 6f6c 6f72 273a 2027 6b27 7d2c 0a20 2020  olor': 'k'},.   
+0001e890: 202e 2e2e 2020 2020 2063 6d61 703d 2762   ...     cmap='b
+0001e8a0: 7772 272c 0a20 2020 202e 2e2e 2029 0a0a  wr',.    ... )..
+0001e8b0: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
+0001e8c0: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
+0001e8d0: 5f72 6561 6428 276c 6574 6865 2f72 6573  _read('lethe/res
+0001e8e0: 756c 745f 7061 7274 6963 6c65 732e 3230  ult_particles.20
+0001e8f0: 3030 302e 3030 3030 2e76 7475 272c 206c  000.0000.vtu', l
+0001e900: 6f61 643d 6c6f 6164 290a 0a0a 6465 6620  oad=load)...def 
+0001e910: 646f 776e 6c6f 6164 5f67 6966 5f73 696d  download_gif_sim
+0001e920: 706c 6528 6c6f 6164 3d54 7275 6529 3a20  ple(load=True): 
+0001e930: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+0001e940: 7665 720a 2020 2020 2222 2244 6f77 6e6c  ver.    """Downl
+0001e950: 6f61 6420 6120 7369 6d70 6c65 2074 6872  oad a simple thr
+0001e960: 6565 2066 7261 6d65 2047 4946 2e0a 0a20  ee frame GIF... 
+0001e970: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0001e980: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001e990: 206c 6f61 6420 3a20 626f 6f6c 2c20 6465   load : bool, de
+0001e9a0: 6661 756c 743a 2054 7275 650a 2020 2020  fault: True.    
+0001e9b0: 2020 2020 4c6f 6164 2074 6865 2064 6174      Load the dat
+0001e9c0: 6173 6574 2061 6674 6572 2064 6f77 6e6c  aset after downl
+0001e9d0: 6f61 6469 6e67 2069 7420 7768 656e 2060  oading it when `
+0001e9e0: 6054 7275 6560 602e 2020 5365 7420 7468  `True``.  Set th
+0001e9f0: 6973 0a20 2020 2020 2020 2074 6f20 6060  is.        to ``
+0001ea00: 4661 6c73 6560 6020 616e 6420 6f6e 6c79  False`` and only
+0001ea10: 2074 6865 2066 696c 656e 616d 6520 7769   the filename wi
+0001ea20: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
+0001ea30: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+0001ea40: 202d 2d2d 2d2d 2d2d 0a20 2020 2070 7976   -------.    pyv
+0001ea50: 6973 7461 2e55 6e69 666f 726d 4772 6964  ista.UniformGrid
+0001ea60: 207c 2073 7472 0a20 2020 2020 2020 2044   | str.        D
+0001ea70: 6174 6153 6574 206f 7220 6669 6c65 6e61  ataSet or filena
+0001ea80: 6d65 2064 6570 656e 6469 6e67 206f 6e20  me depending on 
+0001ea90: 6060 6c6f 6164 6060 2e0a 0a20 2020 2045  ``load``...    E
+0001eaa0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+0001eab0: 2d2d 2d2d 0a20 2020 2044 6f77 6e6c 6f61  ----.    Downloa
+0001eac0: 6420 616e 6420 706c 6f74 2074 6865 2066  d and plot the f
+0001ead0: 6972 7374 2066 7261 6d65 206f 6620 6120  irst frame of a 
+0001eae0: 7369 6d70 6c65 2047 4946 2e0a 0a20 2020  simple GIF...   
+0001eaf0: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
+0001eb00: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
+0001eb10: 730a 2020 2020 3e3e 3e20 6772 6964 203d  s.    >>> grid =
+0001eb20: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
+0001eb30: 6164 5f67 6966 5f73 696d 706c 6528 290a  ad_gif_simple().
+0001eb40: 2020 2020 3e3e 3e20 6772 6964 2e70 6c6f      >>> grid.plo
+0001eb50: 7428 0a20 2020 202e 2e2e 2020 2020 2073  t(.    ...     s
+0001eb60: 6361 6c61 7273 3d27 6672 616d 6530 272c  calars='frame0',
+0001eb70: 0a20 2020 202e 2e2e 2020 2020 2072 6762  .    ...     rgb
+0001eb80: 3d54 7275 652c 0a20 2020 202e 2e2e 2020  =True,.    ...  
+0001eb90: 2020 2062 6163 6b67 726f 756e 643d 2777     background='w
+0001eba0: 272c 0a20 2020 202e 2e2e 2020 2020 2073  ',.    ...     s
+0001ebb0: 686f 775f 7363 616c 6172 5f62 6172 3d46  how_scalar_bar=F
+0001ebc0: 616c 7365 2c0a 2020 2020 2e2e 2e20 2020  alse,.    ...   
+0001ebd0: 2020 6370 6f73 3d27 7879 272c 0a20 2020    cpos='xy',.   
+0001ebe0: 202e 2e2e 2029 0a0a 2020 2020 506c 6f74   ... )..    Plot
+0001ebf0: 2074 6865 2073 6563 6f6e 6420 6672 616d   the second fram
+0001ec00: 652e 0a0a 2020 2020 3e3e 3e20 6772 6964  e...    >>> grid
+0001ec10: 2e70 6c6f 7428 0a20 2020 202e 2e2e 2020  .plot(.    ...  
+0001ec20: 2020 2073 6361 6c61 7273 3d27 6672 616d     scalars='fram
+0001ec30: 6531 272c 0a20 2020 202e 2e2e 2020 2020  e1',.    ...    
+0001ec40: 2072 6762 3d54 7275 652c 0a20 2020 202e   rgb=True,.    .
+0001ec50: 2e2e 2020 2020 2062 6163 6b67 726f 756e  ..     backgroun
+0001ec60: 643d 2777 272c 0a20 2020 202e 2e2e 2020  d='w',.    ...  
+0001ec70: 2020 2073 686f 775f 7363 616c 6172 5f62     show_scalar_b
+0001ec80: 6172 3d46 616c 7365 2c0a 2020 2020 2e2e  ar=False,.    ..
+0001ec90: 2e20 2020 2020 6370 6f73 3d27 7879 272c  .     cpos='xy',
+0001eca0: 0a20 2020 202e 2e2e 2029 0a0a 2020 2020  .    ... )..    
+0001ecb0: 2222 220a 2020 2020 7265 7475 726e 205f  """.    return _
+0001ecc0: 646f 776e 6c6f 6164 5f61 6e64 5f72 6561  download_and_rea
+0001ecd0: 6428 2767 6966 732f 7361 6d70 6c65 2e67  d('gifs/sample.g
+0001ece0: 6966 272c 206c 6f61 643d 6c6f 6164 290a  if', load=load).
+0001ecf0: 0a0a 6465 6620 646f 776e 6c6f 6164 5f63  ..def download_c
+0001ed00: 6c6f 7564 5f64 6172 6b5f 6d61 7474 6572  loud_dark_matter
+0001ed10: 286c 6f61 643d 5472 7565 293a 2020 2320  (load=True):  # 
+0001ed20: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+0001ed30: 0a20 2020 2022 2222 446f 776e 6c6f 6164  .    """Download
+0001ed40: 2070 6172 7469 636c 6573 2066 726f 6d20   particles from 
+0001ed50: 6120 7369 6d75 6c61 7465 6420 6461 726b  a simulated dark
+0001ed60: 206d 6174 7465 7220 6861 6c6f 2e0a 0a20   matter halo... 
+0001ed70: 2020 2054 6869 7320 6461 7461 7365 7420     This dataset 
+0001ed80: 636f 6e74 6169 6e73 2033 322c 3331 3420  contains 32,314 
+0001ed90: 7061 7274 6963 6c65 732e 0a0a 2020 2020  particles...    
+0001eda0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0001edb0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f  ---------.    lo
+0001edc0: 6164 203a 2062 6f6f 6c2c 2064 6566 6175  ad : bool, defau
+0001edd0: 6c74 3a20 5472 7565 0a20 2020 2020 2020  lt: True.       
+0001ede0: 204c 6f61 6420 7468 6520 6461 7461 7365   Load the datase
+0001edf0: 7420 6166 7465 7220 646f 776e 6c6f 6164  t after download
+0001ee00: 696e 6720 6974 2077 6865 6e20 6060 5472  ing it when ``Tr
+0001ee10: 7565 6060 2e20 2053 6574 2074 6869 730a  ue``.  Set this.
+0001ee20: 2020 2020 2020 2020 746f 2060 6046 616c          to ``Fal
+0001ee30: 7365 6060 2061 6e64 206f 6e6c 7920 7468  se`` and only th
+0001ee40: 6520 6669 6c65 6e61 6d65 2077 696c 6c20  e filename will 
+0001ee50: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
+0001ee60: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+0001ee70: 2d2d 2d2d 2d0a 2020 2020 7079 7669 7374  -----.    pyvist
+0001ee80: 612e 506f 696e 7453 6574 207c 2073 7472  a.PointSet | str
+0001ee90: 0a20 2020 2020 2020 2044 6174 6153 6574  .        DataSet
+0001eea0: 206f 7220 6669 6c65 6e61 6d65 2064 6570   or filename dep
+0001eeb0: 656e 6469 6e67 206f 6e20 6060 6c6f 6164  ending on ``load
+0001eec0: 6060 2e0a 0a20 2020 2045 7861 6d70 6c65  ``...    Example
+0001eed0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
+0001eee0: 2020 2044 6f77 6e6c 6f61 6420 7468 6520     Download the 
+0001eef0: 6461 726b 206d 6174 7465 7220 636c 6f75  dark matter clou
+0001ef00: 6420 616e 6420 6469 7370 6c61 7920 6974  d and display it
+0001ef10: 7320 7265 7072 6573 656e 7461 7469 6f6e  s representation
+0001ef20: 2e0a 0a20 2020 203e 3e3e 2069 6d70 6f72  ...    >>> impor
+0001ef30: 7420 6e75 6d70 7920 6173 206e 700a 2020  t numpy as np.  
+0001ef40: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
+0001ef50: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
+0001ef60: 6573 0a20 2020 203e 3e3e 2070 6320 3d20  es.    >>> pc = 
+0001ef70: 6578 616d 706c 6573 2e64 6f77 6e6c 6f61  examples.downloa
+0001ef80: 645f 636c 6f75 645f 6461 726b 5f6d 6174  d_cloud_dark_mat
+0001ef90: 7465 7228 290a 2020 2020 3e3e 3e20 7063  ter().    >>> pc
+0001efa0: 0a20 2020 2050 6f69 6e74 5365 7420 282e  .    PointSet (.
+0001efb0: 2e2e 290a 2020 2020 2020 4e20 4365 6c6c  ..).      N Cell
+0001efc0: 733a 2020 2020 300a 2020 2020 2020 4e20  s:    0.      N 
+0001efd0: 506f 696e 7473 3a20 2020 3332 3331 340a  Points:   32314.
+0001efe0: 2020 2020 2020 5820 426f 756e 6473 3a20        X Bounds: 
+0001eff0: 2020 372e 3435 3165 2b30 312c 2037 2e38    7.451e+01, 7.8
+0001f000: 3932 652b 3031 0a20 2020 2020 2059 2042  92e+01.      Y B
+0001f010: 6f75 6e64 733a 2020 2031 2e36 3136 652b  ounds:   1.616e+
+0001f020: 3031 2c20 322e 3237 3565 2b30 310a 2020  01, 2.275e+01.  
+0001f030: 2020 2020 5a20 426f 756e 6473 3a20 2020      Z Bounds:   
+0001f040: 382e 3930 3065 2b30 312c 2039 2e33 3139  8.900e+01, 9.319
+0001f050: 652b 3031 0a20 2020 2020 204e 2041 7272  e+01.      N Arr
+0001f060: 6179 733a 2020 2030 0a0a 2020 2020 506c  ays:   0..    Pl
+0001f070: 6f74 2074 6865 2070 6f69 6e74 2063 6c6f  ot the point clo
+0001f080: 7564 2e20 436f 6c6f 7220 6261 7365 6420  ud. Color based 
+0001f090: 6f6e 2074 6865 2064 6973 7461 6e63 6520  on the distance 
+0001f0a0: 6672 6f6d 2074 6865 2063 656e 7465 7220  from the center 
+0001f0b0: 6f66 2074 6865 0a20 2020 2063 6c6f 7564  of the.    cloud
+0001f0c0: 2e0a 0a20 2020 203e 3e3e 2070 632e 706c  ...    >>> pc.pl
+0001f0d0: 6f74 280a 2020 2020 2e2e 2e20 2020 2020  ot(.    ...     
+0001f0e0: 7363 616c 6172 733d 6e70 2e6c 696e 616c  scalars=np.linal
+0001f0f0: 672e 6e6f 726d 2870 632e 706f 696e 7473  g.norm(pc.points
+0001f100: 202d 2070 632e 6365 6e74 6572 2c20 6178   - pc.center, ax
+0001f110: 6973 3d31 292c 0a20 2020 202e 2e2e 2020  is=1),.    ...  
+0001f120: 2020 2073 7479 6c65 3d27 706f 696e 7473     style='points
+0001f130: 5f67 6175 7373 6961 6e27 2c0a 2020 2020  _gaussian',.    
+0001f140: 2e2e 2e20 2020 2020 6f70 6163 6974 793d  ...     opacity=
+0001f150: 302e 352c 0a20 2020 202e 2e2e 2020 2020  0.5,.    ...    
+0001f160: 2070 6f69 6e74 5f73 697a 653d 312e 352c   point_size=1.5,
+0001f170: 0a20 2020 202e 2e2e 2020 2020 2073 686f  .    ...     sho
+0001f180: 775f 7363 616c 6172 5f62 6172 3d46 616c  w_scalar_bar=Fal
+0001f190: 7365 2c0a 2020 2020 2e2e 2e20 2020 2020  se,.    ...     
+0001f1a0: 7a6f 6f6d 3d32 2c0a 2020 2020 2e2e 2e20  zoom=2,.    ... 
+0001f1b0: 290a 0a20 2020 2053 6565 2074 6865 203a  )..    See the :
+0001f1c0: 7265 663a 6070 6c6f 7474 696e 675f 706f  ref:`plotting_po
+0001f1d0: 696e 745f 636c 6f75 6473 6020 666f 7220  int_clouds` for 
+0001f1e0: 6120 6675 6c6c 2065 7861 6d70 6c65 2075  a full example u
+0001f1f0: 7369 6e67 2074 6869 7320 6461 7461 7365  sing this datase
+0001f200: 742e 0a0a 2020 2020 2222 220a 2020 2020  t...    """.    
+0001f210: 6669 6c65 6e61 6d65 203d 2064 6f77 6e6c  filename = downl
+0001f220: 6f61 645f 6669 6c65 2827 706f 696e 742d  oad_file('point-
+0001f230: 636c 6f75 6473 2f66 696e 6475 7332 332f  clouds/findus23/
+0001f240: 6861 6c6f 5f6c 6f77 5f72 6573 2e6e 7079  halo_low_res.npy
+0001f250: 2729 0a0a 2020 2020 6966 206c 6f61 643a  ')..    if load:
+0001f260: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001f270: 7079 7669 7374 612e 506f 696e 7453 6574  pyvista.PointSet
+0001f280: 286e 702e 6c6f 6164 2866 696c 656e 616d  (np.load(filenam
+0001f290: 6529 290a 2020 2020 7265 7475 726e 2066  e)).    return f
+0001f2a0: 696c 656e 616d 650a 0a0a 6465 6620 646f  ilename...def do
+0001f2b0: 776e 6c6f 6164 5f63 6c6f 7564 5f64 6172  wnload_cloud_dar
+0001f2c0: 6b5f 6d61 7474 6572 5f64 656e 7365 286c  k_matter_dense(l
+0001f2d0: 6f61 643d 5472 7565 293a 2020 2320 7072  oad=True):  # pr
+0001f2e0: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+0001f2f0: 2020 2022 2222 446f 776e 6c6f 6164 2061     """Download a
+0001f300: 2070 6172 7469 636c 6573 2066 726f 6d20   particles from 
+0001f310: 6120 7369 6d75 6c61 7465 6420 6461 726b  a simulated dark
+0001f320: 206d 6174 7465 7220 6861 6c6f 2e0a 0a20   matter halo... 
+0001f330: 2020 2054 6869 7320 6461 7461 7365 7420     This dataset 
+0001f340: 636f 6e74 6169 6e73 2032 2c30 3632 2c32  contains 2,062,2
+0001f350: 3536 2070 6172 7469 636c 6573 2e0a 0a20  56 particles... 
+0001f360: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0001f370: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001f380: 206c 6f61 6420 3a20 626f 6f6c 2c20 6465   load : bool, de
+0001f390: 6661 756c 743a 2054 7275 650a 2020 2020  fault: True.    
+0001f3a0: 2020 2020 4c6f 6164 2074 6865 2064 6174      Load the dat
+0001f3b0: 6173 6574 2061 6674 6572 2064 6f77 6e6c  aset after downl
+0001f3c0: 6f61 6469 6e67 2069 7420 7768 656e 2060  oading it when `
+0001f3d0: 6054 7275 6560 602e 2020 5365 7420 7468  `True``.  Set th
+0001f3e0: 6973 0a20 2020 2020 2020 2074 6f20 6060  is.        to ``
+0001f3f0: 4661 6c73 6560 6020 616e 6420 6f6e 6c79  False`` and only
+0001f400: 2074 6865 2066 696c 656e 616d 6520 7769   the filename wi
+0001f410: 6c6c 2062 6520 7265 7475 726e 6564 2e0a  ll be returned..
+0001f420: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+0001f430: 202d 2d2d 2d2d 2d2d 0a20 2020 2070 7976   -------.    pyv
+0001f440: 6973 7461 2e50 6f69 6e74 5365 7420 7c20  ista.PointSet | 
+0001f450: 7374 720a 2020 2020 2020 2020 4461 7461  str.        Data
+0001f460: 5365 7420 6f72 2066 696c 656e 616d 6520  Set or filename 
+0001f470: 6465 7065 6e64 696e 6720 6f6e 2060 606c  depending on ``l
+0001f480: 6f61 6460 602e 0a0a 2020 2020 4578 616d  oad``...    Exam
+0001f490: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+0001f4a0: 2d0a 2020 2020 446f 776e 6c6f 6164 2074  -.    Download t
+0001f4b0: 6865 2064 6172 6b20 6d61 7474 6572 2063  he dark matter c
+0001f4c0: 6c6f 7564 2061 6e64 2064 6973 706c 6179  loud and display
+0001f4d0: 2069 7473 2072 6570 7265 7365 6e74 6174   its representat
+0001f4e0: 696f 6e2e 0a0a 2020 2020 3e3e 3e20 696d  ion...    >>> im
+0001f4f0: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+0001f500: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
+0001f510: 7669 7374 6120 696d 706f 7274 2065 7861  vista import exa
+0001f520: 6d70 6c65 730a 2020 2020 3e3e 3e20 7063  mples.    >>> pc
+0001f530: 203d 2065 7861 6d70 6c65 732e 646f 776e   = examples.down
+0001f540: 6c6f 6164 5f63 6c6f 7564 5f64 6172 6b5f  load_cloud_dark_
+0001f550: 6d61 7474 6572 5f64 656e 7365 2829 0a20  matter_dense(). 
+0001f560: 2020 203e 3e3e 2070 630a 2020 2020 506f     >>> pc.    Po
+0001f570: 696e 7453 6574 2028 2e2e 2e29 0a20 2020  intSet (...).   
+0001f580: 2020 204e 2043 656c 6c73 3a20 2020 2030     N Cells:    0
+0001f590: 0a20 2020 2020 204e 2050 6f69 6e74 733a  .      N Points:
+0001f5a0: 2020 2032 3036 3232 3536 0a20 2020 2020     2062256.     
+0001f5b0: 2058 2042 6f75 6e64 733a 2020 2037 2e34   X Bounds:   7.4
+0001f5c0: 3632 652b 3031 2c20 372e 3836 3365 2b30  62e+01, 7.863e+0
+0001f5d0: 310a 2020 2020 2020 5920 426f 756e 6473  1.      Y Bounds
+0001f5e0: 3a20 2020 312e 3630 3465 2b30 312c 2032  :   1.604e+01, 2
+0001f5f0: 2e32 3434 652b 3031 0a20 2020 2020 205a  .244e+01.      Z
+0001f600: 2042 6f75 6e64 733a 2020 2038 2e38 3933   Bounds:   8.893
+0001f610: 652b 3031 2c20 392e 3333 3765 2b30 310a  e+01, 9.337e+01.
+0001f620: 2020 2020 2020 4e20 4172 7261 7973 3a20        N Arrays: 
+0001f630: 2020 300a 0a20 2020 2050 6c6f 7420 7468    0..    Plot th
+0001f640: 6520 706f 696e 7420 636c 6f75 642e 2043  e point cloud. C
+0001f650: 6f6c 6f72 2062 6173 6564 206f 6e20 7468  olor based on th
+0001f660: 6520 6469 7374 616e 6365 2066 726f 6d20  e distance from 
+0001f670: 7468 6520 6365 6e74 6572 206f 6620 7468  the center of th
+0001f680: 650a 2020 2020 636c 6f75 642e 0a0a 2020  e.    cloud...  
+0001f690: 2020 3e3e 3e20 7063 2e70 6c6f 7428 0a20    >>> pc.plot(. 
+0001f6a0: 2020 202e 2e2e 2020 2020 2073 6361 6c61     ...     scala
+0001f6b0: 7273 3d6e 702e 6c69 6e61 6c67 2e6e 6f72  rs=np.linalg.nor
+0001f6c0: 6d28 7063 2e70 6f69 6e74 7320 2d20 7063  m(pc.points - pc
+0001f6d0: 2e63 656e 7465 722c 2061 7869 733d 3129  .center, axis=1)
+0001f6e0: 2c0a 2020 2020 2e2e 2e20 2020 2020 7374  ,.    ...     st
+0001f6f0: 796c 653d 2770 6f69 6e74 735f 6761 7573  yle='points_gaus
+0001f700: 7369 616e 272c 0a20 2020 202e 2e2e 2020  sian',.    ...  
+0001f710: 2020 206f 7061 6369 7479 3d30 2e30 3330     opacity=0.030
+0001f720: 2c0a 2020 2020 2e2e 2e20 2020 2020 706f  ,.    ...     po
+0001f730: 696e 745f 7369 7a65 3d32 2e30 2c0a 2020  int_size=2.0,.  
+0001f740: 2020 2e2e 2e20 2020 2020 7368 6f77 5f73    ...     show_s
+0001f750: 6361 6c61 725f 6261 723d 4661 6c73 652c  calar_bar=False,
+0001f760: 0a20 2020 202e 2e2e 2020 2020 207a 6f6f  .    ...     zoo
+0001f770: 6d3d 322c 0a20 2020 202e 2e2e 2029 0a0a  m=2,.    ... )..
+0001f780: 2020 2020 5365 6520 7468 6520 3a72 6566      See the :ref
+0001f790: 3a60 706c 6f74 7469 6e67 5f70 6f69 6e74  :`plotting_point
+0001f7a0: 5f63 6c6f 7564 7360 2066 6f72 206d 6f72  _clouds` for mor
+0001f7b0: 6520 6465 7461 696c 7320 6f6e 2068 6f77  e details on how
+0001f7c0: 2074 6f20 706c 6f74 2070 6f69 6e74 0a20   to plot point. 
+0001f7d0: 2020 2063 6c6f 7564 732e 0a0a 2020 2020     clouds...    
+0001f7e0: 2222 220a 2020 2020 6669 6c65 6e61 6d65  """.    filename
+0001f7f0: 203d 2064 6f77 6e6c 6f61 645f 6669 6c65   = download_file
+0001f800: 2827 706f 696e 742d 636c 6f75 6473 2f66  ('point-clouds/f
+0001f810: 696e 6475 7332 332f 6861 6c6f 5f68 6967  indus23/halo_hig
+0001f820: 685f 7265 732e 6e70 7927 290a 0a20 2020  h_res.npy')..   
+0001f830: 2069 6620 6c6f 6164 3a0a 2020 2020 2020   if load:.      
+0001f840: 2020 7265 7475 726e 2070 7976 6973 7461    return pyvista
+0001f850: 2e50 6f69 6e74 5365 7428 6e70 2e6c 6f61  .PointSet(np.loa
+0001f860: 6428 6669 6c65 6e61 6d65 2929 0a20 2020  d(filename)).   
+0001f870: 2072 6574 7572 6e20 6669 6c65 6e61 6d65   return filename
+0001f880: 0a0a 0a64 6566 2064 6f77 6e6c 6f61 645f  ...def download_
+0001f890: 7374 6172 735f 636c 6f75 645f 6879 6728  stars_cloud_hyg(
+0001f8a0: 6c6f 6164 3d54 7275 6529 3a20 2023 2070  load=True):  # p
+0001f8b0: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
+0001f8c0: 2020 2020 2222 2244 6f77 6e6c 6f61 6420      """Download 
+0001f8d0: 6120 706f 696e 7420 636c 6f75 6420 6f66  a point cloud of
+0001f8e0: 2073 7461 7273 2061 7320 636f 6d70 7574   stars as comput
+0001f8f0: 6564 2062 7920 7468 6520 4859 4720 4461  ed by the HYG Da
+0001f900: 7461 6261 7365 2e0a 0a20 2020 2053 6565  tabase...    See
+0001f910: 2060 4859 472d 4461 7461 6261 7365 203c   `HYG-Database <
+0001f920: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0001f930: 6f6d 2f61 7374 726f 6e65 7875 732f 4859  om/astronexus/HY
+0001f940: 472d 4461 7461 6261 7365 3e60 5f20 666f  G-Database>`_ fo
+0001f950: 7220 6d6f 7265 0a20 2020 2064 6574 6169  r more.    detai
+0001f960: 6c73 2e0a 0a20 2020 2054 6869 7320 6461  ls...    This da
+0001f970: 7461 2073 6574 2069 7320 6c69 6365 6e73  ta set is licens
+0001f980: 6564 2062 7920 6120 4372 6561 7469 7665  ed by a Creative
+0001f990: 2043 6f6d 6d6f 6e73 2041 7474 7269 6275   Commons Attribu
+0001f9a0: 7469 6f6e 2d53 6861 7265 416c 696b 650a  tion-ShareAlike.
+0001f9b0: 2020 2020 6c69 6365 6e73 652e 2046 6f72      license. For
+0001f9c0: 206d 6f72 6520 6465 7461 696c 732c 2072   more details, r
+0001f9d0: 6561 6420 7468 6520 6043 7265 6174 6976  ead the `Creativ
+0001f9e0: 6520 436f 6d6d 6f6e 7320 7061 6765 0a20  e Commons page. 
+0001f9f0: 2020 203c 6874 7470 733a 2f2f 6372 6561     <https://crea
+0001fa00: 7469 7665 636f 6d6d 6f6e 732e 6f72 672f  tivecommons.org/
+0001fa10: 6c69 6365 6e73 6573 2f62 792d 7361 2f32  licenses/by-sa/2
+0001fa20: 2e35 2f3e 605f 0a0a 2020 2020 5365 6520  .5/>`_..    See 
+0001fa30: 7468 6520 6052 4541 444d 452e 6d64 0a20  the `README.md. 
+0001fa40: 2020 203c 6874 7470 733a 2f2f 6769 7468     <https://gith
+0001fa50: 7562 2e63 6f6d 2f70 7976 6973 7461 2f76  ub.com/pyvista/v
+0001fa60: 746b 2d64 6174 612f 626c 6f62 2f6d 6173  tk-data/blob/mas
+0001fa70: 7465 722f 4461 7461 2f70 6f69 6e74 2d63  ter/Data/point-c
+0001fa80: 6c6f 7564 732f 6879 672d 6461 7461 6261  louds/hyg-databa
+0001fa90: 7365 2f52 4541 444d 452e 6d64 3e60 5f0a  se/README.md>`_.
+0001faa0: 2020 2020 666f 7220 6d6f 7265 2064 6574      for more det
+0001fab0: 6169 6c73 2066 6f72 2068 6f77 2074 6865  ails for how the
+0001fac0: 2073 7461 7220 636f 6c6f 7273 2077 6572   star colors wer
+0001fad0: 6520 636f 6d70 7574 6564 2e0a 0a20 2020  e computed...   
+0001fae0: 2044 6973 7461 6e63 6573 2061 7265 2069   Distances are i
+0001faf0: 6e20 7061 7273 6563 7320 6672 6f6d 2045  n parsecs from E
+0001fb00: 6172 7468 2e0a 0a20 2020 2050 6172 616d  arth...    Param
+0001fb10: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+0001fb20: 2d2d 2d2d 0a20 2020 206c 6f61 6420 3a20  ----.    load : 
+0001fb30: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
+0001fb40: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
+0001fb50: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
+0001fb60: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
+0001fb70: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
+0001fb80: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
+0001fb90: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
+0001fba0: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
+0001fbb0: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
+0001fbc0: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
+0001fbd0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+0001fbe0: 0a20 2020 2070 7976 6973 7461 2e50 6f6c  .    pyvista.Pol
+0001fbf0: 7944 6174 6120 7c20 7374 720a 2020 2020  yData | str.    
+0001fc00: 2020 2020 4461 7461 5365 7420 6f72 2066      DataSet or f
+0001fc10: 696c 656e 616d 6520 6465 7065 6e64 696e  ilename dependin
+0001fc20: 6720 6f6e 2060 606c 6f61 6460 602e 0a0a  g on ``load``...
+0001fc30: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+0001fc40: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 446f   --------.    Do
+0001fc50: 776e 6c6f 6164 2061 6e64 2070 6c6f 7420  wnload and plot 
+0001fc60: 6120 706f 696e 7420 636c 6f75 6420 6f66  a point cloud of
+0001fc70: 2073 7461 7273 2077 6974 6869 6e20 332c   stars within 3,
+0001fc80: 3030 3020 6c69 6768 7420 7965 6172 732e  000 light years.
+0001fc90: 2053 7461 7273 0a20 2020 2061 7265 2063   Stars.    are c
+0001fca0: 6f6c 6f72 6564 2061 6363 6f72 6469 6e67  olored according
+0001fcb0: 2074 6f20 7468 6569 7220 5247 4241 2063   to their RGBA c
+0001fcc0: 6f6c 6f72 732e 0a0a 2020 2020 3e3e 3e20  olors...    >>> 
+0001fcd0: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
+0001fce0: 6e70 0a20 2020 203e 3e3e 2066 726f 6d20  np.    >>> from 
+0001fcf0: 7079 7669 7374 6120 696d 706f 7274 2065  pyvista import e
+0001fd00: 7861 6d70 6c65 730a 2020 2020 3e3e 3e20  xamples.    >>> 
+0001fd10: 7374 6172 7320 3d20 6578 616d 706c 6573  stars = examples
+0001fd20: 2e64 6f77 6e6c 6f61 645f 7374 6172 735f  .download_stars_
+0001fd30: 636c 6f75 645f 6879 6728 290a 2020 2020  cloud_hyg().    
+0001fd40: 3e3e 3e20 7374 6172 732e 706c 6f74 280a  >>> stars.plot(.
+0001fd50: 2020 2020 2e2e 2e20 2020 2020 7374 796c      ...     styl
+0001fd60: 653d 2770 6f69 6e74 735f 6761 7573 7369  e='points_gaussi
+0001fd70: 616e 272c 0a20 2020 202e 2e2e 2020 2020  an',.    ...    
+0001fd80: 2062 6163 6b67 726f 756e 643d 276b 272c   background='k',
+0001fd90: 0a20 2020 202e 2e2e 2020 2020 2070 6f69  .    ...     poi
+0001fda0: 6e74 5f73 697a 653d 302e 352c 0a20 2020  nt_size=0.5,.   
+0001fdb0: 202e 2e2e 2020 2020 2073 6361 6c61 7273   ...     scalars
+0001fdc0: 3d27 5f72 6762 6127 2c0a 2020 2020 2e2e  ='_rgba',.    ..
+0001fdd0: 2e20 2020 2020 7265 6e64 6572 5f70 6f69  .     render_poi
+0001fde0: 6e74 735f 6173 5f73 7068 6572 6573 3d46  nts_as_spheres=F
+0001fdf0: 616c 7365 2c0a 2020 2020 2e2e 2e20 2020  alse,.    ...   
+0001fe00: 2020 7a6f 6f6d 3d33 2e30 2c0a 2020 2020    zoom=3.0,.    
+0001fe10: 2e2e 2e20 290a 0a20 2020 203e 3e3e 2073  ... )..    >>> s
+0001fe20: 7461 7273 0a20 2020 2050 6f6c 7944 6174  tars.    PolyDat
+0001fe30: 6120 282e 2e2e 290a 2020 2020 2020 4e20  a (...).      N 
+0001fe40: 4365 6c6c 733a 2020 2020 3130 3738 3537  Cells:    107857
+0001fe50: 0a20 2020 2020 204e 2050 6f69 6e74 733a  .      N Points:
+0001fe60: 2020 2031 3037 3835 370a 2020 2020 2020     107857.      
+0001fe70: 4e20 5374 7269 7073 3a20 2020 300a 2020  N Strips:   0.  
+0001fe80: 2020 2020 5820 426f 756e 6473 3a20 2020      X Bounds:   
+0001fe90: 2d39 2e37 3535 652b 3032 2c20 392e 3737  -9.755e+02, 9.77
+0001fea0: 3465 2b30 320a 2020 2020 2020 5920 426f  4e+02.      Y Bo
+0001feb0: 756e 6473 3a20 2020 2d39 2e36 3230 652b  unds:   -9.620e+
+0001fec0: 3032 2c20 392e 3636 3265 2b30 320a 2020  02, 9.662e+02.  
+0001fed0: 2020 2020 5a20 426f 756e 6473 3a20 2020      Z Bounds:   
+0001fee0: 2d39 2e37 3838 652b 3032 2c20 392e 3730  -9.788e+02, 9.70
+0001fef0: 3265 2b30 320a 2020 2020 2020 4e20 4172  2e+02.      N Ar
+0001ff00: 7261 7973 3a20 2020 330a 0a20 2020 2053  rays:   3..    S
+0001ff10: 6565 2074 6865 203a 7265 663a 6070 6c6f  ee the :ref:`plo
+0001ff20: 7474 696e 675f 706f 696e 745f 636c 6f75  tting_point_clou
+0001ff30: 6473 6020 666f 7220 6d6f 7265 2064 6574  ds` for more det
+0001ff40: 6169 6c73 206f 6e20 686f 7720 746f 2070  ails on how to p
+0001ff50: 6c6f 7420 706f 696e 740a 2020 2020 636c  lot point.    cl
+0001ff60: 6f75 6473 2e0a 0a20 2020 2022 2222 0a20  ouds...    """. 
+0001ff70: 2020 2072 6574 7572 6e20 5f64 6f77 6e6c     return _downl
+0001ff80: 6f61 645f 616e 645f 7265 6164 2827 706f  oad_and_read('po
+0001ff90: 696e 742d 636c 6f75 6473 2f68 7967 2d64  int-clouds/hyg-d
+0001ffa0: 6174 6162 6173 652f 7374 6172 732e 7674  atabase/stars.vt
+0001ffb0: 7027 2c20 6c6f 6164 3d6c 6f61 6429 0a0a  p', load=load)..
+0001ffc0: 0a64 6566 2064 6f77 6e6c 6f61 645f 6665  .def download_fe
+0001ffd0: 615f 6272 6163 6b65 7428 6c6f 6164 3d54  a_bracket(load=T
+0001ffe0: 7275 6529 3a20 2023 2070 7261 676d 613a  rue):  # pragma:
+0001fff0: 206e 6f20 636f 7665 720a 2020 2020 2222   no cover.    ""
+00020000: 2244 6f77 6e6c 6f61 6420 7468 6520 6669  "Download the fi
+00020010: 6e69 7465 2065 6c65 6d65 6e74 2073 6f6c  nite element sol
+00020020: 7574 696f 6e20 6f66 2061 2062 7261 636b  ution of a brack
+00020030: 6574 2e0a 0a20 2020 2043 6f6e 7461 696e  et...    Contain
+00020040: 7320 766f 6e2d 6d69 7365 7320 6571 7569  s von-mises equi
+00020050: 7661 6c65 6e74 2063 656c 6c20 7374 7265  valent cell stre
+00020060: 7373 2061 7373 756d 696e 6720 6120 7665  ss assuming a ve
+00020070: 7274 6963 616c 2028 792d 6178 6973 2920  rtical (y-axis) 
+00020080: 6c6f 6164 2e0a 0a20 2020 2050 6172 616d  load...    Param
+00020090: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+000200a0: 2d2d 2d2d 0a20 2020 206c 6f61 6420 3a20  ----.    load : 
+000200b0: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
+000200c0: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
+000200d0: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
+000200e0: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
+000200f0: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
+00020100: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
+00020110: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
+00020120: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
+00020130: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
+00020140: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
+00020150: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+00020160: 0a20 2020 2070 7976 6973 7461 2e55 6e73  .    pyvista.Uns
+00020170: 7472 7563 7475 7265 6447 7269 6420 7c20  tructuredGrid | 
+00020180: 7374 720a 2020 2020 2020 2020 4461 7461  str.        Data
+00020190: 5365 7420 6f72 2066 696c 656e 616d 6520  Set or filename 
+000201a0: 6465 7065 6e64 696e 6720 6f6e 2060 606c  depending on ``l
+000201b0: 6f61 6460 602e 0a0a 2020 2020 4578 616d  oad``...    Exam
+000201c0: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+000201d0: 2d0a 2020 2020 446f 776e 6c6f 6164 2061  -.    Download a
+000201e0: 6e64 2070 6c6f 7420 6571 7569 7661 6c65  nd plot equivale
+000201f0: 6e74 2063 656c 6c20 7374 7265 7373 2e0a  nt cell stress..
+00020200: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
+00020210: 7669 7374 6120 696d 706f 7274 2065 7861  vista import exa
+00020220: 6d70 6c65 730a 2020 2020 3e3e 3e20 6772  mples.    >>> gr
+00020230: 6964 203d 2065 7861 6d70 6c65 732e 646f  id = examples.do
+00020240: 776e 6c6f 6164 5f66 6561 5f62 7261 636b  wnload_fea_brack
+00020250: 6574 2829 0a20 2020 203e 3e3e 2067 7269  et().    >>> gri
+00020260: 642e 706c 6f74 2829 0a0a 2020 2020 506c  d.plot()..    Pl
+00020270: 6f74 2074 6865 2070 6f69 6e74 2073 7472  ot the point str
+00020280: 6573 7320 7573 696e 6720 7468 6520 6060  ess using the ``
+00020290: 276a 6574 2760 6020 636f 6c6f 7220 6d61  'jet'`` color ma
+000202a0: 702e 2043 6f6e 7665 7274 2074 6865 2063  p. Convert the c
+000202b0: 656c 6c20 6461 7461 0a20 2020 2074 6f20  ell data.    to 
+000202c0: 706f 696e 7420 6461 7461 2e0a 0a20 2020  point data...   
+000202d0: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
+000202e0: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
+000202f0: 730a 2020 2020 3e3e 3e20 6772 6964 203d  s.    >>> grid =
+00020300: 2065 7861 6d70 6c65 732e 646f 776e 6c6f   examples.downlo
+00020310: 6164 5f66 6561 5f62 7261 636b 6574 2829  ad_fea_bracket()
+00020320: 0a20 2020 203e 3e3e 2067 7269 6420 3d20  .    >>> grid = 
+00020330: 6772 6964 2e63 656c 6c5f 6461 7461 5f74  grid.cell_data_t
+00020340: 6f5f 706f 696e 745f 6461 7461 2829 0a20  o_point_data(). 
+00020350: 2020 203e 3e3e 2067 7269 642e 706c 6f74     >>> grid.plot
+00020360: 2873 6d6f 6f74 685f 7368 6164 696e 673d  (smooth_shading=
+00020370: 5472 7565 2c20 7370 6c69 745f 7368 6172  True, split_shar
+00020380: 705f 6564 6765 733d 5472 7565 2c20 636d  p_edges=True, cm
+00020390: 6170 3d27 6a65 7427 290a 0a20 2020 2022  ap='jet')..    "
+000203a0: 2222 0a20 2020 2072 6574 7572 6e20 5f64  "".    return _d
+000203b0: 6f77 6e6c 6f61 645f 616e 645f 7265 6164  ownload_and_read
+000203c0: 2827 6665 612f 6b69 6566 6572 2f64 6174  ('fea/kiefer/dat
+000203d0: 6173 6574 2e76 7475 272c 206c 6f61 643d  aset.vtu', load=
+000203e0: 6c6f 6164 290a 0a0a 6465 6620 646f 776e  load)...def down
+000203f0: 6c6f 6164 5f66 6561 5f68 6572 747a 6961  load_fea_hertzia
+00020400: 6e5f 636f 6e74 6163 745f 6379 6c69 6e64  n_contact_cylind
+00020410: 6572 286c 6f61 643d 5472 7565 293a 2020  er(load=True):  
+00020420: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+00020430: 6572 0a20 2020 2022 2222 446f 776e 6c6f  er.    """Downlo
+00020440: 6164 2061 2068 6572 747a 6961 6e20 636f  ad a hertzian co
+00020450: 6e74 6163 7420 6669 6e69 7465 2065 6c65  ntact finite ele
+00020460: 6d65 6e74 2073 6f6c 7574 696f 6e2e 0a0a  ment solution...
+00020470: 2020 2020 4865 7274 7a69 616e 2063 6f6e      Hertzian con
+00020480: 7461 6374 2069 7320 7265 6665 7272 6564  tact is referred
+00020490: 2074 6f20 7468 6520 6672 6963 7469 6f6e   to the friction
+000204a0: 6c65 7373 2063 6f6e 7461 6374 2062 6574  less contact bet
+000204b0: 7765 656e 2074 776f 0a20 2020 2062 6f64  ween two.    bod
+000204c0: 6965 732e 2053 7068 6572 6963 616c 2063  ies. Spherical c
+000204d0: 6f6e 7461 6374 2069 7320 6120 7370 6563  ontact is a spec
+000204e0: 6961 6c20 6361 7365 206f 6620 7468 6520  ial case of the 
+000204f0: 4865 7274 7a20 636f 6e74 6163 742c 2077  Hertz contact, w
+00020500: 6869 6368 2069 730a 2020 2020 6265 7477  hich is.    betw
+00020510: 6565 6e20 7477 6f20 7370 6865 7265 732c  een two spheres,
+00020520: 206f 7220 6173 2069 6e20 7468 6520 6361   or as in the ca
+00020530: 7365 206f 6620 7468 6973 2064 6174 6173  se of this datas
+00020540: 6574 2c20 6265 7477 6565 6e20 6120 7370  et, between a sp
+00020550: 6865 7265 0a20 2020 2061 6e64 2074 6865  here.    and the
+00020560: 2073 7572 6661 6365 206f 6620 6120 6861   surface of a ha
+00020570: 6c66 2073 7061 6365 2028 666c 6174 2070  lf space (flat p
+00020580: 6c61 6e65 292e 0a0a 2020 2020 5061 7261  lane)...    Para
+00020590: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+000205a0: 2d2d 2d2d 2d0a 2020 2020 6c6f 6164 203a  -----.    load :
+000205b0: 2062 6f6f 6c2c 2064 6566 6175 6c74 3a20   bool, default: 
+000205c0: 5472 7565 0a20 2020 2020 2020 204c 6f61  True.        Loa
+000205d0: 6420 7468 6520 6461 7461 7365 7420 6166  d the dataset af
+000205e0: 7465 7220 646f 776e 6c6f 6164 696e 6720  ter downloading 
+000205f0: 6974 2077 6865 6e20 6060 5472 7565 6060  it when ``True``
+00020600: 2e20 2053 6574 2074 6869 730a 2020 2020  .  Set this.    
+00020610: 2020 2020 746f 2060 6046 616c 7365 6060      to ``False``
+00020620: 2061 6e64 206f 6e6c 7920 7468 6520 6669   and only the fi
+00020630: 6c65 6e61 6d65 2077 696c 6c20 6265 2072  lename will be r
+00020640: 6574 7572 6e65 642e 0a0a 2020 2020 5265  eturned...    Re
+00020650: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+00020660: 2d0a 2020 2020 7079 7669 7374 612e 556e  -.    pyvista.Un
+00020670: 7374 7275 6374 7572 6564 4772 6964 207c  structuredGrid |
+00020680: 2073 7472 0a20 2020 2020 2020 2044 6174   str.        Dat
+00020690: 6153 6574 206f 7220 6669 6c65 6e61 6d65  aSet or filename
+000206a0: 2064 6570 656e 6469 6e67 206f 6e20 6060   depending on ``
+000206b0: 6c6f 6164 6060 2e0a 0a20 2020 2045 7861  load``...    Exa
+000206c0: 6d70 6c65 730a 2020 2020 2d2d 2d2d 2d2d  mples.    ------
+000206d0: 2d2d 0a20 2020 2050 6c6f 7420 6279 2070  --.    Plot by p
+000206e0: 6172 7420 4944 2e0a 0a20 2020 203e 3e3e  art ID...    >>>
+000206f0: 2069 6d70 6f72 7420 6e75 6d70 7920 6173   import numpy as
+00020700: 206e 700a 2020 2020 3e3e 3e20 696d 706f   np.    >>> impo
+00020710: 7274 2070 7976 6973 7461 2061 7320 7076  rt pyvista as pv
+00020720: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
+00020730: 7669 7374 6120 696d 706f 7274 2065 7861  vista import exa
+00020740: 6d70 6c65 730a 2020 2020 3e3e 3e20 6772  mples.    >>> gr
+00020750: 6964 203d 2065 7861 6d70 6c65 732e 646f  id = examples.do
+00020760: 776e 6c6f 6164 5f66 6561 5f68 6572 747a  wnload_fea_hertz
+00020770: 6961 6e5f 636f 6e74 6163 745f 6379 6c69  ian_contact_cyli
+00020780: 6e64 6572 2829 0a20 2020 203e 3e3e 2067  nder().    >>> g
+00020790: 7269 642e 706c 6f74 280a 2020 2020 2e2e  rid.plot(.    ..
+000207a0: 2e20 2020 2020 7363 616c 6172 733d 2750  .     scalars='P
+000207b0: 6172 7449 4427 2c20 636d 6170 3d5b 2767  artID', cmap=['g
+000207c0: 7265 656e 272c 2027 626c 7565 275d 2c20  reen', 'blue'], 
+000207d0: 7368 6f77 5f73 6361 6c61 725f 6261 723d  show_scalar_bar=
+000207e0: 4661 6c73 650a 2020 2020 2e2e 2e20 290a  False.    ... ).
+000207f0: 0a20 2020 2050 6c6f 7420 7468 6520 6162  .    Plot the ab
+00020800: 736f 6c75 7465 2076 616c 7565 206f 6620  solute value of 
+00020810: 7468 6520 636f 6d70 6f6e 656e 7420 7374  the component st
+00020820: 7265 7373 2069 6e20 7468 6520 5a20 6469  ress in the Z di
+00020830: 7265 6374 696f 6e2e 0a0a 2020 2020 3e3e  rection...    >>
+00020840: 3e20 706c 203d 2070 762e 506c 6f74 7465  > pl = pv.Plotte
+00020850: 7228 290a 2020 2020 3e3e 3e20 7a5f 7374  r().    >>> z_st
+00020860: 7265 7373 203d 206e 702e 6162 7328 6772  ress = np.abs(gr
+00020870: 6964 5b27 5374 7265 7373 275d 5b3a 2c20  id['Stress'][:, 
+00020880: 325d 290a 2020 2020 3e3e 3e20 5f20 3d20  2]).    >>> _ = 
+00020890: 706c 2e61 6464 5f6d 6573 6828 0a20 2020  pl.add_mesh(.   
+000208a0: 202e 2e2e 2020 2020 2067 7269 642c 0a20   ...     grid,. 
+000208b0: 2020 202e 2e2e 2020 2020 2073 6361 6c61     ...     scala
+000208c0: 7273 3d7a 5f73 7472 6573 732c 0a20 2020  rs=z_stress,.   
+000208d0: 202e 2e2e 2020 2020 2063 6c69 6d3d 5b30   ...     clim=[0
+000208e0: 2c20 312e 3265 395d 2c0a 2020 2020 2e2e  , 1.2e9],.    ..
+000208f0: 2e20 2020 2020 636d 6170 3d27 6a65 7427  .     cmap='jet'
+00020900: 2c0a 2020 2020 2e2e 2e20 2020 2020 6c69  ,.    ...     li
+00020910: 6768 7469 6e67 3d54 7275 652c 0a20 2020  ghting=True,.   
+00020920: 202e 2e2e 2020 2020 2073 686f 775f 6564   ...     show_ed
+00020930: 6765 733d 4661 6c73 652c 0a20 2020 202e  ges=False,.    .
+00020940: 2e2e 2020 2020 2061 6d62 6965 6e74 3d30  ..     ambient=0
+00020950: 2e32 2c0a 2020 2020 2e2e 2e20 290a 2020  .2,.    ... ).  
+00020960: 2020 3e3e 3e20 706c 2e63 616d 6572 615f    >>> pl.camera_
+00020970: 706f 7369 7469 6f6e 203d 2027 787a 270a  position = 'xz'.
+00020980: 2020 2020 3e3e 3e20 706c 2e63 616d 6572      >>> pl.camer
+00020990: 612e 7a6f 6f6d 2831 2e34 290a 2020 2020  a.zoom(1.4).    
+000209a0: 3e3e 3e20 706c 2e73 686f 7728 290a 0a20  >>> pl.show().. 
+000209b0: 2020 2022 2222 0a20 2020 2066 696c 656e     """.    filen
+000209c0: 616d 6520 3d20 5f64 6f77 6e6c 6f61 645f  ame = _download_
+000209d0: 6172 6368 6976 6528 0a20 2020 2020 2020  archive(.       
+000209e0: 2027 6665 612f 6865 7274 7a69 616e 5f63   'fea/hertzian_c
+000209f0: 6f6e 7461 6374 5f63 796c 696e 6465 722f  ontact_cylinder/
+00020a00: 4865 7274 7a69 616e 5f63 796c 696e 6465  Hertzian_cylinde
+00020a10: 725f 6f6e 5f70 6c61 7465 2e7a 6970 272c  r_on_plate.zip',
+00020a20: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
+00020a30: 6669 6c65 3d27 6266 6163 3966 6431 2d65  file='bfac9fd1-e
+00020a40: 3938 322d 3438 3235 2d39 6139 352d 3965  982-4825-9a95-9e
+00020a50: 3564 3863 3562 3464 3365 5f72 6573 756c  5d8c5b4d3e_resul
+00020a60: 745f 312e 7076 7475 272c 0a20 2020 2029  t_1.pvtu',.    )
+00020a70: 0a20 2020 2069 6620 6c6f 6164 3a0a 2020  .    if load:.  
+00020a80: 2020 2020 2020 7265 7475 726e 2070 7976        return pyv
+00020a90: 6973 7461 2e72 6561 6428 6669 6c65 6e61  ista.read(filena
+00020aa0: 6d65 290a 2020 2020 7265 7475 726e 2066  me).    return f
+00020ab0: 696c 656e 616d 650a 0a0a 6465 6620 646f  ilename...def do
+00020ac0: 776e 6c6f 6164 5f62 6c61 636b 5f76 6173  wnload_black_vas
+00020ad0: 6528 6c6f 6164 3d54 7275 6529 3a20 2023  e(load=True):  #
+00020ae0: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+00020af0: 720a 2020 2020 2222 2244 6f77 6e6c 6f61  r.    """Downloa
+00020b00: 6420 6120 626c 6163 6b20 7661 7365 2073  d a black vase s
+00020b10: 6361 6e20 6372 6561 7465 6420 6279 2049  can created by I
+00020b20: 7661 6e20 4e69 6b6f 6c6f 762e 0a0a 2020  van Nikolov...  
+00020b30: 2020 5468 6520 6461 7461 7365 7420 7761    The dataset wa
+00020b40: 7320 646f 776e 6c6f 6164 6564 2066 726f  s downloaded fro
+00020b50: 6d20 6047 4747 2d42 656e 6368 6d61 726b  m `GGG-Benchmark
+00020b60: 5366 4d3a 2044 6174 6173 6574 2066 6f72  SfM: Dataset for
+00020b70: 2042 656e 6368 6d61 726b 696e 670a 2020   Benchmarking.  
+00020b80: 2020 436c 6f73 652d 7261 6e67 6520 5366    Close-range Sf
+00020b90: 4d20 536f 6674 7761 7265 2050 6572 666f  M Software Perfo
+00020ba0: 726d 616e 6365 2075 6e64 6572 2056 6172  rmance under Var
+00020bb0: 7969 6e67 2043 6170 7475 7269 6e67 2043  ying Capturing C
+00020bc0: 6f6e 6469 7469 6f6e 730a 2020 2020 3c68  onditions.    <h
+00020bd0: 7474 7073 3a2f 2f64 6174 612e 6d65 6e64  ttps://data.mend
+00020be0: 656c 6579 2e63 6f6d 2f64 6174 6173 6574  eley.com/dataset
+00020bf0: 732f 627a 786b 326e 3738 7339 2f34 3e60  s/bzxk2n78s9/4>`
+00020c00: 5f0a 0a20 2020 204f 7269 6769 6e61 6c20  _..    Original 
+00020c10: 6461 7461 7365 7473 2061 7265 2075 6e64  datasets are und
+00020c20: 6572 2074 6865 2043 4320 4259 2034 2e30  er the CC BY 4.0
+00020c30: 206c 6963 656e 7365 2e0a 0a20 2020 2046   license...    F
+00020c40: 6f72 206d 6f72 6520 6465 7461 696c 732c  or more details,
+00020c50: 2073 6565 2060 4976 616e 204e 696b 6f6c   see `Ivan Nikol
+00020c60: 6f76 2044 6174 6173 6574 730a 2020 2020  ov Datasets.    
+00020c70: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+00020c80: 636f 6d2f 7079 7669 7374 612f 7674 6b2d  com/pyvista/vtk-
+00020c90: 6461 7461 2f74 7265 652f 6d61 7374 6572  data/tree/master
+00020ca0: 2f44 6174 612f 6976 616e 2d6e 696b 6f6c  /Data/ivan-nikol
+00020cb0: 6f76 3e60 5f0a 0a20 2020 2050 6172 616d  ov>`_..    Param
+00020cc0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00020cd0: 2d2d 2d2d 0a20 2020 206c 6f61 6420 3a20  ----.    load : 
+00020ce0: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
+00020cf0: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
+00020d00: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
+00020d10: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
+00020d20: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
+00020d30: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
+00020d40: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
+00020d50: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
+00020d60: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
+00020d70: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
+00020d80: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+00020d90: 0a20 2020 2070 7976 6973 7461 2e50 6f6c  .    pyvista.Pol
+00020da0: 7944 6174 6120 7c20 7374 720a 2020 2020  yData | str.    
+00020db0: 2020 2020 4461 7461 5365 7420 6f72 2066      DataSet or f
+00020dc0: 696c 656e 616d 6520 6465 7065 6e64 696e  ilename dependin
+00020dd0: 6720 6f6e 2060 606c 6f61 6460 602e 0a0a  g on ``load``...
+00020de0: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+00020df0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 446f   --------.    Do
+00020e00: 776e 6c6f 6164 2061 6e64 2070 6c6f 7420  wnload and plot 
+00020e10: 7468 6520 6461 7461 7365 742e 0a0a 2020  the dataset...  
+00020e20: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
+00020e30: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
+00020e40: 6573 0a20 2020 203e 3e3e 206d 6573 6820  es.    >>> mesh 
+00020e50: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
+00020e60: 6f61 645f 626c 6163 6b5f 7661 7365 2829  oad_black_vase()
+00020e70: 0a20 2020 203e 3e3e 206d 6573 682e 706c  .    >>> mesh.pl
+00020e80: 6f74 2829 0a0a 2020 2020 5265 7475 726e  ot()..    Return
+00020e90: 2074 6865 2073 7461 7469 7374 6963 7320   the statistics 
+00020ea0: 6f66 2074 6865 2064 6174 6173 6574 2e0a  of the dataset..
+00020eb0: 0a20 2020 203e 3e3e 206d 6573 680a 2020  .    >>> mesh.  
+00020ec0: 2020 506f 6c79 4461 7461 2028 2e2e 2e29    PolyData (...)
+00020ed0: 0a20 2020 2020 204e 2043 656c 6c73 3a20  .      N Cells: 
+00020ee0: 2020 2033 3133 3636 3532 0a20 2020 2020     3136652.     
+00020ef0: 204e 2050 6f69 6e74 733a 2020 2031 3631   N Points:   161
+00020f00: 3137 3839 0a20 2020 2020 204e 2053 7472  1789.      N Str
+00020f10: 6970 733a 2020 2030 0a20 2020 2020 2058  ips:   0.      X
+00020f20: 2042 6f75 6e64 733a 2020 202d 312e 3039   Bounds:   -1.09
+00020f30: 3265 2b30 322c 2031 2e35 3333 652b 3032  2e+02, 1.533e+02
+00020f40: 0a20 2020 2020 2059 2042 6f75 6e64 733a  .      Y Bounds:
+00020f50: 2020 202d 312e 3230 3065 2b30 322c 2031     -1.200e+02, 1
+00020f60: 2e34 3135 652b 3032 0a20 2020 2020 205a  .415e+02.      Z
+00020f70: 2042 6f75 6e64 733a 2020 2031 2e36 3636   Bounds:   1.666
+00020f80: 652b 3031 2c20 342e 3037 3765 2b30 320a  e+01, 4.077e+02.
+00020f90: 2020 2020 2020 4e20 4172 7261 7973 3a20        N Arrays: 
+00020fa0: 2020 300a 0a0a 2020 2020 2222 220a 2020    0...    """.  
+00020fb0: 2020 6669 6c65 6e61 6d65 203d 205f 646f    filename = _do
+00020fc0: 776e 6c6f 6164 5f61 7263 6869 7665 280a  wnload_archive(.
+00020fd0: 2020 2020 2020 2020 2769 7661 6e2d 6e69          'ivan-ni
+00020fe0: 6b6f 6c6f 762f 626c 6163 6b56 6173 652e  kolov/blackVase.
+00020ff0: 7a69 7027 2c0a 2020 2020 2020 2020 2762  zip',.        'b
+00021000: 6c61 636b 5661 7365 2e76 7470 272c 0a20  lackVase.vtp',. 
+00021010: 2020 2029 0a20 2020 2069 6620 6c6f 6164     ).    if load
+00021020: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00021030: 2070 7976 6973 7461 2e72 6561 6428 6669   pyvista.read(fi
+00021040: 6c65 6e61 6d65 290a 2020 2020 7265 7475  lename).    retu
+00021050: 726e 2066 696c 656e 616d 650a 0a0a 6465  rn filename...de
+00021060: 6620 646f 776e 6c6f 6164 5f69 7661 6e5f  f download_ivan_
+00021070: 616e 6765 6c28 6c6f 6164 3d54 7275 6529  angel(load=True)
+00021080: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+00021090: 636f 7665 720a 2020 2020 2222 2244 6f77  cover.    """Dow
+000210a0: 6e6c 6f61 6420 6120 7363 616e 206f 6620  nload a scan of 
+000210b0: 616e 2061 6e67 656c 2073 7461 7475 6520  an angel statue 
+000210c0: 6372 6561 7465 6420 6279 2049 7661 6e20  created by Ivan 
+000210d0: 4e69 6b6f 6c6f 762e 0a0a 2020 2020 5468  Nikolov...    Th
+000210e0: 6520 6461 7461 7365 7420 7761 7320 646f  e dataset was do
+000210f0: 776e 6c6f 6164 6564 2066 726f 6d20 6047  wnloaded from `G
+00021100: 4747 2d42 656e 6368 6d61 726b 5366 4d3a  GG-BenchmarkSfM:
+00021110: 2044 6174 6173 6574 2066 6f72 2042 656e   Dataset for Ben
+00021120: 6368 6d61 726b 696e 670a 2020 2020 436c  chmarking.    Cl
+00021130: 6f73 652d 7261 6e67 6520 5366 4d20 536f  ose-range SfM So
+00021140: 6674 7761 7265 2050 6572 666f 726d 616e  ftware Performan
+00021150: 6365 2075 6e64 6572 2056 6172 7969 6e67  ce under Varying
+00021160: 2043 6170 7475 7269 6e67 2043 6f6e 6469   Capturing Condi
+00021170: 7469 6f6e 730a 2020 2020 3c68 7474 7073  tions.    <https
+00021180: 3a2f 2f64 6174 612e 6d65 6e64 656c 6579  ://data.mendeley
+00021190: 2e63 6f6d 2f64 6174 6173 6574 732f 627a  .com/datasets/bz
+000211a0: 786b 326e 3738 7339 2f34 3e60 5f0a 0a20  xk2n78s9/4>`_.. 
+000211b0: 2020 204f 7269 6769 6e61 6c20 6461 7461     Original data
+000211c0: 7365 7473 2061 7265 2075 6e64 6572 2074  sets are under t
+000211d0: 6865 2043 4320 4259 2034 2e30 206c 6963  he CC BY 4.0 lic
+000211e0: 656e 7365 2e0a 0a20 2020 2046 6f72 206d  ense...    For m
+000211f0: 6f72 6520 6465 7461 696c 732c 2073 6565  ore details, see
+00021200: 2060 4976 616e 204e 696b 6f6c 6f76 2044   `Ivan Nikolov D
+00021210: 6174 6173 6574 730a 2020 2020 3c68 7474  atasets.    <htt
+00021220: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00021230: 7079 7669 7374 612f 7674 6b2d 6461 7461  pyvista/vtk-data
+00021240: 2f74 7265 652f 6d61 7374 6572 2f44 6174  /tree/master/Dat
+00021250: 612f 6976 616e 2d6e 696b 6f6c 6f76 3e60  a/ivan-nikolov>`
+00021260: 5f0a 0a20 2020 2050 6172 616d 6574 6572  _..    Parameter
+00021270: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00021280: 0a20 2020 206c 6f61 6420 3a20 626f 6f6c  .    load : bool
+00021290: 2c20 6465 6661 756c 743a 2054 7275 650a  , default: True.
+000212a0: 2020 2020 2020 2020 4c6f 6164 2074 6865          Load the
+000212b0: 2064 6174 6173 6574 2061 6674 6572 2064   dataset after d
+000212c0: 6f77 6e6c 6f61 6469 6e67 2069 7420 7768  ownloading it wh
+000212d0: 656e 2060 6054 7275 6560 602e 2020 5365  en ``True``.  Se
+000212e0: 7420 7468 6973 0a20 2020 2020 2020 2074  t this.        t
+000212f0: 6f20 6060 4661 6c73 6560 6020 616e 6420  o ``False`` and 
+00021300: 6f6e 6c79 2074 6865 2066 696c 656e 616d  only the filenam
+00021310: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
+00021320: 6564 2e0a 0a20 2020 2052 6574 7572 6e73  ed...    Returns
+00021330: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00021340: 2070 7976 6973 7461 2e50 6f6c 7944 6174   pyvista.PolyDat
+00021350: 6120 7c20 7374 720a 2020 2020 2020 2020  a | str.        
+00021360: 4461 7461 5365 7420 6f72 2066 696c 656e  DataSet or filen
+00021370: 616d 6520 6465 7065 6e64 696e 6720 6f6e  ame depending on
+00021380: 2060 606c 6f61 6460 602e 0a0a 2020 2020   ``load``...    
+00021390: 4578 616d 706c 6573 0a20 2020 202d 2d2d  Examples.    ---
+000213a0: 2d2d 2d2d 2d0a 2020 2020 446f 776e 6c6f  -----.    Downlo
+000213b0: 6164 2061 6e64 2070 6c6f 7420 7468 6520  ad and plot the 
+000213c0: 6461 7461 7365 742e 0a0a 2020 2020 3e3e  dataset...    >>
+000213d0: 3e20 6672 6f6d 2070 7976 6973 7461 2069  > from pyvista i
+000213e0: 6d70 6f72 7420 6578 616d 706c 6573 0a20  mport examples. 
+000213f0: 2020 203e 3e3e 206d 6573 6820 3d20 6578     >>> mesh = ex
+00021400: 616d 706c 6573 2e64 6f77 6e6c 6f61 645f  amples.download_
+00021410: 6976 616e 5f61 6e67 656c 2829 0a20 2020  ivan_angel().   
+00021420: 203e 3e3e 2063 706f 7320 3d20 5b0a 2020   >>> cpos = [.  
+00021430: 2020 2e2e 2e20 2020 2020 282d 3437 362e    ...     (-476.
+00021440: 3134 2c20 2d33 3933 2e37 332c 2032 3832  14, -393.73, 282
+00021450: 2e31 3429 2c0a 2020 2020 2e2e 2e20 2020  .14),.    ...   
+00021460: 2020 282d 3135 2e30 302c 2031 312e 3235    (-15.00, 11.25
+00021470: 2c20 3434 2e30 3829 2c0a 2020 2020 2e2e  , 44.08),.    ..
+00021480: 2e20 2020 2020 2830 2e32 362c 2030 2e32  .     (0.26, 0.2
+00021490: 342c 2030 2e39 3329 2c0a 2020 2020 2e2e  4, 0.93),.    ..
+000214a0: 2e20 5d0a 2020 2020 3e3e 3e20 6d65 7368  . ].    >>> mesh
+000214b0: 2e70 6c6f 7428 6370 6f73 3d63 706f 7329  .plot(cpos=cpos)
+000214c0: 0a0a 2020 2020 5265 7475 726e 2074 6865  ..    Return the
+000214d0: 2073 7461 7469 7374 6963 7320 6f66 2074   statistics of t
+000214e0: 6865 2064 6174 6173 6574 2e0a 0a20 2020  he dataset...   
+000214f0: 203e 3e3e 206d 6573 680a 2020 2020 506f   >>> mesh.    Po
+00021500: 6c79 4461 7461 2028 2e2e 2e29 0a20 2020  lyData (...).   
+00021510: 2020 204e 2043 656c 6c73 3a20 2020 2033     N Cells:    3
+00021520: 3538 3034 3534 0a20 2020 2020 204e 2050  580454.      N P
+00021530: 6f69 6e74 733a 2020 2031 3831 3135 3331  oints:   1811531
+00021540: 0a20 2020 2020 204e 2053 7472 6970 733a  .      N Strips:
+00021550: 2020 2030 0a20 2020 2020 2058 2042 6f75     0.      X Bou
+00021560: 6e64 733a 2020 202d 312e 3134 3765 2b30  nds:   -1.147e+0
+00021570: 322c 2038 2e34 3638 652b 3031 0a20 2020  2, 8.468e+01.   
+00021580: 2020 2059 2042 6f75 6e64 733a 2020 202d     Y Bounds:   -
+00021590: 362e 3939 3665 2b30 312c 2039 2e32 3437  6.996e+01, 9.247
+000215a0: 652b 3031 0a20 2020 2020 205a 2042 6f75  e+01.      Z Bou
+000215b0: 6e64 733a 2020 202d 312e 3137 3165 2b30  nds:   -1.171e+0
+000215c0: 322c 2032 2e30 3532 652b 3032 0a20 2020  2, 2.052e+02.   
+000215d0: 2020 204e 2041 7272 6179 733a 2020 2030     N Arrays:   0
+000215e0: 0a0a 2020 2020 2222 220a 2020 2020 6669  ..    """.    fi
+000215f0: 6c65 6e61 6d65 203d 205f 646f 776e 6c6f  lename = _downlo
+00021600: 6164 5f61 7263 6869 7665 280a 2020 2020  ad_archive(.    
+00021610: 2020 2020 2769 7661 6e2d 6e69 6b6f 6c6f      'ivan-nikolo
+00021620: 762f 416e 6765 6c2e 7a69 7027 2c0a 2020  v/Angel.zip',.  
+00021630: 2020 2020 2020 2741 6e67 656c 2e76 7470        'Angel.vtp
+00021640: 272c 0a20 2020 2029 0a20 2020 2069 6620  ',.    ).    if 
+00021650: 6c6f 6164 3a0a 2020 2020 2020 2020 7265  load:.        re
+00021660: 7475 726e 2070 7976 6973 7461 2e72 6561  turn pyvista.rea
+00021670: 6428 6669 6c65 6e61 6d65 290a 2020 2020  d(filename).    
+00021680: 7265 7475 726e 2066 696c 656e 616d 650a  return filename.
+00021690: 0a0a 6465 6620 646f 776e 6c6f 6164 5f62  ..def download_b
+000216a0: 6972 645f 6261 7468 286c 6f61 643d 5472  ird_bath(load=Tr
+000216b0: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
+000216c0: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
+000216d0: 446f 776e 6c6f 6164 2061 2073 6361 6e20  Download a scan 
+000216e0: 6f66 2061 2062 6972 6420 6261 7468 2063  of a bird bath c
+000216f0: 7265 6174 6564 2062 7920 4976 616e 204e  reated by Ivan N
+00021700: 696b 6f6c 6f76 2e0a 0a20 2020 2054 6865  ikolov...    The
+00021710: 2064 6174 6173 6574 2077 6173 2064 6f77   dataset was dow
+00021720: 6e6c 6f61 6465 6420 6672 6f6d 2060 4747  nloaded from `GG
+00021730: 472d 4265 6e63 686d 6172 6b53 664d 3a20  G-BenchmarkSfM: 
+00021740: 4461 7461 7365 7420 666f 7220 4265 6e63  Dataset for Benc
+00021750: 686d 6172 6b69 6e67 0a20 2020 2043 6c6f  hmarking.    Clo
+00021760: 7365 2d72 616e 6765 2053 664d 2053 6f66  se-range SfM Sof
+00021770: 7477 6172 6520 5065 7266 6f72 6d61 6e63  tware Performanc
+00021780: 6520 756e 6465 7220 5661 7279 696e 6720  e under Varying 
+00021790: 4361 7074 7572 696e 6720 436f 6e64 6974  Capturing Condit
+000217a0: 696f 6e73 0a20 2020 203c 6874 7470 733a  ions.    <https:
+000217b0: 2f2f 6461 7461 2e6d 656e 6465 6c65 792e  //data.mendeley.
+000217c0: 636f 6d2f 6461 7461 7365 7473 2f62 7a78  com/datasets/bzx
+000217d0: 6b32 6e37 3873 392f 343e 605f 0a0a 2020  k2n78s9/4>`_..  
+000217e0: 2020 4f72 6967 696e 616c 2064 6174 6173    Original datas
+000217f0: 6574 7320 6172 6520 756e 6465 7220 7468  ets are under th
+00021800: 6520 4343 2042 5920 342e 3020 6c69 6365  e CC BY 4.0 lice
+00021810: 6e73 652e 0a0a 2020 2020 466f 7220 6d6f  nse...    For mo
+00021820: 7265 2064 6574 6169 6c73 2c20 7365 6520  re details, see 
+00021830: 6049 7661 6e20 4e69 6b6f 6c6f 7620 4461  `Ivan Nikolov Da
+00021840: 7461 7365 7473 0a20 2020 203c 6874 7470  tasets.    <http
+00021850: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00021860: 7976 6973 7461 2f76 746b 2d64 6174 612f  yvista/vtk-data/
+00021870: 7472 6565 2f6d 6173 7465 722f 4461 7461  tree/master/Data
+00021880: 2f69 7661 6e2d 6e69 6b6f 6c6f 763e 605f  /ivan-nikolov>`_
+00021890: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+000218a0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+000218b0: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
+000218c0: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
+000218d0: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
+000218e0: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
+000218f0: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
+00021900: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
+00021910: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
+00021920: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
+00021930: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
+00021940: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+00021950: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
+00021960: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00021970: 7079 7669 7374 612e 506f 6c79 4461 7461  pyvista.PolyData
+00021980: 207c 2073 7472 0a20 2020 2020 2020 2044   | str.        D
+00021990: 6174 6153 6574 206f 7220 6669 6c65 6e61  ataSet or filena
+000219a0: 6d65 2064 6570 656e 6469 6e67 206f 6e20  me depending on 
+000219b0: 6060 6c6f 6164 6060 2e0a 0a20 2020 2045  ``load``...    E
+000219c0: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+000219d0: 2d2d 2d2d 0a20 2020 2044 6f77 6e6c 6f61  ----.    Downloa
+000219e0: 6420 616e 6420 706c 6f74 2074 6865 2064  d and plot the d
+000219f0: 6174 6173 6574 2e0a 0a20 2020 203e 3e3e  ataset...    >>>
+00021a00: 2066 726f 6d20 7079 7669 7374 6120 696d   from pyvista im
+00021a10: 706f 7274 2065 7861 6d70 6c65 730a 2020  port examples.  
+00021a20: 2020 3e3e 3e20 6d65 7368 203d 2065 7861    >>> mesh = exa
+00021a30: 6d70 6c65 732e 646f 776e 6c6f 6164 5f62  mples.download_b
+00021a40: 6972 645f 6261 7468 2829 0a20 2020 203e  ird_bath().    >
+00021a50: 3e3e 206d 6573 682e 706c 6f74 2829 0a0a  >> mesh.plot()..
+00021a60: 2020 2020 5265 7475 726e 2074 6865 2073      Return the s
+00021a70: 7461 7469 7374 6963 7320 6f66 2074 6865  tatistics of the
+00021a80: 2064 6174 6173 6574 2e0a 0a20 2020 203e   dataset...    >
+00021a90: 3e3e 206d 6573 680a 2020 2020 506f 6c79  >> mesh.    Poly
+00021aa0: 4461 7461 2028 2e2e 2e29 0a20 2020 2020  Data (...).     
+00021ab0: 204e 2043 656c 6c73 3a20 2020 2033 3530   N Cells:    350
+00021ac0: 3739 3335 0a20 2020 2020 204e 2050 6f69  7935.      N Poi
+00021ad0: 6e74 733a 2020 2031 3833 3133 3833 0a20  nts:   1831383. 
+00021ae0: 2020 2020 204e 2053 7472 6970 733a 2020       N Strips:  
+00021af0: 2030 0a20 2020 2020 2058 2042 6f75 6e64   0.      X Bound
+00021b00: 733a 2020 202d 312e 3630 3165 2b30 322c  s:   -1.601e+02,
+00021b10: 2031 2e34 3833 652b 3032 0a20 2020 2020   1.483e+02.     
+00021b20: 2059 2042 6f75 6e64 733a 2020 202d 312e   Y Bounds:   -1.
+00021b30: 3532 3165 2b30 322c 2031 2e35 3437 652b  521e+02, 1.547e+
+00021b40: 3032 0a20 2020 2020 205a 2042 6f75 6e64  02.      Z Bound
+00021b50: 733a 2020 202d 342e 3234 3165 2b30 302c  s:   -4.241e+00,
+00021b60: 2031 2e34 3039 652b 3032 0a20 2020 2020   1.409e+02.     
+00021b70: 204e 2041 7272 6179 733a 2020 2030 0a0a   N Arrays:   0..
+00021b80: 2020 2020 2222 220a 2020 2020 6669 6c65      """.    file
+00021b90: 6e61 6d65 203d 205f 646f 776e 6c6f 6164  name = _download
+00021ba0: 5f61 7263 6869 7665 280a 2020 2020 2020  _archive(.      
+00021bb0: 2020 2769 7661 6e2d 6e69 6b6f 6c6f 762f    'ivan-nikolov/
+00021bc0: 6269 7264 4261 7468 2e7a 6970 272c 0a20  birdBath.zip',. 
+00021bd0: 2020 2020 2020 2027 6269 7264 4261 7468         'birdBath
+00021be0: 2e76 7470 272c 0a20 2020 2029 0a20 2020  .vtp',.    ).   
+00021bf0: 2069 6620 6c6f 6164 3a0a 2020 2020 2020   if load:.      
+00021c00: 2020 7265 7475 726e 2070 7976 6973 7461    return pyvista
+00021c10: 2e72 6561 6428 6669 6c65 6e61 6d65 290a  .read(filename).
+00021c20: 2020 2020 7265 7475 726e 2066 696c 656e      return filen
+00021c30: 616d 650a 0a0a 6465 6620 646f 776e 6c6f  ame...def downlo
+00021c40: 6164 5f6f 776c 286c 6f61 643d 5472 7565  ad_owl(load=True
+00021c50: 293a 2020 2320 7072 6167 6d61 3a20 6e6f  ):  # pragma: no
+00021c60: 2063 6f76 6572 0a20 2020 2022 2222 446f   cover.    """Do
+00021c70: 776e 6c6f 6164 2061 2073 6361 6e20 6f66  wnload a scan of
+00021c80: 2061 6e20 6f77 6c20 7374 6174 7565 2063   an owl statue c
+00021c90: 7265 6174 6564 2062 7920 4976 616e 204e  reated by Ivan N
+00021ca0: 696b 6f6c 6f76 2e0a 0a20 2020 2054 6865  ikolov...    The
+00021cb0: 2064 6174 6173 6574 2077 6173 2064 6f77   dataset was dow
+00021cc0: 6e6c 6f61 6465 6420 6672 6f6d 2060 4747  nloaded from `GG
+00021cd0: 472d 4265 6e63 686d 6172 6b53 664d 3a20  G-BenchmarkSfM: 
+00021ce0: 4461 7461 7365 7420 666f 7220 4265 6e63  Dataset for Benc
+00021cf0: 686d 6172 6b69 6e67 0a20 2020 2043 6c6f  hmarking.    Clo
+00021d00: 7365 2d72 616e 6765 2053 664d 2053 6f66  se-range SfM Sof
+00021d10: 7477 6172 6520 5065 7266 6f72 6d61 6e63  tware Performanc
+00021d20: 6520 756e 6465 7220 5661 7279 696e 6720  e under Varying 
+00021d30: 4361 7074 7572 696e 6720 436f 6e64 6974  Capturing Condit
+00021d40: 696f 6e73 0a20 2020 203c 6874 7470 733a  ions.    <https:
+00021d50: 2f2f 6461 7461 2e6d 656e 6465 6c65 792e  //data.mendeley.
+00021d60: 636f 6d2f 6461 7461 7365 7473 2f62 7a78  com/datasets/bzx
+00021d70: 6b32 6e37 3873 392f 343e 605f 0a0a 2020  k2n78s9/4>`_..  
+00021d80: 2020 4f72 6967 696e 616c 2064 6174 6173    Original datas
+00021d90: 6574 7320 6172 6520 756e 6465 7220 7468  ets are under th
+00021da0: 6520 4343 2042 5920 342e 3020 6c69 6365  e CC BY 4.0 lice
+00021db0: 6e73 652e 0a0a 2020 2020 466f 7220 6d6f  nse...    For mo
+00021dc0: 7265 2064 6574 6169 6c73 2c20 7365 6520  re details, see 
+00021dd0: 6049 7661 6e20 4e69 6b6f 6c6f 7620 4461  `Ivan Nikolov Da
+00021de0: 7461 7365 7473 0a20 2020 203c 6874 7470  tasets.    <http
+00021df0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00021e00: 7976 6973 7461 2f76 746b 2d64 6174 612f  yvista/vtk-data/
+00021e10: 7472 6565 2f6d 6173 7465 722f 4461 7461  tree/master/Data
+00021e20: 2f69 7661 6e2d 6e69 6b6f 6c6f 763e 605f  /ivan-nikolov>`_
+00021e30: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00021e40: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00021e50: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
+00021e60: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
+00021e70: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
+00021e80: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
+00021e90: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
+00021ea0: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
+00021eb0: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
+00021ec0: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
+00021ed0: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
+00021ee0: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+00021ef0: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
+00021f00: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00021f10: 7079 7669 7374 612e 506f 6c79 4461 7461  pyvista.PolyData
+00021f20: 207c 2073 7472 0a20 2020 2020 2020 2044   | str.        D
+00021f30: 6174 6153 6574 206f 7220 6669 6c65 6e61  ataSet or filena
+00021f40: 6d65 2064 6570 656e 6469 6e67 206f 6e20  me depending on 
+00021f50: 6060 6c6f 6164 6060 2e0a 0a20 2020 2045  ``load``...    E
+00021f60: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+00021f70: 2d2d 2d2d 0a20 2020 2044 6f77 6e6c 6f61  ----.    Downloa
+00021f80: 6420 616e 6420 706c 6f74 2074 6865 2064  d and plot the d
+00021f90: 6174 6173 6574 2e0a 0a20 2020 203e 3e3e  ataset...    >>>
+00021fa0: 2066 726f 6d20 7079 7669 7374 6120 696d   from pyvista im
+00021fb0: 706f 7274 2065 7861 6d70 6c65 730a 2020  port examples.  
+00021fc0: 2020 3e3e 3e20 6d65 7368 203d 2065 7861    >>> mesh = exa
+00021fd0: 6d70 6c65 732e 646f 776e 6c6f 6164 5f6f  mples.download_o
+00021fe0: 776c 2829 0a20 2020 203e 3e3e 2063 706f  wl().    >>> cpo
+00021ff0: 7320 3d20 5b0a 2020 2020 2e2e 2e20 2020  s = [.    ...   
+00022000: 2020 282d 3331 352e 3138 2c20 2d34 3032    (-315.18, -402
+00022010: 2e32 312c 2032 3330 2e37 3129 2c0a 2020  .21, 230.71),.  
+00022020: 2020 2e2e 2e20 2020 2020 2836 2e30 362c    ...     (6.06,
+00022030: 202d 312e 3734 2c20 3130 312e 3438 292c   -1.74, 101.48),
+00022040: 0a20 2020 202e 2e2e 2020 2020 2028 302e  .    ...     (0.
+00022050: 3130 382c 2030 2e32 3236 2c20 302e 3936  108, 0.226, 0.96
+00022060: 3829 2c0a 2020 2020 2e2e 2e20 5d0a 2020  8),.    ... ].  
+00022070: 2020 3e3e 3e20 6d65 7368 2e70 6c6f 7428    >>> mesh.plot(
+00022080: 6370 6f73 3d63 706f 7329 0a0a 2020 2020  cpos=cpos)..    
+00022090: 5265 7475 726e 2074 6865 2073 7461 7469  Return the stati
+000220a0: 7374 6963 7320 6f66 2074 6865 2064 6174  stics of the dat
+000220b0: 6173 6574 2e0a 0a20 2020 203e 3e3e 206d  aset...    >>> m
+000220c0: 6573 680a 2020 2020 506f 6c79 4461 7461  esh.    PolyData
+000220d0: 2028 2e2e 2e29 0a20 2020 2020 204e 2043   (...).      N C
+000220e0: 656c 6c73 3a20 2020 2032 3434 3037 3037  ells:    2440707
+000220f0: 0a20 2020 2020 204e 2050 6f69 6e74 733a  .      N Points:
+00022100: 2020 2031 3232 3137 3536 0a20 2020 2020     1221756.     
+00022110: 204e 2053 7472 6970 733a 2020 2030 0a20   N Strips:   0. 
+00022120: 2020 2020 2058 2042 6f75 6e64 733a 2020       X Bounds:  
+00022130: 202d 352e 3833 3465 2b30 312c 2037 2e30   -5.834e+01, 7.0
+00022140: 3437 652b 3031 0a20 2020 2020 2059 2042  47e+01.      Y B
+00022150: 6f75 6e64 733a 2020 202d 372e 3030 3665  ounds:   -7.006e
+00022160: 2b30 312c 2036 2e36 3538 652b 3031 0a20  +01, 6.658e+01. 
+00022170: 2020 2020 205a 2042 6f75 6e64 733a 2020       Z Bounds:  
+00022180: 2031 2e36 3736 652b 3030 2c20 322e 3031   1.676e+00, 2.01
+00022190: 3365 2b30 320a 2020 2020 2020 4e20 4172  3e+02.      N Ar
+000221a0: 7261 7973 3a20 2020 300a 0a20 2020 2022  rays:   0..    "
+000221b0: 2222 0a20 2020 2066 696c 656e 616d 6520  "".    filename 
+000221c0: 3d20 5f64 6f77 6e6c 6f61 645f 6172 6368  = _download_arch
+000221d0: 6976 6528 0a20 2020 2020 2020 2027 6976  ive(.        'iv
+000221e0: 616e 2d6e 696b 6f6c 6f76 2f6f 776c 2e7a  an-nikolov/owl.z
+000221f0: 6970 272c 0a20 2020 2020 2020 2027 6f77  ip',.        'ow
+00022200: 6c2e 7674 7027 2c0a 2020 2020 290a 2020  l.vtp',.    ).  
+00022210: 2020 6966 206c 6f61 643a 0a20 2020 2020    if load:.     
+00022220: 2020 2072 6574 7572 6e20 7079 7669 7374     return pyvist
+00022230: 612e 7265 6164 2866 696c 656e 616d 6529  a.read(filename)
+00022240: 0a20 2020 2072 6574 7572 6e20 6669 6c65  .    return file
+00022250: 6e61 6d65 0a0a 0a64 6566 2064 6f77 6e6c  name...def downl
+00022260: 6f61 645f 706c 6173 7469 635f 7661 7365  oad_plastic_vase
+00022270: 286c 6f61 643d 5472 7565 293a 2020 2320  (load=True):  # 
+00022280: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+00022290: 0a20 2020 2022 2222 446f 776e 6c6f 6164  .    """Download
+000222a0: 2061 2073 6361 6e20 6f66 2061 2070 6c61   a scan of a pla
+000222b0: 7374 6963 2076 6173 6520 6372 6561 7465  stic vase create
+000222c0: 6420 6279 2049 7661 6e20 4e69 6b6f 6c6f  d by Ivan Nikolo
+000222d0: 762e 0a0a 2020 2020 5468 6520 6461 7461  v...    The data
+000222e0: 7365 7420 7761 7320 646f 776e 6c6f 6164  set was download
+000222f0: 6564 2066 726f 6d20 6047 4747 2d42 656e  ed from `GGG-Ben
+00022300: 6368 6d61 726b 5366 4d3a 2044 6174 6173  chmarkSfM: Datas
+00022310: 6574 2066 6f72 2042 656e 6368 6d61 726b  et for Benchmark
+00022320: 696e 670a 2020 2020 436c 6f73 652d 7261  ing.    Close-ra
+00022330: 6e67 6520 5366 4d20 536f 6674 7761 7265  nge SfM Software
+00022340: 2050 6572 666f 726d 616e 6365 2075 6e64   Performance und
+00022350: 6572 2056 6172 7969 6e67 2043 6170 7475  er Varying Captu
+00022360: 7269 6e67 2043 6f6e 6469 7469 6f6e 730a  ring Conditions.
+00022370: 2020 2020 3c68 7474 7073 3a2f 2f64 6174      <https://dat
+00022380: 612e 6d65 6e64 656c 6579 2e63 6f6d 2f64  a.mendeley.com/d
+00022390: 6174 6173 6574 732f 627a 786b 326e 3738  atasets/bzxk2n78
+000223a0: 7339 2f34 3e60 5f0a 0a20 2020 204f 7269  s9/4>`_..    Ori
+000223b0: 6769 6e61 6c20 6461 7461 7365 7473 2061  ginal datasets a
+000223c0: 7265 2075 6e64 6572 2074 6865 2043 4320  re under the CC 
+000223d0: 4259 2034 2e30 206c 6963 656e 7365 2e0a  BY 4.0 license..
+000223e0: 0a20 2020 2046 6f72 206d 6f72 6520 6465  .    For more de
+000223f0: 7461 696c 732c 2073 6565 2060 4976 616e  tails, see `Ivan
+00022400: 204e 696b 6f6c 6f76 2044 6174 6173 6574   Nikolov Dataset
+00022410: 730a 2020 2020 3c68 7474 7073 3a2f 2f67  s.    <https://g
+00022420: 6974 6875 622e 636f 6d2f 7079 7669 7374  ithub.com/pyvist
+00022430: 612f 7674 6b2d 6461 7461 2f74 7265 652f  a/vtk-data/tree/
+00022440: 6d61 7374 6572 2f44 6174 612f 6976 616e  master/Data/ivan
+00022450: 2d6e 696b 6f6c 6f76 3e60 5f0a 0a20 2020  -nikolov>`_..   
+00022460: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00022470: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206c  ----------.    l
+00022480: 6f61 6420 3a20 626f 6f6c 2c20 6465 6661  oad : bool, defa
+00022490: 756c 743a 2054 7275 650a 2020 2020 2020  ult: True.      
+000224a0: 2020 4c6f 6164 2074 6865 2064 6174 6173    Load the datas
+000224b0: 6574 2061 6674 6572 2064 6f77 6e6c 6f61  et after downloa
+000224c0: 6469 6e67 2069 7420 7768 656e 2060 6054  ding it when ``T
+000224d0: 7275 6560 602e 2020 5365 7420 7468 6973  rue``.  Set this
+000224e0: 0a20 2020 2020 2020 2074 6f20 6060 4661  .        to ``Fa
+000224f0: 6c73 6560 6020 616e 6420 6f6e 6c79 2074  lse`` and only t
+00022500: 6865 2066 696c 656e 616d 6520 7769 6c6c  he filename will
+00022510: 2062 6520 7265 7475 726e 6564 2e0a 0a20   be returned... 
+00022520: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00022530: 2d2d 2d2d 2d2d 0a20 2020 2070 7976 6973  ------.    pyvis
+00022540: 7461 2e50 6f6c 7944 6174 6120 7c20 7374  ta.PolyData | st
+00022550: 720a 2020 2020 2020 2020 4461 7461 5365  r.        DataSe
+00022560: 7420 6f72 2066 696c 656e 616d 6520 6465  t or filename de
+00022570: 7065 6e64 696e 6720 6f6e 2060 606c 6f61  pending on ``loa
+00022580: 6460 602e 0a0a 2020 2020 4578 616d 706c  d``...    Exampl
+00022590: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
+000225a0: 2020 2020 446f 776e 6c6f 6164 2061 6e64      Download and
+000225b0: 2070 6c6f 7420 7468 6520 6461 7461 7365   plot the datase
+000225c0: 742e 0a0a 2020 2020 3e3e 3e20 6672 6f6d  t...    >>> from
+000225d0: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
+000225e0: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
+000225f0: 206d 6573 6820 3d20 6578 616d 706c 6573   mesh = examples
+00022600: 2e64 6f77 6e6c 6f61 645f 706c 6173 7469  .download_plasti
+00022610: 635f 7661 7365 2829 0a20 2020 203e 3e3e  c_vase().    >>>
+00022620: 206d 6573 682e 706c 6f74 2829 0a0a 2020   mesh.plot()..  
+00022630: 2020 5265 7475 726e 2074 6865 2073 7461    Return the sta
+00022640: 7469 7374 6963 7320 6f66 2074 6865 2064  tistics of the d
+00022650: 6174 6173 6574 2e0a 0a20 2020 203e 3e3e  ataset...    >>>
+00022660: 206d 6573 680a 2020 2020 506f 6c79 4461   mesh.    PolyDa
+00022670: 7461 2028 2e2e 2e29 0a20 2020 2020 204e  ta (...).      N
+00022680: 2043 656c 6c73 3a20 2020 2033 3537 3039   Cells:    35709
+00022690: 3637 0a20 2020 2020 204e 2050 6f69 6e74  67.      N Point
+000226a0: 733a 2020 2031 3739 3638 3035 0a20 2020  s:   1796805.   
+000226b0: 2020 204e 2053 7472 6970 733a 2020 2030     N Strips:   0
+000226c0: 0a20 2020 2020 2058 2042 6f75 6e64 733a  .      X Bounds:
+000226d0: 2020 202d 312e 3336 3465 2b30 322c 2031     -1.364e+02, 1
+000226e0: 2e39 3239 652b 3032 0a20 2020 2020 2059  .929e+02.      Y
+000226f0: 2042 6f75 6e64 733a 2020 202d 312e 3637   Bounds:   -1.67
+00022700: 3765 2b30 322c 2031 2e36 3033 652b 3032  7e+02, 1.603e+02
+00022710: 0a20 2020 2020 205a 2042 6f75 6e64 733a  .      Z Bounds:
+00022720: 2020 2031 2e32 3039 652b 3032 2c20 342e     1.209e+02, 4.
+00022730: 3039 3065 2b30 320a 2020 2020 2020 4e20  090e+02.      N 
+00022740: 4172 7261 7973 3a20 2020 300a 0a20 2020  Arrays:   0..   
+00022750: 2022 2222 0a20 2020 2066 696c 656e 616d   """.    filenam
+00022760: 6520 3d20 5f64 6f77 6e6c 6f61 645f 6172  e = _download_ar
+00022770: 6368 6976 6528 0a20 2020 2020 2020 2027  chive(.        '
+00022780: 6976 616e 2d6e 696b 6f6c 6f76 2f70 6c61  ivan-nikolov/pla
+00022790: 7374 6963 5661 7365 2e7a 6970 272c 0a20  sticVase.zip',. 
+000227a0: 2020 2020 2020 2027 706c 6173 7469 6356         'plasticV
+000227b0: 6173 652e 7674 7027 2c0a 2020 2020 290a  ase.vtp',.    ).
+000227c0: 2020 2020 6966 206c 6f61 643a 0a20 2020      if load:.   
+000227d0: 2020 2020 2072 6574 7572 6e20 7079 7669       return pyvi
+000227e0: 7374 612e 7265 6164 2866 696c 656e 616d  sta.read(filenam
+000227f0: 6529 0a20 2020 2072 6574 7572 6e20 6669  e).    return fi
+00022800: 6c65 6e61 6d65 0a0a 0a64 6566 2064 6f77  lename...def dow
+00022810: 6e6c 6f61 645f 7365 615f 7661 7365 286c  nload_sea_vase(l
+00022820: 6f61 643d 5472 7565 293a 2020 2320 7072  oad=True):  # pr
+00022830: 6167 6d61 3a20 6e6f 2063 6f76 6572 0a20  agma: no cover. 
+00022840: 2020 2022 2222 446f 776e 6c6f 6164 2061     """Download a
+00022850: 2073 6361 6e20 6f66 2061 2073 6561 2076   scan of a sea v
+00022860: 6173 6520 6372 6561 7465 6420 6279 2049  ase created by I
+00022870: 7661 6e20 4e69 6b6f 6c6f 762e 0a0a 2020  van Nikolov...  
+00022880: 2020 5468 6520 6461 7461 7365 7420 7761    The dataset wa
+00022890: 7320 646f 776e 6c6f 6164 6564 2066 726f  s downloaded fro
+000228a0: 6d20 6047 4747 2d42 656e 6368 6d61 726b  m `GGG-Benchmark
+000228b0: 5366 4d3a 2044 6174 6173 6574 2066 6f72  SfM: Dataset for
+000228c0: 2042 656e 6368 6d61 726b 696e 670a 2020   Benchmarking.  
+000228d0: 2020 436c 6f73 652d 7261 6e67 6520 5366    Close-range Sf
+000228e0: 4d20 536f 6674 7761 7265 2050 6572 666f  M Software Perfo
+000228f0: 726d 616e 6365 2075 6e64 6572 2056 6172  rmance under Var
+00022900: 7969 6e67 2043 6170 7475 7269 6e67 2043  ying Capturing C
+00022910: 6f6e 6469 7469 6f6e 730a 2020 2020 3c68  onditions.    <h
+00022920: 7474 7073 3a2f 2f64 6174 612e 6d65 6e64  ttps://data.mend
+00022930: 656c 6579 2e63 6f6d 2f64 6174 6173 6574  eley.com/dataset
+00022940: 732f 627a 786b 326e 3738 7339 2f34 3e60  s/bzxk2n78s9/4>`
+00022950: 5f0a 0a20 2020 204f 7269 6769 6e61 6c20  _..    Original 
+00022960: 6461 7461 7365 7473 2061 7265 2075 6e64  datasets are und
+00022970: 6572 2074 6865 2043 4320 4259 2034 2e30  er the CC BY 4.0
+00022980: 206c 6963 656e 7365 2e0a 0a20 2020 2046   license...    F
+00022990: 6f72 206d 6f72 6520 6465 7461 696c 732c  or more details,
+000229a0: 2073 6565 2060 4976 616e 204e 696b 6f6c   see `Ivan Nikol
+000229b0: 6f76 2044 6174 6173 6574 730a 2020 2020  ov Datasets.    
+000229c0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+000229d0: 636f 6d2f 7079 7669 7374 612f 7674 6b2d  com/pyvista/vtk-
+000229e0: 6461 7461 2f74 7265 652f 6d61 7374 6572  data/tree/master
+000229f0: 2f44 6174 612f 6976 616e 2d6e 696b 6f6c  /Data/ivan-nikol
+00022a00: 6f76 3e60 5f0a 0a20 2020 2050 6172 616d  ov>`_..    Param
+00022a10: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+00022a20: 2d2d 2d2d 0a20 2020 206c 6f61 6420 3a20  ----.    load : 
+00022a30: 626f 6f6c 2c20 6465 6661 756c 743a 2054  bool, default: T
+00022a40: 7275 650a 2020 2020 2020 2020 4c6f 6164  rue.        Load
+00022a50: 2074 6865 2064 6174 6173 6574 2061 6674   the dataset aft
+00022a60: 6572 2064 6f77 6e6c 6f61 6469 6e67 2069  er downloading i
+00022a70: 7420 7768 656e 2060 6054 7275 6560 602e  t when ``True``.
+00022a80: 2020 5365 7420 7468 6973 0a20 2020 2020    Set this.     
+00022a90: 2020 2074 6f20 6060 4661 6c73 6560 6020     to ``False`` 
+00022aa0: 616e 6420 6f6e 6c79 2074 6865 2066 696c  and only the fil
+00022ab0: 656e 616d 6520 7769 6c6c 2062 6520 7265  ename will be re
+00022ac0: 7475 726e 6564 2e0a 0a20 2020 2052 6574  turned...    Ret
+00022ad0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+00022ae0: 0a20 2020 2070 7976 6973 7461 2e50 6f6c  .    pyvista.Pol
+00022af0: 7944 6174 6120 7c20 7374 720a 2020 2020  yData | str.    
+00022b00: 2020 2020 4461 7461 5365 7420 6f72 2066      DataSet or f
+00022b10: 696c 656e 616d 6520 6465 7065 6e64 696e  ilename dependin
+00022b20: 6720 6f6e 2060 606c 6f61 6460 602e 0a0a  g on ``load``...
+00022b30: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
+00022b40: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 446f   --------.    Do
+00022b50: 776e 6c6f 6164 2061 6e64 2070 6c6f 7420  wnload and plot 
+00022b60: 7468 6520 6461 7461 7365 742e 0a0a 2020  the dataset...  
+00022b70: 2020 3e3e 3e20 6672 6f6d 2070 7976 6973    >>> from pyvis
+00022b80: 7461 2069 6d70 6f72 7420 6578 616d 706c  ta import exampl
+00022b90: 6573 0a20 2020 203e 3e3e 206d 6573 6820  es.    >>> mesh 
+00022ba0: 3d20 6578 616d 706c 6573 2e64 6f77 6e6c  = examples.downl
+00022bb0: 6f61 645f 7365 615f 7661 7365 2829 0a20  oad_sea_vase(). 
+00022bc0: 2020 203e 3e3e 206d 6573 682e 706c 6f74     >>> mesh.plot
+00022bd0: 2829 0a0a 2020 2020 5265 7475 726e 2074  ()..    Return t
+00022be0: 6865 2073 7461 7469 7374 6963 7320 6f66  he statistics of
+00022bf0: 2074 6865 2064 6174 6173 6574 2e0a 0a20   the dataset... 
+00022c00: 2020 203e 3e3e 206d 6573 680a 2020 2020     >>> mesh.    
+00022c10: 506f 6c79 4461 7461 2028 2e2e 2e29 0a20  PolyData (...). 
+00022c20: 2020 2020 204e 2043 656c 6c73 3a20 2020       N Cells:   
+00022c30: 2033 3534 3834 3733 0a20 2020 2020 204e   3548473.      N
+00022c40: 2050 6f69 6e74 733a 2020 2031 3831 3030   Points:   18100
+00022c50: 3132 0a20 2020 2020 204e 2053 7472 6970  12.      N Strip
+00022c60: 733a 2020 2030 0a20 2020 2020 2058 2042  s:   0.      X B
+00022c70: 6f75 6e64 733a 2020 202d 312e 3636 3665  ounds:   -1.666e
+00022c80: 2b30 322c 2031 2e34 3635 652b 3032 0a20  +02, 1.465e+02. 
+00022c90: 2020 2020 2059 2042 6f75 6e64 733a 2020       Y Bounds:  
+00022ca0: 202d 312e 3734 3265 2b30 322c 2031 2e33   -1.742e+02, 1.3
+00022cb0: 3834 652b 3032 0a20 2020 2020 205a 2042  84e+02.      Z B
+00022cc0: 6f75 6e64 733a 2020 202d 312e 3530 3065  ounds:   -1.500e
+00022cd0: 2b30 322c 2032 2e39 3932 652b 3032 0a20  +02, 2.992e+02. 
+00022ce0: 2020 2020 204e 2041 7272 6179 733a 2020       N Arrays:  
+00022cf0: 2030 0a0a 2020 2020 2222 220a 2020 2020   0..    """.    
+00022d00: 6669 6c65 6e61 6d65 203d 205f 646f 776e  filename = _down
+00022d10: 6c6f 6164 5f61 7263 6869 7665 280a 2020  load_archive(.  
+00022d20: 2020 2020 2020 2769 7661 6e2d 6e69 6b6f        'ivan-niko
+00022d30: 6c6f 762f 7365 6156 6173 652e 7a69 7027  lov/seaVase.zip'
+00022d40: 2c0a 2020 2020 2020 2020 2773 6561 5661  ,.        'seaVa
+00022d50: 7365 2e76 7470 272c 0a20 2020 2029 0a20  se.vtp',.    ). 
+00022d60: 2020 2069 6620 6c6f 6164 3a0a 2020 2020     if load:.    
+00022d70: 2020 2020 7265 7475 726e 2070 7976 6973      return pyvis
+00022d80: 7461 2e72 6561 6428 6669 6c65 6e61 6d65  ta.read(filename
+00022d90: 290a 2020 2020 7265 7475 726e 2066 696c  ).    return fil
+00022da0: 656e 616d 650a 0a0a 6465 6620 646f 776e  ename...def down
+00022db0: 6c6f 6164 5f64 696b 686f 6c6f 6c6f 5f6e  load_dikhololo_n
+00022dc0: 6967 6874 2829 3a20 2023 2070 7261 676d  ight():  # pragm
+00022dd0: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
+00022de0: 2222 2244 6f77 6e6c 6f61 6420 616e 6420  """Download and 
+00022df0: 7265 6164 2074 6865 2064 696b 686f 6c6f  read the dikholo
+00022e00: 206e 6967 6874 2068 6472 2074 6578 7475   night hdr textu
+00022e10: 7265 2065 7861 6d70 6c65 2e0a 0a20 2020  re example...   
+00022e20: 2046 696c 6573 2068 6f73 7465 6420 6174   Files hosted at
+00022e30: 2068 7474 7073 3a2f 2f70 6f6c 7968 6176   https://polyhav
+00022e40: 656e 2e63 6f6d 2f0a 0a20 2020 2052 6574  en.com/..    Ret
+00022e50: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+00022e60: 0a20 2020 2070 7976 6973 7461 2e54 6578  .    pyvista.Tex
+00022e70: 7475 7265 0a20 2020 2020 2020 2048 4452  ture.        HDR
+00022e80: 2054 6578 7475 7265 2e0a 0a20 2020 2045   Texture...    E
+00022e90: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+00022ea0: 2d2d 2d2d 0a20 2020 203e 3e3e 2069 6d70  ----.    >>> imp
+00022eb0: 6f72 7420 7079 7669 7374 610a 2020 2020  ort pyvista.    
+00022ec0: 3e3e 3e20 6672 6f6d 2070 7976 6973 7461  >>> from pyvista
+00022ed0: 2069 6d70 6f72 7420 6578 616d 706c 6573   import examples
+00022ee0: 0a20 2020 203e 3e3e 2067 6c74 665f 6669  .    >>> gltf_fi
+00022ef0: 6c65 203d 2065 7861 6d70 6c65 732e 676c  le = examples.gl
+00022f00: 7466 2e64 6f77 6e6c 6f61 645f 6461 6d61  tf.download_dama
+00022f10: 6765 645f 6865 6c6d 6574 2829 0a20 2020  ged_helmet().   
+00022f20: 203e 3e3e 2074 6578 7475 7265 203d 2065   >>> texture = e
+00022f30: 7861 6d70 6c65 732e 646f 776e 6c6f 6164  xamples.download
+00022f40: 5f64 696b 686f 6c6f 6c6f 5f6e 6967 6874  _dikhololo_night
+00022f50: 2829 0a20 2020 203e 3e3e 2070 6c20 3d20  ().    >>> pl = 
+00022f60: 7079 7669 7374 612e 506c 6f74 7465 7228  pyvista.Plotter(
+00022f70: 290a 2020 2020 3e3e 3e20 706c 2e69 6d70  ).    >>> pl.imp
+00022f80: 6f72 745f 676c 7466 2867 6c74 665f 6669  ort_gltf(gltf_fi
+00022f90: 6c65 290a 2020 2020 3e3e 3e20 706c 2e73  le).    >>> pl.s
+00022fa0: 6574 5f65 6e76 6972 6f6e 6d65 6e74 5f74  et_environment_t
+00022fb0: 6578 7475 7265 2874 6578 7475 7265 290a  exture(texture).
+00022fc0: 2020 2020 3e3e 3e20 706c 2e73 686f 7728      >>> pl.show(
+00022fd0: 290a 0a20 2020 2022 2222 0a20 2020 2074  )..    """.    t
+00022fe0: 6578 7475 7265 203d 205f 646f 776e 6c6f  exture = _downlo
+00022ff0: 6164 5f61 6e64 5f72 6561 6428 2764 696b  ad_and_read('dik
+00023000: 686f 6c6f 6c6f 5f6e 6967 6874 5f34 6b2e  hololo_night_4k.
+00023010: 6864 7227 2c20 7465 7874 7572 653d 5472  hdr', texture=Tr
+00023020: 7565 290a 2020 2020 7465 7874 7572 652e  ue).    texture.
+00023030: 5365 7443 6f6c 6f72 4d6f 6465 546f 4469  SetColorModeToDi
+00023040: 7265 6374 5363 616c 6172 7328 290a 2020  rectScalars().  
+00023050: 2020 7465 7874 7572 652e 5365 744d 6970    texture.SetMip
+00023060: 6d61 7028 5472 7565 290a 2020 2020 7465  map(True).    te
+00023070: 7874 7572 652e 5365 7449 6e74 6572 706f  xture.SetInterpo
+00023080: 6c61 7465 2854 7275 6529 0a20 2020 2072  late(True).    r
+00023090: 6574 7572 6e20 7465 7874 7572 650a 0a0a  eturn texture...
+000230a0: 6465 6620 646f 776e 6c6f 6164 5f63 6164  def download_cad
+000230b0: 5f6d 6f64 656c 5f63 6173 6528 6c6f 6164  _model_case(load
+000230c0: 3d54 7275 6529 3a20 2023 2070 7261 676d  =True):  # pragm
+000230d0: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
+000230e0: 2222 2244 6f77 6e6c 6f61 6420 6120 4341  """Download a CA
+000230f0: 4420 6d6f 6465 6c20 6f66 2061 2052 6173  D model of a Ras
+00023100: 7062 6572 7279 2050 4920 3420 6361 7365  pberry PI 4 case
+00023110: 2e0a 0a20 2020 2054 6865 2064 6174 6173  ...    The datas
+00023120: 6574 2077 6173 2064 6f77 6e6c 6f61 6465  et was downloade
+00023130: 6420 6672 6f6d 2060 5468 696e 6769 7665  d from `Thingive
+00023140: 7273 650a 2020 2020 3c68 7474 7073 3a2f  rse.    <https:/
+00023150: 2f77 7777 2e74 6869 6e67 6976 6572 7365  /www.thingiverse
+00023160: 2e63 6f6d 2f74 6869 6e67 3a34 3934 3737  .com/thing:49477
+00023170: 3436 3e60 5f0a 0a20 2020 204f 7269 6769  46>`_..    Origi
+00023180: 6e61 6c20 6461 7461 7365 7473 2061 7265  nal datasets are
+00023190: 2075 6e64 6572 2074 6865 2060 4372 6561   under the `Crea
+000231a0: 7469 7665 2043 6f6d 6d6f 6e73 202d 2041  tive Commons - A
+000231b0: 7474 7269 6275 7469 6f6e 0a20 2020 203c  ttribution.    <
+000231c0: 6874 7470 733a 2f2f 6372 6561 7469 7665  https://creative
+000231d0: 636f 6d6d 6f6e 732e 6f72 672f 6c69 6365  commons.org/lice
+000231e0: 6e73 6573 2f62 792f 342e 302f 3e60 5f20  nses/by/4.0/>`_ 
+000231f0: 6c69 6365 6e73 652e 0a0a 2020 2020 5061  license...    Pa
+00023200: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00023210: 2d2d 2d2d 2d2d 2d0a 2020 2020 6c6f 6164  -------.    load
+00023220: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
+00023230: 3a20 5472 7565 0a20 2020 2020 2020 204c  : True.        L
+00023240: 6f61 6420 7468 6520 6461 7461 7365 7420  oad the dataset 
+00023250: 6166 7465 7220 646f 776e 6c6f 6164 696e  after downloadin
+00023260: 6720 6974 2077 6865 6e20 6060 5472 7565  g it when ``True
+00023270: 6060 2e20 2053 6574 2074 6869 730a 2020  ``.  Set this.  
+00023280: 2020 2020 2020 746f 2060 6046 616c 7365        to ``False
+00023290: 6060 2061 6e64 206f 6e6c 7920 7468 6520  `` and only the 
+000232a0: 6669 6c65 6e61 6d65 2077 696c 6c20 6265  filename will be
+000232b0: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
+000232c0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+000232d0: 2d2d 2d0a 2020 2020 7079 7669 7374 612e  ---.    pyvista.
+000232e0: 506f 6c79 4461 7461 207c 2073 7472 0a20  PolyData | str. 
+000232f0: 2020 2020 2020 2044 6174 6153 6574 206f         DataSet o
+00023300: 7220 6669 6c65 6e61 6d65 2064 6570 656e  r filename depen
+00023310: 6469 6e67 206f 6e20 6060 6c6f 6164 6060  ding on ``load``
+00023320: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
+00023330: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+00023340: 2044 6f77 6e6c 6f61 6420 616e 6420 706c   Download and pl
+00023350: 6f74 2074 6865 2064 6174 6173 6574 2e0a  ot the dataset..
+00023360: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
+00023370: 7669 7374 6120 696d 706f 7274 2065 7861  vista import exa
+00023380: 6d70 6c65 730a 2020 2020 3e3e 3e20 6d65  mples.    >>> me
+00023390: 7368 203d 2065 7861 6d70 6c65 732e 646f  sh = examples.do
+000233a0: 776e 6c6f 6164 5f63 6164 5f6d 6f64 656c  wnload_cad_model
+000233b0: 5f63 6173 6528 290a 2020 2020 3e3e 3e20  _case().    >>> 
+000233c0: 6d65 7368 2e70 6c6f 7428 290a 0a20 2020  mesh.plot()..   
+000233d0: 2052 6574 7572 6e20 7468 6520 7374 6174   Return the stat
+000233e0: 6973 7469 6373 206f 6620 7468 6520 6461  istics of the da
+000233f0: 7461 7365 742e 0a0a 2020 2020 3e3e 3e20  taset...    >>> 
+00023400: 6d65 7368 0a20 2020 2050 6f6c 7944 6174  mesh.    PolyDat
+00023410: 6120 282e 2e2e 290a 2020 2020 2020 4e20  a (...).      N 
+00023420: 4365 6c6c 733a 2020 2020 3135 3434 360a  Cells:    15446.
+00023430: 2020 2020 2020 4e20 506f 696e 7473 3a20        N Points: 
+00023440: 2020 3736 3737 0a20 2020 2020 204e 2053    7677.      N S
+00023450: 7472 6970 733a 2020 2030 0a20 2020 2020  trips:   0.     
+00023460: 2058 2042 6f75 6e64 733a 2020 202d 362e   X Bounds:   -6.
+00023470: 3436 3065 2d33 312c 2039 2e30 3030 652b  460e-31, 9.000e+
+00023480: 3031 0a20 2020 2020 2059 2042 6f75 6e64  01.      Y Bound
+00023490: 733a 2020 202d 332e 3533 3565 2d33 322c  s:   -3.535e-32,
+000234a0: 2031 2e34 3830 652b 3032 0a20 2020 2020   1.480e+02.     
+000234b0: 205a 2042 6f75 6e64 733a 2020 2030 2e30   Z Bounds:   0.0
+000234c0: 3030 652b 3030 2c20 322e 3030 3065 2b30  00e+00, 2.000e+0
+000234d0: 310a 2020 2020 2020 4e20 4172 7261 7973  1.      N Arrays
+000234e0: 3a20 2020 320a 0a20 2020 2022 2222 0a20  :   2..    """. 
+000234f0: 2020 2072 6574 7572 6e20 5f64 6f77 6e6c     return _downl
+00023500: 6f61 645f 616e 645f 7265 6164 2827 6361  oad_and_read('ca
+00023510: 642f 3439 3437 3734 362f 5665 6e74 6564  d/4947746/Vented
+00023520: 5f52 6561 725f 4361 7365 5f57 6974 685f  _Rear_Case_With_
+00023530: 5069 5f53 7570 706f 7274 732e 7674 7027  Pi_Supports.vtp'
+00023540: 2c20 6c6f 6164 3d6c 6f61 6429 0a0a 0a64  , load=load)...d
+00023550: 6566 2064 6f77 6e6c 6f61 645f 6165 726f  ef download_aero
+00023560: 5f62 7261 636b 6574 286c 6f61 643d 5472  _bracket(load=Tr
+00023570: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
+00023580: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
+00023590: 446f 776e 6c6f 6164 2074 6865 2066 696e  Download the fin
+000235a0: 6974 6520 656c 656d 656e 7420 736f 6c75  ite element solu
+000235b0: 7469 6f6e 206f 6620 616e 2061 6572 6f20  tion of an aero 
+000235c0: 6272 6163 6b65 742e 0a0a 2020 2020 4461  bracket...    Da
+000235d0: 7461 2067 656e 6572 6174 6564 2066 726f  ta generated fro
+000235e0: 6d20 7075 626c 6963 2053 696d 5363 616c  m public SimScal
+000235f0: 6520 6578 616d 706c 6573 2061 7420 6053  e examples at `S
+00023600: 696d 5363 616c 6520 5072 6f6a 6563 7420  imScale Project 
+00023610: 4c69 6272 6172 7920 2d0a 2020 2020 5475  Library -.    Tu
+00023620: 7262 6f20 3c68 7474 7073 3a2f 2f77 7777  rbo <https://www
+00023630: 2e73 696d 7363 616c 652e 636f 6d2f 7072  .simscale.com/pr
+00023640: 6f6a 6563 7473 2f61 7961 726e 6f7a 2f74  ojects/ayarnoz/t
+00023650: 7572 626f 2f3e 605f 2e0a 0a20 2020 204c  urbo/>`_...    L
+00023660: 6963 656e 7369 6e67 2066 6f72 2074 6869  icensing for thi
+00023670: 7320 6461 7461 7365 7420 6973 2067 7261  s dataset is gra
+00023680: 6e74 6564 2074 6f20 6672 6565 6c79 2061  nted to freely a
+00023690: 6e64 2077 6974 686f 7574 2072 6573 7472  nd without restr
+000236a0: 6963 7469 6f6e 0a20 2020 2072 6570 726f  iction.    repro
+000236b0: 6475 6365 2c20 6469 7374 7269 6275 7465  duce, distribute
+000236c0: 2c20 7075 626c 6973 6820 6163 636f 7264  , publish accord
+000236d0: 696e 6720 746f 2074 6865 2060 5369 6d53  ing to the `SimS
+000236e0: 6361 6c65 2054 6572 6d73 2061 6e64 0a20  cale Terms and. 
+000236f0: 2020 2043 6f6e 6469 7469 6f6e 7320 3c68     Conditions <h
+00023700: 7474 7073 3a2f 2f77 7777 2e73 696d 7363  ttps://www.simsc
+00023710: 616c 652e 636f 6d2f 7465 726d 732d 616e  ale.com/terms-an
+00023720: 642d 636f 6e64 6974 696f 6e73 2f3e 605f  d-conditions/>`_
+00023730: 2e0a 0a20 2020 2054 6869 7320 7072 6f6a  ...    This proj
+00023740: 6563 7420 6465 6d6f 6e73 7472 6174 6573  ect demonstrates
+00023750: 2074 6865 2073 7461 7469 6320 7374 7265   the static stre
+00023760: 7373 2061 6e61 6c79 7369 7320 6f66 2074  ss analysis of t
+00023770: 6872 6565 2061 6972 6372 6166 740a 2020  hree aircraft.  
+00023780: 2020 656e 6769 6e65 2062 6561 7269 6e67    engine bearing
+00023790: 2062 7261 636b 6574 206d 6f64 656c 7320   bracket models 
+000237a0: 636f 6e73 6964 6572 696e 6720 626f 7468  considering both
+000237b0: 206c 696e 6561 7220 616e 6420 6e6f 6e6c   linear and nonl
+000237c0: 696e 6561 720a 2020 2020 6d61 7465 7269  inear.    materi
+000237d0: 616c 2064 6566 696e 6974 696f 6e2e 2054  al definition. T
+000237e0: 6865 206d 6f64 656c 7320 6172 6520 7465  he models are te
+000237f0: 7374 6564 2077 6974 6820 686f 7269 7a6f  sted with horizo
+00023800: 6e74 616c 2061 6e64 2076 6572 7469 6361  ntal and vertica
+00023810: 6c0a 2020 2020 6c6f 6164 696e 6720 636f  l.    loading co
+00023820: 6e64 6974 696f 6e73 2061 7320 7072 6f76  nditions as prov
+00023830: 6964 6564 206f 6e20 7468 6520 6047 7261  ided on the `Gra
+00023840: 6243 4144 202d 2041 6972 706c 616e 6520  bCAD - Airplane 
+00023850: 4265 6172 696e 6720 4272 6163 6b65 740a  Bearing Bracket.
+00023860: 2020 2020 4368 616c 6c65 6e67 650a 2020      Challenge.  
+00023870: 2020 3c68 7474 7073 3a2f 2f67 7261 6263    <https://grabc
+00023880: 6164 2e63 6f6d 2f63 6861 6c6c 656e 6765  ad.com/challenge
+00023890: 732f 6169 7270 6c61 6e65 2d62 6561 7269  s/airplane-beari
+000238a0: 6e67 2d62 7261 636b 6574 2d63 6861 6c6c  ng-bracket-chall
+000238b0: 656e 6765 2f65 6e74 7269 6573 3e60 5f2e  enge/entries>`_.
+000238c0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+000238d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+000238e0: 2020 2020 6c6f 6164 203a 2062 6f6f 6c2c      load : bool,
+000238f0: 2064 6566 6175 6c74 3a20 5472 7565 0a20   default: True. 
+00023900: 2020 2020 2020 204c 6f61 6420 7468 6520         Load the 
+00023910: 6461 7461 7365 7420 6166 7465 7220 646f  dataset after do
+00023920: 776e 6c6f 6164 696e 6720 6974 2077 6865  wnloading it whe
+00023930: 6e20 6060 5472 7565 6060 2e20 2053 6574  n ``True``.  Set
+00023940: 2074 6869 730a 2020 2020 2020 2020 746f   this.        to
+00023950: 2060 6046 616c 7365 6060 2061 6e64 206f   ``False`` and o
+00023960: 6e6c 7920 7468 6520 6669 6c65 6e61 6d65  nly the filename
+00023970: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+00023980: 642e 0a0a 2020 2020 5265 7475 726e 730a  d...    Returns.
+00023990: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+000239a0: 7079 7669 7374 612e 556e 7374 7275 6374  pyvista.Unstruct
+000239b0: 7572 6564 4772 6964 207c 2073 7472 0a20  uredGrid | str. 
+000239c0: 2020 2020 2020 2044 6174 6153 6574 206f         DataSet o
+000239d0: 7220 6669 6c65 6e61 6d65 2064 6570 656e  r filename depen
+000239e0: 6469 6e67 206f 6e20 6060 6c6f 6164 6060  ding on ``load``
+000239f0: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
+00023a00: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+00023a10: 2044 6f77 6e6c 6f61 6420 7468 6520 6165   Download the ae
+00023a20: 726f 2062 7261 636b 6574 2e0a 0a20 2020  ro bracket...   
+00023a30: 203e 3e3e 2066 726f 6d20 7079 7669 7374   >>> from pyvist
+00023a40: 6120 696d 706f 7274 2065 7861 6d70 6c65  a import example
+00023a50: 730a 2020 2020 3e3e 3e20 6461 7461 7365  s.    >>> datase
+00023a60: 7420 3d20 6578 616d 706c 6573 2e64 6f77  t = examples.dow
+00023a70: 6e6c 6f61 645f 6165 726f 5f62 7261 636b  nload_aero_brack
+00023a80: 6574 2829 0a20 2020 203e 3e3e 2064 6174  et().    >>> dat
+00023a90: 6173 6574 0a20 2020 2055 6e73 7472 7563  aset.    Unstruc
+00023aa0: 7475 7265 6447 7269 6420 282e 2e2e 290a  turedGrid (...).
+00023ab0: 2020 2020 2020 4e20 4365 6c6c 733a 2020        N Cells:  
+00023ac0: 2020 3131 3732 3932 0a20 2020 2020 204e    117292.      N
+00023ad0: 2050 6f69 6e74 733a 2020 2031 3837 3033   Points:   18703
+00023ae0: 370a 2020 2020 2020 5820 426f 756e 6473  7.      X Bounds
+00023af0: 3a20 2020 2d36 2e38 3538 652d 3033 2c20  :   -6.858e-03, 
+00023b00: 312e 3131 3865 2d30 310a 2020 2020 2020  1.118e-01.      
+00023b10: 5920 426f 756e 6473 3a20 2020 2d31 2e32  Y Bounds:   -1.2
+00023b20: 3337 652d 3032 2c20 362e 3633 3465 2d30  37e-02, 6.634e-0
+00023b30: 320a 2020 2020 2020 5a20 426f 756e 6473  2.      Z Bounds
+00023b40: 3a20 2020 2d31 2e36 3338 652d 3032 2c20  :   -1.638e-02, 
+00023b50: 312e 3633 3865 2d30 320a 2020 2020 2020  1.638e-02.      
+00023b60: 4e20 4172 7261 7973 3a20 2020 330a 0a20  N Arrays:   3.. 
+00023b70: 2020 2053 686f 7720 7468 6520 6176 6169     Show the avai
+00023b80: 6c61 626c 6520 706f 696e 7420 6461 7461  lable point data
+00023b90: 2061 7272 6179 732e 0a0a 2020 2020 3e3e   arrays...    >>
+00023ba0: 3e20 6461 7461 7365 742e 706f 696e 745f  > dataset.point_
+00023bb0: 6461 7461 0a20 2020 2070 7976 6973 7461  data.    pyvista
+00023bc0: 2044 6174 6153 6574 4174 7472 6962 7574   DataSetAttribut
+00023bd0: 6573 0a20 2020 2041 7373 6f63 6961 7469  es.    Associati
+00023be0: 6f6e 2020 2020 203a 2050 4f49 4e54 0a20  on     : POINT. 
+00023bf0: 2020 2041 6374 6976 6520 5363 616c 6172     Active Scalar
+00023c00: 7320 203a 204e 6f6e 650a 2020 2020 4163  s  : None.    Ac
+00023c10: 7469 7665 2056 6563 746f 7273 2020 3a20  tive Vectors  : 
+00023c20: 4e6f 6e65 0a20 2020 2041 6374 6976 6520  None.    Active 
+00023c30: 5465 7874 7572 6520 203a 204e 6f6e 650a  Texture  : None.
+00023c40: 2020 2020 4163 7469 7665 204e 6f72 6d61      Active Norma
+00023c50: 6c73 2020 3a20 4e6f 6e65 0a20 2020 2043  ls  : None.    C
+00023c60: 6f6e 7461 696e 7320 6172 7261 7973 203a  ontains arrays :
+00023c70: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
+00023c80: 656d 656e 7420 2020 2020 2020 2020 2020  ement           
+00023c90: 2066 6c6f 6174 3332 2020 2020 2831 3837   float32    (187
+00023ca0: 3033 372c 2033 290a 2020 2020 2020 2020  037, 3).        
+00023cb0: 746f 7461 6c20 6e6f 6e6c 696e 6561 7220  total nonlinear 
+00023cc0: 7374 7261 696e 2020 666c 6f61 7433 3220  strain  float32 
+00023cd0: 2020 2028 3138 3730 3337 2c20 3629 0a20     (187037, 6). 
+00023ce0: 2020 2020 2020 2076 6f6e 204d 6973 6573         von Mises
+00023cf0: 2073 7472 6573 7320 2020 2020 2020 2066   stress        f
+00023d00: 6c6f 6174 3332 2020 2020 2831 3837 3033  loat32    (18703
+00023d10: 372c 290a 0a20 2020 2050 6c6f 7420 7468  7,)..    Plot th
+00023d20: 6520 766f 6e20 4d69 7365 7320 7374 7265  e von Mises stre
+00023d30: 7373 2e0a 0a20 2020 203e 3e3e 2063 706f  ss...    >>> cpo
+00023d40: 7320 3d20 5b0a 2020 2020 2e2e 2e20 2020  s = [.    ...   
+00023d50: 2020 282d 302e 3035 3033 2c20 302e 3133    (-0.0503, 0.13
+00023d60: 322c 202d 302e 3137 3929 2c0a 2020 2020  2, -0.179),.    
+00023d70: 2e2e 2e20 2020 2020 2830 2e30 3530 352c  ...     (0.0505,
+00023d80: 2030 2e30 3138 352c 202d 302e 3030 3230   0.0185, -0.0020
+00023d90: 3129 2c0a 2020 2020 2e2e 2e20 2020 2020  1),.    ...     
+00023da0: 2830 2e32 3735 2c20 302e 3837 322c 2030  (0.275, 0.872, 0
+00023db0: 2e34 3035 292c 0a20 2020 202e 2e2e 205d  .405),.    ... ]
+00023dc0: 0a20 2020 203e 3e3e 2064 6174 6173 6574  .    >>> dataset
+00023dd0: 2e70 6c6f 7428 0a20 2020 202e 2e2e 2020  .plot(.    ...  
+00023de0: 2020 2073 6d6f 6f74 685f 7368 6164 696e     smooth_shadin
+00023df0: 673d 5472 7565 2c0a 2020 2020 2e2e 2e20  g=True,.    ... 
+00023e00: 2020 2020 7370 6c69 745f 7368 6172 705f      split_sharp_
+00023e10: 6564 6765 733d 5472 7565 2c0a 2020 2020  edges=True,.    
+00023e20: 2e2e 2e20 2020 2020 7363 616c 6172 733d  ...     scalars=
+00023e30: 2776 6f6e 204d 6973 6573 2073 7472 6573  'von Mises stres
+00023e40: 7327 2c0a 2020 2020 2e2e 2e20 2020 2020  s',.    ...     
+00023e50: 636d 6170 3d27 6277 7227 2c0a 2020 2020  cmap='bwr',.    
+00023e60: 2e2e 2e20 2020 2020 6370 6f73 3d63 706f  ...     cpos=cpo
+00023e70: 732c 0a20 2020 202e 2e2e 2020 2020 2061  s,.    ...     a
+00023e80: 6e74 695f 616c 6961 7369 6e67 3d27 6678  nti_aliasing='fx
+00023e90: 6161 272c 0a20 2020 202e 2e2e 2029 0a0a  aa',.    ... )..
+00023ea0: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
+00023eb0: 726e 205f 646f 776e 6c6f 6164 5f61 6e64  rn _download_and
+00023ec0: 5f72 6561 6428 2766 6561 2f61 6572 6f5f  _read('fea/aero_
+00023ed0: 6272 6163 6b65 742f 6165 726f 5f62 7261  bracket/aero_bra
+00023ee0: 636b 6574 2e76 7475 272c 206c 6f61 643d  cket.vtu', load=
+00023ef0: 6c6f 6164 290a 0a0a 6465 6620 646f 776e  load)...def down
+00023f00: 6c6f 6164 5f63 6f69 6c5f 6d61 676e 6574  load_coil_magnet
+00023f10: 6963 5f66 6965 6c64 286c 6f61 643d 5472  ic_field(load=Tr
+00023f20: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
+00023f30: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
+00023f40: 446f 776e 6c6f 6164 2074 6865 206d 6167  Download the mag
+00023f50: 6e65 7469 6320 6669 656c 6420 6f66 2061  netic field of a
+00023f60: 2063 6f69 6c2e 0a0a 2020 2020 5468 6573   coil...    Thes
+00023f70: 6520 6578 616d 706c 6573 2077 6572 6520  e examples were 
+00023f80: 6765 6e65 7261 7465 6420 6672 6f6d 2074  generated from t
+00023f90: 6865 2066 6f6c 6c6f 7769 6e67 2060 7363  he following `sc
+00023fa0: 7269 7074 0a20 2020 203c 6874 7470 733a  ript.    <https:
+00023fb0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7976  //github.com/pyv
+00023fc0: 6973 7461 2f76 746b 2d64 6174 612f 7472  ista/vtk-data/tr
+00023fd0: 6565 2f6d 6173 7465 722f 4461 7461 2f6d  ee/master/Data/m
+00023fe0: 6167 7079 6c69 622f 3e60 5f2e 0a0a 2020  agpylib/>`_...  
+00023ff0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00024000: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00024010: 6c6f 6164 203a 2062 6f6f 6c2c 2064 6566  load : bool, def
+00024020: 6175 6c74 3a20 5472 7565 0a20 2020 2020  ault: True.     
+00024030: 2020 204c 6f61 6420 7468 6520 6461 7461     Load the data
+00024040: 7365 7420 6166 7465 7220 646f 776e 6c6f  set after downlo
+00024050: 6164 696e 6720 6974 2077 6865 6e20 6060  ading it when ``
+00024060: 5472 7565 6060 2e20 2053 6574 2074 6869  True``.  Set thi
+00024070: 730a 2020 2020 2020 2020 746f 2060 6046  s.        to ``F
+00024080: 616c 7365 6060 2061 6e64 206f 6e6c 7920  alse`` and only 
+00024090: 7468 6520 6669 6c65 6e61 6d65 2077 696c  the filename wil
+000240a0: 6c20 6265 2072 6574 7572 6e65 642e 0a0a  l be returned...
+000240b0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+000240c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7079 7669  -------.    pyvi
+000240d0: 7374 612e 556e 6966 6f72 6d47 7269 6420  sta.UniformGrid 
+000240e0: 6f72 2073 7472 0a20 2020 2020 2020 2044  or str.        D
+000240f0: 6174 6153 6574 206f 7220 6669 6c65 6e61  ataSet or filena
+00024100: 6d65 2064 6570 656e 6469 6e67 206f 6e20  me depending on 
+00024110: 6060 6c6f 6164 6060 2e0a 0a20 2020 2045  ``load``...    E
+00024120: 7861 6d70 6c65 730a 2020 2020 2d2d 2d2d  xamples.    ----
+00024130: 2d2d 2d2d 0a20 2020 2044 6f77 6e6c 6f61  ----.    Downloa
+00024140: 6420 7468 6520 6d61 676e 6574 6963 2066  d the magnetic f
+00024150: 6965 6c64 2064 6174 6173 6574 2061 6e64  ield dataset and
+00024160: 2067 656e 6572 6174 6520 7374 7265 616d   generate stream
+00024170: 6c69 6e65 7320 6672 6f6d 2074 6865 2066  lines from the f
+00024180: 6965 6c64 2e0a 0a20 2020 203e 3e3e 2069  ield...    >>> i
+00024190: 6d70 6f72 7420 7079 7669 7374 6120 6173  mport pyvista as
+000241a0: 2070 760a 2020 2020 3e3e 3e20 6672 6f6d   pv.    >>> from
+000241b0: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
+000241c0: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
+000241d0: 2067 7269 6420 3d20 6578 616d 706c 6573   grid = examples
+000241e0: 2e64 6f77 6e6c 6f61 645f 636f 696c 5f6d  .download_coil_m
+000241f0: 6167 6e65 7469 635f 6669 656c 6428 290a  agnetic_field().
+00024200: 2020 2020 3e3e 3e20 7365 6564 203d 2070      >>> seed = p
+00024210: 762e 4469 7363 2869 6e6e 6572 3d31 2c20  v.Disc(inner=1, 
+00024220: 6f75 7465 723d 352e 322c 2072 5f72 6573  outer=5.2, r_res
+00024230: 3d33 2c20 635f 7265 733d 3132 290a 2020  =3, c_res=12).  
+00024240: 2020 3e3e 3e20 7374 726c 203d 2067 7269    >>> strl = gri
+00024250: 642e 7374 7265 616d 6c69 6e65 735f 6672  d.streamlines_fr
+00024260: 6f6d 5f73 6f75 7263 6528 0a20 2020 202e  om_source(.    .
+00024270: 2e2e 2020 2020 2073 6565 642c 0a20 2020  ..     seed,.   
+00024280: 202e 2e2e 2020 2020 2076 6563 746f 7273   ...     vectors
+00024290: 3d27 4227 2c0a 2020 2020 2e2e 2e20 2020  ='B',.    ...   
+000242a0: 2020 6d61 785f 7469 6d65 3d31 3830 2c0a    max_time=180,.
+000242b0: 2020 2020 2e2e 2e20 2020 2020 696e 6974      ...     init
+000242c0: 6961 6c5f 7374 6570 5f6c 656e 6774 683d  ial_step_length=
+000242d0: 302e 312c 0a20 2020 202e 2e2e 2020 2020  0.1,.    ...    
+000242e0: 2069 6e74 6567 7261 7469 6f6e 5f64 6972   integration_dir
+000242f0: 6563 7469 6f6e 3d27 626f 7468 272c 0a20  ection='both',. 
+00024300: 2020 202e 2e2e 2029 0a20 2020 203e 3e3e     ... ).    >>>
+00024310: 2073 7472 6c2e 706c 6f74 280a 2020 2020   strl.plot(.    
+00024320: 2e2e 2e20 2020 2020 636d 6170 3d27 706c  ...     cmap='pl
+00024330: 6173 6d61 272c 0a20 2020 202e 2e2e 2020  asma',.    ...  
+00024340: 2020 2072 656e 6465 725f 6c69 6e65 735f     render_lines_
+00024350: 6173 5f74 7562 6573 3d54 7275 652c 0a20  as_tubes=True,. 
+00024360: 2020 202e 2e2e 2020 2020 206c 696e 655f     ...     line_
+00024370: 7769 6474 683d 322c 0a20 2020 202e 2e2e  width=2,.    ...
+00024380: 2020 2020 206c 6967 6874 696e 673d 4661       lighting=Fa
+00024390: 6c73 652c 0a20 2020 202e 2e2e 2020 2020  lse,.    ...    
+000243a0: 207a 6f6f 6d3d 322c 0a20 2020 202e 2e2e   zoom=2,.    ...
+000243b0: 2029 0a0a 2020 2020 506c 6f74 2074 6865   )..    Plot the
+000243c0: 206d 6167 6e65 7420 6669 656c 6420 7374   magnet field st
+000243d0: 7265 6e67 7468 2069 6e20 7468 6520 5a20  rength in the Z 
+000243e0: 6469 7265 6374 696f 6e2e 0a0a 2020 2020  direction...    
+000243f0: 3e3e 3e20 696d 706f 7274 206e 756d 7079  >>> import numpy
+00024400: 2061 7320 6e70 0a20 2020 203e 3e3e 2069   as np.    >>> i
+00024410: 6d70 6f72 7420 7079 7669 7374 6120 6173  mport pyvista as
+00024420: 2070 760a 2020 2020 3e3e 3e20 6672 6f6d   pv.    >>> from
+00024430: 2070 7976 6973 7461 2069 6d70 6f72 7420   pyvista import 
+00024440: 6578 616d 706c 6573 0a20 2020 203e 3e3e  examples.    >>>
+00024450: 2067 7269 6420 3d20 6578 616d 706c 6573   grid = examples
+00024460: 2e64 6f77 6e6c 6f61 645f 636f 696c 5f6d  .download_coil_m
+00024470: 6167 6e65 7469 635f 6669 656c 6428 290a  agnetic_field().
+00024480: 2020 2020 3e3e 3e20 2320 6372 6561 7465      >>> # create
+00024490: 2063 6f69 6c73 0a20 2020 203e 3e3e 2063   coils.    >>> c
+000244a0: 6f69 6c73 203d 205b 5d0a 2020 2020 3e3e  oils = [].    >>
+000244b0: 3e20 666f 7220 7a20 696e 206e 702e 6c69  > for z in np.li
+000244c0: 6e73 7061 6365 282d 382c 2038 2c20 3136  nspace(-8, 8, 16
+000244d0: 293a 0a20 2020 202e 2e2e 2020 2020 2063  ):.    ...     c
+000244e0: 6f69 6c73 2e61 7070 656e 6428 0a20 2020  oils.append(.   
+000244f0: 202e 2e2e 2020 2020 2020 2020 2070 762e   ...         pv.
+00024500: 506f 6c79 676f 6e28 2830 2c20 302c 207a  Polygon((0, 0, z
+00024510: 292c 2072 6164 6975 733d 352c 206e 5f73  ), radius=5, n_s
+00024520: 6964 6573 3d31 3030 2c20 6669 6c6c 3d46  ides=100, fill=F
+00024530: 616c 7365 290a 2020 2020 2e2e 2e20 2020  alse).    ...   
+00024540: 2020 290a 2020 2020 2e2e 2e0a 2020 2020    ).    ....    
+00024550: 3e3e 3e20 636f 696c 7320 3d20 7076 2e4d  >>> coils = pv.M
+00024560: 756c 7469 426c 6f63 6b28 636f 696c 7329  ultiBlock(coils)
+00024570: 0a20 2020 203e 3e3e 2023 2070 6c6f 7420  .    >>> # plot 
+00024580: 7468 6520 6d61 676e 6574 2066 6965 6c64  the magnet field
+00024590: 2073 7472 656e 6774 6820 696e 2074 6865   strength in the
+000245a0: 205a 2064 6972 6563 7469 6f6e 0a20 2020   Z direction.   
+000245b0: 203e 3e3e 2073 6361 6c61 7273 203d 206e   >>> scalars = n
+000245c0: 702e 6162 7328 6772 6964 5b27 4227 5d5b  p.abs(grid['B'][
+000245d0: 3a2c 2032 5d29 0a20 2020 203e 3e3e 2070  :, 2]).    >>> p
+000245e0: 6c20 3d20 7076 2e50 6c6f 7474 6572 2829  l = pv.Plotter()
+000245f0: 0a20 2020 203e 3e3e 205f 203d 2070 6c2e  .    >>> _ = pl.
+00024600: 6164 645f 6d65 7368 280a 2020 2020 2e2e  add_mesh(.    ..
+00024610: 2e20 2020 2020 636f 696c 732c 2072 656e  .     coils, ren
+00024620: 6465 725f 6c69 6e65 735f 6173 5f74 7562  der_lines_as_tub
+00024630: 6573 3d54 7275 652c 206c 696e 655f 7769  es=True, line_wi
+00024640: 6474 683d 352c 2063 6f6c 6f72 3d27 7727  dth=5, color='w'
+00024650: 0a20 2020 202e 2e2e 2029 0a20 2020 203e  .    ... ).    >
+00024660: 3e3e 2076 6f6c 203d 2070 6c2e 6164 645f  >> vol = pl.add_
+00024670: 766f 6c75 6d65 280a 2020 2020 2e2e 2e20  volume(.    ... 
+00024680: 2020 2020 6772 6964 2c0a 2020 2020 2e2e      grid,.    ..
+00024690: 2e20 2020 2020 7363 616c 6172 733d 7363  .     scalars=sc
+000246a0: 616c 6172 732c 0a20 2020 202e 2e2e 2020  alars,.    ...  
+000246b0: 2020 2063 6d61 703d 2770 6c61 736d 6127     cmap='plasma'
+000246c0: 2c0a 2020 2020 2e2e 2e20 2020 2020 7368  ,.    ...     sh
+000246d0: 6f77 5f73 6361 6c61 725f 6261 723d 4661  ow_scalar_bar=Fa
+000246e0: 6c73 652c 0a20 2020 202e 2e2e 2020 2020  lse,.    ...    
+000246f0: 206c 6f67 5f73 6361 6c65 3d54 7275 652c   log_scale=True,
+00024700: 0a20 2020 202e 2e2e 2020 2020 206f 7061  .    ...     opa
+00024710: 6369 7479 3d27 7369 676d 6f69 645f 3227  city='sigmoid_2'
+00024720: 2c0a 2020 2020 2e2e 2e20 290a 2020 2020  ,.    ... ).    
+00024730: 3e3e 3e20 766f 6c2e 7072 6f70 2e69 6e74  >>> vol.prop.int
+00024740: 6572 706f 6c61 7469 6f6e 5f74 7970 6520  erpolation_type 
+00024750: 3d20 276c 696e 6561 7227 0a20 2020 203e  = 'linear'.    >
+00024760: 3e3e 205f 203d 2070 6c2e 6164 645f 766f  >> _ = pl.add_vo
+00024770: 6c75 6d65 5f63 6c69 705f 706c 616e 6528  lume_clip_plane(
+00024780: 0a20 2020 202e 2e2e 2020 2020 2076 6f6c  .    ...     vol
+00024790: 2c0a 2020 2020 2e2e 2e20 2020 2020 6e6f  ,.    ...     no
+000247a0: 726d 616c 3d27 2d78 272c 0a20 2020 202e  rmal='-x',.    .
+000247b0: 2e2e 2020 2020 206e 6f72 6d61 6c5f 726f  ..     normal_ro
+000247c0: 7461 7469 6f6e 3d46 616c 7365 2c0a 2020  tation=False,.  
+000247d0: 2020 2e2e 2e20 2020 2020 696e 7465 7261    ...     intera
+000247e0: 6374 696f 6e5f 6576 656e 743d 2761 6c77  ction_event='alw
+000247f0: 6179 7327 2c0a 2020 2020 2e2e 2e20 2020  ays',.    ...   
+00024800: 2020 7769 6467 6574 5f63 6f6c 6f72 3d70    widget_color=p
+00024810: 762e 436f 6c6f 7228 6f70 6163 6974 793d  v.Color(opacity=
+00024820: 302e 3029 2c0a 2020 2020 2e2e 2e20 290a  0.0),.    ... ).
+00024830: 2020 2020 3e3e 3e20 706c 2e65 6e61 626c      >>> pl.enabl
+00024840: 655f 616e 7469 5f61 6c69 6173 696e 6728  e_anti_aliasing(
+00024850: 290a 2020 2020 3e3e 3e20 706c 2e63 616d  ).    >>> pl.cam
+00024860: 6572 612e 7a6f 6f6d 2832 290a 2020 2020  era.zoom(2).    
+00024870: 3e3e 3e20 706c 2e73 686f 7728 290a 0a20  >>> pl.show().. 
+00024880: 2020 2053 6565 2074 6865 203a 7265 663a     See the :ref:
+00024890: 606d 6167 6e65 7469 635f 6669 656c 6473  `magnetic_fields
+000248a0: 5f65 7861 6d70 6c65 6020 666f 7220 6d6f  _example` for mo
+000248b0: 7265 2064 6574 6169 6c73 206f 6e20 686f  re details on ho
+000248c0: 7720 746f 2070 6c6f 7420 7769 7468 0a20  w to plot with. 
+000248d0: 2020 2074 6869 7320 6461 7461 7365 742e     this dataset.
+000248e0: 0a0a 2020 2020 2222 220a 2020 2020 7265  ..    """.    re
+000248f0: 7475 726e 205f 646f 776e 6c6f 6164 5f61  turn _download_a
+00024900: 6e64 5f72 6561 6428 276d 6167 7079 6c69  nd_read('magpyli
+00024910: 622f 636f 696c 5f66 6965 6c64 2e76 7469  b/coil_field.vti
+00024920: 272c 206c 6f61 643d 6c6f 6164 290a 0a0a  ', load=load)...
+00024930: 6465 6620 646f 776e 6c6f 6164 5f6d 6573  def download_mes
+00024940: 6869 6f5f 7864 6d66 286c 6f61 643d 5472  hio_xdmf(load=Tr
+00024950: 7565 293a 2020 2320 7072 6167 6d61 3a20  ue):  # pragma: 
+00024960: 6e6f 2063 6f76 6572 0a20 2020 2022 2222  no cover.    """
+00024970: 446f 776e 6c6f 6164 2078 646d 6620 6669  Download xdmf fi
+00024980: 6c65 2063 7265 6174 6564 2062 7920 6d65  le created by me
+00024990: 7368 696f 2e0a 0a20 2020 2054 6865 2064  shio...    The d
+000249a0: 6174 6173 6574 2077 6173 2063 7265 6174  ataset was creat
+000249b0: 6564 2062 7920 6060 7465 7374 5f74 696d  ed by ``test_tim
+000249c0: 655f 7365 7269 6573 6060 2074 6573 7420  e_series`` test 
+000249d0: 6675 6e63 7469 6f6e 2069 6e20 6d65 7368  function in mesh
+000249e0: 696f 2e0a 0a20 2020 2050 6172 616d 6574  io...    Paramet
+000249f0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00024a00: 2d2d 0a20 2020 206c 6f61 6420 3a20 626f  --.    load : bo
+00024a10: 6f6c 2c20 6465 6661 756c 743a 2054 7275  ol, default: Tru
+00024a20: 650a 2020 2020 2020 2020 4c6f 6164 2074  e.        Load t
+00024a30: 6865 2064 6174 6173 6574 2061 6674 6572  he dataset after
+00024a40: 2064 6f77 6e6c 6f61 6469 6e67 2069 7420   downloading it 
+00024a50: 7768 656e 2060 6054 7275 6560 602e 2020  when ``True``.  
+00024a60: 5365 7420 7468 6973 0a20 2020 2020 2020  Set this.       
+00024a70: 2074 6f20 6060 4661 6c73 6560 6020 616e   to ``False`` an
+00024a80: 6420 6f6e 6c79 2074 6865 2066 696c 656e  d only the filen
+00024a90: 616d 6520 7769 6c6c 2062 6520 7265 7475  ame will be retu
+00024aa0: 726e 6564 2e0a 0a20 2020 2052 6574 7572  rned...    Retur
+00024ab0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00024ac0: 2020 2070 7976 6973 7461 2e55 6e73 7472     pyvista.Unstr
+00024ad0: 7563 7475 7265 6447 7269 6420 6f72 2073  ucturedGrid or s
+00024ae0: 7472 0a20 2020 2020 2020 2044 6174 6153  tr.        DataS
+00024af0: 6574 206f 7220 6669 6c65 6e61 6d65 2064  et or filename d
+00024b00: 6570 656e 6469 6e67 206f 6e20 6060 6c6f  epending on ``lo
+00024b10: 6164 6060 2e0a 0a20 2020 2045 7861 6d70  ad``...    Examp
+00024b20: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
+00024b30: 0a20 2020 203e 3e3e 2066 726f 6d20 7079  .    >>> from py
+00024b40: 7669 7374 6120 696d 706f 7274 2065 7861  vista import exa
+00024b50: 6d70 6c65 730a 2020 2020 3e3e 3e20 6461  mples.    >>> da
+00024b60: 7461 7365 7420 3d20 6578 616d 706c 6573  taset = examples
+00024b70: 2e64 6f77 6e6c 6f61 645f 6d65 7368 696f  .download_meshio
+00024b80: 5f78 646d 6628 290a 2020 2020 3e3e 3e20  _xdmf().    >>> 
+00024b90: 6461 7461 7365 742e 706c 6f74 2829 0a0a  dataset.plot()..
+00024ba0: 2020 2020 2222 220a 2020 2020 5f20 3d20      """.    _ = 
+00024bb0: 646f 776e 6c6f 6164 5f66 696c 6528 226d  download_file("m
+00024bc0: 6573 6869 6f2f 6f75 742e 6835 2229 0a20  eshio/out.h5"). 
+00024bd0: 2020 2072 6574 7572 6e20 5f64 6f77 6e6c     return _downl
+00024be0: 6f61 645f 616e 645f 7265 6164 2822 6d65  oad_and_read("me
+00024bf0: 7368 696f 2f6f 7574 2e78 646d 6622 2c20  shio/out.xdmf", 
+00024c00: 6c6f 6164 3d6c 6f61 6429 0a              load=load).
```

### Comparing `pyvista-0.39.0/pyvista/examples/examples.py` & `pyvista-0.39.1/pyvista/examples/examples.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/globe.vtk` & `pyvista-0.39.1/pyvista/examples/globe.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/gltf.py` & `pyvista-0.39.1/pyvista/examples/gltf.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,23 +27,21 @@
     -------
     str
         Filename of the gltf file.
 
     Examples
     --------
     >>> import pyvista
-    >>> from pyvista import examples  # doctest:+SKIP
-    >>> gltf_file = (
-    ...     examples.gltf.download_damaged_helmet()
-    ... )  # doctest:+SKIP
-    >>> cubemap = examples.download_sky_box_cube_map()  # doctest:+SKIP
-    >>> pl = pyvista.Plotter()  # doctest:+SKIP
-    >>> pl.import_gltf(gltf_file)  # doctest:+SKIP
-    >>> pl.set_environment_texture(cubemap)  # doctest:+SKIP
-    >>> pl.show()  # doctest:+SKIP
+    >>> from pyvista import examples
+    >>> gltf_file = examples.gltf.download_damaged_helmet()
+    >>> cubemap = examples.download_sky_box_cube_map()
+    >>> pl = pyvista.Plotter()
+    >>> pl.import_gltf(gltf_file)
+    >>> pl.set_environment_texture(cubemap)
+    >>> pl.show()
 
     """
     return GLTF_FETCHER.fetch('DamagedHelmet/glTF-Embedded/DamagedHelmet.gltf')
 
 
 def download_sheen_chair():  # pragma: no cover
     """Download the sheen chair example.
@@ -54,17 +52,17 @@
     -------
     str
         Filename of the gltf file.
 
     Examples
     --------
     >>> import pyvista
-    >>> from pyvista import examples  # doctest:+SKIP
-    >>> gltf_file = examples.gltf.download_sheen_chair()  # doctest:+SKIP
-    >>> cubemap = examples.download_sky_box_cube_map()  # doctest:+SKIP
+    >>> from pyvista import examples
+    >>> gltf_file = examples.gltf.download_sheen_chair()
+    >>> cubemap = examples.download_sky_box_cube_map()
     >>> pl = pyvista.Plotter()  # doctest:+SKIP
     >>> pl.import_gltf(gltf_file)  # doctest:+SKIP
     >>> pl.set_environment_texture(cubemap)  # doctest:+SKIP
     >>> pl.show()  # doctest:+SKIP
 
     """
     return GLTF_FETCHER.fetch('SheenChair/glTF-Binary/SheenChair.glb')
@@ -79,19 +77,19 @@
     -------
     str
         Filename of the gltf file.
 
     Examples
     --------
     >>> import pyvista
-    >>> from pyvista import examples  # doctest:+SKIP
-    >>> gltf_file = examples.gltf.download_gearbox()  # doctest:+SKIP
-    >>> pl = pyvista.Plotter()  # doctest:+SKIP
-    >>> pl.import_gltf(gltf_file)  # doctest:+SKIP
-    >>> pl.show()  # doctest:+SKIP
+    >>> from pyvista import examples
+    >>> gltf_file = examples.gltf.download_gearbox()
+    >>> pl = pyvista.Plotter()
+    >>> pl.import_gltf(gltf_file)
+    >>> pl.show()
 
     """
     return GLTF_FETCHER.fetch('GearboxAssy/glTF-Binary/GearboxAssy.glb')
 
 
 def download_avocado():  # pragma: no cover
     """Download the avocado example.
@@ -102,19 +100,19 @@
     -------
     str
         Filename of the gltf file.
 
     Examples
     --------
     >>> import pyvista
-    >>> from pyvista import examples  # doctest:+SKIP
-    >>> gltf_file = examples.gltf.download_avocado()  # doctest:+SKIP
-    >>> pl = pyvista.Plotter()  # doctest:+SKIP
-    >>> pl.import_gltf(gltf_file)  # doctest:+SKIP
-    >>> pl.show()  # doctest:+SKIP
+    >>> from pyvista import examples
+    >>> gltf_file = examples.gltf.download_avocado()
+    >>> pl = pyvista.Plotter()
+    >>> pl.import_gltf(gltf_file)
+    >>> pl.show()
 
     """
     return GLTF_FETCHER.fetch('Avocado/glTF-Binary/Avocado.glb')
 
 
 def download_milk_truck():  # pragma: no cover
     """Download the milk truck example.
@@ -125,15 +123,15 @@
     -------
     str
         Filename of the gltf file.
 
     Examples
     --------
     >>> import pyvista
-    >>> from pyvista import examples  # doctest:+SKIP
-    >>> gltf_file = examples.gltf.download_milk_truck()  # doctest:+SKIP
-    >>> pl = pyvista.Plotter()  # doctest:+SKIP
-    >>> pl.import_gltf(gltf_file)  # doctest:+SKIP
-    >>> pl.show()  # doctest:+SKIP
+    >>> from pyvista import examples
+    >>> gltf_file = examples.gltf.download_milk_truck()
+    >>> pl = pyvista.Plotter()
+    >>> pl.import_gltf(gltf_file)
+    >>> pl.show()
 
     """
     return GLTF_FETCHER.fetch('CesiumMilkTruck/glTF-Binary/CesiumMilkTruck.glb')
```

### Comparing `pyvista-0.39.0/pyvista/examples/hexbeam.vtk` & `pyvista-0.39.1/pyvista/examples/hexbeam.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/nut.ply` & `pyvista-0.39.1/pyvista/examples/nut.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/planets.py` & `pyvista-0.39.1/pyvista/examples/planets.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/rectilinear.vtk` & `pyvista-0.39.1/pyvista/examples/rectilinear.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/sphere.ply` & `pyvista-0.39.1/pyvista/examples/sphere.ply`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/uniform.vtk` & `pyvista-0.39.1/pyvista/examples/uniform.vtk`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/examples/vrml.py` & `pyvista-0.39.1/pyvista/examples/vrml.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/ext/coverage.py` & `pyvista-0.39.1/pyvista/ext/coverage.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/ext/plot_directive.py` & `pyvista-0.39.1/pyvista/ext/plot_directive.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/jupyter/__init__.py` & `pyvista-0.39.1/pyvista/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/jupyter/notebook.py` & `pyvista-0.39.1/pyvista/jupyter/notebook.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/jupyter/pv_ipygany.py` & `pyvista-0.39.1/pyvista/jupyter/pv_ipygany.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/jupyter/pv_pythreejs.py` & `pyvista-0.39.1/pyvista/jupyter/pv_pythreejs.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/__init__.py` & `pyvista-0.39.1/pyvista/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/_plotting.py` & `pyvista-0.39.1/pyvista/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/_property.py` & `pyvista-0.39.1/pyvista/plotting/_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/actor.py` & `pyvista-0.39.1/pyvista/plotting/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     --------
     Create an actor without using :class:`pyvista.Plotter`.
 
     >>> import pyvista as pv
     >>> mesh = pv.Sphere()
     >>> mapper = pv.DataSetMapper(mesh)
     >>> actor = pv.Actor(mapper=mapper)
-    >>> actor  # doctest:+SKIP
-    Actor (0x7f54c4d65ee0)
+    >>> actor
+    Actor (...)
       Center:                     (0.0, 0.0, 0.0)
       Pickable:                   True
       Position:                   (0.0, 0.0, 0.0)
       Scale:                      (1.0, 1.0, 1.0)
       Visible:                    True
       X Bounds                    -4.993E-01, 4.993E-01
       Y Bounds                    -4.965E-01, 4.965E-01
@@ -110,32 +110,31 @@
         --------
         Create an actor and assign a mapper to it.
 
         >>> import pyvista as pv
         >>> dataset = pv.Sphere()
         >>> actor = pv.Actor()
         >>> actor.mapper = pv.DataSetMapper(dataset)
-        >>> actor.mapper  # doctest:+SKIP
-        DataSetMapper (0x7f34dcec5040)
+        >>> actor.mapper
+        DataSetMapper (...)
           Scalar visibility:           True
           Scalar range:                (0.0, 1.0)
-          Interpolate before mapping:  False
+          Interpolate before mapping:  True
           Scalar map mode:             default
           Color mode:                  direct
         <BLANKLINE>
         Attached dataset:
-        PolyData (0x7f34dcec5f40)
-          N Cells:  1680
-          N Points: 842
-          N Strips: 0
-          X Bounds: -4.993e-01, 4.993e-01
-          Y Bounds: -4.965e-01, 4.965e-01
-          Z Bounds: -5.000e-01, 5.000e-01
-          N Arrays: 1
-        <BLANKLINE>
+        PolyData (...)
+          N Cells:    1680
+          N Points:   842
+          N Strips:   0
+          X Bounds:   -4.993e-01, 4.993e-01
+          Y Bounds:   -4.965e-01, 4.965e-01
+          Z Bounds:   -5.000e-01, 5.000e-01
+          N Arrays:   1
 
         """
         return self.GetMapper()
 
     @mapper.setter
     def mapper(self, obj):
         return self.SetMapper(obj)
@@ -180,16 +179,19 @@
         >>> from pyvista import examples
         >>> plane = pv.Plane()
         >>> plane.active_t_coords is not None
         True
         >>> pl = pv.Plotter()
         >>> actor = pl.add_mesh(plane)
         >>> actor.texture = examples.download_masonry_texture()
-        >>> actor.texture  # doctest:+SKIP
-        <Texture(0x378c920) at 0x7f7af577e700>
+        >>> actor.texture
+        Texture (...)
+          Components:   3
+          Cube Map:     False
+          Dimensions:   256, 256
 
         """
         return self.GetTexture()
 
     @texture.setter
     def texture(self, obj):
         self.SetTexture(obj)
```

### Comparing `pyvista-0.39.0/pyvista/plotting/actor_properties.py` & `pyvista-0.39.1/pyvista/plotting/actor_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     >>> axes = pv.Axes()
     >>> z_axes_prop = axes.axes_actor.z_axis_shaft_properties
     >>> z_axes_prop.color = (1, 1, 0)
     >>> z_axes_prop.opacity = 0.5
     >>> axes.axes_actor.shaft_type = axes.axes_actor.ShaftType.CYLINDER
 
     >>> pl = pv.Plotter()
-    >>> pl.add_actor(axes.axes_actor)  # doctest:+SKIP
-    >>> pl.add_mesh(pv.Sphere())  # doctest:+SKIP
-    >>> pl.show()  # doctest:+SKIP
+    >>> _ = pl.add_actor(axes.axes_actor)
+    >>> _ = pl.add_mesh(pv.Sphere())
+    >>> pl.show()
 
     """
 
     def __init__(self, properties: pv._vtk.vtkProperty) -> None:
         super().__init__()
         self.properties = properties
```

### Comparing `pyvista-0.39.0/pyvista/plotting/axes.py` & `pyvista-0.39.1/pyvista/plotting/axes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/axes_actor.py` & `pyvista-0.39.1/pyvista/plotting/axes_actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     >>> axes = pv.Axes()
     >>> axes.axes_actor.z_axis_shaft_properties.color = (0, 1, 1)
     >>> axes.axes_actor.shaft_type = axes.axes_actor.ShaftType.CYLINDER
     >>> pl = pv.Plotter()
     >>> _ = pl.add_actor(axes.axes_actor)
     >>> _ = pl.add_mesh(pv.Sphere())
-    >>> pl.show()  # doctest:+SKIP
+    >>> pl.show()
 
     Or you can use this as a custom orientation widget with
     :func:`add_orientation_widget() <pyvista.Renderer.add_orientation_widget>`:
 
     >>> import pyvista as pv
 
     >>> axes = pv.Axes()
@@ -50,15 +50,15 @@
 
     >>> pl = pv.Plotter()
     >>> _ = pl.add_mesh(pv.Cone())
     >>> _ = pl.add_orientation_widget(
     ...     axes_actor,
     ...     viewport=(0, 0, 0.5, 0.5),
     ... )
-    >>> pl.show()  # doctest:+SKIP
+    >>> pl.show()
 
     """
 
     class ShaftType(Enum):
         """Types of shaft shapes available."""
 
         CYLINDER = 0
```

### Comparing `pyvista-0.39.0/pyvista/plotting/background_renderer.py` & `pyvista-0.39.1/pyvista/plotting/background_renderer.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/camera.py` & `pyvista-0.39.1/pyvista/plotting/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -602,17 +602,17 @@
     @property
     def direction(self):
         """Vector from the camera position to the focal point.
 
         Examples
         --------
         >>> import pyvista
-        >>> plotter = pyvista.Plotter()
-        >>> plotter.camera.direction  # doctest:+SKIP
-        (0.0, 0.0, -1.0)
+        >>> pl = pyvista.Plotter()
+        >>> pl.camera.direction  # doctest:+SKIP
+        (-0.5773502691896257, -0.5773502691896257, -0.5773502691896257)
 
         """
         return self.GetDirectionOfProjection()
 
     def view_frustum(self, aspect=1.0):
         """Get the view frustum.
```

### Comparing `pyvista-0.39.0/pyvista/plotting/charts.py` & `pyvista-0.39.1/pyvista/plotting/charts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/colors.py` & `pyvista-0.39.1/pyvista/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/composite_mapper.py` & `pyvista-0.39.1/pyvista/plotting/composite_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -456,29 +456,29 @@
 
         >>> import pyvista as pv
         >>> dataset = pv.MultiBlock(
         ...     [pv.Cube(), pv.Sphere(center=(0, 0, 1))]
         ... )
         >>> pl = pv.Plotter()
         >>> actor, mapper = pl.add_composite(dataset)
-        >>> mapper.block_attr.get_block(0)  # doctest:+SKIP
+        >>> mapper.block_attr.get_block(0)
         MultiBlock (...)
-          N Blocks:	2
-          X Bounds:	-0.500, 0.500
-          Y Bounds:	-0.500, 0.500
-          Z Bounds:	-0.500, 1.500
+          N Blocks    2
+          X Bounds    -0.500, 0.500
+          Y Bounds    -0.500, 0.500
+          Z Bounds    -0.500, 1.500
 
         Note this is the same as using ``__getitem__``
 
-        >>> mapper.block_attr[0]  # doctest:+SKIP
-        MultiBlock (...)
-          N Blocks:	2
-          X Bounds:	-0.500, 0.500
-          Y Bounds:	-0.500, 0.500
-          Z Bounds:	-0.500, 1.500
+        >>> mapper.block_attr[0]
+        Composite Block Addr=... Attributes
+        Visible:   None
+        Opacity:   None
+        Color:     None
+        Pickable   None
 
         """
         try:
             if vtk_version_info <= (9, 0, 3):  # pragma: no cover
                 vtk_ref = _vtk.reference(0)  # needed for <=9.0.3
                 block = self.DataObjectFromIndex(index, self._dataset, vtk_ref)
             else:
@@ -565,20 +565,20 @@
         --------
         >>> import pyvista as pv
         >>> dataset = pv.MultiBlock(
         ...     [pv.Cube(), pv.Sphere(center=(0, 0, 1))]
         ... )
         >>> pl = pv.Plotter()
         >>> actor, mapper = pl.add_composite(dataset)
-        >>> mapper.dataset  # doctest:+SKIP
+        >>> mapper.dataset
         MultiBlock (...)
-          N Blocks:     2
-          X Bounds:     -0.500, 0.500
-          Y Bounds:     -0.500, 0.500
-          Z Bounds:     -0.500, 1.500
+          N Blocks    2
+          X Bounds    -0.500, 0.500
+          Y Bounds    -0.500, 0.500
+          Z Bounds    -0.500, 1.500
 
         """
         return self._dataset
 
     @property
     def block_attr(self) -> CompositeAttributes:
         """Return the block attributes.
```

### Comparing `pyvista-0.39.0/pyvista/plotting/cube_axes_actor.py` & `pyvista-0.39.1/pyvista/plotting/cube_axes_actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/export_vtkjs.py` & `pyvista-0.39.1/pyvista/plotting/export_vtkjs.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/helpers.py` & `pyvista-0.39.1/pyvista/plotting/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/lights.py` & `pyvista-0.39.1/pyvista/plotting/lights.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/lookup_table.py` & `pyvista-0.39.1/pyvista/plotting/lookup_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,42 +152,41 @@
 
     Examples
     --------
     Plot the lookup table with the default VTK color map.
 
     >>> import pyvista as pv
     >>> lut = pv.LookupTable()
-    >>> lut  # doctest:+SKIP
-    LookupTable (0x7ff3de60d580)
+    >>> lut
+    LookupTable (...)
       Table Range:                (0.0, 1.0)
       N Values:                   256
       Above Range Color:          None
       Below Range Color:          None
-      NAN Color:                  Color(name='maroon', hex='#800000ff')
+      NAN Color:                  Color(name='maroon', hex='#800000ff', opacity=255)
       Log Scale:                  False
-      Color Map:                  "VTK lookup table"
+      Color Map:                  "PyVista Lookup Table"
         Alpha Range:              (1.0, 1.0)
         Hue Range:                (0.0, 0.66667)
         Saturation Range          (1.0, 1.0)
         Value Range               (1.0, 1.0)
         Ramp                      s-curve
-        Is Opaque                 True
     >>> lut.plot()
 
     Plot the lookup table with the ``'inferno'`` color map.
 
     >>> import pyvista as pv
     >>> lut = pv.LookupTable('inferno', n_values=32)
-    >>> lut  # doctest:+SKIP
-    LookupTable (0x7ff3c053f3a0)
+    >>> lut
+    LookupTable (...)
       Table Range:                (0.0, 1.0)
       N Values:                   32
       Above Range Color:          None
       Below Range Color:          None
-      NAN Color:                  Color(name='maroon', hex='#800000ff')
+      NAN Color:                  Color(name='maroon', hex='#800000ff', opacity=255)
       Log Scale:                  False
       Color Map:                  "inferno"
     >>> lut.plot()
 
     """
 
     _nan_color_set = False
@@ -1026,16 +1025,16 @@
             VTK color transfer function.
 
         Examples
         --------
         >>> import pyvista
         >>> lut = pyvista.LookupTable()
         >>> tf = lut.to_color_tf()
-        >>> tf  # doctest:+SKIP
-        <vtkmodules.vtkRenderingCore.vtkColorTransferFunction(0x339bd40) at 0x7ffabf634700>
+        >>> tf
+        <vtkmodules.vtkRenderingCore.vtkColorTransferFunction(...) at ...>
 
         """
         color_tf = _vtk.vtkColorTransferFunction()
         mn, mx = self.scalar_range
         for ii, value in enumerate(np.linspace(mn, mx, self.n_values)):
             color_tf.AddRGBPoint(ii, *self.map_value(value, False))
         return color_tf
@@ -1049,16 +1048,16 @@
             Piecewise function of the opacity of this color table.
 
         Examples
         --------
         >>> import pyvista
         >>> lut = pyvista.LookupTable()
         >>> tf = lut.to_opacity_tf()
-        >>> tf  # doctest:+SKIP
-        <vtkmodules.vtkCommonDataModel.vtkPiecewiseFunction(0x32fa410) at 0x7fe963d6d5e0>
+        >>> tf
+        <vtkmodules.vtkCommonDataModel.vtkPiecewiseFunction(...) at ...>
 
         """
         opacity_tf = _vtk.vtkPiecewiseFunction()
         for ii, value in enumerate(self.values[:, 3]):
             opacity_tf.AddPoint(ii, value / self.n_values)
         return opacity_tf
```

### Comparing `pyvista-0.39.0/pyvista/plotting/mapper.py` & `pyvista-0.39.1/pyvista/plotting/mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,34 +126,34 @@
 
         >>> import pyvista as pv
         >>> mesh = pv.Sphere()
         >>> pl = pv.Plotter()
         >>> actor = pl.add_mesh(
         ...     mesh, scalars=mesh.points[:, 2], cmap='bwr'
         ... )
-        >>> actor.mapper.lookup_table  # doctest:+SKIP
-        LookupTable (0x7ff3be8d8c40)
+        >>> actor.mapper.lookup_table
+        LookupTable (...)
           Table Range:                (-0.5, 0.5)
           N Values:                   256
           Above Range Color:          None
           Below Range Color:          None
-          NAN Color:                  Color(name='darkgray', hex='#a9a9a9ff')
+          NAN Color:                  Color(name='darkgray', hex='#a9a9a9ff', opacity=255)
           Log Scale:                  False
-          Color Map:                  "From values array"
+          Color Map:                  "bwr"
 
         Return the lookup table of a composite dataset mapper.
 
         >>> import pyvista as pv
         >>> dataset = pv.MultiBlock(
         ...     [pv.Cube(), pv.Sphere(center=(0, 0, 1))]
         ... )
         >>> pl = pv.Plotter()
         >>> actor, mapper = pl.add_composite(dataset)
         >>> mapper.lookup_table  # doctest:+SKIP
-        <vtkmodules.vtkCommonCore.vtkLookupTable(0x2d4c6e0) at 0x7fce74a89fa0>
+        <vtkmodules.vtkCommonCore.vtkLookupTable(...) at ...>
 
         """
         return self.GetLookupTable()
 
     @lookup_table.setter
     def lookup_table(self, table):
         self.SetLookupTable(table)
```

### Comparing `pyvista-0.39.0/pyvista/plotting/opts.py` & `pyvista-0.39.1/pyvista/plotting/opts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/picking.py` & `pyvista-0.39.1/pyvista/plotting/picking.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/plotting.py` & `pyvista-0.39.1/pyvista/plotting/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -824,16 +824,16 @@
         >>> _ = plotter.add_mesh(sphere)
         >>> plotter.scalar_bars
         Scalar Bar Title     Interactive
         "Data"               False
 
         Select a scalar bar actor based on the title of the bar.
 
-        >>> plotter.scalar_bars['Data']  # doctest:+SKIP
-        (vtkmodules.vtkRenderingAnnotation.vtkScalarBarActor)0x7fcd3567ca00
+        >>> plotter.scalar_bars['Data']
+        <vtkmodules.vtkRenderingAnnotation.vtkScalarBarActor(...) at ...>
 
         """
         return self._scalar_bars
 
     @property
     def _before_close_callback(self):
         """Return the cached function (expecting a reference)."""
@@ -867,16 +867,16 @@
     def renderer(self):
         """Return the active renderer.
 
         Examples
         --------
         >>> import pyvista
         >>> pl = pyvista.Plotter()
-        >>> pl.renderer  # doctest:+SKIP
-        (Renderer)0x7f916129bfa0
+        >>> pl.renderer
+        <Renderer(...) at ...>
 
         """
         return self.renderers.active_renderer
 
     @property
     def store_image(self):
         """Store last rendered frame on close.
```

### Comparing `pyvista-0.39.0/pyvista/plotting/prop3d.py` & `pyvista-0.39.1/pyvista/plotting/prop3d.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -164,30 +164,14 @@
         """Return or set the entity orientation.
 
         Orientation is defined as the rotation from the global axes in degrees
         about the actor's x, y, and z axes.
 
         Examples
         --------
-        Show that the orientation changes with rotation.
-
-        >>> import pyvista as pv
-        >>> mesh = pv.Cube()
-        >>> pl = pv.Plotter()
-        >>> actor = pl.add_mesh(mesh)
-        >>> actor.rotate_x(90)
-        >>> actor.orientation  # doctest:+SKIP
-        (90, 0, 0)
-
-        Set the orientation directly.
-
-        >>> actor.orientation = (0, 45, 45)
-        >>> actor.orientation  # doctest:+SKIP
-        (0, 45, 45)
-
         Reorient just the actor and plot it. Note how the actor is rotated
         about its own axes as defined by its position.
 
         >>> import pyvista as pv
         >>> mesh = pv.Cube()
         >>> pl = pv.Plotter()
         >>> _ = pl.add_mesh(mesh, color='b')
@@ -199,14 +183,30 @@
         ...     lighting=False,
         ... )
         >>> actor.position = (0, 0, 1)
         >>> actor.orientation = (45, 0, 0)
         >>> pl.show_axes()
         >>> pl.show()
 
+        Show that the orientation changes with rotation.
+
+        >>> import pyvista as pv
+        >>> mesh = pv.Cube()
+        >>> pl = pv.Plotter()
+        >>> actor = pl.add_mesh(mesh)
+        >>> actor.rotate_x(90)
+        >>> actor.orientation  # doctest:+SKIP
+        (90, 0, 0)
+
+        Set the orientation directly.
+
+        >>> actor.orientation = (0, 45, 45)
+        >>> actor.orientation  # doctest:+SKIP
+        (0, 45, 45)
+
         """
         return self.GetOrientation()
 
     @orientation.setter
     def orientation(self, value: tuple):
         self.SetOrientation(value)
```

### Comparing `pyvista-0.39.0/pyvista/plotting/render_passes.py` & `pyvista-0.39.1/pyvista/plotting/render_passes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/render_window_interactor.py` & `pyvista-0.39.1/pyvista/plotting/render_window_interactor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/renderer.py` & `pyvista-0.39.1/pyvista/plotting/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2037,15 +2037,15 @@
             Lights in the renderer.
 
         Examples
         --------
         >>> import pyvista
         >>> pl = pyvista.Plotter()
         >>> pl.renderer.lights  # doctest:+SKIP
-        [<Light (Headlight) at 0x7f1dd8155820>,
+        [<Light (Headlight) at ...>,
          <Light (Camera Light) at 0x7f1dd8155760>,
          <Light (Camera Light) at 0x7f1dd8155340>,
          <Light (Camera Light) at 0x7f1dd8155460>,
          <Light (Camera Light) at 0x7f1dd8155f40>]
 
         """
         return list(self.GetLights())
```

### Comparing `pyvista-0.39.0/pyvista/plotting/renderers.py` & `pyvista-0.39.1/pyvista/plotting/renderers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/scalar_bars.py` & `pyvista-0.39.1/pyvista/plotting/scalar_bars.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/tools.py` & `pyvista-0.39.1/pyvista/plotting/tools.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/volume.py` & `pyvista-0.39.1/pyvista/plotting/volume.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/volume_property.py` & `pyvista-0.39.1/pyvista/plotting/volume_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/plotting/widgets.py` & `pyvista-0.39.1/pyvista/plotting/widgets.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/themes.py` & `pyvista-0.39.1/pyvista/themes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/trame/__init__.py` & `pyvista-0.39.1/pyvista/trame/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/trame/jupyter.py` & `pyvista-0.39.1/pyvista/trame/jupyter.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/trame/ui.py` & `pyvista-0.39.1/pyvista/trame/ui.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/trame/views.py` & `pyvista-0.39.1/pyvista/trame/views.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/__init__.py` & `pyvista-0.39.1/pyvista/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/algorithms.py` & `pyvista-0.39.1/pyvista/utilities/algorithms.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/arrays.py` & `pyvista-0.39.1/pyvista/utilities/arrays.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/cell_type_helper.py` & `pyvista-0.39.1/pyvista/utilities/cell_type_helper.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/cells.py` & `pyvista-0.39.1/pyvista/utilities/cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/common.py` & `pyvista-0.39.1/pyvista/utilities/common.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/docs.py` & `pyvista-0.39.1/pyvista/utilities/docs.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/errors.py` & `pyvista-0.39.1/pyvista/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/features.py` & `pyvista-0.39.1/pyvista/utilities/features.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/fileio.py` & `pyvista-0.39.1/pyvista/utilities/fileio.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/geometric_objects.py` & `pyvista-0.39.1/pyvista/utilities/geometric_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/helpers.py` & `pyvista-0.39.1/pyvista/utilities/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -918,39 +918,23 @@
     --------
     Wrap a numpy array representing a random point cloud.
 
     >>> import numpy as np
     >>> import pyvista
     >>> points = np.random.random((10, 3))
     >>> cloud = pyvista.wrap(points)
-    >>> cloud  # doctest:+SKIP
-    PolyData (0x7fc52db83d70)
-      N Cells:  10
-      N Points: 10
-      X Bounds: 1.123e-01, 7.457e-01
-      Y Bounds: 1.009e-01, 9.877e-01
-      Z Bounds: 2.346e-03, 9.640e-01
-      N Arrays: 0
-
-    Wrap a Trimesh object.
-
-    >>> import trimesh
-    >>> import pyvista
-    >>> points = [[0, 0, 0], [0, 0, 1], [0, 1, 0]]
-    >>> faces = [[0, 1, 2]]
-    >>> tmesh = trimesh.Trimesh(points, faces=faces, process=False)
-    >>> mesh = pyvista.wrap(tmesh)
-    >>> mesh  # doctest:+SKIP
-    PolyData (0x7fc55ff27ad0)
-      N Cells:  1
-      N Points: 3
-      X Bounds: 0.000e+00, 0.000e+00
-      Y Bounds: 0.000e+00, 1.000e+00
-      Z Bounds: 0.000e+00, 1.000e+00
-      N Arrays: 0
+    >>> cloud
+    PolyData (...)
+      N Cells:    10
+      N Points:   10
+      N Strips:   0
+      X Bounds:   ...
+      Y Bounds:   ...
+      Z Bounds:   ...
+      N Arrays:   0
 
     Wrap a VTK object.
 
     >>> import pyvista
     >>> import vtk
     >>> points = vtk.vtkPoints()
     >>> p = [1.0, 2.0, 3.0]
@@ -958,14 +942,32 @@
     >>> pid = points.InsertNextPoint(p)
     >>> _ = vertices.InsertNextCell(1)
     >>> _ = vertices.InsertCellPoint(pid)
     >>> point = vtk.vtkPolyData()
     >>> _ = point.SetPoints(points)
     >>> _ = point.SetVerts(vertices)
     >>> mesh = pyvista.wrap(point)
+    >>> mesh
+    PolyData (...)
+      N Cells:    1
+      N Points:   1
+      N Strips:   0
+      X Bounds:   1.000e+00, 1.000e+00
+      Y Bounds:   2.000e+00, 2.000e+00
+      Z Bounds:   3.000e+00, 3.000e+00
+      N Arrays:   0
+
+    Wrap a Trimesh object.
+
+    >>> import trimesh
+    >>> import pyvista
+    >>> points = [[0, 0, 0], [0, 0, 1], [0, 1, 0]]
+    >>> faces = [[0, 1, 2]]
+    >>> tmesh = trimesh.Trimesh(points, faces=faces, process=False)
+    >>> mesh = pyvista.wrap(tmesh)
     >>> mesh  # doctest:+SKIP
     PolyData (0x7fc55ff27ad0)
       N Cells:  1
       N Points: 3
       X Bounds: 0.000e+00, 0.000e+00
       Y Bounds: 0.000e+00, 1.000e+00
       Z Bounds: 0.000e+00, 1.000e+00
```

### Comparing `pyvista-0.39.0/pyvista/utilities/misc.py` & `pyvista-0.39.1/pyvista/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/parametric_objects.py` & `pyvista-0.39.1/pyvista/utilities/parametric_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/reader.py` & `pyvista-0.39.1/pyvista/utilities/reader.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/regression.py` & `pyvista-0.39.1/pyvista/utilities/regression.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/sphinx_gallery.py` & `pyvista-0.39.1/pyvista/utilities/sphinx_gallery.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,13 +51,14 @@
         image_names = list()
         image_path_iterator = block_vars["image_path_iterator"]
         figures = pyvista.plotting._ALL_PLOTTERS
         for _, plotter in figures.items():
             fname = next(image_path_iterator)
             if hasattr(plotter, '_gif_filename'):
                 # move gif to fname
+                fname = fname[:-3] + "gif"
                 shutil.move(plotter._gif_filename, fname)
             else:
                 plotter.screenshot(fname)
             image_names.append(fname)
         pyvista.close_all()  # close and clear all plotters
         return figure_rst(image_names, gallery_conf["src_dir"])
```

### Comparing `pyvista-0.39.0/pyvista/utilities/transformations.py` & `pyvista-0.39.1/pyvista/utilities/transformations.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/wrappers.py` & `pyvista-0.39.1/pyvista/utilities/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista/utilities/xvfb.py` & `pyvista-0.39.1/pyvista/utilities/xvfb.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista.egg-info/PKG-INFO` & `pyvista-0.39.1/pyvista.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvista
-Version: 0.39.0
+Version: 0.39.1
 Summary: Easier Pythonic interface to VTK
 Author-email: PyVista Developers <info@pyvista.org>
 License: MIT
 Project-URL: Documentation, https://docs.pyvista.org/
 Project-URL: Bug Tracker, https://github.com/pyvista/pyvista/issues
 Project-URL: Source Code, https://github.com/pyvista/pyvista
 Keywords: vtk,numpy,plotting,mesh
```

### Comparing `pyvista-0.39.0/pyvista.egg-info/SOURCES.txt` & `pyvista-0.39.1/pyvista.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/pyvista.egg-info/requires.txt` & `pyvista-0.39.1/pyvista.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_actor.py` & `pyvista-0.39.1/tests/test_actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_axes.py` & `pyvista-0.39.1/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_camera.py` & `pyvista-0.39.1/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_cells.py` & `pyvista-0.39.1/tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_charts.py` & `pyvista-0.39.1/tests/test_charts.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_composite.py` & `pyvista-0.39.1/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_cube_axes_actor.py` & `pyvista-0.39.1/tests/test_cube_axes_actor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_dataobject.py` & `pyvista-0.39.1/tests/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_dataset.py` & `pyvista-0.39.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_datasetattributes.py` & `pyvista-0.39.1/tests/test_datasetattributes.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_demos.py` & `pyvista-0.39.1/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_export.py` & `pyvista-0.39.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_filters.py` & `pyvista-0.39.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_geometric_objects.py` & `pyvista-0.39.1/tests/test_geometric_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_grid.py` & `pyvista-0.39.1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_helpers.py` & `pyvista-0.39.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_imaging.py` & `pyvista-0.39.1/tests/test_imaging.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_init.py` & `pyvista-0.39.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_lights.py` & `pyvista-0.39.1/tests/test_lights.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_lookup_table.py` & `pyvista-0.39.1/tests/test_lookup_table.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_meshio.py` & `pyvista-0.39.1/tests/test_meshio.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_objects.py` & `pyvista-0.39.1/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_parametric_geometry.py` & `pyvista-0.39.1/tests/test_parametric_geometry.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_picking.py` & `pyvista-0.39.1/tests/test_picking.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_plotter.py` & `pyvista-0.39.1/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_pointset.py` & `pyvista-0.39.1/tests/test_pointset.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_polydata.py` & `pyvista-0.39.1/tests/test_polydata.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,24 @@
     assert merged.n_points == sphere.n_points + sphere_shifted.n_points
 
     # test in-place merge
     mesh = sphere.copy()
     merged = mesh.merge(sphere_shifted, inplace=True)
     assert merged is mesh
 
+    # test merge with lines
+    arc_1 = pyvista.CircularArc([0, 0, 0], [10, 10, 0], [10, 0, 0], negative=False, resolution=3)
+    arc_2 = pyvista.CircularArc([10, 10, 0], [20, 0, 0], [10, 0, 0], negative=False, resolution=3)
+    merged = arc_1 + arc_2
+    assert merged.n_lines == 2
+
+    # test merge with lines as iterable
+    merged = arc_1.merge((arc_2, arc_2))
+    assert merged.n_lines == 3
+
     # test main_has_priority
     mesh = sphere.copy()
     data_main = np.arange(mesh.n_points, dtype=float)
     mesh.point_data['present_in_both'] = data_main
     other = mesh.copy()
     data_other = -data_main
     other.point_data['present_in_both'] = data_other
```

### Comparing `pyvista-0.39.0/tests/test_property.py` & `pyvista-0.39.1/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_pyvista_ndarray.py` & `pyvista-0.39.1/tests/test_pyvista_ndarray.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_regression.py` & `pyvista-0.39.1/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_render_pass.py` & `pyvista-0.39.1/tests/test_render_pass.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_render_window_interactor.py` & `pyvista-0.39.1/tests/test_render_window_interactor.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_renderer.py` & `pyvista-0.39.1/tests/test_renderer.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_scalar_bars.py` & `pyvista-0.39.1/tests/test_scalar_bars.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_scraper.py` & `pyvista-0.39.1/tests/test_scraper.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,31 +14,45 @@
 
 @pytest.mark.parametrize('n_win', [1, 2])
 def test_scraper(tmpdir, monkeypatch, n_win):
     pytest.importorskip('sphinx_gallery')
     monkeypatch.setattr(pyvista, 'BUILDING_GALLERY', True)
     pyvista.close_all()
     plotters = [pyvista.Plotter(off_screen=True) for _ in range(n_win)]
+    plotter_gif = pyvista.Plotter()
+
     scraper = Scraper()
     src_dir = str(tmpdir)
     out_dir = op.join(str(tmpdir), '_build', 'html')
+
     img_fnames = [
         op.join(src_dir, 'auto_examples', 'images', f'sg_img_{n}.png') for n in range(n_win)
     ]
+
+    # create and save GIF to tmpdir
+    gif_path = op.abspath(tmpdir + 'sg_img_0.gif')
+    plotter_gif.open_gif(gif_path)
+    plotter_gif.write_frame()
+    plotter_gif.close()
+
     gallery_conf = {"src_dir": src_dir, "builder_name": "html"}
     target_file = op.join(src_dir, 'auto_examples', 'sg.py')
     block = None
     block_vars = dict(
         image_path_iterator=iter(img_fnames),
         example_globals=dict(a=1),
         target_file=target_file,
     )
+
     os.makedirs(op.dirname(img_fnames[0]))
     for img_fname in img_fnames:
         assert not os.path.isfile(img_fname)
+
+    # add gif to list after checking other filenames are empty
+    img_fnames.append(gif_path)
     os.makedirs(out_dir)
     scraper(block, block_vars, gallery_conf)
     for img_fname in img_fnames:
         assert os.path.isfile(img_fname)
     for plotter in plotters:
         plotter.close()
```

### Comparing `pyvista-0.39.0/tests/test_texture.py` & `pyvista-0.39.1/tests/test_texture.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     assert not np.allclose(flipped.to_array(), texture.to_array())
 
 
 def test_texture_repr(texture):
     tex_repr = repr(texture)
     assert 'Components:   3' in tex_repr
     assert 'Cube Map:     False' in tex_repr
-    assert 'Dimensions:   300, 200\n' in tex_repr
+    assert 'Dimensions:   300, 200' in tex_repr
 
 
 def test_interpolate(texture):
     assert isinstance(texture.interpolate, bool)
     for value in [True, False]:
         texture.interpolate = value
         assert texture.interpolate is value
```

### Comparing `pyvista-0.39.0/tests/test_theme.py` & `pyvista-0.39.1/tests/test_theme.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_tinypages.py` & `pyvista-0.39.1/tests/test_tinypages.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_utilities.py` & `pyvista-0.39.1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pyvista-0.39.0/tests/test_volume_property.py` & `pyvista-0.39.1/tests/test_volume_property.py`

 * *Files identical despite different names*

