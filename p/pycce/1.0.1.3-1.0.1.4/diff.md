# Comparing `tmp/pycce-1.0.1.3.tar.gz` & `tmp/pycce-1.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PyCCE/PyCCE/dist/tmpmdohllj0/pycce-1.0.1.3.tar", last modified: Sun Jun  5 03:36:33 2022, max compression
+gzip compressed data, was "/home/runner/work/PyCCE/PyCCE/dist/.tmp-j40mfljb/pycce-1.0.1.4.tar", last modified: Fri Jun 30 16:35:50 2023, max compression
```

## Comparing `pycce-1.0.1.3.tar` & `pycce-1.0.1.4.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 03:36:33.000000 pycce-1.0.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-06-05 03:36:19.000000 pycce-1.0.1.3/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-05 03:36:19.000000 pycce-1.0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-06-05 03:36:33.000000 pycce-1.0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-06-05 03:36:19.000000 pycce-1.0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 03:36:33.000000 pycce-1.0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-05 03:36:19.000000 pycce-1.0.1.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce/bath/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/bath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    63692 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/bath/array.py
--rw-r--r--   0 runner    (1001) docker     (121)    27636 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/bath/cell.py
--rw-r--r--   0 runner    (1001) docker     (121)    12027 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/bath/cube.py
--rw-r--r--   0 runner    (1001) docker     (121)    23293 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/bath/isotopes.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11908 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/bath/map.py
--rw-r--r--   0 runner    (1001) docker     (121)    14684 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/bath/state.py
--rw-r--r--   0 runner    (1001) docker     (121)    36195 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/center.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3417 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    22108 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/find_clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce/h/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/h/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3839 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/h/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    20574 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/h/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6892 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/h/total.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce/io/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7599 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/io/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6011 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/io/orca.py
--rw-r--r--   0 runner    (1001) docker     (121)    27241 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/io/qe.py
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/io/xyz.py
--rw-r--r--   0 runner    (1001) docker     (121)    50447 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce/run/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30818 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/run/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    23349 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/run/cce.py
--rw-r--r--   0 runner    (1001) docker     (121)    16467 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/run/clusters.py
--rw-r--r--   0 runner    (1001) docker     (121)    10405 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/run/corr.py
--rw-r--r--   0 runner    (1001) docker     (121)    17734 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/run/gcce.py
--rw-r--r--   0 runner    (1001) docker     (121)     4773 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/run/mc.py
--rw-r--r--   0 runner    (1001) docker     (121)    12419 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/run/pulses.py
--rw-r--r--   0 runner    (1001) docker     (121)     7026 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/sm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce/u/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/u/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5883 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/u/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    10820 2022-06-05 03:36:19.000000 pycce-1.0.1.3/pycce/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-05 03:36:33.000000 pycce-1.0.1.3/pycce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-05 03:36:33.000000 pycce-1.0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-06-05 03:36:19.000000 pycce-1.0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 16:35:40.000000 pycce-1.0.1.4/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 16:35:40.000000 pycce-1.0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 16:35:50.000000 pycce-1.0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-30 16:35:40.000000 pycce-1.0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 16:35:40.000000 pycce-1.0.1.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce/bath/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/bath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63692 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/bath/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27636 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/bath/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/bath/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/bath/isotopes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/bath/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/bath/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36200 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22108 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/find_clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce/h/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/h/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/h/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/h/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/h/total.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/io/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27241 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/io/qe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/io/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50447 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce/run/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30818 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/run/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23349 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/run/cce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/run/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/run/corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17734 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/run/gcce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/run/mc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/run/pulses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/sm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce/u/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/u/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/u/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-06-30 16:35:40.000000 pycce-1.0.1.4/pycce/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 16:35:50.000000 pycce-1.0.1.4/pycce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:35:50.000000 pycce-1.0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-30 16:35:40.000000 pycce-1.0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:35:50.000000 pycce-1.0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 16:35:40.000000 pycce-1.0.1.4/tests/test_pycce.py
```

### Comparing `pycce-1.0.1.3/LICENCE.md` & `pycce-1.0.1.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/PKG-INFO` & `pycce-1.0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycce
-Version: 1.0.1.3
+Version: 1.0.1.4
 Summary: A package to compute spin dynamics using CCE method
 Home-page: 
 Author: Nikita Onizhuk
 Author-email: onizhuk@uchicago.edu
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
```

### Comparing `pycce-1.0.1.3/README.md` & `pycce-1.0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/bath/array.py` & `pycce-1.0.1.4/pycce/bath/array.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/bath/cell.py` & `pycce-1.0.1.4/pycce/bath/cell.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/bath/cube.py` & `pycce-1.0.1.4/pycce/bath/cube.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/bath/isotopes.txt` & `pycce-1.0.1.4/pycce/bath/isotopes.txt`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/bath/map.py` & `pycce-1.0.1.4/pycce/bath/map.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/bath/state.py` & `pycce-1.0.1.4/pycce/bath/state.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/center.py` & `pycce-1.0.1.4/pycce/center.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
             bath (BathArray with shape (m,) or ndarray with shape (m, 3, 3):
                 Array of all bath spins or array of hyperfine tensors.
             projected_bath_state (ndarray with shape (m,) or (m, 3)):
                 Array of :math:`I_z` projections for each bath spin.
         """
 
         self.generate_hamiltonian(magnetic_field=magnetic_field, bath=bath, projected_bath_state=projected_bath_state)
-        self.energies, self.eigenvectors = np.linalg.eigh(self.hamiltonian, UPLO='U')
+        self.energies, self.eigenvectors = np.linalg.eigh(self.hamiltonian.data, UPLO='U')
 
         if self.alpha_index is not None:
             self._alpha = np.ascontiguousarray(self.eigenvectors[:, self.alpha_index])
         if self.beta_index is not None:
             self._beta = np.ascontiguousarray(self.eigenvectors[:, self.beta_index])
 
     def __repr__(self):
```

### Comparing `pycce-1.0.1.3/pycce/constants.py` & `pycce-1.0.1.4/pycce/constants.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/filter.py` & `pycce-1.0.1.4/pycce/filter.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/find_clusters.py` & `pycce-1.0.1.4/pycce/find_clusters.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/h/base.py` & `pycce-1.0.1.4/pycce/h/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,20 @@
 
     def __setitem__(self, key, value):
         self.data.__setitem__(key, value)
 
     def __delitem__(self, key):
         self.data.__delitem__(key)
 
-    def __getattr__(self, item):
-        if item in dir(self):
-            return getattr(self, item)
-        else:
-            return getattr(self.data, item)
+    #
+    # def __getattr__(self, item):
+    #     if item in dir(self):
+    #         return getattr(self, item)
+    #     else:
+    #         return getattr(self.data, item)
 
     @classmethod
     def from_bath(cls, bath, center=None):
         dim, vectors = dimensions_spinvectors(bath, central_spin=center)
         return cls(dim, vectors=vectors)
 
     def __add__(self, other):
```

### Comparing `pycce-1.0.1.3/pycce/h/functions.py` & `pycce-1.0.1.4/pycce/h/functions.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/h/total.py` & `pycce-1.0.1.4/pycce/h/total.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/io/base.py` & `pycce-1.0.1.4/pycce/io/base.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/io/orca.py` & `pycce-1.0.1.4/pycce/io/orca.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/io/qe.py` & `pycce-1.0.1.4/pycce/io/qe.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/io/xyz.py` & `pycce-1.0.1.4/pycce/io/xyz.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/main.py` & `pycce-1.0.1.4/pycce/main.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/run/base.py` & `pycce-1.0.1.4/pycce/run/base.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/run/cce.py` & `pycce-1.0.1.4/pycce/run/cce.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/run/clusters.py` & `pycce-1.0.1.4/pycce/run/clusters.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/run/corr.py` & `pycce-1.0.1.4/pycce/run/corr.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/run/gcce.py` & `pycce-1.0.1.4/pycce/run/gcce.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/run/mc.py` & `pycce-1.0.1.4/pycce/run/mc.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,15 +135,16 @@
             if self.masked is not None:
                 if rank == 0:
                     divider_shape = divider.shape
                 else:
                     divider_shape = None
 
                 divider_shape = comm.bcast(divider_shape, root=0)
-
+                if np.array(divider).shape != divider_shape:
+                    divider = np.zeros(divider_shape, dtype=np.int32)
                 root_divider = np.zeros(divider_shape, dtype=np.int32)
                 comm.Allreduce(divider, root_divider, MPI.SUM)
 
         else:
             root_result = total
             if self.masked is not None:
                 root_divider = divider
```

### Comparing `pycce-1.0.1.3/pycce/run/pulses.py` & `pycce-1.0.1.4/pycce/run/pulses.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/sm.py` & `pycce-1.0.1.4/pycce/sm.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/u/base.py` & `pycce-1.0.1.4/pycce/u/base.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce/utilities.py` & `pycce-1.0.1.4/pycce/utilities.py`

 * *Files identical despite different names*

### Comparing `pycce-1.0.1.3/pycce.egg-info/PKG-INFO` & `pycce-1.0.1.4/pycce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycce
-Version: 1.0.1.3
+Version: 1.0.1.4
 Summary: A package to compute spin dynamics using CCE method
 Home-page: 
 Author: Nikita Onizhuk
 Author-email: onizhuk@uchicago.edu
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
```

### Comparing `pycce-1.0.1.3/pycce.egg-info/SOURCES.txt` & `pycce-1.0.1.4/pycce.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 pycce/run/cce.py
 pycce/run/clusters.py
 pycce/run/corr.py
 pycce/run/gcce.py
 pycce/run/mc.py
 pycce/run/pulses.py
 pycce/u/__init__.py
-pycce/u/base.py
+pycce/u/base.py
+tests/test_pycce.py
```

### Comparing `pycce-1.0.1.3/setup.py` & `pycce-1.0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name='pycce',
-    version='1.0.1.3',
+    version='1.0.1.4',
     url='',
     license='',
     author='Nikita Onizhuk',
     author_email='onizhuk@uchicago.edu',
     description='A package to compute spin dynamics using CCE method',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

