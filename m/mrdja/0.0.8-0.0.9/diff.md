# Comparing `tmp/mrdja-0.0.8.tar.gz` & `tmp/mrdja-0.0.9.tar.gz`

## Comparing `mrdja-0.0.8.tar` & `mrdja-0.0.9.tar`

### file list

```diff
@@ -1,77 +1,12 @@
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 mrdja-0.0.8/test.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 mrdja-0.0.8/test2.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.buildinfo
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/genindex.html
--rw-r--r--   0        0        0     9201 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/index.html
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/objects.inv
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/py-modindex.html
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/search.html
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/searchindex.js
--rw-r--r--   0        0        0    28410 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/environment.pickle
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/index.doctree
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/sampling.doctree
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sample_point_circle_2d.doctree
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sample_point_circle_3d_rejection.doctree
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sample_point_cuboid.doctree
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sample_point_parallelogram.doctree
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sample_point_sphere.doctree
--rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sampling_circle_2d.doctree
--rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sampling_circle_3d_rejection.doctree
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sampling_cuboid.doctree
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sampling_parallelogram_2d.doctree
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/.doctrees/api/sampling.sampling_sphere.doctree
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_modules/index.html
--rw-r--r--   0        0        0    23821 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_modules/sampling.html
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/index.rst.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sample_point_circle_2d.rst.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sample_point_circle_3d_rejection.rst.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sample_point_cuboid.rst.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sample_point_parallelogram.rst.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sample_point_sphere.rst.txt
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sampling_circle_2d.rst.txt
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sampling_circle_3d_rejection.rst.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sampling_cuboid.rst.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sampling_parallelogram_2d.rst.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_sources/api/sampling.sampling_sphere.rst.txt
--rw-r--r--   0        0        0    14667 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/basic.css
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/classic.css
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/doctools.js
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/file.png
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/graphviz.css
--rw-r--r--   0        0        0   288550 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/jquery.js
--rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/plus.png
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/pygments.css
--rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/searchtools.js
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/sidebar.js
--rw-r--r--   0        0        0    68398 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/_static/underscore.js
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sample_point_circle_2d.html
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sample_point_circle_3d_rejection.html
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sample_point_cuboid.html
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sample_point_parallelogram.html
--rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sample_point_sphere.html
--rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sampling_circle_2d.html
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sampling_circle_3d_rejection.html
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sampling_cuboid.html
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sampling_parallelogram_2d.html
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/build/api/sampling.sampling_sphere.html
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/conf.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/index.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sample_point_circle_2d.rst
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sample_point_circle_3d_rejection.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sample_point_cuboid.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sample_point_parallelogram.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sample_point_sphere.rst
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sampling_circle_2d.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sampling_circle_3d_rejection.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sampling_cuboid.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sampling_parallelogram_2d.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 mrdja-0.0.8/doc/source/api/sampling.sampling_sphere.rst
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mrdja-0.0.8/mrdja/sampling/__init__.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 mrdja-0.0.8/mrdja/sampling/sampling.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 mrdja-0.0.8/.gitignore
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 mrdja-0.0.8/README.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 mrdja-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 mrdja-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 mrdja-0.0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 mrdja-0.0.9/test.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 mrdja-0.0.9/test2.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mrdja-0.0.9/doc/requirements.txt
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 mrdja-0.0.9/doc/source/conf.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 mrdja-0.0.9/doc/source/index.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mrdja-0.0.9/mrdja/sampling/__init__.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 mrdja-0.0.9/mrdja/sampling/sampling.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 mrdja-0.0.9/.gitignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mrdja-0.0.9/README.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 mrdja-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 mrdja-0.0.9/PKG-INFO
```

### Comparing `mrdja-0.0.8/test.py` & `mrdja-0.0.9/test.py`

 * *Files identical despite different names*

### Comparing `mrdja-0.0.8/test2.py` & `mrdja-0.0.9/test2.py`

 * *Files identical despite different names*

### Comparing `mrdja-0.0.8/doc/source/conf.py` & `mrdja-0.0.9/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 # extensions = ['sphinx.ext.autodoc', 'sphinx_automodapi.automodapi']
-extensions = ['sphinx.ext.todo', 'sphinx.ext.viewcode', 'sphinx.ext.autodoc', 'sphinx.ext.imgmath', 'sphinx.ext.autosummary', 'numpydoc', 'sphinx_automodapi.automodapi']
+extensions = ['sphinx.ext.todo', 'sphinx.ext.viewcode', 'sphinx.ext.autodoc', 'sphinx.ext.imgmath', 'sphinx.ext.autosummary', 'sphinx_automodapi.automodapi']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
```

### Comparing `mrdja-0.0.8/mrdja/sampling/sampling.py` & `mrdja-0.0.9/mrdja/sampling/sampling.py`

 * *Files identical despite different names*

### Comparing `mrdja-0.0.8/pyproject.toml` & `mrdja-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mrdja"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="José María Martínez Otzeta", email="jmartinezot@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,7 +16,10 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/mrdja"
 "Bug Tracker" = "https://github.com/pypa/mrdja/issues"
+
+[tool.poetry.dependencies]
+sphinx-automodapi = "*"
```

