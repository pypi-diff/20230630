# Comparing `tmp/pyfds-0.1.6.tar.gz` & `tmp/pyfds-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfds-0.1.6.tar", last modified: Thu Mar 30 12:41:33 2023, max compression
+gzip compressed data, was "pyfds-0.2.0.tar", last modified: Fri Jun 30 08:52:36 2023, max compression
```

## Comparing `pyfds-0.1.6.tar` & `pyfds-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-03-30 12:41:33.710306 pyfds-0.1.6/
--rwxrwx---   0 leanderc (50967) user     (10000)     2194 2017-01-02 12:00:53.000000 pyfds-0.1.6/.gitignore
--rwxrwx---   0 leanderc (50967) user     (10000)      118 2021-10-20 12:26:35.000000 pyfds-0.1.6/AUTHORS.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     2145 2023-03-30 12:32:22.000000 pyfds-0.1.6/CHANGELOG.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     1477 2017-05-16 12:52:30.000000 pyfds-0.1.6/LICENSE
--rwxrwx---   0 leanderc (50967) user     (10000)     1144 2023-03-30 12:41:33.708215 pyfds-0.1.6/PKG-INFO
--rwxrwx---   0 leanderc (50967) user     (10000)      641 2023-03-30 12:28:36.000000 pyfds-0.1.6/README.rst
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-03-30 12:41:33.573302 pyfds-0.1.6/doc/
--rwxrwx---   0 leanderc (50967) user     (10000)       79 2023-03-30 12:24:43.000000 pyfds-0.1.6/doc/acoustic_flow.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       67 2017-02-02 09:31:23.000000 pyfds-0.1.6/doc/acoustics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     2305 2021-10-20 12:31:28.000000 pyfds-0.1.6/doc/conf.py
--rwxrwx---   0 leanderc (50967) user     (10000)       82 2021-12-20 08:34:47.000000 pyfds-0.1.6/doc/electrostatics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     3790 2017-06-13 12:30:59.000000 pyfds-0.1.6/doc/ex_acoustics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     3339 2017-06-12 15:06:37.000000 pyfds-0.1.6/doc/ex_visualization.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       78 2017-06-08 09:07:55.000000 pyfds-0.1.6/doc/examples.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       58 2017-01-02 09:14:37.000000 pyfds-0.1.6/doc/fields.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       49 2017-02-02 09:31:55.000000 pyfds-0.1.6/doc/gfx.rst
--rwxrwx---   0 leanderc (50967) user     (10000)      440 2023-03-30 12:25:41.000000 pyfds-0.1.6/doc/index.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       97 2017-06-06 12:12:26.000000 pyfds-0.1.6/doc/nonlinear_acoustics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       61 2017-02-02 09:30:58.000000 pyfds-0.1.6/doc/regions.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       61 2021-12-20 08:34:52.000000 pyfds-0.1.6/doc/thermal.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     8935 2021-10-20 12:13:52.000000 pyfds-0.1.6/doc/usage.rst
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-03-30 12:41:33.640815 pyfds-0.1.6/pyfds/
--rwxrwx---   0 leanderc (50967) user     (10000)      469 2023-03-30 09:43:26.000000 pyfds-0.1.6/pyfds/__init__.py
--rwxrwx---   0 leanderc (50967) user     (10000)     2140 2023-03-30 12:06:55.000000 pyfds-0.1.6/pyfds/acoustic_flow.py
--rwxrwx---   0 leanderc (50967) user     (10000)    12646 2021-05-10 14:29:33.000000 pyfds-0.1.6/pyfds/acoustics.py
--rwxrwx---   0 leanderc (50967) user     (10000)     4791 2023-03-22 07:43:55.000000 pyfds-0.1.6/pyfds/electrostatics.py
--rwxrwx---   0 leanderc (50967) user     (10000)    23330 2021-05-10 15:01:18.000000 pyfds-0.1.6/pyfds/fields.py
--rwxrwx---   0 leanderc (50967) user     (10000)    17009 2022-01-04 14:59:51.000000 pyfds-0.1.6/pyfds/gfx.py
--rwxrwx---   0 leanderc (50967) user     (10000)     8130 2021-05-10 14:29:52.000000 pyfds-0.1.6/pyfds/nonlinear_acoustics.py
--rwxrwx---   0 leanderc (50967) user     (10000)     4586 2019-06-28 08:41:13.000000 pyfds-0.1.6/pyfds/regions.py
--rwxrwx---   0 leanderc (50967) user     (10000)     8211 2023-03-30 07:45:05.000000 pyfds-0.1.6/pyfds/thermal.py
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-03-30 12:41:33.677605 pyfds-0.1.6/pyfds.egg-info/
--rwxrwx---   0 leanderc (50967) user     (10000)     1144 2023-03-30 12:41:33.000000 pyfds-0.1.6/pyfds.egg-info/PKG-INFO
--rwxrwx---   0 leanderc (50967) user     (10000)      701 2023-03-30 12:41:33.000000 pyfds-0.1.6/pyfds.egg-info/SOURCES.txt
--rwxrwx---   0 leanderc (50967) user     (10000)        1 2023-03-30 12:41:33.000000 pyfds-0.1.6/pyfds.egg-info/dependency_links.txt
--rwxrwx---   0 leanderc (50967) user     (10000)       23 2023-03-30 12:41:33.000000 pyfds-0.1.6/pyfds.egg-info/requires.txt
--rwxrwx---   0 leanderc (50967) user     (10000)        6 2023-03-30 12:41:33.000000 pyfds-0.1.6/pyfds.egg-info/top_level.txt
--rwxrwx---   0 leanderc (50967) user     (10000)       38 2023-03-30 12:41:33.712033 pyfds-0.1.6/setup.cfg
--rwxrwx---   0 leanderc (50967) user     (10000)     1260 2017-05-16 13:10:15.000000 pyfds-0.1.6/setup.py
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-03-30 12:41:33.700406 pyfds-0.1.6/test/
--rwxrwx---   0 leanderc (50967) user     (10000)     3680 2018-07-16 14:29:17.000000 pyfds-0.1.6/test/test_acoustics.py
--rwxrwx---   0 leanderc (50967) user     (10000)     5668 2017-02-02 09:13:26.000000 pyfds-0.1.6/test/test_fields.py
--rwxrwx---   0 leanderc (50967) user     (10000)      286 2017-02-02 09:14:25.000000 pyfds-0.1.6/test/test_regions.py
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.700352 pyfds-0.2.0/
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.370438 pyfds-0.2.0/.github/
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.440495 pyfds-0.2.0/.github/workflows/
+-rwxrwx---   0 leanderc (50967) user     (10000)     1321 2023-06-30 08:00:31.000000 pyfds-0.2.0/.github/workflows/python-package.yml
+-rwxrwx---   0 leanderc (50967) user     (10000)     2194 2017-01-02 12:00:53.000000 pyfds-0.2.0/.gitignore
+-rwxrwx---   0 leanderc (50967) user     (10000)      118 2021-10-20 12:26:35.000000 pyfds-0.2.0/AUTHORS.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     2476 2023-06-30 08:29:53.000000 pyfds-0.2.0/CHANGELOG.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     1477 2017-05-16 12:52:30.000000 pyfds-0.2.0/LICENSE
+-rwxrwx---   0 leanderc (50967) user     (10000)     3108 2023-06-30 08:52:36.697927 pyfds-0.2.0/PKG-INFO
+-rwxrwx---   0 leanderc (50967) user     (10000)      641 2023-03-30 12:28:36.000000 pyfds-0.2.0/README.rst
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.548937 pyfds-0.2.0/doc/
+-rwxrwx---   0 leanderc (50967) user     (10000)       79 2023-03-30 12:24:43.000000 pyfds-0.2.0/doc/acoustic_flow.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       67 2017-02-02 09:31:23.000000 pyfds-0.2.0/doc/acoustics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     2551 2023-06-30 07:07:46.000000 pyfds-0.2.0/doc/conf.py
+-rwxrwx---   0 leanderc (50967) user     (10000)       82 2021-12-20 08:34:47.000000 pyfds-0.2.0/doc/electrostatics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     3790 2017-06-13 12:30:59.000000 pyfds-0.2.0/doc/ex_acoustics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     3339 2017-06-12 15:06:37.000000 pyfds-0.2.0/doc/ex_visualization.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       78 2017-06-08 09:07:55.000000 pyfds-0.2.0/doc/examples.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       58 2017-01-02 09:14:37.000000 pyfds-0.2.0/doc/fields.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       49 2017-02-02 09:31:55.000000 pyfds-0.2.0/doc/gfx.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)      440 2023-06-29 15:37:34.000000 pyfds-0.2.0/doc/index.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       97 2017-06-06 12:12:26.000000 pyfds-0.2.0/doc/nonlinear_acoustics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       61 2017-02-02 09:30:58.000000 pyfds-0.2.0/doc/regions.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       61 2021-12-20 08:34:52.000000 pyfds-0.2.0/doc/thermal.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     8935 2021-10-20 12:13:52.000000 pyfds-0.2.0/doc/usage.rst
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.623709 pyfds-0.2.0/pyfds/
+-rwxrwx---   0 leanderc (50967) user     (10000)      469 2023-06-07 14:22:40.000000 pyfds-0.2.0/pyfds/__init__.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     2140 2023-06-07 14:42:38.000000 pyfds-0.2.0/pyfds/acoustic_flow.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    12683 2023-06-07 14:42:36.000000 pyfds-0.2.0/pyfds/acoustics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     4793 2023-06-07 14:52:41.000000 pyfds-0.2.0/pyfds/electrostatics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    24599 2023-06-29 15:28:24.000000 pyfds-0.2.0/pyfds/fields.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    17365 2023-06-30 07:22:59.000000 pyfds-0.2.0/pyfds/gfx.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     8125 2023-06-30 06:47:34.000000 pyfds-0.2.0/pyfds/nonlinear_acoustics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     5127 2023-06-07 14:45:45.000000 pyfds-0.2.0/pyfds/regions.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     8213 2023-06-07 14:45:55.000000 pyfds-0.2.0/pyfds/thermal.py
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.664885 pyfds-0.2.0/pyfds.egg-info/
+-rwxrwx---   0 leanderc (50967) user     (10000)     3108 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/PKG-INFO
+-rwxrwx---   0 leanderc (50967) user     (10000)      753 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/SOURCES.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)        1 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/dependency_links.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)       84 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/requires.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)        6 2023-06-30 08:52:36.000000 pyfds-0.2.0/pyfds.egg-info/top_level.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)     1032 2023-06-29 15:49:48.000000 pyfds-0.2.0/pyproject.toml
+-rwxrwx---   0 leanderc (50967) user     (10000)       38 2023-06-30 08:52:36.701856 pyfds-0.2.0/setup.cfg
+-rwxrwx---   0 leanderc (50967) user     (10000)     1261 2023-06-29 15:48:20.000000 pyfds-0.2.0/setup.py
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2023-06-30 08:52:36.689468 pyfds-0.2.0/test/
+-rwxrwx---   0 leanderc (50967) user     (10000)     3700 2023-06-30 07:12:49.000000 pyfds-0.2.0/test/test_acoustics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     6098 2023-06-30 08:21:57.000000 pyfds-0.2.0/test/test_fields.py
+-rwxrwx---   0 leanderc (50967) user     (10000)      286 2017-02-02 09:14:25.000000 pyfds-0.2.0/test/test_regions.py
```

### Comparing `pyfds-0.1.6/.gitignore` & `pyfds-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfds-0.1.6/CHANGELOG.rst` & `pyfds-0.2.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,35 @@
 This project follows the guidelines of `Keep a changelog`_ and adheres to
 `Semantic versioning`_.
 
 .. _Keep a changelog: http://keepachangelog.com/
 .. _Semantic versioning: https://semver.org/
 
 
+`Unreleased`_
+=============
+
+
+`0.2.0`_ - 2023-06-30
+=====================
+
+Added
+-----
+* Support for elliptic regions.
+
+Fixed
+-----
+* Code style and documentation issues.
+* Boundary test cases.
+
+Changed
+-------
+* From setup.py to pyproject.toml.
+
+
 `0.1.6`_ - 2023-03-30
 =====================
 
 Added
 -----
 * Acoustic simulation with moving medium.
 * Asymmetric scaling for animations.
@@ -94,14 +115,15 @@
 
 Added
 -----
 * First preview release.
 
 
 .. _Unreleased: https://github.com/emtpb/pyfds
+.. _0.2.0: https://github.com/emtpb/pyfds/releases/tag/0.2.0
 .. _0.1.6: https://github.com/emtpb/pyfds/releases/tag/0.1.6
 .. _0.1.5: https://github.com/emtpb/pyfds/releases/tag/0.1.5
 .. _0.1.4: https://github.com/emtpb/pyfds/releases/tag/0.1.4
 .. _0.1.3: https://github.com/emtpb/pyfds/releases/tag/0.1.3
 .. _0.1.2: https://github.com/emtpb/pyfds/releases/tag/0.1.2
 .. _0.1.1: https://github.com/emtpb/pyfds/releases/tag/0.1.1
 .. _0.1.0: https://github.com/emtpb/pyfds/releases/tag/0.1.0
```

### Comparing `pyfds-0.1.6/LICENSE` & `pyfds-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfds-0.1.6/README.rst` & `pyfds-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.1.6/doc/conf.py` & `pyfds-0.2.0/doc/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,30 +23,38 @@
 napoleon_numpy_docstring = False
 napoleon_use_ivar = True
 napoleon_use_param = True
 napoleon_use_rtype = True
 napoleon_use_admonition_for_examples = True
 napoleon_use_admonition_for_notes = True
 napoleon_use_admonition_for_references = True
+napoleon_custom_sections = [('Returns', 'params_style')]
 
 # Configure remote documenation via intersphinx
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'numpy': ('https://docs.scipy.org/doc/numpy/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
 }
 
 templates_path = ['_templates']
 source_suffix = '.rst'
 master_doc = 'index'
-language = None
+language = 'en'
 today_fmt = '%Y-%m-%d'
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 pygments_style = 'sphinx'
 todo_include_todos = False
+autodoc_default_options = {
+    'members': True,
+    'member-order': 'bysource',
+    'special-members': '__init__',
+    'undoc-members': True,
+    'exclude-members': '__weakref__'
+}
 
 # -- Project-specific configuration
 
 project = 'pyfds'
 description = 'Modular field simulation tool using finite differences.'
 author = 'Leander Claes'
 copyright = '{year}, {author}'.format(year=datetime.date.today().year,
@@ -65,13 +73,13 @@
     '**': ['about.html', 'navigation.html', 'searchbox.html']
 }
 htmlhelp_basename = '{0}doc'.format(project)
 
 # -- Options for LaTeX output
 
 latex_elements = {
-     'papersize': 'a4paper',
+    'papersize': 'a4paper',
 }
 latex_documents = [
     (master_doc, '{0}.tex'.format(project_without_spaces),
      '{0} Documentation'.format(project), author, 'manual'),
 ]
```

### Comparing `pyfds-0.1.6/doc/ex_acoustics.rst` & `pyfds-0.2.0/doc/ex_acoustics.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.1.6/doc/ex_visualization.rst` & `pyfds-0.2.0/doc/ex_visualization.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.1.6/doc/usage.rst` & `pyfds-0.2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.1.6/pyfds/acoustic_flow.py` & `pyfds-0.2.0/pyfds/acoustic_flow.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.1.6/pyfds/acoustics.py` & `pyfds-0.2.0/pyfds/acoustics.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,48 +19,48 @@
         self.a_p_v = None
         self.a_v_p = None
         self.a_v_v = None
 
     def assemble_matrices(self):
         """Assemble the a_* matrices required for simulation."""
 
-        self.a_p_v = self.d_x(factors=(self.t.increment / self.x.increment *
-                                       self.material_vector('sound_velocity') ** 2 *
-                                       self.material_vector('density')))
-        self.a_v_p = self.d_x(factors=(self.t.increment / self.x.increment /
-                                       self.material_vector('density')), variant='backward')
-        self.a_v_v = self.d_x2(factors=(self.t.increment / self.x.increment ** 2 *
-                                        self.material_vector('absorption_coef') /
-                                        self.material_vector('density')))
+        self.a_p_v = self.d_x(factors=(self.t.increment / self.x.increment
+                                       * self.material_vector('sound_velocity') ** 2
+                                       * self.material_vector('density')))
+        self.a_v_p = self.d_x(factors=(self.t.increment / self.x.increment
+                                       / self.material_vector('density')), variant='backward')
+        self.a_v_v = self.d_x2(factors=(self.t.increment / self.x.increment ** 2
+                                        * self.material_vector('absorption_coef')
+                                        / self.material_vector('density')))
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.pressure.apply_bounds(self.step)
         self.pressure.write_outputs()
 
-        self.velocity.values -= (self.a_v_p.dot(self.pressure.values) -
-                                 self.a_v_v.dot(self.velocity.values))
+        self.velocity.values -= (self.a_v_p.dot(self.pressure.values)
+                                 - self.a_v_v.dot(self.velocity.values))
 
         self.velocity.apply_bounds(self.step)
         self.velocity.write_outputs()
 
         self.pressure.values -= self.a_p_v.dot(self.velocity.values)
 
     def is_stable(self):
         """Checks if simulation satisfies stability conditions. Does not account for instability
         due to high absorption and includes a little headroom (1%).
 
         Returns:
             True if stable, False if not.
         """
 
-        return np.all(self.material_vector('sound_velocity') <
-                      0.99 * self.x.increment / self.t.increment)
+        return np.all(self.material_vector('sound_velocity')
+                      < 0.99 * self.x.increment / self.t.increment)
 
 
 class Acoustic2D(fld.Field2D):
     """Class for simulation of two-dimensional acoustic fields."""
 
     def __init__(self, *args, **kwargs):
         """Class constructor.
@@ -81,62 +81,62 @@
         self.a_vy_p = None
         self.a_vx_vx = None
         self.a_vy_vy = None
 
     def assemble_matrices(self):
         """Assemble the a_* matrices required for simulation."""
 
-        self.a_p_vx = self.d_x(factors=(self.t.increment / self.x.increment *
-                                        self.material_vector('sound_velocity') ** 2 *
-                                        self.material_vector('density')))
-        self.a_p_vy = self.d_y(factors=(self.t.increment / self.y.increment *
-                                        self.material_vector('sound_velocity') ** 2 *
-                                        self.material_vector('density')))
-        self.a_vx_p = self.d_x(factors=(self.t.increment / self.x.increment /
-                                        self.material_vector('density')), variant='backward')
-        self.a_vy_p = self.d_y(factors=(self.t.increment / self.y.increment /
-                                        self.material_vector('density')), variant='backward')
-        self.a_vx_vx = (self.d_x2(factors=(self.t.increment / self.x.increment ** 2 *
-                                           self.material_vector('absorption_coef') /
-                                           self.material_vector('density'))) +
-                        self.d_y2(factors=(self.t.increment / self.y.increment ** 2 *
-                                           self.material_vector('absorption_coef') /
-                                           self.material_vector('density')))).todia()
+        self.a_p_vx = self.d_x(factors=(self.t.increment / self.x.increment
+                                        * self.material_vector('sound_velocity') ** 2
+                                        * self.material_vector('density')))
+        self.a_p_vy = self.d_y(factors=(self.t.increment / self.y.increment
+                                        * self.material_vector('sound_velocity') ** 2
+                                        * self.material_vector('density')))
+        self.a_vx_p = self.d_x(factors=(self.t.increment / self.x.increment
+                                        / self.material_vector('density')), variant='backward')
+        self.a_vy_p = self.d_y(factors=(self.t.increment / self.y.increment
+                                        / self.material_vector('density')), variant='backward')
+        self.a_vx_vx = (self.d_x2(factors=(self.t.increment / self.x.increment ** 2
+                                           * self.material_vector('absorption_coef')
+                                           / self.material_vector('density')))
+                        + self.d_y2(factors=(self.t.increment / self.y.increment ** 2
+                                             * self.material_vector('absorption_coef')
+                                             / self.material_vector('density')))).todia()
         self.a_vy_vy = self.a_vx_vx
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.pressure.apply_bounds(self.step)
         self.pressure.write_outputs()
 
-        self.velocity_x.values -= (self.a_vx_p.dot(self.pressure.values) -
-                                   self.a_vx_vx.dot(self.velocity_x.values))
-        self.velocity_y.values -= (self.a_vy_p.dot(self.pressure.values) -
-                                   self.a_vy_vy.dot(self.velocity_y.values))
+        self.velocity_x.values -= (self.a_vx_p.dot(self.pressure.values)
+                                   - self.a_vx_vx.dot(self.velocity_x.values))
+        self.velocity_y.values -= (self.a_vy_p.dot(self.pressure.values)
+                                   - self.a_vy_vy.dot(self.velocity_y.values))
 
         self.velocity_x.apply_bounds(self.step)
         self.velocity_x.write_outputs()
         self.velocity_y.apply_bounds(self.step)
         self.velocity_y.write_outputs()
 
-        self.pressure.values -= (self.a_p_vx.dot(self.velocity_x.values) +
-                                 self.a_p_vy.dot(self.velocity_y.values))
+        self.pressure.values -= (self.a_p_vx.dot(self.velocity_x.values)
+                                 + self.a_p_vy.dot(self.velocity_y.values))
 
     def is_stable(self):
         """Checks if simulation satisfies stability conditions. Does not account for instability
         due to high absorption and includes a little headroom (1%).
 
         Returns:
             True if stable, False if not.
         """
 
-        return np.all(self.material_vector('sound_velocity') <
-                      0.99 * min(self.x.increment, self.y.increment) / self.t.increment)
+        return np.all(self.material_vector('sound_velocity')
+                      < 0.99 * min(self.x.increment, self.y.increment) / self.t.increment)
 
 
 class Acoustic3DAxi(fld.Field2D):
     """Class for simulation of three-dimensional, axial-symmetric acoustic fields. Note the x is
     the radial direction, and y is the z direction."""
 
     def __init__(self, *args, **kwargs):
@@ -165,75 +165,75 @@
         symmetric fields, this is the radius, which is required to formulate the differential
         operators.
 
         Returns
             Radius of each velocity point.
         """
 
-        return np.tile(self.x.vector, self.y.samples) + self.x.increment/2
+        return np.tile(self.x.vector, self.y.samples) + self.x.increment / 2
 
     def assemble_matrices(self):
         """Assemble the a_* matrices required for simulation."""
 
-        self.a_p_vx = self.d_x(factors=(self.t.increment / self.x.increment *
-                                        self.material_vector('sound_velocity') ** 2 *
-                                        self.material_vector('density') /
-                                        self._radii()))
-        self.a_p_vy = self.d_y(factors=(self.t.increment / self.y.increment *
-                                        self.material_vector('sound_velocity') ** 2 *
-                                        self.material_vector('density')))
-        self.a_vx_p = self.d_x(factors=(self.t.increment / self.x.increment /
-                                        self.material_vector('density')), variant='backward')
-        self.a_vy_p = self.d_y(factors=(self.t.increment / self.y.increment /
-                                        self.material_vector('density')), variant='backward')
-        self.a_vx_vx = (self.d_x2(factors=(self.t.increment / self.x.increment ** 2 *
-                                           self.material_vector('absorption_coef') /
-                                           self.material_vector('density'))) +
-                        self.d_y2(factors=(self.t.increment / self.y.increment ** 2 *
-                                           self.material_vector('absorption_coef') /
-                                           self.material_vector('density'))) +
-                        self.d_x(factors=(self.t.increment / self.x.increment *
-                                          self.material_vector('absorption_coef') /
-                                          self.material_vector('density') / self._radii()),
-                                 variant='central')).todia()
+        self.a_p_vx = self.d_x(factors=(self.t.increment / self.x.increment
+                                        * self.material_vector('sound_velocity') ** 2
+                                        * self.material_vector('density')
+                                        / self._radii()))
+        self.a_p_vy = self.d_y(factors=(self.t.increment / self.y.increment
+                                        * self.material_vector('sound_velocity') ** 2
+                                        * self.material_vector('density')))
+        self.a_vx_p = self.d_x(factors=(self.t.increment / self.x.increment
+                                        / self.material_vector('density')), variant='backward')
+        self.a_vy_p = self.d_y(factors=(self.t.increment / self.y.increment
+                                        / self.material_vector('density')), variant='backward')
+        self.a_vx_vx = (self.d_x2(factors=(self.t.increment / self.x.increment ** 2
+                                           * self.material_vector('absorption_coef')
+                                           / self.material_vector('density')))
+                        + self.d_y2(factors=(self.t.increment / self.y.increment ** 2
+                                             * self.material_vector('absorption_coef')
+                                             / self.material_vector('density')))
+                        + self.d_x(factors=(self.t.increment / self.x.increment
+                                            * self.material_vector('absorption_coef')
+                                            / self.material_vector('density') / self._radii()),
+                                   variant='central')).todia()
         self.a_vy_vy = self.a_vx_vx
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.pressure.apply_bounds(self.step)
         self.pressure.write_outputs()
 
-        self.velocity_x.values -= (self.a_vx_p.dot(self.pressure.values) -
-                                   self.a_vx_vx.dot(self.velocity_x.values) +
-                                   self.t.increment * self.material_vector('absorption_coef') /
-                                   self.material_vector('density') * self.velocity_x.values /
-                                   self._radii() ** 2)
-        self.velocity_y.values -= (self.a_vy_p.dot(self.pressure.values) -
-                                   self.a_vy_vy.dot(self.velocity_y.values))
+        self.velocity_x.values -= (self.a_vx_p.dot(self.pressure.values)
+                                   - self.a_vx_vx.dot(self.velocity_x.values)
+                                   + self.t.increment * self.material_vector('absorption_coef')
+                                   / self.material_vector('density') * self.velocity_x.values
+                                   / self._radii() ** 2)
+        self.velocity_y.values -= (self.a_vy_p.dot(self.pressure.values)
+                                   - self.a_vy_vy.dot(self.velocity_y.values))
 
         self.velocity_x.apply_bounds(self.step)
         self.velocity_x.write_outputs()
         self.velocity_y.apply_bounds(self.step)
         self.velocity_y.write_outputs()
 
-        self.pressure.values -= (self.a_p_vx.dot(self.velocity_x.values * self._radii()) +
-                                 self.a_p_vy.dot(self.velocity_y.values))
+        self.pressure.values -= (self.a_p_vx.dot(self.velocity_x.values * self._radii())
+                                 + self.a_p_vy.dot(self.velocity_y.values))
 
     def is_stable(self):
         """Checks if simulation satisfies stability conditions. Does not account for instability
         due to high absorption and includes a little headroom (1%).
 
         Returns:
             True if stable, False if not.
         """
 
-        return np.all(self.material_vector('sound_velocity') <
-                      0.99 * min(self.x.increment, self.y.increment) / self.t.increment)
+        return np.all(self.material_vector('sound_velocity')
+                      < 0.99 * min(self.x.increment, self.y.increment) / self.t.increment)
 
 
 class AcousticMaterial:
     """Class for specification of acoustic material parameters."""
 
     def __init__(self, sound_velocity, density,
                  shear_viscosity=0, bulk_viscosity=0,
@@ -245,17 +245,17 @@
             sound_velocity: Sound velocity.
             density: Density.
             shear_viscosity: Shear viscosity.
             bulk_viscosity: Bulk viscosity.
             thermal_conductivity: Thermal conductivity coefficient.
             isobaric_heat_cap: Isobaric heat capacitance (at constant pressure).
             isochoric_heat_cap: Isochoric heat capacitance (at constant volume).
-            absorption_coef: Sum of losses (4/3 * shear_viscosity + bulk_viscosity + 
+            absorption_coef: Sum of losses (4/3 * shear_viscosity + bulk_viscosity +
                 thermal_conductivity * (isobaric_heat_cap - isochoric_heat_cap) /
-                (isobaric_heat_cap * isochoric_heat_cap)). If set, the given value is used 
+                (isobaric_heat_cap * isochoric_heat_cap)). If set, the given value is used
                 directly instead of calculating if from the other properties.
         """
 
         self.sound_velocity = sound_velocity
         self.density = density
         self.shear_viscosity = shear_viscosity
         self.bulk_viscosity = bulk_viscosity
@@ -266,16 +266,17 @@
 
     @property
     def absorption_coef(self):
         """Returns a helper variable (called mu in publications by L. Claes) that sums up all
         losses into a single quantity."""
 
         if not self._absorption_coef:
-            return (4/3 * self.shear_viscosity + self.bulk_viscosity + self.thermal_conductivity *
-                    (self.isobaric_heat_cap - self.isochoric_heat_cap) /
-                    (self.isobaric_heat_cap * self.isochoric_heat_cap))
+            return (4 / 3 * self.shear_viscosity + self.bulk_viscosity
+                    + self.thermal_conductivity
+                    * (self.isobaric_heat_cap - self.isochoric_heat_cap)
+                    / (self.isobaric_heat_cap * self.isochoric_heat_cap))
         else:
             return self._absorption_coef
 
     @absorption_coef.setter
     def absorption_coef(self, value):
         self._absorption_coef = value
```

### Comparing `pyfds-0.1.6/pyfds/electrostatics.py` & `pyfds-0.2.0/pyfds/electrostatics.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         self.a_phi_rho = None
 
     def assemble_matrices(self):
         """Assemble the a_* matrices required for simulation."""
 
         # Conversion to Compressed Sparse Column format is necessary for efficient inversion
         a_rho_phi = sp.csc_matrix(
-            self.d_x2(factors=(self.material_vector('permittivity_x') /
-                               self.x.increment ** 2)))
+            self.d_x2(factors=(self.material_vector('permittivity_x')
+                               / self.x.increment ** 2)))
         self.a_phi_rho = sl.inv(a_rho_phi)
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.charge_density.apply_bounds(self.step)
@@ -74,18 +74,18 @@
         self.a_phi_rho = None
 
     def assemble_matrices(self):
         """Assemble the a_* matrices required for simulation."""
 
         # Conversion to Compressed Sparse Column format is necessary for efficient inversion
         a_rho_phi = sp.csc_matrix(
-            self.d_x2(factors=(self.material_vector('permittivity_x') /
-                               self.x.increment ** 2)) +
-            self.d_y2(factors=(self.material_vector('permittivity_y') /
-                               self.y.increment ** 2)))
+            self.d_x2(factors=(self.material_vector('permittivity_x')
+                               / self.x.increment ** 2))
+            + self.d_y2(factors=(self.material_vector('permittivity_y')
+                                 / self.y.increment ** 2)))
         self.a_phi_rho = sl.inv(a_rho_phi)
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.charge_density.apply_bounds(self.step)
```

### Comparing `pyfds-0.1.6/pyfds/fields.py` & `pyfds-0.2.0/pyfds/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         self.material_regions.append(new_material_region)
         logger.info('Material region {} added.'.format(new_material_region.region.name))
 
     def reset(self):
         """Reset the field to all-zero but keep all boundaries to enable repeated simulation using
         the same field object."""
         for name in dir(self):
-            if type(getattr(self, name)) == FieldComponent:
+            if isinstance(getattr(self, name), FieldComponent):
                 getattr(self, name).values = np.zeros_like(getattr(self, name).values)
         self.step = 0
 
 
 class Field1D(Field):
     """Class for one-dimensional fields."""
 
@@ -199,15 +199,15 @@
             Sparse matrix the calculate second derivatives of field components.
         """
 
         # use ones as factors if none are specified
         if factors is None:
             factors = np.array(1).repeat(self.num_points)
 
-        return sp.dia_matrix((np.array([factors, -2*factors, factors]), [-1, 0, 1]),
+        return sp.dia_matrix((np.array([factors, -2 * factors, factors]), [-1, 0, 1]),
                              shape=(self.num_points, self.num_points))
 
     def get_index(self, position):
         """Returns the index of a point at the given position.
 
         Args:
             position: Position of the requested point.
@@ -291,15 +291,15 @@
         if factors is None:
             factors = np.array(1).repeat(self.num_points)
 
         if variant == 'forward':
             return sp.dia_matrix((np.array([-factors, factors]), [0, 1]),
                                  shape=(self.num_points, self.num_points))
         elif variant == 'central':
-            return sp.dia_matrix((np.array([-factors/2, factors/2]), [-1, 1]),
+            return sp.dia_matrix((np.array([-factors / 2, factors / 2]), [-1, 1]),
                                  shape=(self.num_points, self.num_points))
         elif variant == 'backward':
             return sp.dia_matrix((np.array([-factors, factors]), [-1, 0]),
                                  shape=(self.num_points, self.num_points))
         else:
             raise ValueError('Unknown difference quotient variant {}.'.format(variant))
 
@@ -320,15 +320,15 @@
             factors = np.array(1).repeat(self.num_points)
 
         if variant == 'forward':
             return sp.dia_matrix((np.array([-factors, factors]), [0, self.x.samples]),
                                  shape=(self.num_points, self.num_points))
         elif variant == 'central':
             return sp.dia_matrix(
-                (np.array([-factors/2, factors/2]), [-self.x.samples, self.x.samples]),
+                (np.array([-factors / 2, factors / 2]), [-self.x.samples, self.x.samples]),
                 shape=(self.num_points, self.num_points))
         elif variant == 'backward':
             return sp.dia_matrix((np.array([-factors, factors]), [-self.x.samples, 0]),
                                  shape=(self.num_points, self.num_points))
         else:
             raise ValueError('Unknown difference quotient variant {}.'.format(variant))
 
@@ -343,15 +343,15 @@
             Sparse matrix the calculate second derivatives of field components.
         """
 
         # use ones as factors if none are specified
         if factors is None:
             factors = np.array(1).repeat(self.num_points)
 
-        return sp.dia_matrix((np.array([factors, -2*factors, factors]), [-1, 0, 1]),
+        return sp.dia_matrix((np.array([factors, -2 * factors, factors]), [-1, 0, 1]),
                              shape=(self.num_points, self.num_points))
 
     def d_y2(self, factors=None):
         """Creates a sparse matrix for computing the second derivative with respect to y multiplied
         by factors given for every point. Uses central difference quotient.
 
         Args:
@@ -361,15 +361,15 @@
             Sparse matrix the calculate second derivatives of field components.
         """
 
         # use ones as factors if none are specified
         if factors is None:
             factors = np.array(1).repeat(self.num_points)
 
-        return sp.dia_matrix((np.array([factors, -2*factors, factors]),
+        return sp.dia_matrix((np.array([factors, -2 * factors, factors]),
                               [-self.x.samples, 0, self.x.samples]),
                              shape=(self.num_points, self.num_points))
 
     def get_index(self, position):
         """Returns the index of a point at the given position.
 
         Args:
@@ -495,21 +495,52 @@
                    (coordinates[1] - position[5]) * (position[0] - position[4])
 
         point_indices = (self.get_index(position[:2]),
                          self.get_index(position[2:4]),
                          self.get_index(position[4:]))
 
         inside_indices = []
-        for ii in range(min(point_indices), max(point_indices)+1):
+        for ii in range(min(point_indices), max(point_indices) + 1):
             point = self.get_position(ii)
             if edge_01(point) >= 0 and edge_12(point) >= 0 and edge_20(point) >= 0:
                 inside_indices.append(ii)
 
         return reg.TriRegion(inside_indices, position, name)
 
+    def get_ellipse_region(self, centre, radii, name=''):
+        """Create an elliptic region with the given parameters.
+
+        Args:
+            centre: Coordinates of the centre of the ellipse.
+            radii: Radii/half axes of the ellipse in x and y direction.
+            name: Name of the region.
+        """
+        if np.isscalar(radii):
+            radii = (radii, radii)
+
+        def inside(coordiantes):
+            """Check if given coordinates are inside the ellipse.
+
+            Returns:
+                True if inside, False if outside the ellipse.
+            """
+            return (centre[0] - coordiantes[0]) ** 2 / radii[0] ** 2 \
+                + (centre[1] - coordiantes[1]) ** 2 / radii[1] ** 2 <= 1
+
+        # Limit point index range so not all points on the grid have to be checked.
+        min_point_index = self.get_index((centre[0], centre[1] - radii[1]))
+        max_point_index = self.get_index((centre[0], centre[1] + radii[1]))
+
+        inside_indices = []
+        for ii in range(min_point_index, max_point_index):
+            if inside(self.get_position(ii)):
+                inside_indices.append(ii)
+
+        return reg.EllipseRegion(inside_indices, centre, radii, name)
+
 
 class Dimension:
     """Represents a space or time axis."""
 
     def __init__(self, samples, increment):
         """Class constructor.
 
@@ -562,15 +593,15 @@
         # list with objects of type Output
         self.outputs = []
 
     def apply_bounds(self, step):
         """Applies the boundary conditions to the field component.
 
         Args:
-            step: Simulation step, required if boundary is a signal that changes of time.
+            step: Simulation step, required if boundary is a signal that changes over time.
         """
 
         for bound in self.boundaries:
             self.values[bound.region.indices] = bound.apply(self.values[bound.region.indices],
                                                             step=step)
 
     def write_outputs(self):
```

### Comparing `pyfds-0.1.6/pyfds/gfx.py` & `pyfds-0.2.0/pyfds/gfx.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             frame_delay: Delay between animation updates.
             save_video: Save animation as video (requires ffmpeg).
             video_file_name: File name for the video.
         """
 
         self.field = field
         self.field_components = {name: getattr(self.field, name) for name in dir(self.field)
-                                 if type(getattr(self.field, name)) == fld.FieldComponent}
+                                 if isinstance(getattr(self.field, name), fld.FieldComponent)}
         if observed_component:
             if observed_component in self.field_components.keys():
                 self.observed_component = observed_component
             else:
                 raise KeyError('Field component {} not found in given field.'
                                .format(observed_component))
         else:
@@ -78,23 +78,23 @@
             queue.put((self.field.t.vector[self.field.step - 1],
                        getattr(self.field, self.observed_component).values))
 
         # return field when simulation finishes to get output signals
         queue.put(self.field)
 
     def _update_components(self, message):
-        """Function to be called when simulation process finished to update the field components 
+        """Function to be called when simulation process finished to update the field components
         the main process including the output signals
-        
+
         Args:
             message: Field object returned by the simulation process.
         """
 
         for name in dir(self.field):
-            if type(getattr(self.field, name)) == fld.FieldComponent:
+            if isinstance(getattr(self.field, name), fld.FieldComponent):
                 setattr(self.field, name, getattr(message, name))
 
     def _save_frame(self):
         """Save current frame of animation to a png file for video creation."""
 
         file_name = 'frame{0:06d}.png'.format(len(self.image_files))
         pp.savefig(file_name, dpi=self.video_dpi)
@@ -108,16 +108,16 @@
             answer = input('File {} already exists. Overwrite? [y/N]'.format(self.video_file_name))
             if answer.capitalize() == 'Y':
                 os.remove(self.video_file_name)
 
         if not answer or answer.capitalize() == 'Y':
             # video codec requires the image size to be dividable by 2. Numbers (6.4 and 4.78)
             # result from matplotlibs standard figure size.
-            width = int((self.video_dpi * 6.4)//2 * 2)
-            height = int((self.video_dpi * 4.78)//2 * 2)
+            width = int((self.video_dpi * 6.4) // 2 * 2)
+            height = int((self.video_dpi * 4.78) // 2 * 2)
             os.system('{} -loglevel error -framerate {} -i frame%06d.png -pix_fmt yuv420p -vf '
                       'scale={}:{} {}'.format(self.ffmpeg_path, self.video_fps, width, height,
                                               self.video_file_name))
 
         for file in self.image_files:
             os.remove(file)
 
@@ -138,29 +138,29 @@
     def plot_region(self, region):
         """Shows the given region in the field plot.
 
         Args:
             region: Region to be plotted.
         """
 
-        if type(region) == reg.PointRegion:
+        if isinstance(region, reg.PointRegion):
             self.axes.plot(np.ones(2) * region.point_coordinates / self._x_axis_factor,
                            self.scale, color='black')
-        elif type(region) == reg.LineRegion:
+        elif isinstance(region, reg.LineRegion):
             self.axes.plot(np.ones(2) * region.line_coordinates[0] / self._x_axis_factor,
                            self.scale, color='black')
             self.axes.plot(np.ones(2) * region.line_coordinates[1] / self._x_axis_factor,
                            self.scale, color='black')
         else:
             raise TypeError('Unknown type in region list: {}'.format(type(region)))
 
     def show_setup(self, halt=True):
-        """Open a plot window that shows the simulation setup including boundaries, outputs and 
+        """Open a plot window that shows the simulation setup including boundaries, outputs and
         material regions.
-        
+
         Args:
             halt: Halt script execution until plot window is closed.
         """
 
         pp.figure()
         self.axes = pp.gca()
         self.axes.set_xlim(0, max(self.field.x.vector) / self._x_axis_factor)
@@ -218,15 +218,15 @@
                     # update main process field components with simulation result
                     self._update_components(message)
                     finished = True
                 else:
                     time, data = message
                     self.axes.title.set_text('{title} $t$ = {time:.{prec}f} {prefix}s'
                                              .format(title=self.plot_title,
-                                                     time=time/self._t_factor,
+                                                     time=time / self._t_factor,
                                                      prec=self.time_precision,
                                                      prefix=self._t_prefix))
                     main_plot.set_data(self.field.x.vector / self._x_axis_factor, data)
                     pp.pause(self.frame_delay)
                     if self.save_video:
                         self._save_frame()
 
@@ -257,38 +257,44 @@
     def plot_region(self, region):
         """Shows the given region in the field plot.
 
         Args:
             region: Region to be plotted.
         """
 
-        if type(region) == reg.PointRegion:
+        if isinstance(region, reg.PointRegion):
             self.axes.scatter(region.point_coordinates[0] / self._x_axis_factor,
                               region.point_coordinates[1] / self._y_axis_factor, color='black')
-        elif type(region) == reg.LineRegion:
+        elif isinstance(region, reg.LineRegion):
             self.axes.plot([region.line_coordinates[0] / self._x_axis_factor,
                             region.line_coordinates[2] / self._x_axis_factor],
                            [region.line_coordinates[1] / self._y_axis_factor,
                             region.line_coordinates[3] / self._y_axis_factor],
                            color='black')
-        elif type(region) == reg.RectRegion:
+        elif isinstance(region, reg.RectRegion):
             self.axes.add_patch(pa.Rectangle((region.rect_coordinates[0] / self._x_axis_factor,
                                               region.rect_coordinates[1] / self._y_axis_factor),
                                              region.rect_coordinates[2] / self._x_axis_factor,
                                              region.rect_coordinates[3] / self._y_axis_factor,
                                              fill=False))
-        elif type(region) == reg.TriRegion:
+        elif isinstance(region, reg.TriRegion):
             self.axes.add_patch(pa.Polygon(
                 np.array([[region.tri_coordinates[0] / self._x_axis_factor,
                            region.tri_coordinates[1] / self._y_axis_factor],
                           [region.tri_coordinates[2] / self._x_axis_factor,
                            region.tri_coordinates[3] / self._y_axis_factor],
                           [region.tri_coordinates[4] / self._x_axis_factor,
                            region.tri_coordinates[5] / self._y_axis_factor]]),
                 fill=False))
+        elif isinstance(region, reg.EllipseRegion):
+            self.axes.add_patch(pa.Ellipse(
+                (region.centre[0] / self._x_axis_factor, region.centre[1] / self._y_axis_factor),
+                2 * region.radii[0] / self._x_axis_factor,
+                2 * region.radii[1] / self._y_axis_factor,
+                fill=False))
         else:
             raise TypeError('Unknown type in region list: {}'.format(type(region)))
 
     def field_as_matrix(self, component=None):
         """Returns a field component (observed component by default) as a numpy matrix.
 
         Args:
@@ -300,15 +306,15 @@
 
         if component is None:
             component = getattr(self.field, self.observed_component).values
 
         return np.reshape(component, (self.field.y.samples, self.field.x.samples))
 
     def show_setup(self, halt=True):
-        """Open a plot window that shows the simulation setup including boundaries, outputs and 
+        """Open a plot window that shows the simulation setup including boundaries, outputs and
         material regions.
 
         Args:
             halt: Halt script execution until plot window is closed.
         """
 
         pp.figure()
@@ -374,15 +380,15 @@
                     # update main process field components with simulation result
                     self._update_components(message)
                     finished = True
                 else:
                     time, data = message
                     self.axes.title.set_text('{title} $t$ = {time:.{prec}f} {prefix}s'
                                              .format(title=self.plot_title,
-                                                     time=time/self._t_factor,
+                                                     time=time / self._t_factor,
                                                      prec=self.time_precision,
                                                      prefix=self._t_prefix))
                     main_plot.set_data(self.field_as_matrix(data))
                     pp.pause(self.frame_delay)
                     if self.save_video:
                         self._save_frame()
 
@@ -391,21 +397,21 @@
                 self._create_video()
 
         pp.show()
 
 
 def get_prefix(value):
     """Determine the metric prefix for a given value.
-    
+
     Args:
         value: Value to determine the prefix for.
 
     Returns:
         prefix: String specifying the prefix.
-        factor: Scale factor of the prefix.        
+        factor: Scale factor of the prefix.
     """
     for factor, prefix in sorted(prefixes.items()):
         if value / factor < 1e3:
             break
     return prefix, factor
```

### Comparing `pyfds-0.1.6/pyfds/nonlinear_acoustics.py` & `pyfds-0.2.0/pyfds/nonlinear_acoustics.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Class for simulation of one-dimensional nonlinear acoustic fields in ideal gases."""
 
     def __init__(self, convective=True, nl_state=True, *args, **kwargs):
         """Class constructor.
 
         Args:
             convective: Account for convective terms.
-            nl_adiabatic: Account for nonlinear equation of state.
+            nl_state: Account for nonlinear equation of state.
             See pyfds.fields.Field1D constructor arguments.
         """
 
         super().__init__(*args, **kwargs)
         self.convective = convective
         self.nl_state = nl_state
         self.pressure = fld.FieldComponent(self.num_points)
@@ -31,51 +31,51 @@
         self.stat_density = None
         self.sound_velocity = None
         self.heat_cap_ratio = None
 
     def assemble_matrices(self):
         """Assemble the a_* matrices and buffer material parameters required for simulation."""
 
-        self.a_d_v = self.d_x(factors=(self.t.increment / self.x.increment *
-                                       np.ones(self.x.samples)))
-        self.a_v_p = self.d_x(factors=(self.t.increment / self.x.increment) *
-                              np.ones(self.x.samples), variant='backward')
-        self.a_v_v = self.d_x2(factors=(self.t.increment / self.x.increment ** 2 *
-                                        self.material_vector('absorption_coef')))
-        self.a_v_v2 = self.d_x(factors=(self.t.increment / self.x.increment / 2) *
-                               np.ones(self.x.samples), variant='central')
+        self.a_d_v = self.d_x(factors=(self.t.increment / self.x.increment
+                                       * np.ones(self.x.samples)))
+        self.a_v_p = self.d_x(factors=(self.t.increment / self.x.increment)
+                              * np.ones(self.x.samples), variant='backward')
+        self.a_v_v = self.d_x2(factors=(self.t.increment / self.x.increment ** 2
+                                        * self.material_vector('absorption_coef')))
+        self.a_v_v2 = self.d_x(factors=(self.t.increment / self.x.increment / 2)
+                               * np.ones(self.x.samples), variant='central')
         self.stat_density = self.material_vector('density')
         self.sound_velocity = self.material_vector('sound_velocity')
-        self.heat_cap_ratio = (self.material_vector('isobaric_heat_cap') /
-                               self.material_vector('isochoric_heat_cap'))
+        self.heat_cap_ratio = (self.material_vector('isobaric_heat_cap')
+                               / self.material_vector('isochoric_heat_cap'))
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.pressure.apply_bounds(self.step)
         self.pressure.write_outputs()
 
         if self.convective:
-            self.velocity.values -= (self.a_v_p.dot(self.pressure.values) /
-                                     (self.stat_density + self.density.values) +
-                                     self.a_v_v2.dot(self.velocity.values) -
-                                     self.a_v_v.dot(self.velocity.values) /
-                                     (self.stat_density + self.density.values))
+            self.velocity.values -= (self.a_v_p.dot(self.pressure.values)
+                                     / (self.stat_density + self.density.values)
+                                     + self.a_v_v2.dot(self.velocity.values)
+                                     - self.a_v_v.dot(self.velocity.values)
+                                     / (self.stat_density + self.density.values))
         else:
-            self.velocity.values -= (self.a_v_p.dot(self.pressure.values) /
-                                     (self.stat_density + self.density.values) -
-                                     self.a_v_v.dot(self.velocity.values) /
-                                     (self.stat_density + self.density.values))
+            self.velocity.values -= (self.a_v_p.dot(self.pressure.values)
+                                     / (self.stat_density + self.density.values)
+                                     - self.a_v_v.dot(self.velocity.values)
+                                     / (self.stat_density + self.density.values))
 
         self.velocity.apply_bounds(self.step)
         self.velocity.write_outputs()
 
-        self.density.values -= self.a_d_v.dot((self.density.values + self.stat_density) *
-                                              self.velocity.values)
+        self.density.values -= self.a_d_v.dot((self.density.values + self.stat_density)
+                                              * self.velocity.values)
 
         self.density.apply_bounds(self.step)
         self.density.write_outputs()
 
         if self.nl_state:
             # using modified equation of state, so static pressure is not required
             self.pressure.values = \
@@ -89,31 +89,31 @@
         """Checks if simulation satisfies stability conditions. Does not account for instability
         due to high absorption or nonlinear effects. Includes a little headroom (1%).
 
         Returns:
             True if stable, False if not.
         """
 
-        return np.all(self.material_vector('sound_velocity') <
-                      0.99 * self.x.increment / self.t.increment)
+        return np.all(self.material_vector('sound_velocity')
+                      < 0.99 * self.x.increment / self.t.increment)
 
 
 class Acoustic2ndOrder1D(fld.Field1D):
-    """Class for simulation of one-dimensional nonlinear acoustic fields using second order 
+    """Class for simulation of one-dimensional nonlinear acoustic fields using second order
     approximation."""
 
     def __init__(self, *args, **kwargs):
         """Class constructor.
 
         Args:
             See pyfds.fields.Field1D constructor arguments.
         """
 
-        if not (hasattr(kwargs['material'], 'd_rho_p') and
-                hasattr(kwargs['material'], 'd_rho2_p')):
+        if not (hasattr(kwargs['material'], 'd_rho_p')
+                and hasattr(kwargs['material'], 'd_rho2_p')):
             wn.warn('Material with properties d_rho_p and d_rho2_p is required for 2nd order '
                     'nonlinear acoustic simulation.')
         super().__init__(*args, **kwargs)
 
         self.pressure = fld.FieldComponent(self.num_points)
         self.velocity = fld.FieldComponent(self.num_points)
         self.density = fld.FieldComponent(self.num_points)
@@ -126,44 +126,44 @@
         self.stat_density = None
         self.d_rho_p = None
         self.d_rho2_p = None
 
     def assemble_matrices(self):
         """Assemble the a_* matrices and buffer material parameters required for simulation."""
 
-        self.a_d_v = self.d_x(factors=(self.t.increment / self.x.increment *
-                                       np.ones(self.x.samples)))
-        self.a_v_p = self.d_x(factors=(self.t.increment / self.x.increment) *
-                              np.ones(self.x.samples), variant='backward')
-        self.a_v_v = self.d_x2(factors=(self.t.increment / self.x.increment ** 2 *
-                                        self.material_vector('absorption_coef')))
-        self.a_v_v2 = self.d_x(factors=(self.t.increment / self.x.increment / 2) *
-                               np.ones(self.x.samples), variant='central')
+        self.a_d_v = self.d_x(factors=(self.t.increment / self.x.increment
+                                       * np.ones(self.x.samples)))
+        self.a_v_p = self.d_x(factors=(self.t.increment / self.x.increment)
+                              * np.ones(self.x.samples), variant='backward')
+        self.a_v_v = self.d_x2(factors=(self.t.increment / self.x.increment ** 2
+                                        * self.material_vector('absorption_coef')))
+        self.a_v_v2 = self.d_x(factors=(self.t.increment / self.x.increment / 2)
+                               * np.ones(self.x.samples), variant='central')
         self.stat_density = self.material_vector('density')
         self.d_rho_p = self.material_vector('d_rho_p')
         self.d_rho2_p = self.material_vector('d_rho2_p')
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.pressure.apply_bounds(self.step)
         self.pressure.write_outputs()
 
-        self.velocity.values -= (self.a_v_p.dot(self.pressure.values) /
-                                 (self.stat_density + self.density.values) +
-                                 self.a_v_v2.dot(self.velocity.values) -
-                                 self.a_v_v.dot(self.velocity.values) /
-                                 (self.stat_density + self.density.values))
+        self.velocity.values -= (self.a_v_p.dot(self.pressure.values)
+                                 / (self.stat_density + self.density.values)
+                                 + self.a_v_v2.dot(self.velocity.values)
+                                 - self.a_v_v.dot(self.velocity.values)
+                                 / (self.stat_density + self.density.values))
 
         self.velocity.apply_bounds(self.step)
         self.velocity.write_outputs()
 
-        self.density.values -= self.a_d_v.dot((self.density.values + self.stat_density) *
-                                              self.velocity.values)
+        self.density.values -= self.a_d_v.dot((self.density.values + self.stat_density)
+                                              * self.velocity.values)
 
         self.density.apply_bounds(self.step)
         self.density.write_outputs()
 
         self.pressure.values = self.d_rho_p * self.density.values + \
             self.d_rho2_p / 2 * self.density.values**2
```

### Comparing `pyfds-0.1.6/pyfds/regions.py` & `pyfds-0.2.0/pyfds/regions.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,14 +77,32 @@
             name: Name of the region.
         """
 
         super().__init__(indices, name)
         self.tri_coordinates = coordinates
 
 
+class EllipseRegion(Region):
+    """Region specified by a elliptic field of points."""
+
+    def __init__(self, indices, centre, radii, name=''):
+        """Class constructor.
+
+        Args:
+            indices: Point indices of the region.
+            centre: Coordinates of the centre of the ellipse.
+            radii: Radii/half axes of the ellipse in x and y direction.
+            name: Name of the region.
+        """
+
+        super().__init__(indices, name)
+        self.centre = centre
+        self.radii = radii
+
+
 class Boundary:
     """Specifies values that are to be written to a FieldComponent after each simulation step
     (like excitation signals and fixed boundaries)."""
 
     def __init__(self, region, value=0, additive=False):
         """Class constructor.
 
@@ -109,16 +127,16 @@
 
         Returns:
             New values for the points in the boundary.
         """
 
         if np.ndim(self.value) == 0:
             # if a single value is given
-                return self.additive * old_values + self.value
-        elif type(self.value) == np.ndarray:
+            return self.additive * old_values + self.value
+        elif isinstance(self.value, np.ndarray):
             # if a signal is given
             return self.additive * old_values + self.value[step]
         else:
             # if a list of signals for each index is given
             return [self.additive * old_values[ii] + signal[step]
                     for ii, signal in enumerate(self.value)]
```

### Comparing `pyfds-0.1.6/pyfds/thermal.py` & `pyfds-0.2.0/pyfds/thermal.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
         # initialize attributes sparse matrices
         self.a_t_q = None
         self.a_q_t = None
 
     def assemble_matrices(self):
         """Assemble the a_* matrices required for simulation."""
 
-        self.a_t_q = self.d_x(factors=(self.t.increment / self.x.increment /
-                                       self.material_vector('density') /
-                                       self.material_vector('heat_capacity')))
-        self.a_q_t = self.d_x(factors=(1 / self.x.increment *
-                                       self.material_vector('thermal_conductivity_x')),
+        self.a_t_q = self.d_x(factors=(self.t.increment / self.x.increment
+                                       / self.material_vector('density')
+                                       / self.material_vector('heat_capacity')))
+        self.a_q_t = self.d_x(factors=(1 / self.x.increment
+                                       * self.material_vector('thermal_conductivity_x')),
                               variant='backward')
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.temperature.apply_bounds(self.step)
@@ -67,25 +67,25 @@
         self.a_t_qy = None
         self.a_qx_t = None
         self.a_qy_t = None
 
     def assemble_matrices(self):
         """Assemble the a_* matrices required for simulation."""
 
-        self.a_t_qx = self.d_x(factors=(self.t.increment / self.x.increment /
-                                        self.material_vector('density') /
-                                        self.material_vector('heat_capacity')))
-        self.a_t_qy = self.d_y(factors=(self.t.increment / self.y.increment /
-                                        self.material_vector('density') /
-                                        self.material_vector('heat_capacity')))
-        self.a_qx_t = self.d_x(factors=(1 / self.x.increment *
-                                        self.material_vector('thermal_conductivity_x')),
+        self.a_t_qx = self.d_x(factors=(self.t.increment / self.x.increment
+                                        / self.material_vector('density')
+                                        / self.material_vector('heat_capacity')))
+        self.a_t_qy = self.d_y(factors=(self.t.increment / self.y.increment
+                                        / self.material_vector('density')
+                                        / self.material_vector('heat_capacity')))
+        self.a_qx_t = self.d_x(factors=(1 / self.x.increment
+                                        * self.material_vector('thermal_conductivity_x')),
                                variant='backward')
-        self.a_qy_t = self.d_y(factors=(1 / self.y.increment *
-                                        self.material_vector('thermal_conductivity_y')),
+        self.a_qy_t = self.d_y(factors=(1 / self.y.increment
+                                        * self.material_vector('thermal_conductivity_y')),
                                variant='backward')
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.temperature.apply_bounds(self.step)
@@ -95,16 +95,16 @@
         self.heat_flux_y.values = -self.a_qy_t.dot(self.temperature.values)
 
         self.heat_flux_x.apply_bounds(self.step)
         self.heat_flux_x.write_outputs()
         self.heat_flux_y.apply_bounds(self.step)
         self.heat_flux_y.write_outputs()
 
-        self.temperature.values -= (self.a_t_qx.dot(self.heat_flux_x.values) +
-                                    self.a_t_qy.dot(self.heat_flux_y.values))
+        self.temperature.values -= (self.a_t_qx.dot(self.heat_flux_x.values)
+                                    + self.a_t_qy.dot(self.heat_flux_y.values))
 
 
 class Thermal3DAxi(fld.Field2D):
     """Class for simulation of three-dimensional, axial-symmetric thermal fields. Note the x is
     the radial direction, and y is the z direction."""
 
     def __init__(self, *args, **kwargs):
@@ -131,30 +131,30 @@
         symmetric fields, this is the radius, which is required to formulate the differential
         operators.
 
         Returns
             Radius of each heat flux point.
         """
 
-        return np.tile(self.x.vector, self.y.samples) + self.x.increment/2
+        return np.tile(self.x.vector, self.y.samples) + self.x.increment / 2
 
     def assemble_matrices(self):
         """Assemble the a_* matrices required for simulation."""
 
-        self.a_t_qx = self.d_x(factors=(self.t.increment / self.x.increment /
-                                        self.material_vector('density') /
-                                        self.material_vector('heat_capacity') / self._radii()))
-        self.a_t_qy = self.d_y(factors=(self.t.increment / self.y.increment /
-                                        self.material_vector('density') /
-                                        self.material_vector('heat_capacity')))
-        self.a_qx_t = self.d_x(factors=(1 / self.x.increment *
-                                        self.material_vector('thermal_conductivity_x')),
+        self.a_t_qx = self.d_x(factors=(self.t.increment / self.x.increment
+                                        / self.material_vector('density')
+                                        / self.material_vector('heat_capacity') / self._radii()))
+        self.a_t_qy = self.d_y(factors=(self.t.increment / self.y.increment
+                                        / self.material_vector('density')
+                                        / self.material_vector('heat_capacity')))
+        self.a_qx_t = self.d_x(factors=(1 / self.x.increment
+                                        * self.material_vector('thermal_conductivity_x')),
                                variant='backward')
-        self.a_qy_t = self.d_y(factors=(1 / self.y.increment *
-                                        self.material_vector('thermal_conductivity_y')),
+        self.a_qy_t = self.d_y(factors=(1 / self.y.increment
+                                        * self.material_vector('thermal_conductivity_y')),
                                variant='backward')
         self.matrices_assembled = True
 
     def sim_step(self):
         """Simulate one step."""
 
         self.temperature.apply_bounds(self.step)
@@ -164,16 +164,16 @@
         self.heat_flux_y.values = -self.a_qy_t.dot(self.temperature.values)
 
         self.heat_flux_x.apply_bounds(self.step)
         self.heat_flux_x.write_outputs()
         self.heat_flux_y.apply_bounds(self.step)
         self.heat_flux_y.write_outputs()
 
-        self.temperature.values -= (self.a_t_qx.dot(self.heat_flux_x.values * self._radii()) +
-                                    self.a_t_qy.dot(self.heat_flux_y.values))
+        self.temperature.values -= (self.a_t_qx.dot(self.heat_flux_x.values * self._radii())
+                                    + self.a_t_qy.dot(self.heat_flux_y.values))
 
 
 class ThermalMaterial:
     """Class for specification of thermal material parameters."""
 
     def __init__(self, heat_capacity, density, thermal_conductivity):
         """Class constructor.
```

### Comparing `pyfds-0.1.6/pyfds.egg-info/SOURCES.txt` & `pyfds-0.2.0/pyfds.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 .gitignore
 AUTHORS.rst
 CHANGELOG.rst
 LICENSE
 README.rst
+pyproject.toml
 setup.py
+.github/workflows/python-package.yml
 doc/acoustic_flow.rst
 doc/acoustics.rst
 doc/conf.py
 doc/electrostatics.rst
 doc/ex_acoustics.rst
 doc/ex_visualization.rst
 doc/examples.rst
```

### Comparing `pyfds-0.1.6/setup.py` & `pyfds-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     name='pyfds',
 
     description='Modular field simulation tool using finite differences.',
     long_description=long_description,
 
-    url='http://emt.uni-paderborn.de',
+    url='https://emt.uni-paderborn.de',
     author='Leander Claes',
     author_email='claes@emt.uni-paderborn.de',
     license='BSD',
 
     # Automatically generate version number from git tags
     use_scm_version=True,
```

### Comparing `pyfds-0.1.6/test/test_acoustics.py` & `pyfds-0.2.0/test/test_acoustics.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 
 def test_acoustic3d_axi_create_matrices():
     fld = fds.Acoustic3DAxi(t_delta=1, t_samples=1,
                             x_delta=1, x_samples=2,
                             y_delta=1, y_samples=2,
                             material=fds.AcousticMaterial(1, 1, bulk_viscosity=1))
     fld.assemble_matrices()
-    assert np.allclose(fld.a_p_vx.toarray(), [[-2, 2/3, 0, 0], [0, -2/3, 2, 0],
-                                              [0, 0, -2, 2/3], [0, 0, 0, -2/3]])
+    assert np.allclose(fld.a_p_vx.toarray(), [[-2, 2 / 3, 0, 0], [0, -2 / 3, 2, 0],
+                                              [0, 0, -2, 2 / 3], [0, 0, 0, -2 / 3]])
     assert np.allclose(fld.a_p_vy.toarray(), [[-1, 0, 1, 0], [0, -1, 0, 1],
                                               [0, 0, -1, 0], [0, 0, 0, -1]])
     assert np.allclose(fld.a_vx_p.toarray(), [[1, 0, 0, 0], [-1, 1, 0, 0], [0, -1, 1, 0],
                                               [0, 0, -1, 1]])
     assert np.allclose(fld.a_vy_p.toarray(), [[1, 0, 0, 0], [0, 1, 0, 0], [-1, 0, 1, 0],
                                               [0, -1, 0, 1]])
-    assert np.allclose(fld.a_vx_vx.toarray(), [[-4, 4/3, 1, 0], [0, -4, 2, 1],
-                                               [1, 2/3, -4, 4/3], [0, 1, 0, -4]])
-    assert np.allclose(fld.a_vy_vy.toarray(), [[-4, 4/3, 1, 0], [0, -4, 2, 1],
-                                               [1, 2/3, -4, 4/3], [0, 1, 0, -4]])
+    assert np.allclose(fld.a_vx_vx.toarray(), [[-4, 4 / 3, 1, 0], [0, -4, 2, 1],
+                                               [1, 2 / 3, -4, 4 / 3], [0, 1, 0, -4]])
+    assert np.allclose(fld.a_vy_vy.toarray(), [[-4, 4 / 3, 1, 0], [0, -4, 2, 1],
+                                               [1, 2 / 3, -4, 4 / 3], [0, 1, 0, -4]])
```

### Comparing `pyfds-0.1.6/test/test_fields.py` & `pyfds-0.2.0/test/test_fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,20 +18,30 @@
     assert np.allclose(fc.values[[5, 6, 7]], [23, 23, 23])
 
 
 def test_field_component_boundary_2():
     fc = fls.FieldComponent(100)
     fc.values = np.ones(100)
     fc.boundaries = [reg.Boundary(reg.LineRegion([5, 6, 7], [0, 0.2], 'test boundary'))]
-    fc.boundaries[0].value = [23, 42, 23]
+    fc.boundaries[0].value = [np.arange(0, 3) * 23, np.arange(0, 3) * 42, np.arange(0, 3) * 23]
     fc.boundaries[0].additive = True
-    fc.apply_bounds(step=0)
+    fc.apply_bounds(step=1)
     assert np.allclose(fc.values[[5, 6, 7]], [24, 43, 24])
 
 
+def test_field_component_boundary_3():
+    fc = fls.FieldComponent(100)
+    fc.values = np.ones(100)
+    fc.boundaries = [reg.Boundary(reg.LineRegion([5, 6, 7], [0, 0.2], 'test boundary'))]
+    fc.boundaries[0].value = np.arange(0, 3) * 23
+    fc.boundaries[0].additive = True
+    fc.apply_bounds(step=2)
+    assert np.allclose(fc.values[[5, 6, 7]], [47, 47, 47])
+
+
 def test_field_component_output():
     fc = fls.FieldComponent(100)
     fc.outputs = [reg.Output(reg.LineRegion([0, 1, 2], [0, 0.2], 'test output'))]
     fc.write_outputs()
     fc.write_outputs()
     assert np.allclose(fc.outputs[0].signals, [[0, 0], [0, 0], [0, 0]])
     assert np.allclose(fc.outputs[0].mean_signal, np.zeros(2))
```

