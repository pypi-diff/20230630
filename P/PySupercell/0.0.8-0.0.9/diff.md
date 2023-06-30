# Comparing `tmp/PySupercell-0.0.8.tar.gz` & `tmp/PySupercell-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySupercell-0.0.8.tar", last modified: Sun Jun  4 08:44:37 2023, max compression
+gzip compressed data, was "PySupercell-0.0.9.tar", last modified: Sun Jun  4 11:17:47 2023, max compression
```

## Comparing `PySupercell-0.0.8.tar` & `PySupercell-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.866731 PySupercell-0.0.8/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 15:54:33.000000 PySupercell-0.0.8/LICENSE.txt
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      204 2023-06-04 08:16:08.000000 PySupercell-0.0.8/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      499 2023-06-04 08:44:37.866731 PySupercell-0.0.8/PKG-INFO
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.854731 PySupercell-0.0.8/PySupercell.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      499 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1344 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       23 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-04 08:44:37.000000 PySupercell-0.0.8/PySupercell.egg-info/top_level.txt
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 15:54:33.000000 PySupercell-0.0.8/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.854731 PySupercell-0.0.8/bin/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10217 2023-06-03 15:54:33.000000 PySupercell-0.0.8/bin/pysc
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    11607 2023-06-04 07:24:48.000000 PySupercell-0.0.8/bin/v2qe
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.854731 PySupercell-0.0.8/examples/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.858731 PySupercell-0.0.8/examples/example1/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      364 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example1/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      369 2023-06-04 07:23:49.000000 PySupercell-0.0.8/examples/example1/POSCAR_1
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      376 2023-06-04 08:41:34.000000 PySupercell-0.0.8/examples/example1/POSCAR_Primitive
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      824 2023-06-04 08:15:00.000000 PySupercell-0.0.8/examples/example1/POSCAR_redefine
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1582 2023-06-04 08:15:01.000000 PySupercell-0.0.8/examples/example1/POSCAR_slab_111
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      735 2023-06-04 07:23:49.000000 PySupercell-0.0.8/examples/example1/POSCAR_std
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      676 2023-06-04 08:39:59.000000 PySupercell-0.0.8/examples/example1/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.858731 PySupercell-0.0.8/examples/example1/reference/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      704 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example1/reference/POSCAR_redefine
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1312 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example1/reference/POSCAR_slab
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      610 2023-06-04 08:41:34.000000 PySupercell-0.0.8/examples/example1/rx.in
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      761 2023-06-04 07:23:48.000000 PySupercell-0.0.8/examples/example1/test_phonopy.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.858731 PySupercell-0.0.8/examples/example2/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      437 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example2/POSCAR
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12072 2023-06-04 08:15:04.000000 PySupercell-0.0.8/examples/example2/POSCAR_sc
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12078 2023-06-04 08:15:04.000000 PySupercell-0.0.8/examples/example2/POSCAR_tube_4_6
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)       34 2023-06-04 08:39:59.000000 PySupercell-0.0.8/examples/example2/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example2/reference/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9732 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example2/reference/POSCAR_sc
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9738 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example2/reference/POSCAR_tube
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example3/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      948 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/POSCAR
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54936 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/POSCAR_redefine
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      596 2023-06-04 08:39:59.000000 PySupercell-0.0.8/examples/example3/README.md
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/make_screw_diamond.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example3/reference/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44136 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/reference/POSCAR_redefine
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54957 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example3/reference/POSCAR_screw
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example4/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      534 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example4/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     2656 2023-06-04 08:15:08.000000 PySupercell-0.0.8/examples/example4/POSCAR_bending
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     2648 2023-06-04 08:15:07.000000 PySupercell-0.0.8/examples/example4/POSCAR_flat
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      118 2023-06-04 08:39:59.000000 PySupercell-0.0.8/examples/example4/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.862731 PySupercell-0.0.8/examples/example4/reference/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2176 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example4/reference/POSCAR_bending
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2168 2023-06-03 15:54:34.000000 PySupercell-0.0.8/examples/example4/reference/POSCAR_flat
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1794 2023-06-04 08:39:31.000000 PySupercell-0.0.8/examples/run_all_examples.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 08:44:37.866731 PySupercell-0.0.8/pysupercell/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8665 2023-06-03 15:54:34.000000 PySupercell-0.0.8/pysupercell/QE_ibrav_lib.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      293 2023-06-04 08:40:44.000000 PySupercell-0.0.8/pysupercell/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4589 2023-06-04 07:02:36.000000 PySupercell-0.0.8/pysupercell/arguments.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44519 2023-06-04 08:43:58.000000 PySupercell-0.0.8/pysupercell/pysupercell.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-04 08:44:37.866731 PySupercell-0.0.8/setup.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3782 2023-06-04 08:44:33.000000 PySupercell-0.0.8/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:47.007823 PySupercell-0.0.9/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 15:54:33.000000 PySupercell-0.0.9/LICENSE.txt
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      204 2023-06-04 08:16:08.000000 PySupercell-0.0.9/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      499 2023-06-04 11:17:47.003823 PySupercell-0.0.9/PKG-INFO
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:46.991823 PySupercell-0.0.9/PySupercell.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      499 2023-06-04 11:17:46.000000 PySupercell-0.0.9/PySupercell.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1344 2023-06-04 11:17:46.000000 PySupercell-0.0.9/PySupercell.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-04 11:17:46.000000 PySupercell-0.0.9/PySupercell.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       23 2023-06-04 11:17:46.000000 PySupercell-0.0.9/PySupercell.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-04 11:17:46.000000 PySupercell-0.0.9/PySupercell.egg-info/top_level.txt
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 15:54:33.000000 PySupercell-0.0.9/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:46.991823 PySupercell-0.0.9/bin/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10217 2023-06-03 15:54:33.000000 PySupercell-0.0.9/bin/pysc
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    11607 2023-06-04 07:24:48.000000 PySupercell-0.0.9/bin/v2qe
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:46.991823 PySupercell-0.0.9/examples/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:46.995823 PySupercell-0.0.9/examples/example1/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      364 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example1/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      369 2023-06-04 07:23:49.000000 PySupercell-0.0.9/examples/example1/POSCAR_1
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      376 2023-06-04 08:41:34.000000 PySupercell-0.0.9/examples/example1/POSCAR_Primitive
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      824 2023-06-04 08:15:00.000000 PySupercell-0.0.9/examples/example1/POSCAR_redefine
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1582 2023-06-04 08:15:01.000000 PySupercell-0.0.9/examples/example1/POSCAR_slab_111
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      735 2023-06-04 07:23:49.000000 PySupercell-0.0.9/examples/example1/POSCAR_std
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      676 2023-06-04 08:39:59.000000 PySupercell-0.0.9/examples/example1/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:46.995823 PySupercell-0.0.9/examples/example1/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      704 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example1/reference/POSCAR_redefine
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1312 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example1/reference/POSCAR_slab
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      610 2023-06-04 08:41:34.000000 PySupercell-0.0.9/examples/example1/rx.in
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)      761 2023-06-04 07:23:48.000000 PySupercell-0.0.9/examples/example1/test_phonopy.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:46.995823 PySupercell-0.0.9/examples/example2/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      437 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example2/POSCAR
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12072 2023-06-04 08:15:04.000000 PySupercell-0.0.9/examples/example2/POSCAR_sc
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12078 2023-06-04 08:15:04.000000 PySupercell-0.0.9/examples/example2/POSCAR_tube_4_6
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)       34 2023-06-04 08:39:59.000000 PySupercell-0.0.9/examples/example2/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:46.995823 PySupercell-0.0.9/examples/example2/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9732 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example2/reference/POSCAR_sc
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9738 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example2/reference/POSCAR_tube
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:46.999823 PySupercell-0.0.9/examples/example3/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      948 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example3/POSCAR
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54936 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example3/POSCAR_redefine
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      596 2023-06-04 08:39:59.000000 PySupercell-0.0.9/examples/example3/README.md
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example3/make_screw_diamond.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:46.999823 PySupercell-0.0.9/examples/example3/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44136 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example3/reference/POSCAR_redefine
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    54957 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example3/reference/POSCAR_screw
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:47.003823 PySupercell-0.0.9/examples/example4/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      534 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example4/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     2656 2023-06-04 08:15:08.000000 PySupercell-0.0.9/examples/example4/POSCAR_bending
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     2648 2023-06-04 08:15:07.000000 PySupercell-0.0.9/examples/example4/POSCAR_flat
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      118 2023-06-04 08:39:59.000000 PySupercell-0.0.9/examples/example4/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:47.003823 PySupercell-0.0.9/examples/example4/reference/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2176 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example4/reference/POSCAR_bending
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2168 2023-06-03 15:54:34.000000 PySupercell-0.0.9/examples/example4/reference/POSCAR_flat
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1794 2023-06-04 08:39:31.000000 PySupercell-0.0.9/examples/run_all_examples.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-04 11:17:47.003823 PySupercell-0.0.9/pysupercell/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8665 2023-06-03 15:54:34.000000 PySupercell-0.0.9/pysupercell/QE_ibrav_lib.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)      293 2023-06-04 08:44:38.000000 PySupercell-0.0.9/pysupercell/__init__.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4589 2023-06-04 07:02:36.000000 PySupercell-0.0.9/pysupercell/arguments.py
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    44519 2023-06-04 08:43:58.000000 PySupercell-0.0.9/pysupercell/pysupercell.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-04 11:17:47.007823 PySupercell-0.0.9/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3782 2023-06-04 11:17:41.000000 PySupercell-0.0.9/setup.py
```

### Comparing `PySupercell-0.0.8/LICENSE.txt` & `PySupercell-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/PySupercell.egg-info/SOURCES.txt` & `PySupercell-0.0.9/PySupercell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/README.md` & `PySupercell-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/bin/pysc` & `PySupercell-0.0.9/bin/pysc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/bin/v2qe` & `PySupercell-0.0.9/bin/v2qe`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example1/POSCAR_redefine` & `PySupercell-0.0.9/examples/example1/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example1/POSCAR_slab_111` & `PySupercell-0.0.9/examples/example1/POSCAR_slab_111`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example1/POSCAR_std` & `PySupercell-0.0.9/examples/example1/POSCAR_std`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example1/README.md` & `PySupercell-0.0.9/examples/example1/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example1/reference/POSCAR_redefine` & `PySupercell-0.0.9/examples/example1/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example1/reference/POSCAR_slab` & `PySupercell-0.0.9/examples/example1/reference/POSCAR_slab`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example1/rx.in` & `PySupercell-0.0.9/examples/example1/rx.in`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example1/test_phonopy.py` & `PySupercell-0.0.9/examples/example1/test_phonopy.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example2/POSCAR_sc` & `PySupercell-0.0.9/examples/example2/POSCAR_sc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example2/POSCAR_tube_4_6` & `PySupercell-0.0.9/examples/example2/POSCAR_tube_4_6`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example2/reference/POSCAR_sc` & `PySupercell-0.0.9/examples/example2/reference/POSCAR_sc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example2/reference/POSCAR_tube` & `PySupercell-0.0.9/examples/example2/reference/POSCAR_tube`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example3/POSCAR` & `PySupercell-0.0.9/examples/example3/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example3/POSCAR_redefine` & `PySupercell-0.0.9/examples/example3/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example3/README.md` & `PySupercell-0.0.9/examples/example3/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example3/make_screw_diamond.py` & `PySupercell-0.0.9/examples/example3/make_screw_diamond.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example3/reference/POSCAR_redefine` & `PySupercell-0.0.9/examples/example3/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example3/reference/POSCAR_screw` & `PySupercell-0.0.9/examples/example3/reference/POSCAR_screw`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example4/POSCAR` & `PySupercell-0.0.9/examples/example4/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example4/POSCAR_bending` & `PySupercell-0.0.9/examples/example4/POSCAR_bending`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example4/POSCAR_flat` & `PySupercell-0.0.9/examples/example4/POSCAR_flat`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example4/reference/POSCAR_bending` & `PySupercell-0.0.9/examples/example4/reference/POSCAR_bending`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/example4/reference/POSCAR_flat` & `PySupercell-0.0.9/examples/example4/reference/POSCAR_flat`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/examples/run_all_examples.py` & `PySupercell-0.0.9/examples/run_all_examples.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/pysupercell/QE_ibrav_lib.py` & `PySupercell-0.0.9/pysupercell/QE_ibrav_lib.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/pysupercell/arguments.py` & `PySupercell-0.0.9/pysupercell/arguments.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/pysupercell/pysupercell.py` & `PySupercell-0.0.9/pysupercell/pysupercell.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.8/setup.py` & `PySupercell-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 print ('It has been added to ~/.bashrc')
                 print ('Run "source ~/.bashrc" to activate it')
                 add_binpath = 'echo "{0}"|cat >>~/.bashrc'.format(binpath)
                 os.system(add_binpath)
             else:  
                 print ('The utility directory already in the path\n')
         else:
-            print ('You are using {} operating system'.format(sys.plotform))
+            print ('You are using {} operating system'.format(sys.platform))
             print ('Please set the environment variable manually')
 
 
 
 def test_modules(module_list,desc,pkg='asd'):
     import importlib
     import glob
@@ -71,15 +71,15 @@
 scripts_pysupercell = ['bin/pysc','bin/v2qe']
 
 long_desc="A Open-source Python library for playing with crystal structures, such as supercell, dislocation, slab, and nanotube"
 
 
 kwargs_setup=dict(
 name='PySupercell',
-version='0.0.8',
+version='0.0.9',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords=['Python','Crystal structure','supercell'],
 py_modules=core_modules,
 license="MIT License",
```

