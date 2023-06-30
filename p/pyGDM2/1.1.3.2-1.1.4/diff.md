# Comparing `tmp/pyGDM2-1.1.3.2.tar.gz` & `tmp/pyGDM2-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGDM2-1.1.3.2.tar", last modified: Thu Jul  7 10:33:41 2022, max compression
+gzip compressed data, was "pyGDM2-1.1.4.tar", last modified: Fri Jun 30 08:52:52 2023, max compression
```

## Comparing `pyGDM2-1.1.3.2.tar` & `pyGDM2-1.1.4.tar`

### file list

```diff
@@ -1,97 +1,102 @@
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.188863 pyGDM2-1.1.3.2/
--rw-rw-r--   0 hans      (1000) hans      (1000)    35183 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/LICENSE.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)       83 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/MANIFEST.in
--rw-rw-r--   0 hans      (1000) hans      (1000)     5878 2022-07-07 10:33:41.188863 pyGDM2-1.1.3.2/PKG-INFO
--rw-rw-r--   0 hans      (1000) hans      (1000)     4912 2022-07-07 10:33:16.000000 pyGDM2-1.1.3.2/README.rst
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.024863 pyGDM2-1.1.3.2/examples/
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.064863 pyGDM2-1.1.3.2/examples/01_Mie/
--rw-rw-r--   0 hans      (1000) hans      (1000)     5585 2020-02-25 17:30:31.000000 pyGDM2-1.1.3.2/examples/01_Mie/example_mie_01_n2.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3174 2020-11-30 11:24:51.000000 pyGDM2-1.1.3.2/examples/01_Mie/example_mie_02_Au.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3755 2020-02-25 17:30:31.000000 pyGDM2-1.1.3.2/examples/01_Mie/example_mie_03_Si.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    16059 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/01_Mie/scat_mie_Au_D50nm.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)    15042 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/01_Mie/scat_mie_Si_D150nm.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)    16039 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/01_Mie/scat_mie_n2_D300nm.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)     1396 2021-05-10 19:30:14.000000 pyGDM2-1.1.3.2/examples/01_simple_simulation.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.084863 pyGDM2-1.1.3.2/examples/02_other_examples/
--rw-rw-r--   0 hans      (1000) hans      (1000)     3260 2020-02-25 17:30:31.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_01_SiSphere_FW_BW.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4090 2020-11-30 11:24:51.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_02_splitring_dipole_farfield.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3201 2020-02-25 17:30:31.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_03_Lshape_polarconversion.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3275 2020-11-30 11:24:51.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_04_heat.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3197 2019-06-07 07:06:07.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_05_decayrate.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     5128 2020-02-25 17:30:31.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_06_rasterscan_thermoplasmonics.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4043 2020-02-25 17:30:31.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_07_rasterscan_LDOS.py
--rwxrwxr-x   0 hans      (1000) hans      (1000)      106 2018-07-09 08:53:23.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_08_run_via_mpi.sh
--rw-rw-r--   0 hans      (1000) hans      (1000)     2023 2019-06-07 07:06:07.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_08_spectra_via_MPI.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2974 2020-02-25 17:30:31.000000 pyGDM2-1.1.3.2/examples/02_other_examples/example_other_09_multipole_decomposition.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.108863 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/
--rw-rw-r--   0 hans      (1000) hans      (1000)     5033 2019-06-07 07:06:07.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_01_scattering.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2556 2019-06-07 07:06:07.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_01b_scattering_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3086 2019-06-07 07:06:07.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_02_nearfield.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2332 2019-06-07 07:06:07.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_02b_nearfield_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     6331 2020-02-25 17:30:31.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_03_multi_objective.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3745 2020-02-25 17:30:31.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_03b_multi_objective_analyze.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.128863 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.132863 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/eo_out/
--rw-rw-r--   0 hans      (1000) hans      (1000)       52 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/eo_out/readme.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)     3282 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_01_eo.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     1793 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_02_eo_load_final.py
--rw-rw-r--   0 hans      (1000) hans      (1000)      598 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_03_eo_continue_optimization.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4582 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04_ownproblem.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2845 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04b_ownproblem_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     5845 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05_ownmodel.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3030 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05b_ownmodel_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3160 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06_maximize_nearfield.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2140 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06b_maximize_nearfield_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     5199 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07_multi_objective_problem.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     3273 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07b_MO_analyze.py
--rw-rw-r--   0 hans      (1000) hans      (1000)      146 2019-06-07 07:06:07.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/readme.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)      280 2018-02-12 08:58:24.000000 pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/readme.txt
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.140863 pyGDM2-1.1.3.2/examples/04_tutorials/
--rw-rw-r--   0 hans      (1000) hans      (1000)     4753 2019-11-21 14:42:24.000000 pyGDM2-1.1.3.2/examples/04_tutorials/surface_plasmon.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    40882 2022-07-07 10:33:16.000000 pyGDM2-1.1.3.2/examples/04_tutorials/surface_plasmon_gold.png
--rw-rw-r--   0 hans      (1000) hans      (1000)    31794 2022-07-07 10:33:16.000000 pyGDM2-1.1.3.2/examples/04_tutorials/surface_plasmon_silicon.png
--rw-rw-r--   0 hans      (1000) hans      (1000)     2100 2020-11-30 11:24:51.000000 pyGDM2-1.1.3.2/examples/04_tutorials/using_callbacks.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     2278 2020-11-30 11:24:51.000000 pyGDM2-1.1.3.2/examples/04_tutorials/visualize_incident_field.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    40664 2020-03-25 20:50:47.000000 pyGDM2-1.1.3.2/examples/examples.tar.gz
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.156863 pyGDM2-1.1.3.2/pyGDM2/
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.160863 pyGDM2-1.1.3.2/pyGDM2/EO/
--rw-rw-r--   0 hans      (1000) hans      (1000)     1099 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/EO/__init__.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    13621 2021-05-10 19:30:14.000000 pyGDM2-1.1.3.2/pyGDM2/EO/core.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    29883 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/EO/models.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    16581 2021-05-10 19:30:14.000000 pyGDM2-1.1.3.2/pyGDM2/EO/problems.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    21322 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/EO/tools.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     1461 2022-07-07 10:33:16.000000 pyGDM2-1.1.3.2/pyGDM2/__init__.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    49201 2022-07-07 10:33:16.000000 pyGDM2-1.1.3.2/pyGDM2/core.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     9309 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/electron.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.160863 pyGDM2-1.1.3.2/pyGDM2/fields/
--rw-rw-r--   0 hans      (1000) hans      (1000)     2017 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/fields/__init__.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    47658 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/fields/deprecated.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     5187 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/fields/efield_class.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4976 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/fields/electron.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    54581 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/fields/focused_beams.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    35781 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/fields/regular.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    59941 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/linear.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    57352 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/materials.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    75971 2022-07-07 10:33:16.000000 pyGDM2-1.1.3.2/pyGDM2/multipole.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     4691 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/nonlinear.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.168863 pyGDM2-1.1.3.2/pyGDM2/propagators/
--rw-rw-r--   0 hans      (1000) hans      (1000)     1892 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/propagators/__init__.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    35658 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/propagators/propagators.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    36147 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/propagators/propagators_2D.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    53212 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/propagators/propagators_periodic.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    24901 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/propagators/propagators_periodic_slow.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    81917 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/structures.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    90486 2022-07-07 10:33:16.000000 pyGDM2-1.1.3.2/pyGDM2/tools.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    43856 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/visu.py
--rw-rw-r--   0 hans      (1000) hans      (1000)    27130 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/pyGDM2/visu3d.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.156863 pyGDM2-1.1.3.2/pyGDM2.egg-info/
--rw-rw-r--   0 hans      (1000) hans      (1000)     5878 2022-07-07 10:33:40.000000 pyGDM2-1.1.3.2/pyGDM2.egg-info/PKG-INFO
--rw-rw-r--   0 hans      (1000) hans      (1000)     3584 2022-07-07 10:33:40.000000 pyGDM2-1.1.3.2/pyGDM2.egg-info/SOURCES.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)        1 2022-07-07 10:33:40.000000 pyGDM2-1.1.3.2/pyGDM2.egg-info/dependency_links.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)       12 2022-07-07 10:33:40.000000 pyGDM2-1.1.3.2/pyGDM2.egg-info/requires.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)        7 2022-07-07 10:33:40.000000 pyGDM2-1.1.3.2/pyGDM2.egg-info/top_level.txt
--rw-rw-r--   0 hans      (1000) hans      (1000)       80 2022-07-07 10:33:41.188863 pyGDM2-1.1.3.2/setup.cfg
--rw-rw-r--   0 hans      (1000) hans      (1000)     6071 2022-04-26 20:46:57.000000 pyGDM2-1.1.3.2/setup.py
-drwxrwxr-x   0 hans      (1000) hans      (1000)        0 2022-07-07 10:33:41.172863 pyGDM2-1.1.3.2/tests/
--rw-rw-r--   0 hans      (1000) hans      (1000)    14956 2020-11-30 11:24:51.000000 pyGDM2-1.1.3.2/tests/basic_tests.py
--rw-rw-r--   0 hans      (1000) hans      (1000)     1337 2020-12-04 22:18:43.000000 pyGDM2-1.1.3.2/tests/tests_propagators.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.735811 pyGDM2-1.1.4/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    35183 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/LICENSE.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)       83 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/MANIFEST.in
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5933 2023-06-30 08:52:52.735811 pyGDM2-1.1.4/PKG-INFO
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4912 2022-07-07 10:33:16.000000 pyGDM2-1.1.4/README.rst
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.727810 pyGDM2-1.1.4/examples/
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.727810 pyGDM2-1.1.4/examples/01_Mie/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5585 2020-02-25 17:30:31.000000 pyGDM2-1.1.4/examples/01_Mie/example_mie_01_n2.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3174 2020-11-30 11:24:51.000000 pyGDM2-1.1.4/examples/01_Mie/example_mie_02_Au.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3755 2020-02-25 17:30:31.000000 pyGDM2-1.1.4/examples/01_Mie/example_mie_03_Si.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    16059 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/01_Mie/scat_mie_Au_D50nm.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    15042 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/01_Mie/scat_mie_Si_D150nm.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    16039 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/01_Mie/scat_mie_n2_D300nm.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1396 2021-05-10 19:30:14.000000 pyGDM2-1.1.4/examples/01_simple_simulation.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.731811 pyGDM2-1.1.4/examples/02_other_examples/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3260 2020-02-25 17:30:31.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_01_SiSphere_FW_BW.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4090 2020-11-30 11:24:51.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_02_splitring_dipole_farfield.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3201 2020-02-25 17:30:31.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_03_Lshape_polarconversion.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3275 2020-11-30 11:24:51.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_04_heat.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3197 2019-06-07 07:06:07.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_05_decayrate.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5128 2020-02-25 17:30:31.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_06_rasterscan_thermoplasmonics.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4043 2020-02-25 17:30:31.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_07_rasterscan_LDOS.py
+-rwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)      106 2018-07-09 08:53:23.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_08_run_via_mpi.sh
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2023 2019-06-07 07:06:07.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_08_spectra_via_MPI.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2974 2020-02-25 17:30:31.000000 pyGDM2-1.1.4/examples/02_other_examples/example_other_09_multipole_decomposition.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.731811 pyGDM2-1.1.4/examples/03_evolutionary_optimization/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5033 2019-06-07 07:06:07.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_01_scattering.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2556 2019-06-07 07:06:07.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_01b_scattering_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3086 2019-06-07 07:06:07.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_02_nearfield.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2332 2019-06-07 07:06:07.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_02b_nearfield_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     6331 2020-02-25 17:30:31.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_03_multi_objective.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3745 2020-02-25 17:30:31.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_03b_multi_objective_analyze.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.731811 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.731811 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/eo_out/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)       52 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/eo_out/readme.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3282 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_01_eo.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1793 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_02_eo_load_final.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)      598 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_03_eo_continue_optimization.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4582 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04_ownproblem.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2845 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04b_ownproblem_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5845 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05_ownmodel.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3030 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05b_ownmodel_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3160 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06_maximize_nearfield.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2140 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06b_maximize_nearfield_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5199 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07_multi_objective_problem.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3273 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07b_MO_analyze.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)      146 2019-06-07 07:06:07.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/readme.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)      280 2018-02-12 08:58:24.000000 pyGDM2-1.1.4/examples/03_evolutionary_optimization/readme.txt
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.731811 pyGDM2-1.1.4/examples/04_tutorials/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4753 2019-11-21 14:42:24.000000 pyGDM2-1.1.4/examples/04_tutorials/surface_plasmon.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    40882 2022-07-07 10:33:16.000000 pyGDM2-1.1.4/examples/04_tutorials/surface_plasmon_gold.png
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    31794 2022-07-07 10:33:16.000000 pyGDM2-1.1.4/examples/04_tutorials/surface_plasmon_silicon.png
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2100 2020-11-30 11:24:51.000000 pyGDM2-1.1.4/examples/04_tutorials/using_callbacks.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2278 2020-11-30 11:24:51.000000 pyGDM2-1.1.4/examples/04_tutorials/visualize_incident_field.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    40664 2020-03-25 20:50:47.000000 pyGDM2-1.1.4/examples/examples.tar.gz
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.731811 pyGDM2-1.1.4/pyGDM2/
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.735811 pyGDM2-1.1.4/pyGDM2/EO/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1099 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/EO/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    13621 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/EO/core.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    29885 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/EO/models.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    16581 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/EO/problems.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    21324 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/EO/tools.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1483 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    49201 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/core.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     9309 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/electron.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.735811 pyGDM2-1.1.4/pyGDM2/fields/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2017 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/fields/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    47658 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/fields/deprecated.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5607 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/fields/efield_class.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4976 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/fields/electron.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    54581 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/fields/focused_beams.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    35781 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/fields/regular.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    60267 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/linear.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    57352 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/materials.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.735811 pyGDM2-1.1.4/pyGDM2/multipole/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     2017 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/multipole/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     9260 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/multipole/main.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    29233 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/multipole/polarizabilities.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    56642 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/multipole/processing.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     8025 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/multipole/propagators.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     4691 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/nonlinear.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.735811 pyGDM2-1.1.4/pyGDM2/propagators/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1892 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/propagators/__init__.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    35658 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/propagators/propagators.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    36147 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/propagators/propagators_2D.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    53212 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/propagators/propagators_periodic.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    24901 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/propagators/propagators_periodic_slow.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    82788 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/structures.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    90486 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/tools.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    44118 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/visu.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    27130 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/pyGDM2/visu3d.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.731811 pyGDM2-1.1.4/pyGDM2.egg-info/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     5933 2023-06-30 08:52:52.000000 pyGDM2-1.1.4/pyGDM2.egg-info/PKG-INFO
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     3718 2023-06-30 08:52:52.000000 pyGDM2-1.1.4/pyGDM2.egg-info/SOURCES.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)        1 2023-06-30 08:52:52.000000 pyGDM2-1.1.4/pyGDM2.egg-info/dependency_links.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)       12 2023-06-30 08:52:52.000000 pyGDM2-1.1.4/pyGDM2.egg-info/requires.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)        7 2023-06-30 08:52:52.000000 pyGDM2-1.1.4/pyGDM2.egg-info/top_level.txt
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)       80 2023-06-30 08:52:52.735811 pyGDM2-1.1.4/setup.cfg
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     6069 2023-06-30 08:52:10.000000 pyGDM2-1.1.4/setup.py
+drwxrwxr-x   0 pwiecha   (1000) pwiecha   (1000)        0 2023-06-30 08:52:52.735811 pyGDM2-1.1.4/tests/
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)    14956 2020-11-30 11:24:51.000000 pyGDM2-1.1.4/tests/basic_tests.py
+-rw-rw-r--   0 pwiecha   (1000) pwiecha   (1000)     1337 2020-12-04 22:18:43.000000 pyGDM2-1.1.4/tests/tests_propagators.py
```

### Comparing `pyGDM2-1.1.3.2/LICENSE.txt` & `pyGDM2-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/PKG-INFO` & `pyGDM2-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pyGDM2
-Version: 1.1.3.2
+Version: 1.1.4
 Summary: A python full-field electrodynamical solver, based on the Green dyadic method (volume integral technique in frequency domain).
 Home-page: https://gitlab.com/wiechapeter/pyGDM2
-Download-URL: 
 Author: Peter R. Wiecha
 Author-email: pwiecha@laas.fr
 License: GPLv3+
 Keywords: coupled dipoles method,green dyadic method,electrodynamical simulations,nano optics,frequency-domain
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 ***********************************
 Requirements / Installation
 ***********************************
 
 pyGDM is an open source python toolkit for electro-dynamical simulations, implementing the `Green dyadic method (GDM) <https://doi.org/10.1088/0034-4885/68/8/R05>`_, a volume discretization technique. 
@@ -147,7 +148,9 @@
    - P\. R. Wiecha
 
 
 
    
 
 
+
+
```

### Comparing `pyGDM2-1.1.3.2/README.rst` & `pyGDM2-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/01_Mie/example_mie_01_n2.py` & `pyGDM2-1.1.4/examples/01_Mie/example_mie_01_n2.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/01_Mie/example_mie_02_Au.py` & `pyGDM2-1.1.4/examples/01_Mie/example_mie_02_Au.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/01_Mie/example_mie_03_Si.py` & `pyGDM2-1.1.4/examples/01_Mie/example_mie_03_Si.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/01_Mie/scat_mie_Au_D50nm.txt` & `pyGDM2-1.1.4/examples/01_Mie/scat_mie_Au_D50nm.txt`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/01_Mie/scat_mie_Si_D150nm.txt` & `pyGDM2-1.1.4/examples/01_Mie/scat_mie_Si_D150nm.txt`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/01_Mie/scat_mie_n2_D300nm.txt` & `pyGDM2-1.1.4/examples/01_Mie/scat_mie_n2_D300nm.txt`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/01_simple_simulation.py` & `pyGDM2-1.1.4/examples/01_simple_simulation.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/02_other_examples/example_other_01_SiSphere_FW_BW.py` & `pyGDM2-1.1.4/examples/02_other_examples/example_other_01_SiSphere_FW_BW.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/02_other_examples/example_other_02_splitring_dipole_farfield.py` & `pyGDM2-1.1.4/examples/02_other_examples/example_other_02_splitring_dipole_farfield.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/02_other_examples/example_other_03_Lshape_polarconversion.py` & `pyGDM2-1.1.4/examples/02_other_examples/example_other_03_Lshape_polarconversion.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/02_other_examples/example_other_04_heat.py` & `pyGDM2-1.1.4/examples/02_other_examples/example_other_04_heat.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/02_other_examples/example_other_05_decayrate.py` & `pyGDM2-1.1.4/examples/02_other_examples/example_other_05_decayrate.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/02_other_examples/example_other_06_rasterscan_thermoplasmonics.py` & `pyGDM2-1.1.4/examples/02_other_examples/example_other_06_rasterscan_thermoplasmonics.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/02_other_examples/example_other_07_rasterscan_LDOS.py` & `pyGDM2-1.1.4/examples/02_other_examples/example_other_07_rasterscan_LDOS.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/02_other_examples/example_other_08_spectra_via_MPI.py` & `pyGDM2-1.1.4/examples/02_other_examples/example_other_08_spectra_via_MPI.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/02_other_examples/example_other_09_multipole_decomposition.py` & `pyGDM2-1.1.4/examples/02_other_examples/example_other_09_multipole_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_01_scattering.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_01_scattering.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_01b_scattering_analyze.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_01b_scattering_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_02_nearfield.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_02_nearfield.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_02b_nearfield_analyze.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_02b_nearfield_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_03_multi_objective.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_03_multi_objective.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/example_eo_03b_multi_objective_analyze.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/example_eo_03b_multi_objective_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_01_eo.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_01_eo.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_02_eo_load_final.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_02_eo_load_final.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_03_eo_continue_optimization.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_03_eo_continue_optimization.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04_ownproblem.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04_ownproblem.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04b_ownproblem_analyze.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_04b_ownproblem_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05_ownmodel.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05_ownmodel.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05b_ownmodel_analyze.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_05b_ownmodel_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06_maximize_nearfield.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06_maximize_nearfield.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06b_maximize_nearfield_analyze.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_06b_maximize_nearfield_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07_multi_objective_problem.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07_multi_objective_problem.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07b_MO_analyze.py` & `pyGDM2-1.1.4/examples/03_evolutionary_optimization/pagmo1_API/example_eo_07b_MO_analyze.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/04_tutorials/surface_plasmon.py` & `pyGDM2-1.1.4/examples/04_tutorials/surface_plasmon.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/04_tutorials/surface_plasmon_gold.png` & `pyGDM2-1.1.4/examples/04_tutorials/surface_plasmon_gold.png`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/04_tutorials/surface_plasmon_silicon.png` & `pyGDM2-1.1.4/examples/04_tutorials/surface_plasmon_silicon.png`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/04_tutorials/using_callbacks.py` & `pyGDM2-1.1.4/examples/04_tutorials/using_callbacks.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/04_tutorials/visualize_incident_field.py` & `pyGDM2-1.1.4/examples/04_tutorials/visualize_incident_field.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/examples/examples.tar.gz` & `pyGDM2-1.1.4/examples/examples.tar.gz`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/pyGDM2/EO/__init__.py` & `pyGDM2-1.1.4/pyGDM2/EO/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 pyGDM2.EO - evolutionary optimization toolkit for use with pyGDM2. 
 
 
-    Copyright (C) 2017-2022, P. R. Wiecha
+    Copyright (C) 2017-2023, P. R. Wiecha
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/EO/core.py` & `pyGDM2-1.1.4/pyGDM2/EO/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 Main routines of EO submodule of pyGDM2
 
-    Copyright (C) 2017-2021, P. R. Wiecha
+    Copyright (C) 2017-2023, P. R. Wiecha
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/EO/models.py` & `pyGDM2-1.1.4/pyGDM2/EO/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 Collection of structure models for the EO submodule of pyGDM2
 
-    Copyright (C) 2017-2021, P. R. Wiecha
+    Copyright (C) 2017-2023, P. R. Wiecha
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -565,15 +565,15 @@
         for i, val in enumerate(params):
             if i%2==0:
                 POS.append([])
             ## convention for float-->int parameter conversion: int(round(value))
             val = int(round(val))
             POS[-1].append(val)
         
-        return np.array(POS, dtype=np.float)    
+        return np.array(POS, dtype=np.float32)    
     
         
     def generate_structure(self, params):
         """generate the structure"""
         ## --- collect parameters, exception handling
         if self.fit_offset: 
             positions = self.get_position_tuples(params[:-2])
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/EO/problems.py` & `pyGDM2-1.1.4/pyGDM2/EO/problems.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 Collection of problems for the EO submodule of pyGDM2
 
-    Copyright (C) 2017-2021, P. R. Wiecha
+    Copyright (C) 2017-2023, P. R. Wiecha
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/EO/tools.py` & `pyGDM2-1.1.4/pyGDM2/EO/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # encoding: utf-8
 """
 tools for EO submodule of pyGDM2
 
-    Copyright (C) 2017-2021, P. R. Wiecha
+    Copyright (C) 2017-2023, P. R. Wiecha
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -303,15 +303,15 @@
         allpareto[-1] = np.transpose(allpareto[-1])
         allpareto[-1] *= -1
         allpareto[-1] = np.append(allpareto[-1],[np.arange(len(allpareto[-1][0]))], axis=0)
         allpareto[-1] = allpareto[-1].T
         
         ## sort pareto front and get sorting indices
         if np.shape(allpareto[-1])[0] != 1:    
-            allpareto[-1] = np.sort(allpareto[-1].view('f8,f8,i8'), order=['f1'], axis=0).view(np.float).T
+            allpareto[-1] = np.sort(allpareto[-1].view('f8,f8,i8'), order=['f1'], axis=0).view(np.float32).T
             sort_idx = [int(i) for i in allpareto[-1][2]]
         else:
             ## one single element in Pareto front
             sort_idx = [0]
         allpareto[-1] = -1 * allpareto[-1][:-1].T
         
         ## Sort simulations and parameter vectors according to pareto-front order
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/__init__.py` & `pyGDM2-1.1.4/pyGDM2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
@@ -26,20 +26,20 @@
         - C. Majorel
         - A. Patoux
         - G. Colas des Francs
         - Y. Brûlé
     
 """
 __name__ = 'pyGDM2'
-__version__ = '1.1.3.2'
-__date__ = "07/07/2022"   # MM/DD/YYY
+__version__ = '1.1.4'
+__date__ = "06/30/2023"   # MM/DD/YYY
 __author__ = 'Peter R. Wiecha'
 
 __all__ = ["core", "materials", "structures", "fields", 
-           "propagators", "propagators_2D",
+           "propagators", "propagators_2D", "propagators_periodic",
            "linear", "nonlinear", 
            "tools", "visu", 
            "EO"]
 
 
 ## compatibility with deprecated transition modules:
 from pyGDM2 import core as core_py
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/core.py` & `pyGDM2-1.1.4/pyGDM2/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/electron.py` & `pyGDM2-1.1.4/pyGDM2/electron.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha, A. Arbouet
+#Copyright (C) 2017-2023, P. R. Wiecha, A. Arbouet
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/fields/__init__.py` & `pyGDM2-1.1.4/pyGDM2/fields/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/fields/deprecated.py` & `pyGDM2-1.1.4/pyGDM2/fields/deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/fields/efield_class.py` & `pyGDM2-1.1.4/pyGDM2/fields/efield_class.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
@@ -114,14 +114,23 @@
         self.setDtype(np.float32, np.complex64)
     
     
     def setDtype(self, dtypef, dtypec):
         """set dtype of arrays"""
         self.dtypef = dtypef
         self.dtypec = dtypec
+    
+    
+    ## !!! Todo: add automatic field gradient calculation
+    # def get_field_gradient():
+    #     from pyGDM2 import linear
+    #     gradE0 = linear.field_gradient(sim, field_index, r_qe, 
+    #                                    delta=eps_dd, which_fields=['E0'])
+    #     gradH0 = linear.field_gradient(sim, field_index, r_qm, 
+    #                                    delta=eps_dd, which_fields=['H0'])
 
 
     def __repr__(self, verbose=False):
         out_str =  ' ----- incident field -----'
         out_str += '\n' + '   field generator: "{}"'.format(self.field_generator.__name__)
         out_str += '\n' + '   {} wavelengths between {} and {}nm'.format(
                          len(self.wavelengths), self.wavelengths.min(),
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/fields/electron.py` & `pyGDM2-1.1.4/pyGDM2/fields/electron.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/fields/focused_beams.py` & `pyGDM2-1.1.4/pyGDM2/fields/focused_beams.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha, A. Arbouet, Y. Brûlé
+#Copyright (C) 2017-2023, P. R. Wiecha, A. Arbouet, Y. Brûlé
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/fields/regular.py` & `pyGDM2-1.1.4/pyGDM2/fields/regular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/linear.py` & `pyGDM2-1.1.4/pyGDM2/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
@@ -274,21 +274,31 @@
         raise ValueError("Error: Scattering field inside the structure not yet evaluated. Run `core.scatter` simulation first.")
     
     if str(polarizerangle).lower() == 'none':
         polarizer = 0
     else:
         polarizer = polarizerangle * np.pi/180.
     
-    if np.pi < tetamax < 0:
-        raise ValueError("`tetamax` out of range, must be in [0, pi]")
-    
     if r_probe is not None and return_value in ['int_es', 'int_E0', 'int_Etot']:
         raise ValueError("probing farfield on user-defined positions does not support integration " +
                          "of the intensity since no surface differential can be defined. Use spherical " +
                          "coordinate definition to do the integration.")
+    # --- check angles
+    if tetamin < 0  or tetamin >= tetamax:
+        raise ValueError("`tetamin` out of range, must be in [0, tetamax]")
+    
+    if tetamax > np.pi or tetamax < 0:
+        raise ValueError("`tetamax` out of range, must be in [0, pi]")
+    
+    if phimin < 0  or phimin >= phimax:
+        raise ValueError("`phimin` out of range, must be in [0, phimax]")
+    
+    if phimax > 2*np.pi or phimax < 0:
+        raise ValueError("`phimax` out of range, must be in [0, 2*pi]")
+    
     
     
 # =============================================================================
 #     preparation
 # =============================================================================
     from pyGDM2 import tools
 
@@ -311,17 +321,17 @@
     field_params    = tools.get_field_indices(sim)[field_index]
     wavelength      = field_params['wavelength']
     
     ## --- environment
     sim.struct.setWavelength(wavelength)
     conf_dict = sim.dyads.getConfigDictG(wavelength, sim.struct, sim.efield)
     if sim.dyads.n2_material.__name__ != sim.dyads.n3_material.__name__:
-        raise ValueError("`farfield` does not support a cladding layer at the moment. " +
-                         "It implements only an asymptotic Green's tensor for an " +
-                         "environment with a single interface (substrate).")
+        warnings.warn("`farfield` does not support a cladding layer at the moment. " +
+                      "It implements only an asymptotic Green's tensor for an " +
+                      "environment with a single interface (substrate). The results are probably incorrect.")
     
 #==============================================================================
 #     electric polarization of structure, fundamental field
 #==============================================================================        
     ## --- fundamental field - use dummy structure with 
     env_dict = sim.dyads.getConfigDictG(wavelength, sim.struct, sim.efield)
     if return_value == 'int_Es':
@@ -431,17 +441,17 @@
 
 
 
 # =============================================================================
 # nearfield functions
 # =============================================================================
 def nearfield(sim, field_index, r_probe, which_fields=["Es","Et","Bs","Bt"],
-                 val_inside_struct="field", val_outside_struct="field", 
-                 N_neighbors_internal_field=4,
-                 method=''):
+              val_inside_struct="field", val_outside_struct="field", 
+              N_neighbors_internal_field=4,
+              method=''):
     """Nearfield distribution in proximity of nanostructre
     
     For a given incident field, calculate the electro-magnetic field in the 
     proximity of the nanostructure (positions defined by `MAP`).
     
     - Pure python implementation.
     
@@ -872,14 +882,16 @@
 # =============================================================================
     if r_probe is None:
         r_probe = sim.struct.geometry
     if delta is None:
         delta= sim.struct.step
     
     
+    if len(r_probe) == 0:
+        return np.zeros((3,0,6))
     if len(np.shape(r_probe)) == 1:
         if len(r_probe) == 3:
             r_probe = [[r_probe[0]], [r_probe[1]], [r_probe[2]]]
         else: 
             raise ValueError("If 'r_probe' is tuple, must consist of *exactly* 3 elements!")
     elif len(np.shape(r_probe)) == 2:
         if np.shape(r_probe)[0] != 3 and np.shape(r_probe)[1] != 3:
@@ -887,18 +899,14 @@
         if np.shape(r_probe)[0] != 3:
             r_probe = np.transpose(r_probe)
     else:
         raise ValueError("wrong format for 'r_probe'. must consist of *exactly* 3 " +
                          "elements, either floats, or lists.")
     r_probe = np.transpose(r_probe)
     
-    # if sim.E is None: 
-    #     raise ValueError("Error: Scattered field inside the structure not yet evaluated. Run `core.scatter` simulation first.")
-    
-    
     
 # =============================================================================
 #     preparation
 # =============================================================================
     from pyGDM2 import tools
     
     which_fields = [wf.lower() for wf in which_fields]
@@ -1051,17 +1059,14 @@
     else:
         F_tot = np.array([np.sum(Fx), np.sum(Fy), np.sum(Fz)])
         return F_tot
 
 
 
 
-
-
-
 def optical_chirality(sim, field_index, r_probe, which_field="t", **kwargs):
     """calculate the optical chirality of the electromagnetic field
     
     ** ------- FUNCTION STILL UNDER TESTING ------- **
     
     Returns the normalized electromagnetic chirality *C / C_LCP*, as defined in [1-4].
     Normalized to a left circular polarized (LCP) plane wave of amplitude |E_0|=1.
@@ -1102,15 +1107,15 @@
     -------
     list of tuples (X,Y,Z, X). Each tuple consists of the position and the 
     (normalized) optical chirality *C / C_LCP*.
     
     
     Notes
     -----
-    For details on the optical chirality, see:
+    For details on the optical chirality, see e.g.:
     
     [1] Tang, Y. & Cohen, A. E.: **Optical Chirality and Its Interaction 
     with Matter**. Phys. Rev. Lett. 104, 163901 (2010)
     
     [2] Meinzer, N., Hendry, E. & Barnes, W. L.: **Probing the chiral nature 
     of electromagnetic fields surrounding plasmonic nanostructures**. 
     Phys. Rev. B 88, 041407 (2013)
@@ -1141,15 +1146,15 @@
         Bt = B0
     
     ## Ref. [2]: C ~ Im(E* B)
     C = np.concatenate([
                     Et.T[:3].real, # positions
                     [-1*np.sum(np.multiply(np.conjugate(Et.T[3:]), 
                                                      Bt.T[3:]), axis=0).imag]
-                        ]).astype(np.float)
+                        ]).astype(np.float32)
     
     if len(np.shape(r_probe)) == 1 or len(r_probe) == 1:
         return C[3][0]
     else:
         return C
     
 
@@ -1394,15 +1399,14 @@
 
 
 
 
 
 
 
-
 # =============================================================================
 # deprecations - to be removed in a future version
 # =============================================================================
 def multipole_decomp(sim, field_index, r0=None, quadrupoles=False):
     """multipole decomposition of nanostructure optical response
     
     ** ------- DEPRECATED ------- **
@@ -1413,21 +1417,21 @@
     from pyGDM2 import multipole
     
     warnings.warn("This function is deprecated and will be removed in a future version. " +
                   "Please use the `pyGDM2.multipole` module instead.")
     
     if quadrupoles:
         p, m, q, mq = multipole.multipole_decomposition_exact(
-                                    sim, field_index, r0, epsilon=0.01, 
+                                    sim, field_index, r0=r0, epsilon=0.01, 
                                     which_moments=['p', 'm', 'qe', 'qm'])
         return p, m, q, mq
 
     else:
         p, m = multipole.multipole_decomposition_exact(
-                                    sim, field_index, r0, epsilon=0.01, 
+                                    sim, field_index, r0=r0, epsilon=0.01, 
                                     which_moments=['p', 'm'])
         return p, m
 
 
 def multipole_decomp_extinct(sim, field_index, r0=None, eps_dd=0.1, quadrupoles=False):
     """extinction from multipole decomposition
     
@@ -1437,20 +1441,19 @@
     """
     from pyGDM2 import multipole
     
     warnings.warn("This function is deprecated and will be removed in a future version. " +
                   "Please use the `pyGDM2.multipole` module instead.")
     
     sigma_ext_p, sigma_ext_m, sigma_ext_q, sigma_ext_mq = multipole.extinct(
-                                                sim, field_index, r0, eps_dd)
+                                                sim, field_index, r0=r0, eps_dd=eps_dd)
     if quadrupoles:
         return sigma_ext_p, sigma_ext_m, sigma_ext_q, sigma_ext_mq
     else:
         return sigma_ext_p, sigma_ext_m
 
 
 def mutlipole_decomp(sim, field_index, r0=None):
-    return multipole_decomp(sim, field_index, r0, quadrupoles=True)
+    return multipole_decomp(sim, field_index, r0=r0, quadrupoles=True)
 
 def mutlipole_decomp_extinct(sim, field_index, r0=None, eps_dd=0.1):
     return multipole_decomp_extinct(sim, field_index, r0, eps_dd, quadrupoles=True)
-
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/materials.py` & `pyGDM2-1.1.4/pyGDM2/materials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundaeon, either version 3 of the License, or
 #(at your opeon) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/multipole.py` & `pyGDM2-1.1.4/pyGDM2/multipole/processing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
@@ -27,14 +27,21 @@
 
 import numpy as np
 import copy
 import numba
 
 import time
 
+from pyGDM2.multipole.main import multipole_decomposition_exact
+from pyGDM2.multipole.polarizabilities import eval_generalized_polarizability_m
+from pyGDM2.multipole.polarizabilities import eval_generalized_polarizability_p
+from pyGDM2.multipole.polarizabilities import eval_generalized_polarizability_qe
+from pyGDM2.multipole.polarizabilities import eval_generalized_polarizability_qm
+from pyGDM2.multipole.polarizabilities import _test_availability_generalized_polarizability
+from pyGDM2.multipole import propagators as mp_propagators
 
 #==============================================================================
 # GLOBAL PARAMETERS
 #==============================================================================
 DTYPE_C = np.complex64
 
 
@@ -42,224 +49,614 @@
 
 #==============================================================================
 # EXCEPTIONS
 #==============================================================================
 
 
 
-def multipole_decomposition_exact(sim, field_index, r0=None, epsilon=0.01, 
-                                  which_moments=['p', 'm', 'qe', 'qm'],
-                                  long_wavelength_approx=False):
-    """exact multipole decomposition of the nanostructure optical response
+# =============================================================================
+# CONSISTENCY TESTS / HELPER
+# =============================================================================
+def _check_multipole_list(p, m, qe, qm, r_p, r_m, r_qe, r_qm, r0):
     
-    ** ------- FUNCTION STILL UNDER TESTING ------- **
+    # dipole moment definitions
+    if len(p) == 0 and len(m) == 0 and len(qe) == 0 and len(qm) == 0:
+        raise Exception("All multipoles are zero. Please define at least one multipole moment.")
+    if len(p) == 0:
+        p = np.zeros((0, 3), dtype=np.complex64)
+        r_p = np.zeros((0, 3), dtype=np.float32)
+    if len(m) == 0:
+        m = np.zeros((0, 3), dtype=np.complex64)
+        r_m = np.zeros((0, 3), dtype=np.float32)
+    if len(qe) == 0:
+        qe = np.zeros((0, 3), dtype=np.complex64)
+        r_qe = np.zeros((0, 3), dtype=np.float32)
+    if len(qm) == 0:
+        qm = np.zeros((0, 3), dtype=np.complex64)
+        r_qm = np.zeros((0, 3), dtype=np.float32)
+        
+    # positions 
+    if r0 is None:
+        if r_p is None and r_m is None and r_qe is None and r_qm is None:
+            raise Exception("No positions for the multipoles are given.")
+        if len(r_p) != len(p):
+            raise Exception("Same number of dipole positions and dipole moments required! `p` and `r_p` must be lists of same length.")
+        if len(r_m) != len(m):
+            raise Exception("Same number of dipole positions and dipole moments required! `m` and `r_m` must be lists of same length.")
+        if len(r_qe) != len(qe):
+            raise Exception("Same number of quadrupole positions and quadrupole moments required! `qe` and `r_qe` must be lists of same length.")
+        if len(r_qm) != len(qm):
+            raise Exception("Same number of quadrupole positions and quadrupole moments required! `qm` and `r_qm` must be lists of same length.")
+    else:
+        # global r0 defined: override specific positions
+        r0 = np.array(r0)
+        if len(r0) != 3: 
+            raise Exception("Multipole position must be carthesian coordinate (array of 3 float)")
+        if len(p) > 0:
+            r_p = np.array([r0 for _ in p], dtype= np.float32)
+        if len(m) > 0:
+            r_m = np.array([r0 for _ in m], dtype= np.float32)
+        if len(qe) > 0:
+            r_qe = np.array([r0 for _ in qe], dtype= np.float32)
+        if len(qm) > 0:
+            r_qm = np.array([r0 for _ in qm], dtype= np.float32)
     
-    Multipole decomposition of electromagnetic field inside nanostructure for 
-    electric and magnetic dipole and quadrupole moments.
+    return p, m, qe, qm, r_p, r_m, r_qe, r_qm, r0
 
 
-    Parameters
-    ----------
-    sim : :class:`.core.simulation`
-        simulation description
+def _eval_G0(G0func, R1, R2, wl, eps_env):
+    """evaluate a free-space Green's tensor `G0func`
+    """
+    if np.linalg.norm(R1-R2)==0:
+        warnings.warn("Green's tensor singularity. Returning zero.")
+        return np.zeros((3,3), dtype=np.complex64)
+    
+    xx, yy, zz, xy, xz, yx, yz, zx, zy = G0func(R1, R2, wl, eps_env)
+    G0 = np.array([
+        [xx, xy, xz],
+        [yx, yy, yz],
+        [zx, zy, zz],
+        ]).astype(np.complex64)
+    
+    return G0
+
+
+# =============================================================================
+# LOW-LEVEL (working with lists of multipoles)
+# =============================================================================
+def _multipole_extinct(sim, field_index,
+                       p=[], m=[], qe=[], qm=[],
+                       r_p=None, r_m=None, r_qe=None, r_qm=None,
+                       r0=None, eps_dd=0.001, 
+                       normalization_E0=True,
+                       ):
+    """extinction cross-section for an explicit list of multipole moments
     
-    field_index : int
-        index of evaluated self-consistent field to use for calculation. Can be
-        obtained for specific parameter-set using :func:`.tools.get_closest_field_index`
     
-    r0 : array, default: None
-        [x,y,z] position of multipole decomposition development. 
-        If `None`, use structure's center of gravity
+    Parameters
+    ----------
+    wavelength : float
+        radiation wavelength
     
-    epsilon : float, default: 0.01
-        additional step on r0 (in nm) to avoid numerical divergence of the Bessel terms
+    eps_env : float
+        envirnoment permittivity (real part)
         
-    which_moments : list of str, default: ['p', 'm', 'qe', 'qm']
-        which multipole moments to calculate and return. supported dipole moments: 
-            - 'p': electric dipole (full)
-            - 'm': magnetic dipole
-            - 'qe': electric quadrupole (full)
-            - 'qm': magnetic quadrupole
-            - 'p1': electric dipole (first order)
-            - 'pt': toroidal dipole
-            - 'qe1': electric quadrupole (first order)
-            - 'qet': toroidal quadrupole
+    r0 : array. optional
+        [x,y,z] position of mulipole decomposition development.
+        Alternatively the positions of each mutlipole can be specified.
+        The default is `None`.
+        
+    p, m, qe, qm : lists of ndarrays. optional
+        lists of dipole and quadrupole moments to propagate to the farfield.
+        The default is [].
+        
+    r_p, r_m, r_qe, r_qm : ndarrays or list of such. optional
+        Has effect only if r0 is not specified. Carthesian coordinates of 
+        each multipole individually.
     
-    long_wavelength_approx : bool, default: False
-        if True, use long wavelength approximation
-            
     
     Returns
     -------
-    list of multipole moments. Default:
+    total extinction cross sections for each multipole type (in nm^2)
         
-    p : 3-vector
-        electric dipole moment
     
-    m : 3-vector
-        magnetic dipole moment
+    Notes
+    -----
+    For details about the extinction section of multipole moments, see:
+    
+    Evlyukhin, A. B. et al. *Multipole analysis of light scattering by 
+    arbitrary-shaped nanoparticles on a plane surface.*, 
+    JOSA B 30, 2589 (2013)
+    """
+# =============================================================================
+#     exception handling
+# =============================================================================
+    p, m, qe, qm, r_p, r_m, r_qe, r_qm, r0 = _check_multipole_list(
+        p=p, m=m, qe=qe, qm=qm, r_p=r_p, r_m=r_m, r_qe=r_qe, r_qm=r_qm, r0=r0)
+    
+    
+# =============================================================================
+#     preparation
+# =============================================================================  
+    from pyGDM2 import tools 
+    from pyGDM2 import linear
+    
+    field_params = tools.get_field_indices(sim)[field_index]
+    wavelength   = field_params['wavelength']
+    sim.struct.setWavelength(wavelength)
+    k0 = 2*np.pi / wavelength
+    eps_env = sim.dyads.getEnvironmentIndices(wavelength, sim.struct.geometry[:1])[0]  # structure must be fully in one environment zone
+    n_env = (eps_env**0.5).real
+    
+    ## incident field and its gradients at multipole position
+    env_dict = sim.dyads.getConfigDictG(wavelength, sim.struct, sim.efield)
+    E0 = sim.efield.field_generator(r_p, env_dict, **field_params)
+    H0 = sim.efield.field_generator(r_m, env_dict, returnField='H', **field_params)
+    
+    gradE0 = linear.field_gradient(sim, field_index, r_qe, 
+                                   delta=eps_dd, which_fields=['E0'])
+    gradH0 = linear.field_gradient(sim, field_index, r_qm, 
+                                   delta=eps_dd, which_fields=['H0'])
+    gradE0cj = np.conj(np.array(gradE0)[...,3:])
+    gradH0cj = np.conj(np.array(gradH0)[...,3:])
+    
+    ## normalization
+    if normalization_E0:
+        # intensity of incident field at each multipole
+        E2in_p = np.sum(np.abs(sim.efield.field_generator(r_p, env_dict, **field_params))**2, axis=1).real
+        E2in_m = np.sum(np.abs(sim.efield.field_generator(r_m, env_dict, **field_params))**2, axis=1).real
+        E2in_qe = np.sum(np.abs(sim.efield.field_generator(r_qe, env_dict, **field_params))**2, axis=1).real
+        E2in_qm = np.sum(np.abs(sim.efield.field_generator(r_qm, env_dict, **field_params))**2, axis=1).real
+    else:
+        E2in_p = np.ones(len(r_p))
+        E2in_m = np.ones(len(r_m))
+        E2in_qe = np.ones(len(r_qe))
+        E2in_qm = np.ones(len(r_qm))
+    
+    E0 = E0 / E2in_p[:,None]
+    H0 = H0 / E2in_m[:,None]
+    gradE0cj = gradE0cj / E2in_qe[:,None]
+    gradH0cj = gradH0cj / E2in_qm[:,None]
+    
+# =============================================================================
+#     calc the ECS per multipole order
+# =============================================================================
+    prefactor = (4 * np.pi * k0 * 1/n_env).real
+    
+    ecs_p = prefactor * (np.sum(np.conjugate(E0)*p)).imag
+    ecs_m = prefactor / n_env * (np.sum(np.conjugate(H0)*m)).imag
+    ecs_Qe = prefactor / 12. * (np.sum([np.tensordot(gradE0cj[:,i,:] + gradE0cj[:,i,:].T, qe[i]) for i in range(len(qe))] )).imag
+    ecs_Qm = prefactor / n_env / 6 * (np.sum([np.tensordot(gradH0cj[:,i,:].T, qm[i]) for i in range(len(qm))] )).imag
+    
+    return [ecs_p, ecs_m, ecs_Qe, ecs_Qm]
+
+
+def _multipole_scs(sim, field_index,
+                   p=[], m=[], qe=[], qm=[],
+                   r_p=None, r_m=None, r_qe=None, r_qm=None,
+                   r0=None, eps_dd=0.001, 
+                   normalization_E0=True,
+                   ):
+    """scattering cross-section for an explicit list of multipole moments
+    
+    Radiated electro-magnetic field  (E-field) in the far-field 
+    (by default on a sphere of radius `r` around the nanostructure).
+    
+    
+    Parameters
+    ----------
+    wavelength : float
+        radiation wavelength
     
-    Qe : 3x3 tensor
-        electric quadrupole moment
+    eps_env : float
+        envirnoment permittivity (real part)
+        
+    r0 : array. optional
+        [x,y,z] position of mulipole decomposition development.
+        Alternatively the positions of each mutlipole can be specified.
+        The default is `None`.
+        
+    p, m, qe, qm : lists of ndarrays. optional
+        lists of dipole and quadrupole moments to propagate to the farfield.
+        The default is [].
         
-    Qm : 3x3 tensor
-        magnetic quadrupole moment
+    r_p, r_m, r_qe, r_qm : ndarrays or list of such. optional
+        Has effect only if r0 is not specified. Carthesian coordinates of 
+        each multipole individually.
     
+    Returns
+    -------
+    total scattering cross sections for each multipole type (in nm^2)
+        
     
     Notes
     -----
-    For details about the method, see: 
-    
+    For details about the exact multipole formalism and scs calculation, see: 
+        
     Alaee, R., Rockstuhl, C. & Fernandez-Corbaton, I. *An electromagnetic 
     multipole expansion beyond the long-wavelength approximation.*
-    Optics Communications 407, 17–21 (2018)
+    Optics Communications 407, 17–21 (2018)        
     """
 # =============================================================================
-#     Exception handling
+#     exception handling
 # =============================================================================
-    if sim.E is None: 
-        raise ValueError("Error: Scattered field inside the structure not yet " +
-                         "evaluated. Run `core.scatter` simulation first.")
-    
-    which_moments = [wm.lower() for wm in which_moments]
+    p, m, qe, qm, r_p, r_m, r_qe, r_qm, r0 = _check_multipole_list(
+        p=p, m=m, qe=qe, qm=qm, r_p=r_p, r_m=r_m, r_qe=r_qe, r_qm=r_qm, r0=r0)
     
 # =============================================================================
 #     preparation
-# =============================================================================
-    ## structure
-    geo = sim.struct.geometry
-    if r0 is None:
-        r0 = np.average(geo, axis=0)
-        sim.r0 = r0
-    if np.abs(np.linalg.norm(geo - r0, axis=1)).min() > epsilon:
-        epsilon = 0
-    r = geo - r0 + epsilon                   # epsilon: avoid divergence of 1/kr when r=0
-    norm_r = np.linalg.norm(r, axis=1)
-    
-    ## illumination properties
-    field_params = sim.E[field_index][0]
-    wavelength = field_params['wavelength']
+# =============================================================================  
+    from pyGDM2 import tools 
+    
+    field_params = tools.get_field_indices(sim)[field_index]
+    wavelength   = field_params['wavelength']
     sim.struct.setWavelength(wavelength)
-    eps_env = sim.dyads.getEnvironmentIndices(wavelength, r0[None,:])[0]  # assume structure is fully in one environment
-    n_env = eps_env**0.5
-    k = 2*np.pi*n_env / wavelength
-    kr = k * norm_r
-    
-    ## electric polarization density of structure
-    alpha_tensor = sim.dyads.getPolarizabilityTensor(wavelength, sim.struct)
-    E = sim.E[field_index][1]
-    P = np.matmul(alpha_tensor, E[...,None])[...,0]
-    rP = np.einsum('ij, ij->i', r, P)
-    
-    ## bessel functions and pre-factors
-    if not long_wavelength_approx:
-        from scipy.special import spherical_jn as sph_jn
-        j0kr = sph_jn(0, kr)
-        j1kr = sph_jn(1, kr) / kr
-        j2kr = sph_jn(2, kr) / (kr**2)
-        j3kr = sph_jn(3, kr) / (kr**3)
-        f_pt = 1/2; f_ptA=3; f_ptB=-1
-        f_qe = 3; fqe2=2; fqe2A = 5; fqe2B = -1; fqe2C = -1
-        f_m = 3/2; f_qm = 15
+    k0 = 2*np.pi / wavelength
+    eps_env = sim.dyads.getEnvironmentIndices(wavelength, sim.struct.geometry[:1])[0]  # structure must be fully in one environment zone
+    n_env = (eps_env**0.5).real
+    k = k0*n_env
+    
+    ## normalization
+    if normalization_E0:
+        ## incident field intensity at each multipole location
+        env_dict = sim.dyads.getConfigDictG(wavelength, sim.struct, sim.efield)
+        
+        E2in_p = np.sum(np.abs(sim.efield.field_generator(r_p, env_dict, **field_params))**2, axis=1).real
+        E2in_m = np.sum(np.abs(sim.efield.field_generator(r_m, env_dict, **field_params))**2, axis=1).real
+        E2in_qe = np.sum(np.abs(sim.efield.field_generator(r_qe, env_dict, **field_params))**2, axis=1).real
+        E2in_qm = np.sum(np.abs(sim.efield.field_generator(r_qm, env_dict, **field_params))**2, axis=1).real
     else:
-        j0kr = j1kr = j2kr = j3kr = np.ones_like(kr)
-        f_pt = 1/10; f_ptA=1; f_ptB=-2
-        f_qe = 1; fqe2=1/14; fqe2A = 4; fqe2B = -5; fqe2C = 2
-        f_m = 1/2; f_qm = 1
+        E2in_p = np.ones(len(r_p))
+        E2in_m = np.ones(len(r_m))
+        E2in_qe = np.ones(len(r_qe))
+        E2in_qm = np.ones(len(r_qm))
     
 # =============================================================================
-#     multipole calculation
+#     calc the ECS per multipole order
 # =============================================================================
-    ## ----------- dipole moments
-    ## electric dipole
-    if 'p' in which_moments or 'p1' in which_moments or 'pt' in which_moments:
-        p1 = np.sum(P * j0kr[..., None], axis=0)
+    ## factor 100: cm --> m (cgs units)
+    sc_factor_dp = 100/12*(k0**4).real
+    sc_factor_Q = 100/1440*(k0**4).real
+        
+    scs_p = sc_factor_dp * np.sum(np.abs(p)**2 / E2in_p[:,None])
+    scs_m = sc_factor_dp * np.sum(np.abs(m)**2 / E2in_m[:,None])
+    scs_Qe = sc_factor_Q * np.sum(np.abs(k*qe)**2 / E2in_qe[:,None])
+    scs_Qm = sc_factor_Q * np.sum(np.abs(k*qm)**2 / E2in_qm[:,None])
+    
+    return [scs_p, scs_m, scs_Qe, scs_Qm]
+
+
+def _multipole_nearfield(wavelength, r_probe, eps_env=1, 
+                         p=[], m=[], qe=[], qm=[],
+                         r_p=None, r_m=None, r_qe=None, r_qm=None,
+                         r0=None, which_fields=["Es","Bs"]):
+    """calculate scattered field of multiple multipole (valid in the nearfield region)
+    
+    !! not performance optimized !!
+    
+    Parameters
+    ----------
+    wavelength : float
+        radiation wavelength
+        
+    r_probe : tuple (x,y,z) or list of 3-lists/-tuples
+        (list of) coordinate(s) to evaluate nearfield on. 
+        Format: tuple (x,y,z) or list of 3 lists: [Xmap, Ymap, Zmap] 
+        (the latter can be generated e.g. using :func:`.tools.generate_NF_map`)
+    eps_env : float
+        envirnoment permittivity (real part)
+        
+    r0 : array. optional
+        [x,y,z] position of mulipole decomposition development.
+        Alternatively the positions of each mutlipole can be specified.
+        The default is `None`.
         
-        ## "toroidal" dipole
-        p2 = k**2 * f_pt * np.sum((  f_ptA * rP[...,None]*r 
-                                   + f_ptB * norm_r[..., None]**2 * P) * j2kr[..., None], 
-                                  axis=0)
+    p, m, qe, qm : lists of ndarrays. optional
+        lists of dipole and quadrupole moments to propagate to the farfield.
+        The default is [].
+        
+    r_p, r_m, r_qe, r_qm : ndarrays or list of such. optional
+        Has effect only if r0 is not specified. Carthesian coordinates of 
+        each multipole individually.
         
-        p = p1 + p2
+    which_fields : list of str, default: ["Es","Bs"]
+        which fields to calculate and return. available options: 
+            ["Es", "Bs"]
     
-    ## magnetic dipole
-    if 'm' in which_moments:
-        m = -1j*k * f_m * np.sum(np.cross(r, P) * j1kr[..., None], axis=0)
+    Returns
+    -------
+    depending on kwarg `which_fields`, one or two lists of 6-tuples, complex : 
+        - scattered Efield ("Es")
+        - scattered Bfield ("Bs")
     
-    ## ----------- quadrupole moments
-    ## electric quadrupole
-    if 'qe' in which_moments or 'qe1' in which_moments or 'qet' in which_moments:
-        Qe1 = np.zeros((3,3), dtype=np.complex64)
-        Qe2 = np.zeros((3,3), dtype=np.complex64)
-        for i_a in range(3):
-            for i_b in range(3):
-                
-                ## diagonal term
-                if i_a==i_b:
-                    rP_delta = rP
-                else:
-                    rP_delta = 0
-                
-                ## electric quadrupole
-                Qe1[i_a, i_b] = np.sum(
-                    (
-                       3 * (r[:,i_b]*P[...,i_a] + r[:,i_a]*P[...,i_b])
-                     - 2*(rP_delta)
-                     ) * j1kr)
+    the tuples are of shape (X,Y,Z, Ax,Ay,Az) with Ai the corresponding 
+    complex field component
+    
+    Notes
+    -----
+    Details about the calculation of the field scattered by quadrupoles:
+    Babicheva and Evlyukhin
+    **Analytical model of resonant electromagnetic dipole-quadrupole coupling 
+    in nanoparticle arrays**
+    Phys. Rev. B 99, 195444 (2019)
+
+    """
+# =============================================================================
+#     exception handling
+# =============================================================================
+    p, m, qe, qm, r_p, r_m, r_qe, r_qm, r0 = _check_multipole_list(
+        p=p, m=m, qe=qe, qm=qm, r_p=r_p, r_m=r_m, r_qe=r_qe, r_qm=r_qm, r0=r0)
+
+# =============================================================================
+#     the main calculation
+# =============================================================================
+    return_field_list = []
+    for returnfield in which_fields:
+        
+        if returnfield.lower() in ['e', 'es']:
+            func_G_p = mp_propagators.G0_Ep
+            func_G_m = mp_propagators.G0_Em
+            func_G_qe = mp_propagators.G0_Eqe
+            func_G_qm = mp_propagators.G0_Eqm
+        elif returnfield.lower() in ['h', 'b', 'hs', 'bs']:
+            func_G_p = mp_propagators.G0_Hp
+            func_G_m = mp_propagators.G0_Hm
+            func_G_qe = mp_propagators.G0_Hqe
+            func_G_qm = mp_propagators.G0_Hqm
+            
+        ## evaluate the propagators
+        Fp = np.zeros([len(r_probe), 3], dtype=np.complex64)
+        Fm = np.zeros([len(r_probe), 3], dtype=np.complex64)
+        FQe = np.zeros([len(r_probe), 3], dtype=np.complex64)
+        FQm = np.zeros([len(r_probe), 3], dtype=np.complex64)
+        for i, _r in enumerate(r_probe):
+            # ED
+            for j, r0 in enumerate(r_p):
+                n_vec = (_r - r0) / np.linalg.norm((_r - r0)) # scat. direction
+                Gp = _eval_G0(func_G_p, r0, _r, wavelength, eps_env)
+                Fp[i] += np.dot(Gp, p[j]) # add scattered field
                 
-                ## "toroidal" quadrupole
-                Qe2[i_a, i_b] = np.sum(
-                      (fqe2A*r[:,i_a]*r[:,i_b]*rP 
-                      + norm_r**2 * (  fqe2B * (r[:,i_a]*P[:,i_b] + r[:,i_b]*P[:,i_a]) 
-                                     + fqe2C * rP_delta)) * j3kr)
+            # MD
+            for j, r0 in enumerate(r_m):
+                n_vec = (_r - r0) / np.linalg.norm((_r - r0)) # scat. direction                
+                Gm = _eval_G0(func_G_m, r0, _r, wavelength, eps_env)
+                Fm[i] += np.dot(Gm, m[j]) # add scattered field
                 
-        Qe1 = f_qe * Qe1
-        Qe2 = f_qe * fqe2 * k**2 * Qe2
-        Qe = Qe1 + Qe2
+            # QE
+            for j, r0 in enumerate(r_qe):
+                n_vec = (_r - r0) / np.linalg.norm((_r - r0)) # scat. direction                
+                Gqe = _eval_G0(func_G_qe, r0, _r, wavelength, eps_env)
+                qen = np.tensordot(qe, n_vec, axes=(-1,-1))
+                FQe[i] += np.dot(Gqe, qen[j]) # add scattered field
+            
+            # QM    
+            for j, r0 in enumerate(r_qm):
+                Gqm = _eval_G0(func_G_qm, r0, _r, wavelength, eps_env)
+                qmn = np.tensordot(qm, n_vec, axes=(-1,-1))
+                FQm[i] += np.dot(Gqm, qmn[j]) # add scattered field
+            
+        
+        # sum contributions of all multipoles and append calculation positions
+        F = Fp + Fm + FQe + FQm
+        F_iwth_pos = np.concatenate([r_probe, F], axis=1)
+        return_field_list.append(F_iwth_pos)
     
-    ## magnetic quadrupole
-    if 'qm' in which_moments:
-        Qm = np.zeros((3,3), dtype=np.complex64)
-        for i_a in range(3):
-            for i_b in range(3):
-                Qm[i_a, i_b] = np.sum(
-                    (r[:,i_a] * np.cross(r, P)[...,i_b] + 
-                     r[:,i_b] * np.cross(r, P)[...,i_a]) * j2kr)
-                
-        Qm = -1j * k * f_qm * Qm
+    return return_field_list
+
+
+def _multipole_farfield(wavelength, eps_env, r0=None, 
+                        p=[], m=[], qe=[], qm=[],
+                        r_p=None, r_m=None, r_qe=None, r_qm=None,
+                        r_probe=None,
+                        r=100000., 
+                        tetamin=0, tetamax=np.pi/2., Nteta=10, 
+                        phimin=0, phimax=2*np.pi, Nphi=36, 
+                        return_value='map'):
+    """far-field scattering of an explicit list of multipole moments
     
+    Radiated electro-magnetic field  (E-field) in the far-field 
+    (by default on a sphere of radius `r` around the nanostructure).
+    
+    
+    Parameters
+    ----------
+    wavelength : float
+        radiation wavelength
+    
+    eps_env : float
+        envirnoment permittivity (real part)
+        
+    r0 : array. optional
+        [x,y,z] position of mulipole decomposition development.
+        Alternatively the positions of each mutlipole can be specified.
+        The default is `None`.
+        
+    p, m, qe, qm : lists of ndarrays. optional
+        lists of dipole and quadrupole moments to propagate to the farfield.
+        The default is [].
+        
+    r_p, r_m, r_qe, r_qm : ndarrays or list of such. optional
+        Has effect only if r0 is not specified. Carthesian coordinates of 
+        each multipole individually.
+    
+    r_probe : tuple (x,y,z) or list of 3-lists/-tuples. optional
+        defaults to *None*, which means it is not used and a solid angle defined by
+        a spherical coordinate range is used instead. If `r_probe` is given, this
+        overrides `r`, `tetamin`, `tetamax`, `Nteta`, `Nphi`.
+        (list of) coordinate(s) to evaluate farfield on. 
+        Format: tuple (x,y,z) or list of 3 lists: [Xmap, Ymap, Zmap] 
+        The default is None. (Not used)
+        
+    r : float, default: 100000.
+        radius of integration sphere (distance to coordinate origin in nm)
+        
+    tetamin, tetamax : float, float; defaults: 0, np.pi/2
+        minimum and maximum polar angle in radians 
+        (in linear steps from `tetamin` to `tetamax`)
+        
+    phimin, phimax : float, float; defaults: 0, 2*np.pi
+        minimum and maximum azimuth angle in radians, excluding last position
+        (in linear steps from `phimin` to `phimax`)
+        
+    Nteta, Nphi : int, int; defaults: 10, 36
+        number of polar and azimuthal angles on sphere to calculate,
+    
+    return_value : str, default: 'map'
+        Values to be returned. Either 'map' (default) or 'integrated'.
+          - "map" : (default) return spatially resolved farfield intensity at each spherical coordinate (5 lists)
+          - "efield" : return spatially resolved E-fields at each spherical coordinate (5 lists)
+          - "int_Es" : return the integrated scattered field (as float)
+    
+    
+    Returns
+    -------
+    using `r_probe` for position definition:
+        3 lists of 6-tuples (x,y,z, Ex,Ey,Ez), complex : 
+            - scattered Efield or E-intensity
+        
+    if solid angle is defined via spherical coordinate range:
+        - return_value == "map" : 5 arrays of shape (Nteta, Nphi) : 
+            - [tetalist : teta angles - if solid angle range input]
+            - [philist : phi angles - if solid angle range input]
+            - I_sc : intensity of scattered field, 
+        
+        - return_value == "efield" : float
+            - [tetalist : teta angles - if solid angle range input]
+            - [philist : phi angles - if solid angle range input]
+            - E_sc : complex scattered field at each pos.
+            
+        - return_value == "int_XX" : float
+            integrated total intensity over specified solid angle
+        
+    
+    Notes
+    -----
+    See equation (G1) in
+    
+    Alaee, R., Rockstuhl, C. & Fernandez-Corbaton, I. *An electromagnetic 
+    multipole expansion beyond the long-wavelength approximation.*
+    Optics Communications 407, 17–21 (2018)
+        
+    """
 # =============================================================================
-#     return results
+#     exception handling
 # =============================================================================
-    return_list = []
-    for _m in which_moments:
-        if _m.lower() == "p1":
-            return_list.append(p1)
-        if _m.lower() == "pt":
-            return_list.append(p2)
-        if _m.lower() == "p":
-            return_list.append(p)
-            
-        if _m.lower() == "m":
-            return_list.append(m)
-            
-        if _m.lower() == "qe1":
-            return_list.append(Qe1)
-        if _m.lower() == "qet":
-            return_list.append(Qe2)
-        if _m.lower() == "qe":
-            return_list.append(Qe)
-            
-        if _m.lower() in ["qm"]:
-            return_list.append(Qm)
+    if np.pi < tetamax < 0:
+        raise ValueError("`tetamax` out of range, must be in [0, pi]")
     
-    return return_list
+    if r_probe is not None and return_value in ['int_es', 'int_E0', 'int_Etot']:
+        raise ValueError("probing farfield on user-defined positions does not support integration " +
+                         "of the intensity since no surface differential can be defined. Use spherical " +
+                         "coordinate definition to do the integration.")
+    
+    p, m, qe, qm, r_p, r_m, r_qe, r_qm, r0 = _check_multipole_list(
+        p=p, m=m, qe=qe, qm=qm, r_p=r_p, r_m=r_m, r_qe=r_qe, r_qm=r_qm, r0=r0)
+    
+        
+# =============================================================================
+#     preparation
+# =============================================================================
+    ## --- spherical probe coordinates
+    if r_probe is None:
+        tetalist = np.ones((int(Nteta), int(Nphi)))*np.linspace(tetamin, tetamax, int(Nteta))[:,None]
+        philist = np.ones((int(Nteta), int(Nphi)))*np.linspace(phimin, phimax, int(Nphi), endpoint=False)[None,:]
+        xff = (r * np.sin(tetalist) * np.cos(philist)).flatten()
+        yff = (r * np.sin(tetalist) * np.sin(philist)).flatten()
+        zff = (r * np.cos(tetalist)).flatten()
+        _r_probe = np.transpose([xff, yff, zff])
+    else:
+        _r_probe = r_probe
+        
+    ## --- spherical integration steps
+    dteta = (tetamax-tetamin) / float(Nteta-1)  # endpoint included
+    dphi = (phimax-phimin) / float(Nphi)        # endpoint not included
+    
+    ## --- environment
+    k0 = 2*np.pi / wavelength
+    n_env = (eps_env**0.5).real
+    k = k0*n_env
+    
+#==============================================================================
+#     electric polarization of structure, fundamental field
+#==============================================================================        
+    Escat = np.zeros(shape=(len(_r_probe), 3), dtype=DTYPE_C)
+    
+    def eval_prefactors(r0, _r_probe, k, k0):
+        n_vec = _r_probe - r0
+        R_d = np.linalg.norm(n_vec, axis=1)
+        n_vec = n_vec / R_d[:,None]     # unit vector along direction of scattering
+        
+        phase_factor = np.exp(1j*k*R_d)
+        prefactor = k0**2 * phase_factor / R_d
+        
+        return prefactor, n_vec
+    
+    
+    for _r0, _p in zip(r_p, p):
+        prefactor, n0_vec = eval_prefactors(_r0, _r_probe, k, k0)
+        Es_p = prefactor[:,None] * np.cross(n0_vec, np.cross((_p)[None,:], n0_vec))
+        Escat += Es_p     # sum all electric dipole fields
+    
+    for _r0, _m in zip(r_m, m):
+        prefactor, n0_vec = eval_prefactors(_r0, _r_probe, k, k0)
+        Es_m = prefactor[:,None] * np.cross(_m[None,:], n0_vec)
+        Escat += Es_m     # sum all magnetic dipole fields
+    
+    for _r0, _qe in zip(r_qe, qe):
+        prefactor, n0_vec = eval_prefactors(_r0, _r_probe, k, k0)
+        Es_qe = prefactor[:,None] * 1j * k/6 * np.cross(n0_vec, 
+                    np.cross(n0_vec, np.tensordot(_qe, n0_vec, axes=(-1,-1)).T))
+        Escat += Es_qe     # sum all electric quadrupole fields
+    
+    for _r0, _qm in zip(r_qm, qm):
+        prefactor, n0_vec = eval_prefactors(_r0, _r_probe, k, k0)
+        Es_qm = prefactor[:,None] * 1j * k/6 * np.cross(n0_vec, 
+                    np.tensordot(_qm, n0_vec, axes=(-1,-1)).T)
+        Escat += Es_qm     # sum all magnetic quadrupole fields
+
+    
+    Iscat = np.sum((np.abs(Escat)**2), axis=1)
+
+
+
+#==============================================================================
+#     return either of scattered field / intensity / map
+#==============================================================================
+    ## --- total field (no polarizer)
+    if r_probe is None:
+        out_shape = tetalist.shape
+    else:
+        out_shape = len(_r_probe)
+        
+    I_sc  = Iscat.reshape(out_shape)
+    
+    
+    if return_value.lower() in ['map', 'map_i', 'i_map']:
+        if r_probe is None:
+            return tetalist, philist, I_sc
+        else:
+            return I_sc
+    elif return_value.lower() in ['efield', 'fields', 'field']:
+        if r_probe is None:
+            return tetalist, philist, Escat
+        else:
+            return Escat
+    else:
+        d_solid_surf = r**2 * np.sin(tetalist) * dteta * dphi
+        if return_value.lower() in ['int_es', 'int']:
+            return np.sum(I_sc * d_solid_surf)
+        
+        else:
+            raise ValueError("Parameter 'return_value' must be one of ['map', 'int_es', 'efield'].")
 
 
 
+# =============================================================================
+# HIGH-LEVEL (pyGDM2 compatibility)
+# =============================================================================
 def extinct(sim, field_index, with_toroidal=True, r0=None, eps_dd=0.001, 
             use_generalized_polarizabilities=False, normalization_E0=True,
             long_wavelength_approx=False):
     """extinction cross sections from multipole decomposition
     
     ** ------- FUNCTION STILL UNDER TESTING ------- **
     
@@ -316,28 +713,46 @@
     arbitrary-shaped nanoparticles on a plane surface.*, 
     JOSA B 30, 2589 (2013)
     
     """
 # =============================================================================
 #     Exception handling
 # =============================================================================
-    if sim.E is None and not use_generalized_polarizabilities:
-        raise ValueError("Error: Scattered field inside the structure not yet evaluated. Run `core.scatter` simulation first.")
 
 # =============================================================================
 #     extinction section calculation
 # =============================================================================
     from pyGDM2 import linear
     from pyGDM2 import tools
     
     ## by default, use center of gravity for multimode expansion
     geo = sim.struct.geometry
     if r0 is None:
         r0 = np.average(geo, axis=0)
     
+    ## get dipole moments
+    if not use_generalized_polarizabilities:
+        p, p1, m, Qe, Qe1, Qm = multipole_decomposition_exact(
+                sim, field_index, r0=r0, 
+                long_wavelength_approx=long_wavelength_approx, 
+                which_moments=['p', 'p1', 'm', 'qe', 'qe1', 'qm'])
+        if not with_toroidal:
+            p = p1
+            Qe = Qe1
+    else:
+        if with_toroidal:
+            p = eval_generalized_polarizability_p(sim, field_index, which_order='p')
+            Qe = eval_generalized_polarizability_qe(sim, field_index, which_order='qe')
+        else:
+            p = eval_generalized_polarizability_p(sim, field_index, which_order='p1')
+            Qe = eval_generalized_polarizability_qe(sim, field_index, which_order='qe1')
+        m = eval_generalized_polarizability_m(sim, field_index)
+        Qm = eval_generalized_polarizability_qm(sim, field_index)
+        
+    ## prefactors and incident field
     field_params = tools.get_field_indices(sim)[field_index]
     wavelength   = field_params['wavelength']
     sim.struct.setWavelength(wavelength)
     k0 = 2*np.pi / wavelength
     eps_env = sim.dyads.getEnvironmentIndices(wavelength, geo[:1])[0]  # structure must be fully in one environment zone
     n_env = (eps_env**0.5).real
     
@@ -354,49 +769,25 @@
     ## normalization
     if normalization_E0:
         E2in = np.sum(np.abs(E0)**2, axis=1)   # intensity of incident field
     else:
         E2in = 1.0
     prefactor = (4 * np.pi * k0 * 1/n_env * 1/E2in).real
     
-    ## get dipole moments
-    if not use_generalized_polarizabilities:
-        p, p1, m, Qe, Qe1, Qm = multipole_decomposition_exact(
-                sim, field_index, r0=r0, 
-                long_wavelength_approx=long_wavelength_approx, 
-                which_moments=['p', 'p1', 'm', 'qe', 'qe1', 'qm'])
-    else:
-        if with_toroidal:
-            p = eval_generalized_polarizability_p(sim, field_index, which_order='p')
-            Qe = eval_generalized_polarizability_qe(sim, field_index, which_order='qe')
-        else:
-            p1 = eval_generalized_polarizability_p(sim, field_index, which_order='p1')
-            Qe1 = eval_generalized_polarizability_qe(sim, field_index, which_order='qe1')
-        m = eval_generalized_polarizability_m(sim, field_index)
-        Qm = eval_generalized_polarizability_qm(sim, field_index)
-
-    
-    
-    if with_toroidal:
-        ecs_p = prefactor * (np.sum(np.conjugate(E0)*p)).imag
-        ecs_Qe = prefactor / 12. * (np.sum(np.tensordot(gradE0cj + gradE0cj.T, Qe) )).imag
-    else:
-        ecs_p = prefactor * (np.sum(np.conjugate(E0)*p1)).imag
-        ecs_Qe = prefactor / 12. * (np.sum(np.tensordot(gradE0cj + gradE0cj.T, Qe1) )).imag
+    ecs_p = prefactor * (np.sum(np.conjugate(E0)*p)).imag
     ecs_m = prefactor / n_env * (np.sum(np.conjugate(H0)*m)).imag
+    ecs_Qe = prefactor / 12. * (np.sum(np.tensordot(gradE0cj + gradE0cj.T, Qe) )).imag
     ecs_Qm = prefactor / n_env / 6 * (np.sum(np.tensordot(gradH0cj.T, Qm) )).imag
     
     return [ecs_p, ecs_m, ecs_Qe, ecs_Qm]
     
-    
-    
-
 
 def scs(sim, field_index, with_toroidal=True, 
-        use_generalized_polarizabilities=False, r0=None, normalization_E0=True,
+        use_generalized_polarizabilities=False, 
+        r0=None, normalization_E0=True,
         long_wavelength_approx=False):
     """total scattering cross section from multipole decomposition
     
     ** ------- FUNCTION STILL UNDER TESTING ------- **
     
     Returns scattering cross sections for electric and magnetic dipole and 
     quadrupole moments of the multipole decomposition.
@@ -454,25 +845,43 @@
     Optics Communications 407, 17–21 (2018)
     
     """
     from pyGDM2 import tools
 # =============================================================================
 #     Exception handling
 # =============================================================================
-    if sim.E is None and not use_generalized_polarizabilities:
-        raise ValueError("Error: Scattered field inside the structure not yet evaluated. Run `core.scatter` simulation first.")
 
 # =============================================================================
 #     scattering section calculation
 # =============================================================================
     ## by default, use center of gravity for multimode expansion
     geo = sim.struct.geometry
     if r0 is None:
         r0 = np.average(geo, axis=0)
     
+    ## get dipole moments
+    if not use_generalized_polarizabilities:
+        p, p1, m, Qe, Qe1, Qm = multipole_decomposition_exact(
+                sim, field_index, r0=r0,
+                which_moments=['p', 'p1', 'm', 'qe', 'qe1', 'qm'], 
+                long_wavelength_approx=long_wavelength_approx)
+        if not with_toroidal:
+            p = p1
+            Qe = Qe1
+    else:
+        if with_toroidal:
+            p = eval_generalized_polarizability_p(sim, field_index, which_order='p', long_wavelength_approx=long_wavelength_approx)
+            Qe = eval_generalized_polarizability_qe(sim, field_index, which_order='qe', long_wavelength_approx=long_wavelength_approx)
+        else:
+            p = eval_generalized_polarizability_p(sim, field_index, which_order='p1', long_wavelength_approx=long_wavelength_approx)
+            Qe = eval_generalized_polarizability_qe(sim, field_index, which_order='qe1', long_wavelength_approx=long_wavelength_approx)
+        m = eval_generalized_polarizability_m(sim, field_index, long_wavelength_approx=long_wavelength_approx)
+        Qm = eval_generalized_polarizability_qm(sim, field_index, long_wavelength_approx=long_wavelength_approx)
+    
+    ## prefactors / illumination fields
     field_params = tools.get_field_indices(sim)[field_index]
     wavelength   = field_params['wavelength']
     sim.struct.setWavelength(wavelength)
     k0 = 2*np.pi / wavelength
     
     eps_env = sim.dyads.getEnvironmentIndices(wavelength, geo[:1])[0]  # assume structure is fully in one environment
     n_env = (eps_env**0.5).real
@@ -486,41 +895,22 @@
     else:
         E2in = 1.0
     
     ## factor 100: cm --> m (cgs units)
     sc_factor_dp = 100/12*(k0**4 / E2in).real
     sc_factor_Q = 100/1440*(k0**4 / E2in).real
     
-    ## the actual scattering sections
-    if not use_generalized_polarizabilities:
-        p, p1, m, Qe, Qe1, Qm = multipole_decomposition_exact(
-                sim, field_index, r0=r0,
-                which_moments=['p', 'p1', 'm', 'qe', 'qe1', 'qm'], 
-                long_wavelength_approx=long_wavelength_approx)
-    else:
-        if with_toroidal:
-            p = eval_generalized_polarizability_p(sim, field_index, which_order='p', long_wavelength_approx=long_wavelength_approx)
-            Qe = eval_generalized_polarizability_qe(sim, field_index, which_order='qe', long_wavelength_approx=long_wavelength_approx)
-        else:
-            p1 = eval_generalized_polarizability_p(sim, field_index, which_order='p1', long_wavelength_approx=long_wavelength_approx)
-            Qe1 = eval_generalized_polarizability_qe(sim, field_index, which_order='qe1', long_wavelength_approx=long_wavelength_approx)
-        m = eval_generalized_polarizability_m(sim, field_index, long_wavelength_approx=long_wavelength_approx)
-        Qm = eval_generalized_polarizability_qm(sim, field_index, long_wavelength_approx=long_wavelength_approx)
-        
-    if with_toroidal:
-        scs_p = sc_factor_dp * np.sum(np.abs(p)**2)
-        scs_Qe = sc_factor_Q * np.sum(np.abs(k*Qe)**2)
-    else:
-        scs_p = sc_factor_dp * np.sum(np.abs(p1)**2)
-        scs_Qe = sc_factor_Q * np.sum(np.abs(k*Qe1)**2)
+    
+    scs_p = sc_factor_dp * np.sum(np.abs(p)**2)
     scs_m = sc_factor_dp * np.sum(np.abs(m)**2)
+    scs_Qe = sc_factor_Q * np.sum(np.abs(k*Qe)**2)
     scs_Qm = sc_factor_Q * np.sum(np.abs(k*Qm)**2)
             
     return [scs_p, scs_m, scs_Qe, scs_Qm]
-    
+
 
 
 def farfield(sim, field_index, 
              r_probe=None,
              r=100000., 
              tetamin=0, tetamax=np.pi/2., Nteta=10, 
              phimin=0, phimax=2*np.pi, Nphi=36, 
@@ -832,622 +1222,19 @@
 
 
 
 
 
 
 
-def _multipole_farfield(wavelength, eps_env, r0=None, 
-                        p=[], m=[], qe=[], qm=[],
-                        r_p=None, r_m=None, r_qe=None, r_qm=None,
-                        r_probe=None,
-                        r=100000., 
-                        tetamin=0, tetamax=np.pi/2., Nteta=10, 
-                        phimin=0, phimax=2*np.pi, Nphi=36, 
-                        return_value='map'):
-    """far-field scattering of an explicit list of multipole moments
-    
-    Radiated electro-magnetic field  (E-field) in the far-field 
-    (by default on a sphere of radius `r` around the nanostructure).
-    
-    
-    Parameters
-    ----------
-    wavelength : float
-        radiation wavelength
-    
-    eps_env : float
-        envirnoment permittivity (real part)
-        
-    r0 : array. optional
-        [x,y,z] position of mulipole decomposition development.
-        Alternatively the positions of each mutlipole can be specified.
-        The default is `None`.
-        
-    p, m, qe, qm : lists of ndarrays. optional
-        lists of dipole and quadrupole moments to propagate to the farfield.
-        The default is [].
-        
-    r_p, r_m, r_qe, r_qm : ndarrays or list of such. optional
-        Has effect only if r0 is not specified. Carthesian coordinates of 
-        each multipole individually.
-    
-    r_probe : tuple (x,y,z) or list of 3-lists/-tuples. optional
-        defaults to *None*, which means it is not used and a solid angle defined by
-        a spherical coordinate range is used instead. If `r_probe` is given, this
-        overrides `r`, `tetamin`, `tetamax`, `Nteta`, `Nphi`.
-        (list of) coordinate(s) to evaluate farfield on. 
-        Format: tuple (x,y,z) or list of 3 lists: [Xmap, Ymap, Zmap] 
-        The default is None. (Not used)
-        
-    r : float, default: 100000.
-        radius of integration sphere (distance to coordinate origin in nm)
-        
-    tetamin, tetamax : float, float; defaults: 0, np.pi/2
-        minimum and maximum polar angle in radians 
-        (in linear steps from `tetamin` to `tetamax`)
-        
-    phimin, phimax : float, float; defaults: 0, 2*np.pi
-        minimum and maximum azimuth angle in radians, excluding last position
-        (in linear steps from `phimin` to `phimax`)
-        
-    Nteta, Nphi : int, int; defaults: 10, 36
-        number of polar and azimuthal angles on sphere to calculate,
-    
-    return_value : str, default: 'map'
-        Values to be returned. Either 'map' (default) or 'integrated'.
-          - "map" : (default) return spatially resolved farfield intensity at each spherical coordinate (5 lists)
-          - "efield" : return spatially resolved E-fields at each spherical coordinate (5 lists)
-          - "int_Es" : return the integrated scattered field (as float)
-    
-    
-    Returns
-    -------
-    using `r_probe` for position definition:
-        3 lists of 6-tuples (x,y,z, Ex,Ey,Ez), complex : 
-            - scattered Efield or E-intensity
-        
-    if solid angle is defined via spherical coordinate range:
-        - return_value == "map" : 5 arrays of shape (Nteta, Nphi) : 
-            - [tetalist : teta angles - if solid angle range input]
-            - [philist : phi angles - if solid angle range input]
-            - I_sc : intensity of scattered field, 
-        
-        - return_value == "efield" : float
-            - [tetalist : teta angles - if solid angle range input]
-            - [philist : phi angles - if solid angle range input]
-            - E_sc : complex scattered field at each pos.
-            
-        - return_value == "int_XX" : float
-            integrated total intensity over specified solid angle
-        
-    
-    Notes
-    -----
-    See equation (G1) in
-    
-    Alaee, R., Rockstuhl, C. & Fernandez-Corbaton, I. *An electromagnetic 
-    multipole expansion beyond the long-wavelength approximation.*
-    Optics Communications 407, 17–21 (2018)
-        
-    """
-# =============================================================================
-#     exception handling
-# =============================================================================
-    if np.pi < tetamax < 0:
-        raise ValueError("`tetamax` out of range, must be in [0, pi]")
-    
-    if r_probe is not None and return_value in ['int_es', 'int_E0', 'int_Etot']:
-        raise ValueError("probing farfield on user-defined positions does not support integration " +
-                         "of the intensity since no surface differential can be defined. Use spherical " +
-                         "coordinate definition to do the integration.")
-    
-    if r0 is None:
-        if r_p is None and r_m is None and r_qe is None and r_qm is None:
-            raise Exception("No positions for the multipoles are given.")
-        if len(r_p) != len(p):
-            raise Exception("Same number of dipole positions and dipole moments required! `p` and `r_p` must be lists of same length.")
-        if len(r_m) != len(m):
-            raise Exception("Same number of dipole positions and dipole moments required! `m` and `r_m` must be lists of same length.")
-        if len(r_qe) != len(qe):
-            raise Exception("Same number of quadrupole positions and quadrupole moments required! `qe` and `r_qe` must be lists of same length.")
-        if len(r_qm) != len(qm):
-            raise Exception("Same number of quadrupole positions and quadrupole moments required! `qm` and `r_qm` must be lists of same length.")
-    else:
-        r0 = np.array(r0)
-        if len(r0) != 3: 
-            raise Exception("Multipole position must be carthesian coordinate (array of 3 float)")
-        r_p = [r0 for _ in p]
-        r_m = [r0 for _ in m]
-        r_qe = [r0 for _ in qe]
-        r_qm = [r0 for _ in qm]
-        
-# =============================================================================
-#     preparation
-# =============================================================================
-    ## --- spherical probe coordinates
-    if r_probe is None:
-        tetalist = np.ones((int(Nteta), int(Nphi)))*np.linspace(tetamin, tetamax, int(Nteta))[:,None]
-        philist = np.ones((int(Nteta), int(Nphi)))*np.linspace(phimin, phimax, int(Nphi), endpoint=False)[None,:]
-        xff = (r * np.sin(tetalist) * np.cos(philist)).flatten()
-        yff = (r * np.sin(tetalist) * np.sin(philist)).flatten()
-        zff = (r * np.cos(tetalist)).flatten()
-        _r_probe = np.transpose([xff, yff, zff])
-    else:
-        _r_probe = r_probe
-        
-    ## --- spherical integration steps
-    dteta = (tetamax-tetamin) / float(Nteta-1)  # endpoint included
-    dphi = (phimax-phimin) / float(Nphi)        # endpoint not included
-    
-    ## --- environment
-    k0 = 2*np.pi / wavelength
-    n_env = (eps_env**0.5).real
-    k = k0*n_env
-    
-#==============================================================================
-#     electric polarization of structure, fundamental field
-#==============================================================================        
-    Escat = np.zeros(shape=(len(_r_probe), 3), dtype=DTYPE_C)
-    
-    def eval_prefactors(r0, _r_probe, k, k0):
-        n_vec = _r_probe - r0
-        R_d = np.linalg.norm(n_vec, axis=1)
-        n_vec = n_vec / R_d[:,None]     # unit vector along direction of scattering
-        
-        phase_factor = np.exp(1j*k*R_d)
-        prefactor = k0**2 * phase_factor / R_d
-        
-        return prefactor, n_vec
-    
-    
-    for _r0, _p in zip(r_p, p):
-        prefactor, n0_vec = eval_prefactors(_r0, _r_probe, k, k0)
-        Es_p = prefactor[:,None] * np.cross(n0_vec, np.cross((_p)[None,:], n0_vec))
-        Escat += Es_p     # sum all electric dipole fields
-    
-    for _r0, _m in zip(r_m, m):
-        prefactor, n0_vec = eval_prefactors(_r0, _r_probe, k, k0)
-        Es_m = prefactor[:,None] * np.cross(_m[None,:], n0_vec)
-        Escat += Es_m     # sum all magnetic dipole fields
-    
-    for _r0, _qe in zip(r_qe, qe):
-        prefactor, n0_vec = eval_prefactors(_r0, _r_probe, k, k0)
-        Es_qe = prefactor[:,None] * 1j * k/6 * np.cross(n0_vec, 
-                    np.cross(n0_vec, np.tensordot(_qe, n0_vec, axes=(-1,-1)).T))
-        Escat += Es_qe     # sum all electric quadrupole fields
-    
-    for _r0, _qm in zip(r_qm, qm):
-        prefactor, n0_vec = eval_prefactors(_r0, _r_probe, k, k0)
-        Es_qm = prefactor[:,None] * 1j * k/6 * np.cross(n0_vec, 
-                    np.tensordot(_qm, n0_vec, axes=(-1,-1)).T)
-        Escat += Es_qm     # sum all magnetic quadrupole fields
-
-    
-    Iscat = np.sum((np.abs(Escat)**2), axis=1)
-
-
-
-#==============================================================================
-#     Intensities with and without fundamental field / polarizer
-#==============================================================================
-    ## --- total field (no polarizer)
-    if r_probe is None:
-        out_shape = tetalist.shape
-    else:
-        out_shape = len(_r_probe)
-        
-    I_sc  = Iscat.reshape(out_shape)
-    
-    
-    if return_value.lower() == 'map':
-        if r_probe is None:
-            return tetalist, philist, I_sc
-        else:
-            return I_sc
-    elif return_value.lower() in ['efield', 'fields', 'field']:
-        if r_probe is None:
-            return tetalist, philist, Escat
-        else:
-            return Escat
-    else:
-        d_solid_surf = r**2 * np.sin(tetalist) * dteta * dphi
-        if return_value.lower() in ['int_es', 'int']:
-            return np.sum(I_sc * d_solid_surf)
-        
-        else:
-            raise ValueError("Parameter 'return_value' must be one of ['map', 'int_es', 'int_e0', 'int_etot'].")
-
-
-
-
-
-
-
-
-
-
-
-# =============================================================================
-# polarizabilities
-# =============================================================================
-def generalized_polarizability(sim, field_index=None, wavelength=None, 
-                               method='lu', epsilon=0.01, r0=None,
-                               which_moments=['p1', 'pt', 'qe', 'qt', 'm', 'qm'],
-                               long_wavelength_approx=False, verbose=1):
-    """generalized electric and magnetic polarizabilities
-    
-    ** ------- FUNCTION STILL UNDER TESTING ------- **
-    
-    Returns the generalized polarizability tensors that can be used with arbitrary,
-    inhomogeneous illumination fields to calculate the effective 
-    electric and magnetic multipole moments, induced in the nanostructure.
-    
-    
-    Parameters
-    ----------
-    sim : :class:`.core.simulation`
-        simulation description
-    
-    field_index : int, default: None
-        index of evaluated self-consistent field to use for calculation. Can be
-        obtained for specific parameter-set using :func:`.tools.get_closest_field_index`.
-        Either `field_index` or `wavelength` must be given.
-    
-    wavelength : float, default: None
-        Optional wavelength (alternative to `field_index`) at which to 
-        calculate susceptibility matrix (in nm). 
-        Either `field_index` or `wavelength` must be given.
-    
-    method : string, default: "scipyinv"
-        inversion method. One of ["lu", "numpyinv", "scipyinv", "cupy", "cuda"]
-         - "scipyinv" scipy default inversion (`scipy.linalg.inv`)
-         - "numpyinv" numpy inversion (`np.linalg.inv`, if numpy compiled accordingly: LAPACK's `dgesv`)
-         - "cupy" uses CUDA GPU via `cupy`
-         - "cuda" (equivalent to "cupy")
-         - "lu" LU-decomposition (`scipy.linalg.lu_factor`) - inefficient for `decay_rate`!
-    
-    epsilon : float, default: 0.01
-        additional step on r0 (in nm) to avoid numerical divergence of the Bessel terms
-        
-    r0 : array, default: None
-        [x,y,z] position of mulipole decomposition development. 
-        If `None`, use structure's center of gravity
-    
-    which_moments : list of str, default: ['p1', 'pt', 'qe1', 'qt', 'm', 'qm']
-        which generalized polarizability tensors to calculate and return. supported:
-            - 'p1': electric dipole - only first order (rank 2)
-            - 'pt': toroidal dipole (rank 3)
-            - 'qe1': electric quadrupole - only first order (rank 4)
-            - 'qt': toroidal electric quadrupole (rank 4)
-            - 'm': magnetic dipole (rank 2)
-            - 'qm': magnetic quadrupole (rank 3)
-            
-    long_wavelength_approx : bool, default: False
-        if True, use long wavelength approximation
-        
-    verbose : bool default=True
-        print runtime info
-    
-    
-    Returns
-    -------
-    
-    by default 6 lists of N tensors, with N the number of discretization cells (see kwarg `which_moments`):
-        
-    K_P_E, K_T_E, K_QE_E, K_QT_E, K_M_E, K_QM_E
-    
-    Notes
-    -----
-    For details , see: 
-        
-    *PAPER SUBMITTED*
-    
-    For details about the underlying exact multipole decomposition, see: 
-        
-    Alaee, R., Rockstuhl, C. & Fernandez-Corbaton, I. *An electromagnetic 
-    multipole expansion beyond the long-wavelength approximation.*
-    Optics Communications 407, 17–21 (2018)
-    
-    """
-    # =============================================================================
-    #     Exception handling
-    # =============================================================================
-    if field_index is None and wavelength is None:
-        raise Exception("Either `field_index` or `wavelength` must be given!")
-        
-    if field_index is not None and wavelength is not None:
-        warnings.warn("`field_index` AND `wavelength` are given! Ignoring `wavelength`.")
-        
-    
-    
-    # =============================================================================
-    # preparation
-    # =============================================================================
-    from pyGDM2 import core
-    
-    which_moments = [wm.lower() for wm in which_moments]
-    
-    if field_index is not None:
-        from pyGDM2 import tools
-        wavelength = tools.get_field_indices(sim)[field_index]['wavelength']
-    
-    if 'p1' in which_moments and not hasattr(sim, 'K_P_E'):
-        sim.K_P_E = dict()
-    if 'pt' in which_moments and not hasattr(sim, 'K_T_E'):
-        sim.K_T_E = dict()
-    if 'qe' in which_moments and not hasattr(sim, 'K_QE_E'):
-        sim.K_QE_E = dict()
-    if 'qt' in which_moments and not hasattr(sim, 'K_QT_E'):
-        sim.K_QT_E = dict()
-    if 'm' in which_moments and not hasattr(sim, 'K_M_E'):
-        sim.K_M_E = dict()
-    if 'qm' in which_moments and not hasattr(sim, 'K_QM_E'):
-        sim.K_QM_E = dict()
-    
-    
-    
-    if verbose:
-        t0 = time.time()
-        print("wl={}nm. calc. K:".format(np.round(wavelength, 1)), end='')
-    
-    
-    ## structure
-    geo = sim.struct.geometry
-    alpha = sim.dyads.getPolarizabilityTensor(wavelength, sim.struct)
-    if r0 is None:
-        r0 = np.average(geo, axis=0)
-    sim.r0 = r0
-    if np.abs(np.linalg.norm(geo - r0, axis=1)).min() > epsilon:
-        epsilon = 0
-    Dr = geo - r0  #   = r-r0
-    norm_r = np.linalg.norm(Dr + epsilon, axis=1)  # epsilon: avoid divergence of 1/kr at r=0
-    norm_r2 = norm_r**2
-    
-    ## illumination properties
-    sim.struct.setWavelength(wavelength)
-    eps_env = sim.dyads.getEnvironmentIndices(wavelength, r0[None,:])[0]  # assume structure is fully in one environment
-    n_env = eps_env**0.5
-    k0 = 2.0*np.pi / wavelength
-    k = k0*n_env
-    kr = k * norm_r
-    
-    ## bessel functions and pre-factors
-    if not long_wavelength_approx:
-        from scipy.special import spherical_jn as sph_jn
-        j0kr = sph_jn(0, kr)
-        j1kr = sph_jn(1, kr) / kr
-        j2kr = sph_jn(2, kr) / (kr**2)
-        j3kr = sph_jn(3, kr) / (kr**3)
-        f_pt = 1/2; f_ptA=3; f_ptB=-1
-        f_qe = 3; fqe2=2; fqe2A = 5; fqe2B = -1; fqe2C = -1
-        f_m = 3/2; f_qm = 15
-    else:
-        j0kr = j1kr = j2kr = j3kr = np.ones_like(kr)
-        f_pt = 1/10; f_ptA=1; f_ptB=-2
-        f_qe = 1; fqe2=1/14; fqe2A = 4; fqe2B = -5; fqe2C = 2
-        f_m = 1/2; f_qm = 1
-    
-    
-    ## ----- gen. propagator
-    K = core.get_general_propagator(sim, wavelength, method=method)
-    if method.lower() in ['cupy', 'cuda']:
-        K = K.get()
-    if method.lower() == 'lu':
-        import scipy.linalg as la
-        K = la.lu_solve(K, np.identity(K[0].shape[0], dtype=K[0].dtype))
-        
-    if verbose:
-        t1 = time.time()
-        print(" {:.1f}ms.  electric... ".format((t1-t0)*1000), end='')
-    K2 = K.reshape(len(K)//3, 3, -1, 3).swapaxes(1,2).reshape(-1, 3, 3).reshape(len(K)//3,len(K)//3, 3, 3)
-    K2a = np.matmul(alpha[:,None,...], K2)
-    Ka = np.concatenate(np.concatenate(K2a, axis=1), axis=1)
 
 
 # =============================================================================
-#     electric-electric
-# =============================================================================
-    ## ----- electric-electric generalized polarizability - dipole
-    if 'p1' in which_moments:
-        K_P_E = np.sum(K2a * j0kr[:,None,None,None], axis=0)
-        sim.K_P_E[wavelength] = K_P_E       # store in simulation object
-
-
-    ## ----- higher order electric moments
-    if 'pt' in which_moments or 'qe' in which_moments or 'qt' in which_moments:
-        K_re = np.zeros_like(Ka)
-        for i_dp in range(len(Ka)):
-            K_re.T[i_dp] = (Dr * Ka.T[i_dp].reshape((len(Ka)//3,3))).reshape((len(Ka),))
-        K2_re = K_re.reshape(len(Ka)//3, 3, -1, 3).swapaxes(1,2).reshape(-1, 3, 3).reshape(len(Ka)//3,len(Ka)//3, 3, 3)
-            
-        
-    ## ----- toroidal dipole generalized polarizability 
-    if 'pt' in which_moments:
-        Qt1 = np.zeros((len(Ka)//3,3,3,3), dtype=np.complex64)
-        Qt2 = np.zeros((len(Ka)//3,3,3), dtype=np.complex64)
-        for i_a in range(3):
-            for i_b in range(3):
-                Qt1[:, i_a, i_b] = np.sum(
-                    (
-                    K2_re[...,i_b,:] * Dr[:,i_a,None,None]
-                      ) * j2kr[:, None, None], axis=0)
-            Qt2[:, i_a] = np.sum(
-                (K2a[...,i_a,:]) * norm_r2[:,None,None]* j2kr[:, None, None], axis=0)
-                
-        K_T1_E = k**2 * f_pt * f_ptA * Qt1 
-        K_T2_E = k**2 * f_pt * f_ptB * Qt2
-    
-        K_T_E = K_T1_E + K_T2_E[...,None,:]/3
-        sim.K_T_E[wavelength] = K_T_E       # store in simulation object
-
-
-    ## ----- electric quadrupole generalized polarizability 
-    krondelta = np.identity(3)
-    if 'qe' in which_moments:
-        Qe11 = np.zeros((len(Ka)//3,3,3,3), dtype=np.complex64)
-        Qe12 = np.zeros((len(Ka)//3,3,3,3,3), dtype=np.complex64)
-
-        for i_a in range(3):
-            for i_b in range(3):
-                Qe11[:, i_a, i_b] = np.sum(
-                    (
-                    3*(Dr[:,i_b,None,None] * K2a[...,i_a,:] +
-                       Dr[:,i_a,None,None] * K2a[...,i_b,:])
-                      ) * j1kr[:, None,None], axis=0)
-                
-                for i_c in range(3):  # keep separate scalar product elements in last index
-                    Qe12[:, i_a, i_b, i_c] = np.sum(
-                        (
-                        - 2*K2_re[...,i_c,:] * krondelta[i_a,i_b]   # diagonal term
-                          ) * j1kr[:, None,None], axis=0)
-        
-        K_QE_E = f_qe * (Qe12 + Qe11[...,None,:]/3)
-        sim.K_QE_E[wavelength] = K_QE_E
-    
-    
-    ## ----- electric toroidal quadrupole generalized polarizability 
-    if 'qt' in which_moments:
-        Qet1 = np.zeros((len(Ka)//3,3,3,3,3), dtype=np.complex64)
-        Qet2 = np.zeros((len(Ka)//3,3,3,3), dtype=np.complex64)
-        Qet3 = np.zeros((len(Ka)//3,3,3,3,3), dtype=np.complex64)
-
-        for i_a in range(3):
-            for i_b in range(3):
-                Qet2[:, i_a, i_b] = np.sum(
-                    (
-                    fqe2B * (Dr[:,i_a,None,None] * K2a[...,i_b,:] + Dr[:,i_b,None,None] * K2a[...,i_a,:])
-                      ) * norm_r2[:,None,None] * j3kr[:, None,None], axis=0)
-                
-                for i_c in range(3):  # keep separate scalar product elements in last index
-                    Qet1[:, i_a, i_b, i_c] = np.sum(
-                        (
-                         fqe2A * K2_re[...,i_c,:] * Dr[:,i_a,None,None] * Dr[:,i_b,None,None]
-                          ) * j3kr[:, None,None], axis=0)
-                    Qet3[:, i_a, i_b, i_c] = np.sum(
-                        (
-                         fqe2C * K2_re[...,i_c,:] * krondelta[i_a,i_b]  # diagonal term
-                          ) * norm_r2[:,None,None] * j3kr[:, None,None], axis=0)
-        K_QT_E = f_qe * fqe2 * k**2 * (Qet1 + Qet2[...,None,:]/3 + Qet3)
-        sim.K_QT_E[wavelength] = K_QT_E
-
-
-
-# =============================================================================
-#     electric-magnetic
-# =============================================================================
-    if 'm' in which_moments or 'qm' in which_moments:
-        if verbose:
-            t2 = time.time()
-            print("{:.1f}ms.  magnetic... ".format((t2-t1)*1000), end='')
-        K_he = np.zeros_like(Ka)
-        for i_dp in range(len(Ka)):
-            K_he.T[i_dp] = np.cross(Dr, Ka.T[i_dp].reshape((len(Ka)//3,3))).reshape((len(Ka),))
-        K2_he = K_he.reshape(len(Ka)//3, 3, -1, 3).swapaxes(1,2).reshape(-1, 3, 3).reshape(len(Ka)//3,len(Ka)//3, 3, 3)
-    
-    
-    ## ----- electric-magnetic generalized polarizability         
-    if 'm' in which_moments:
-        K_M_E = np.sum(K2_he * j1kr[:, None, None, None], axis=0)
-        K_M_E = -1j*k * f_m * K_M_E
-        sim.K_M_E[wavelength] = K_M_E       # store in simulation object
-
-
-    ## ----- electric-magnetic quadrupole generalized polarizability
-    if 'qm' in which_moments:
-        Qm = np.zeros((len(Ka)//3,3,3,3), dtype=np.complex64)
-        for i_a in range(3):
-            for i_b in range(3):
-                Qm[:, i_a, i_b] = np.sum(
-                    (
-                    Dr[:,i_a,None,None] * K2_he[...,i_b,:]  + 
-                    Dr[:,i_b,None,None] * K2_he[...,i_a,:] 
-                      ) * j2kr[:, None, None], axis=0)
-                
-        K_QM_E = -1j*k * f_qm * Qm 
-        sim.K_QM_E[wavelength] = K_QM_E       # store in simulation object
-    
-    
-    if verbose: 
-        print("{:.1f}ms. Done.".format((time.time()-t2)*1000))
-    
+# multipole modes
 # =============================================================================
-#     return results
-# =============================================================================
-    return_list = []
-    for _m in which_moments:
-        if _m.lower() == "p1":
-            return_list.append(K_P_E)
-        if _m.lower() == "pt":
-            return_list.append(K_T_E)
-        if _m.lower() in ["qe"]:
-            return_list.append(K_QE_E)
-        if _m.lower() in ["qt"]:
-            return_list.append(K_QT_E)
-        if _m.lower() == "m":
-            return_list.append(K_M_E)
-        if _m.lower() in ["qm"]:
-            return_list.append(K_QM_E)
-    
-    return return_list
-
-
-
-def _test_availability_generalized_polarizability(sim, which_moment, wavelength, 
-                      method='lu', verbose=False, long_wavelength_approx=False):
-    which_moment = which_moment.lower()
-    wl = wavelength
-    
-    calc_gp = False
-    if which_moment in ['p1', 'p0', 'p']:
-        if not hasattr(sim, 'K_P_E'):
-            calc_gp = True
-        elif wl not in sim.K_P_E.keys():
-            calc_gp = True
-            
-    if which_moment in ['pt', 'p']:
-        if not hasattr(sim, 'K_T_E'):
-            calc_gp = True
-        elif wl not in sim.K_T_E.keys():
-            calc_gp = True
-            
-    if which_moment == 'm':
-        if not hasattr(sim, 'K_M_E'):
-            calc_gp = True
-        elif wl not in sim.K_M_E.keys():
-            calc_gp = True
-            
-    if which_moment in ['qe1', 'qe0', 'qe']:
-        if not hasattr(sim, 'K_QE_E'):
-            calc_gp = True
-        elif wl not in sim.K_QE_E.keys():
-            calc_gp = True
-            
-    if which_moment in ['qet', 'qe']:
-        if not hasattr(sim, 'K_QT_E'):
-            calc_gp = True
-        elif wl not in sim.K_QT_E.keys():
-            calc_gp = True
-            
-    if which_moment == 'qm':
-        if not hasattr(sim, 'K_QM_E'):
-            calc_gp = True
-        elif wl not in sim.K_QM_E.keys():
-            calc_gp = True
-    
-    if calc_gp:
-        if verbose:
-            warnings.warn('generalized polarizabilities not available. evaluating...')
-        generalized_polarizability(sim, wavelength=wl, method=method, 
-                                   long_wavelength_approx=long_wavelength_approx)
-
-        
-    
-
-
 def density_of_multipolar_modes(sim, field_index=None, wavelength=None, return_mode_energy=True, 
                                 which_moments=['p', 'm', 'qe', 'qm'], 
                                 method='lu', long_wavelength_approx=False):
     """Calculate total density of multipole modes via generalized polarizability
     
     If not yet calculated, will invoke generalize pola. calculation, thus it may
     require some computation time on the first call.
@@ -1550,351 +1337,7 @@
             out_list.append(np.sum(np.linalg.norm(sim.K_QM_E[wavelength], axis=(1,2)))**exp_order)
     
     return out_list
 
 
 
 
-def eval_generalized_polarizability_p(sim, field_index, which_order='p', method='lu', 
-                                      long_wavelength_approx=False):
-    """get electric dipole moment via generalized polarizability
-    
-    will evaluate generalized pola. and store it in simulation, in case it 
-    is not yet calculated.
-    
-    Parameters
-    ----------
-    sim : :class:`.core.simulation`
-        simulation description
-    
-    field_index : int, default: None
-        index of evaluated self-consistent field to use for calculation. Can be
-        obtained for specific parameter-set using :func:`.tools.get_closest_field_index`.
-        Either `field_index` or `wavelength` must be given.
-        
-    which_order : str, optional
-        The default is 'p'. One of:
-            - 'p': full dipole moment including toroidal contribution
-            - 'p1': only first order dipole
-            - 'pt': only toroidal dipole moment
-    
-    method : string, default: "lu"
-        inversion method if generalized pola. not yet calculated. 
-        One of ["lu", "numpyinv", "scipyinv", "cupy", "cuda"]
-        
-    long_wavelength_approx : bool, default: False
-        if True, use long wavelength approximation
-
-
-    Returns
-    -------
-    electric dipole moment (complex vector)
-
-    """
-    from pyGDM2 import tools
-    
-    kws_wl = tools.get_field_indices(sim)[field_index]
-    wl = kws_wl['wavelength']
-    
-    for which_moment in ['p1', 'pt']:
-        _test_availability_generalized_polarizability(sim, which_moment, 
-              wl, method=method, long_wavelength_approx=long_wavelength_approx)
-    
-        
-    K_P_E = sim.K_P_E[wl]
-    K_T_E = sim.K_T_E[wl]
-    
-    ## illuminatin field for 'field_index'
-    env_dict = sim.dyads.getConfigDictG(wl, sim.struct, sim.efield)
-    E0 = sim.efield.field_generator(sim.struct.geometry, env_dict, **kws_wl)
-    
-    if which_order.lower() in ['p', 'p0', 'p1']:  # 'p0' equiv. to 'p1'
-        p1 = np.sum(np.matmul(K_P_E, E0[...,None]), axis=(0,2))
-        if which_order.lower() in ['p0', 'p1']:
-            p = p1
-        
-    if which_order.lower() in ['p', 'pt']:
-        pt = np.array([np.sum(np.matmul(K_T_E[...,i,:,:], E0[:,:,None]), axis=(0,2)) for i in range(3)])
-        pt = np.sum(pt, axis=1)
-        if which_order.lower() == 'p':
-            p = p1 + pt
-        else:
-            p = pt
-    return p
-
-
-def eval_generalized_polarizability_qe(sim, field_index, which_order='qe', method='lu', 
-                                      long_wavelength_approx=False):
-    """get electric quadrupole moment via generalized polarizability
-    
-    will evaluate generalized pola. and store it in simulation, in case it 
-    is not yet calculated.
-    
-    Parameters
-    ----------
-    sim : :class:`.core.simulation`
-        simulation description
-    
-    field_index : int, default: None
-        index of evaluated self-consistent field to use for calculation. Can be
-        obtained for specific parameter-set using :func:`.tools.get_closest_field_index`.
-        Either `field_index` or `wavelength` must be given.
-        
-    which_order : str, optional
-        The default is 'qe'. One of:
-            - 'qe': full electric quadrupole moment (including toroidal contribution)
-            - 'qe1': only first order contribution to quadrupole
-            - 'qet': only toroidal quadrupole moment
-            
-    method : string, default: "lu"
-        inversion method if generalized pola. not yet calculated. 
-        One of ["lu", "numpyinv", "scipyinv", "cupy", "cuda"]
-        
-    long_wavelength_approx : bool, default: False
-        if True, use long wavelength approximation
-
-        
-    Returns
-    -------
-    electric quadrupole moment (complex tensor, 3x3)
-
-    """
-    from pyGDM2 import tools
-    
-    kws_wl = tools.get_field_indices(sim)[field_index]
-    wl = kws_wl['wavelength']
-    
-    for which_moment in ['qe', 'qt']:
-        _test_availability_generalized_polarizability(sim, which_moment, 
-              wl, method=method, long_wavelength_approx=long_wavelength_approx)
-    
-        
-    K_QE_E = sim.K_QE_E[wl]
-    K_QT_E = sim.K_QT_E[wl]
-    
-    ## illumination field for 'field_index'
-    env_dict = sim.dyads.getConfigDictG(wl, sim.struct, sim.efield)
-    E0 = sim.efield.field_generator(sim.struct.geometry, env_dict, **kws_wl)
-    
-    
-    if which_order.lower() in ['q', 'qe', 'qe0', 'qe1']:  # 'qe0' equiv. to 'qe1'
-        qe1 = np.array([
-            [np.sum(np.matmul(K_QE_E[...,i,j,:,:], E0[:,:,None]), axis=(0,2)) 
-                                         for j in range(3)] for i in range(3)])
-        qe1 = np.sum(qe1, axis=-1)
-        if which_order.lower() in ['qe0', 'qe1']:
-            qe = qe1
-        
-    if which_order.lower() in ['q', 'qe', 'qet', 'qt']:
-        qet = np.array([
-            [np.sum(np.matmul(K_QT_E[...,i,j,:,:], E0[:,:,None]), axis=(0,2)) 
-                                         for j in range(3)] for i in range(3)])
-        qet = np.sum(qet, axis=-1)
-        if which_order.lower() in ['q', 'qe']:  # 'q' equiv. to 'qe'
-            qe = qe1 + qet
-        else:
-            qe = qet
-    return qe
-
-
-def eval_generalized_polarizability_m(sim, field_index, method='lu', 
-                                      long_wavelength_approx=False):
-    """get magnetic dipole moment via generalized polarizability
-    
-    will evaluate generalized pola. and store it in simulation, in case it 
-    is not yet calculated.
-    
-    Parameters
-    ----------
-    sim : :class:`.core.simulation`
-        simulation description
-    
-    field_index : int, default: None
-        index of evaluated self-consistent field to use for calculation. Can be
-        obtained for specific parameter-set using :func:`.tools.get_closest_field_index`.
-        Either `field_index` or `wavelength` must be given.
-            
-    method : string, default: "lu"
-        inversion method if generalized pola. not yet calculated. 
-        One of ["lu", "numpyinv", "scipyinv", "cupy", "cuda"]
-        
-    long_wavelength_approx : bool, default: False
-        if True, use long wavelength approximation
-
-        
-    Returns
-    -------
-    magnetic quadrupole moment (complex vector)
-
-    """
-    from pyGDM2 import tools
-    
-    kws_wl = tools.get_field_indices(sim)[field_index]
-    wl = kws_wl['wavelength']
-    
-    for which_moment in ['m']:
-        _test_availability_generalized_polarizability(sim, which_moment, 
-              wl, method=method, long_wavelength_approx=long_wavelength_approx)     
-    
-    K_M_E = sim.K_M_E[wl]
-    
-    ## illuminatin field for 'field_index'
-    env_dict = sim.dyads.getConfigDictG(wl, sim.struct, sim.efield)
-    E0 = sim.efield.field_generator(sim.struct.geometry, env_dict, **kws_wl)
-    
-    m = np.sum(np.matmul(K_M_E, E0[...,None]), axis=(0,2))
-    
-    return m
-
-
-def eval_generalized_polarizability_qm(sim, field_index, method='lu', 
-                                      long_wavelength_approx=False):
-    """get magnetic quadrupole moment via generalized polarizability
-    
-    will evaluate generalized pola. and store it in simulation, in case it 
-    is not yet calculated.
-    
-    Parameters
-    ----------
-    sim : :class:`.core.simulation`
-        simulation description
-    
-    field_index : int, default: None
-        index of evaluated self-consistent field to use for calculation. Can be
-        obtained for specific parameter-set using :func:`.tools.get_closest_field_index`.
-        Either `field_index` or `wavelength` must be given.
-            
-    method : string, default: "lu"
-        inversion method if generalized pola. not yet calculated. 
-        One of ["lu", "numpyinv", "scipyinv", "cupy", "cuda"]
-        
-    long_wavelength_approx : bool, default: False
-        if True, use long wavelength approximation
-
-        
-    Returns
-    -------
-    magnetic quadrupole tensor (complex tensor, 3x3)
-
-    """
-    from pyGDM2 import tools
-    
-    kws_wl = tools.get_field_indices(sim)[field_index]
-    wl = kws_wl['wavelength']
-    
-    for which_moment in ['qm']:
-        _test_availability_generalized_polarizability(sim, which_moment, 
-              wl, method=method, long_wavelength_approx=long_wavelength_approx)
-    
-    K_QM_E = sim.K_QM_E[wl]
-    
-    ## illuminatin field for 'field_index'
-    env_dict = sim.dyads.getConfigDictG(wl, sim.struct, sim.efield)
-    E0 = sim.efield.field_generator(sim.struct.geometry, env_dict, **kws_wl)
-    
-    qm = np.array([np.sum(np.matmul(K_QM_E[...,i,:,:], E0[:,:,None]), axis=(0,2)) for i in range(3)])
-    
-    return qm
-
-
-def extract_effective_polarizability(sim, method='lu',
-                                     which_moments=['p1','m'], long_wavelength_approx=True,
-                                     illumination_mode='dipole', npoints=25, r_sphere=1000):
-    """Extract effective electric and magnetic dipole polarizability for structure
-    
-    solve inverse problem of adjusting polarizability for different illuminations
-    via pseudoinverse
-    
-    *doc to be completed*
-    
-    """
-    from pyGDM2 import fields
-    from pyGDM2 import tools
-    from scipy import linalg
-    
-    def sample_spherical(npoints, ndim=3):
-        """random pos. on sphere (R=1). from: https://stackoverflow.com/questions/33976911"""
-        vec = np.random.randn(ndim, npoints)
-        vec /= np.linalg.norm(vec, axis=0)
-        return vec
-
-    ## dipoles of random position and random orientation
-    wavelengths = sim.efield.wavelengths
-    
-    r0 = np.average(sim.struct.geometry, axis=0)
-    sim.r0 = r0
-    
-
-    if illumination_mode.lower() == 'dipole':
-        rnd_pos = sample_spherical(npoints, ndim=3).T * r_sphere
-        field_kwargs = [
-            dict(x0=rnd_pos[i,0], y0=rnd_pos[i,1], z0=rnd_pos[i,2], 
-                 mx=np.random.random()*r_sphere,
-                 my=np.random.random()*r_sphere,
-                 mz=np.random.random()*r_sphere)
-            for i in range(npoints)
-            ]
-        field_generator = fields.dipole_electric
-    else:
-    ## -- alternative: plane wave with different polarizations / incident angles
-        field_kwargs = [
-            dict(inc_angle=0, inc_plane='xz', E_s=0.0, E_p=1.0),
-            dict(inc_angle=0, inc_plane='xz', E_s=1.0, E_p=0.0),
-            dict(inc_angle=90, inc_plane='xz', E_s=1.0, E_p=0.0),
-            dict(inc_angle=90, inc_plane='xz', E_s=0.0, E_p=1.0),
-            dict(inc_angle=90, inc_plane='yz', E_s=1.0, E_p=0.0),
-            dict(inc_angle=90, inc_plane='yz', E_s=0.0, E_p=1.0),
-            ]
-        field_generator = fields.plane_wave
-    
-    n_illum = len(field_kwargs)
-    efield = fields.efield(field_generator, wavelengths=wavelengths, kwargs=copy.deepcopy(field_kwargs))
-    _sim = sim.copy()
-    _sim.efield = efield
-    _sim.scatter(method=method)
-    
-    ahh = []
-    aee = []
-    for i_wl, wl in enumerate(wavelengths):
-        p_eval = np.zeros((3, n_illum), dtype=np.complex64)
-        m_eval = np.zeros((3, n_illum), dtype=np.complex64)
-        E0_eval = np.zeros((3, n_illum), dtype=np.complex64)
-        H0_eval = np.zeros((3, n_illum), dtype=np.complex64)
-        for idx, kw  in enumerate(field_kwargs):
-            ## illuminatin field for 'field_index'
-            env_dict = _sim.dyads.getConfigDictG(wl, _sim.struct, _sim.efield)
-            E0 = efield.field_generator([_sim.r0], env_dict, wavelength=wl, **kw)[0]
-            # inc. field array shape: (3, n_fields)
-            E0_eval[:, idx] = E0
-            
-            H0 = efield.field_generator([_sim.r0], env_dict, wavelength=wl, returnField='H', **kw)[0]
-            H0_eval[:, idx] = H0
-            
-            kw_wl = kw.copy()
-            kw_wl['wavelength'] = wl
-            field_index = tools.get_closest_field_index(_sim, kw_wl)
-            p, m = multipole_decomposition_exact(_sim, field_index, which_moments=which_moments, 
-                                                 long_wavelength_approx=long_wavelength_approx)
-            p_eval[...,idx] = p
-            m_eval[...,idx] = m
-        
-        ## pseudo-inverse of all illuminations
-        AEinv = linalg.pinv(np.conj(E0_eval).T)
-        AHinv = linalg.pinv(np.conj(H0_eval).T)
-        
-        ## optimum alphas to obtain dipole moments for each illumination
-        alpha_pinv = np.conj(np.dot(AEinv, np.conj(p_eval).T)).T
-        alpha_minv = np.conj(np.dot(AHinv, np.conj(m_eval).T)).T
-        
-        aee.append(alpha_pinv.reshape([3,3]))
-        ahh.append(alpha_minv.reshape([3,3]))
-    
-    dict_pola_pseudo = dict(
-                sim=sim, r0=sim.r0, r0_MD=sim.r0, r0_ED=sim.r0, 
-                alpha_EE=aee, 
-                alpha_HH=ahh, 
-                wavelengths=sim.efield.wavelengths, 
-                k0_spectrum=2 * np.pi / np.array(wavelengths).copy(),
-                 )
-    
-    return dict_pola_pseudo
-
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/nonlinear.py` & `pyGDM2-1.1.4/pyGDM2/nonlinear.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/propagators/__init__.py` & `pyGDM2-1.1.4/pyGDM2/propagators/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/propagators/propagators.py` & `pyGDM2-1.1.4/pyGDM2/propagators/propagators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/propagators/propagators_2D.py` & `pyGDM2-1.1.4/pyGDM2/propagators/propagators_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/propagators/propagators_periodic.py` & `pyGDM2-1.1.4/pyGDM2/propagators/propagators_periodic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/propagators/propagators_periodic_slow.py` & `pyGDM2-1.1.4/pyGDM2/propagators/propagators_periodic_slow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/structures.py` & `pyGDM2-1.1.4/pyGDM2/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
@@ -207,18 +207,23 @@
             if verbose or len(set(self.material)) < 6:  # print details for up to 5 sub-constituents
                 diff_mat = np.unique([s.__name__ for s in self.material])
                 for i, mat in enumerate(set(diff_mat)):
                     out_str += '\n' + '      - {}: "{}"'.format(i, mat)
         out_str += '\n' + '   mesh type:            {}'.format(self.meshtype)
         out_str += '\n' + '   nominal stepsize:     {}nm'.format(self.step)
         out_str += '\n' + '   nr. of meshpoints:    {}'.format(self.n_dipoles)
+        bnds = [self.geometry.T[0].min()-self.step/2, self.geometry.T[0].max()+self.step/2, 
+                self.geometry.T[1].min()-self.step/2, self.geometry.T[1].max()+self.step/2, 
+                self.geometry.T[2].min()-self.step/2, self.geometry.T[2].max()+self.step/2]
         if verbose:
-            out_str += '\n' + '     X-extension    :    {:.1f} - {:.1f} (nm)'.format(self.geometry.T[0].min(), self.geometry.T[0].max() )
-            out_str += '\n' + '     Y-extension    :    {:.1f} - {:.1f} (nm)'.format(self.geometry.T[1].min(), self.geometry.T[1].max() )
-            out_str += '\n' + '     Z-extension    :    {:.1f} - {:.1f} (nm)'.format(self.geometry.T[2].min(), self.geometry.T[2].max() )
+            out_str += '\n' + '     X-extension    :    {:.1f} - {:.1f} (nm)'.format(bnds[0], bnds[1])
+            out_str += '\n' + '     Y-extension    :    {:.1f} - {:.1f} (nm)'.format(bnds[2], bnds[3])
+            out_str += '\n' + '     Z-extension    :    {:.1f} - {:.1f} (nm)'.format(bnds[4], bnds[5])
+        else:
+            out_str += '\n' + '   bounding box:         [{:.1f},{:.1f}], [{:.1f},{:.1f}], [{:.1f},{:.1f}] (nm)'.format(*bnds)
         return out_str
     
     def __add__(self, other):
         if type(other) in [struct, struct_py]:
             ## add a structure: Try combining both
             return combine_geometries([self.copy(), other.copy()], step=self.step)
         elif len(other)==3:
@@ -636,15 +641,15 @@
     
     if mesh == 'cube':
         sp = _meshCubic( (-int(L), int(L)), (-int(W), int(W)+1), (-1, int(H)+1), conditionRect)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-(int(L)), int(L)+1), (-int(W), int(W)+1), (-1, 2*int(H)+1), 
                                     conditionRect, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T
+    sp = np.array(sp, dtype=np.float32).T
     sp *= step
     dipoles = sp.T
     
     
     
     return dipoles
 
@@ -739,15 +744,15 @@
         sp = _meshCubic( (-1*int(NL)-10, int(NL)+10), (-1*int(np.ceil(NL))-10, int(np.ceil(NL))+10), 
                          (-1*int(np.ceil(H))-10, int(np.ceil(H))+10),  conditionPrism)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*int(NL)-10, int(NL)+10), (-1*int(np.ceil(NL))-10, int(np.ceil(NL))+10), 
                                     (-1*int(np.ceil(H))-10, int(np.ceil(H))+10), 
                                     conditionPrism, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift Z so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     dipoles = sp.T
     
     return dipoles
 
 
@@ -795,15 +800,15 @@
     if mesh == 'cube':
         sp = _meshCubic( (-1*int(L)-5, int(L)+5), (-1*int(L)-5, int(L)+5), 
                          (-1, int(H)+1), conditionRhombus)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*int(L)-1, int(L)+1), (-1*int(L)-5, int(L)+5), 
                                     (-1, int(H)+1), conditionRhombus, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift Z so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     dipoles = sp.T
     
     return dipoles
 
 
@@ -848,15 +853,15 @@
         sp = _meshCubic( (-1*int(NL)-10, int(NL)+10), (-1*int(np.ceil(NL))-10, int(np.ceil(NL))+10), 
                          (-1*int(np.ceil(H))-10, int(np.ceil(H))+10),  conditionHexagon)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*int(NL)-10, int(NL)+10), (-1*int(np.ceil(NL))-10, int(np.ceil(NL))+10), 
                                     (-1*int(np.ceil(H))-10, int(np.ceil(H))+10), 
                                     conditionHexagon, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift Z so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     
     rotate *= np.pi/180.
     rotX = sp[0]*np.cos(rotate) - sp[1]*np.sin(rotate)
     rotY = sp[0]*np.sin(rotate) + sp[1]*np.cos(rotate)
     sp[0]=rotX
@@ -927,15 +932,15 @@
                          (-1*int(np.ceil(H)) - 2, int(np.ceil(H)) + 2),  conditionHexagon)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*int(NL) + min([-2,DX-5]), int(NL) + max([2,DX+5])), 
                                     (-1*int(np.ceil(NL)) + min([-2,DY-5]), int(np.ceil(NL)) + max([2,DY+5])), 
                                     (-1*int(np.ceil(H)) - 2, int(np.ceil(H)) + 2), 
                                     conditionHexagon, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift Z so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     
     rotate *= np.pi/180.
     rotX = sp[0]*np.cos(rotate) - sp[1]*np.sin(rotate)
     rotY = sp[0]*np.sin(rotate) + sp[1]*np.cos(rotate)
     sp[0]=rotX
@@ -1023,15 +1028,15 @@
         sp = _meshCubic( (-1*int(NL)-1, int(NL)+1), (-1*int(np.ceil(NL))-1, int(np.ceil(NL))+1), 
                          (-1*int(np.ceil(H))-1, int(np.ceil(H))+1),  conditionPrism)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*int(NL)-1, int(NL)+1), (-1*int(np.ceil(NL))-1, int(np.ceil(NL))+1), 
                                     (-1*int(np.ceil(H))-1, int(np.ceil(H))+1), 
                                     conditionPrism, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift Z so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     dipoles = sp.T
     
     return dipoles
 
 
@@ -1154,15 +1159,15 @@
     elif mesh == 'hex':
         sp = _meshHexagonalCompact(limits_X, limits_Y, limits_Z, 
                                    cond_poly, ORIENTATION)
     
     if verbose:
         print("polygon structure - elapsed time: {:.4f}s".format(time.time()-t0))
     
-    sp = np.array(sp, dtype=np.float).T
+    sp = np.array(sp, dtype=np.float32).T
     sp *= step
     dipoles = sp.T
     
     return dipoles
 
 
 def sphere(step, R, mesh='cube', ORIENTATION=1):
@@ -1193,15 +1198,15 @@
         sp = _meshCubic( (-2*int(R), 2*int(R)+1), (-2*int(R), 2*int(R)+1), 
                          (-2*int(R), 2*int(R)+1),  conditionSphere)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-2*int(R), 2*int(R)+1), (-2*int(R), 2*int(R)+1), 
                                     (-2*int(R), 2*int(R)+1), 
                                     conditionSphere, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     dipoles = sp.T
     
     return dipoles
 
 
@@ -1247,15 +1252,15 @@
         sp = _meshCubic( (-2*int(R1), 2*int(R1)+1), (-2*int(R2), 2*int(R2)+1), 
                          (-2*int(R3), 2*int(R3)+1),  conditionSpheroid)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-2*int(R1), 2*int(R1)+1), (-2*int(R2), 2*int(R2)+1), 
                                     (-2*int(R3), 2*int(R3)+1), 
                                     conditionSpheroid, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     dipoles = sp.T
     
     return dipoles
 
 
@@ -1303,15 +1308,15 @@
         sp = _meshCubic( (-1*int(R)-L/2-2, 1*int(R)+L/2+2), (-1*int(R)-2, 1*int(R)+2), 
                          (0, int(np.ceil(H))),  conditionRod)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact(  (-1*int(R)-5-L/2, 1*int(R)+5+L/2), 
                                      (-1*int(R)-5, 1*int(R)+5), (0, int(np.ceil(H))),
                                     conditionRod, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     dipoles = sp.T
     
     return dipoles
 
 
@@ -1353,15 +1358,15 @@
         sp = _meshCubic( (-1*int(L), 1*int(L)+1), (-2*int(R), 2*int(R)+1), 
                          (-2*int(R), 2*int(R)+1),  conditionRod)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*int(L), 1*int(L)+1), (-2*int(R), 2*int(R)+1), 
                                     (-2*int(R), 2*int(R)+1), 
                                     conditionRod, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     dipoles = sp.T
     
     return dipoles
 
 
@@ -1408,15 +1413,15 @@
         sp = _meshCubic( (-1*int(R)-2, 1*int(R)+2), (-1*int(R)-2, 1*int(R)+2), 
                          (0, H+1),  conditionCone)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact(  (-1*int(R)-5, 1*int(R)+5), 
                                      (-1*int(R)-5, 1*int(R)+5), (0, H+3),
                                     conditionCone, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T*step
+    sp = np.array(sp, dtype=np.float32).T*step
     sp[2] -= np.min(sp[2])  # shift so that bottom at z=0
     sp[2] += step/2         # shift so that bottom at z=step/2
     dipoles = sp.T
     
     return dipoles
 
 
@@ -1456,15 +1461,15 @@
     
     if mesh == 'cube':
         sp = _meshCubic( (-1*abs(DELTA)-W-1, L+abs(DELTA)+2), (-1*abs(DELTA)-W-1, L+abs(DELTA)+2), (0, H+2), conditionRod)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*DELTA-W-1, L+DELTA+2), (-1*DELTA-W-1, L+DELTA+2), (0, H+2), 
                                     conditionRod, ORIENTATION)
     
-    Rect1 = np.array(sp, dtype=np.float).T*step
+    Rect1 = np.array(sp, dtype=np.float32).T*step
     dipoles = Rect1.T
     
     return dipoles
 
 
 def lshape_rect_nonsym(step, L1,W1, L2,W2, H, DELTA, mesh='cube', ORIENTATION=1):
     """
@@ -1508,15 +1513,15 @@
     L=L1+L2
     if mesh == 'cube':
         sp = _meshCubic( (-1*abs(DELTA)-W-1, L+abs(DELTA)+2), (-1*abs(DELTA)-W-1, L+abs(DELTA)+2), (0, H+2), conditionRod)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*DELTA-W-1, L+DELTA+2), (-1*DELTA-W-1, L+DELTA+2), (0, H+2), 
                                     conditionRod, ORIENTATION)
     
-    Rect1 = np.array(sp, dtype=np.float).T*step
+    Rect1 = np.array(sp, dtype=np.float32).T*step
     dipoles = Rect1.T
     
     return dipoles
 
 
 
 def lshape_round(step, L,W,H, DELTA, RAD, mesh='cube', ORIENTATION=1):
@@ -1582,15 +1587,15 @@
     
     if mesh == 'cube':
         sp = _meshCubic( (-1*abs(DELTA)-W-1, L+abs(DELTA)+2), (-1*abs(DELTA)-W-1, L+abs(DELTA)+2), (0, H+2), conditionRod)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*DELTA-W-10, L+DELTA+10), (-1*DELTA-W-10, L+DELTA+10), (0, H+2), 
                                     conditionRod, ORIENTATION)
     
-    Rect1 = np.array(sp, dtype=np.float).T*step
+    Rect1 = np.array(sp, dtype=np.float32).T*step
     dipoles = Rect1.T
     
     return dipoles
 
 
 
 def split_ring(step, R, W, H, G=-1, alphaG=0.0, mesh='cube', ORIENTATION=1):
@@ -1639,15 +1644,15 @@
     
     if mesh == 'cube':
         sp = _meshCubic( (-1*int(R)-5, int(R)+5), (-1*int(R)-5, int(R)+5), (-1, int(H)+1), conditionSR)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1*int(R)-5, int(R)+5), (-1*int(R)-5, int(R)+5), (-1, int(H)+1), 
                                     conditionSR, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T
+    sp = np.array(sp, dtype=np.float32).T
     sp *= step
     dipoles = sp.T
     
     return dipoles
 
 
 
@@ -1692,15 +1697,15 @@
     
     if mesh == 'cube':
         sp = _meshCubic( (-1, int(L1+W)+1), (-1, int(L2+W)+1), (-1, int(H)+1), conditionSR)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact( (-1, int(L1+W)+1), (-1, int(L2+W)+1), (-1, int(H)+1), 
                                     conditionSR, ORIENTATION)
     
-    sp = np.array(sp, dtype=np.float).T
+    sp = np.array(sp, dtype=np.float32).T
     sp[0] -= L1/2; sp[1] -= L2/2
     sp *= step
     dipoles = sp.T
     
     
     
     return dipoles
@@ -1960,45 +1965,51 @@
     def condition(xi,yi,zi):
         return data[int(xi)][int(yi)] != 0
     
     if mesh == 'cube':
         sp = _meshCubic([0, data.shape[0]], [0, data.shape[1]], [0, H], condition)
     elif mesh == 'hex':
         sp = _meshHexagonalCompact([0, data.shape[0]], [0, data.shape[1]], [0, H], condition, ORIENTATION, auto_expand_range=False)
-    sp = np.array(sp, dtype=np.float).T*stepsize
+    sp = np.array(sp, dtype=np.float32).T*stepsize
     sp[2] -= np.min(sp[2])  # shift Z so that bottom at z=0
     sp[2] += stepsize/2         # shift Z so that bottom at z=step/2
     struct = sp.T
     
     if center_structure:
         struct = center_struct(struct)
     
     if returnImage:
         return data0, struct
     else:
         return struct
 
 
 
-def struct_to_image(STRUCT, RGB=True, minimum_size=-1, projection='XY'):
+def struct_to_image(STRUCT, RGB=True, minimum_size=-1, center_struct='half', projection='XY'):
     """generate image-compatible array from structure geometry
     
     Parameters
     ----------
     struct : list of tuple *or* :class:`.core.simulation`
         list of coordinate tuples or instance of :class:`.core.simulation`
     
     RGB : bool, default: True
         If True, generates an RGB array. If False, generate a 2D array with 
         simply 0 and 1 as entries (0: no material, 1: material)
     
     minimum_size : int, default: -1
-        minimum canvas size in pixels. -1: use structure extensions. If >0:
-        enlarge canvas and center structure if structure extensions smaller
-        than image.
+        minimum canvas size in pixels. 
+        -1: use structure extensions. absolute position will be lost!
+        If >0: enlarge canvas and center structure if structure extensions 
+        smaller than image.
+        
+    center_struct : str, default: 'half'
+        Has no effect if minimum_size==-1.
+        how to place structure in canvas. 'half': origin (0,0) is at half x/y.
+        'auto': center structure relative to image. absolute position will be lost!
     
     projection : str, default: "XY"
         2D plane for projection. One of ['XY', 'XZ', 'YZ']
     
     Returns
     -------
     np.array for image conisting of rgb tuples for each pixel.
@@ -2013,28 +2024,32 @@
     elif projection.lower() == 'yz':
         X,Y = _Y,_Z
     elif projection.lower() == 'xz':
         X,Y = _X,_Z
         
     X /= float(step)
     Y /= float(step)
-    X -= X.min()
-    Y -= Y.min()
+    if center_struct.lower()=='auto' or minimum_size==-1:
+        X -= X.min()
+        Y -= Y.min()
+    else:
+        X += minimum_size//2
+        Y += minimum_size//2
     
     ## -- optionally enlarge canvas and center struct
     if minimum_size <= X.max():
         DX = int(X.max()+1)
     else:
-        X += int((minimum_size - X.max())/2.)
+        if center_struct.lower()=='auto': X += int((minimum_size - X.max())/2.)
         DX = minimum_size
         
     if minimum_size <= Y.max():
         DY = int(Y.max()+1)
     else:
-        Y += int((minimum_size - Y.max())/2.)
+        if center_struct.lower()=='auto': Y += int((minimum_size - Y.max())/2.)
         DY = minimum_size
     
     struct=np.transpose([X,Y])
     
     ## -- generate 2D image array
     if RGB:
         arr = np.full( (DX,DY,3), 255 , dtype=np.uint8 )
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/tools.py` & `pyGDM2-1.1.4/pyGDM2/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/visu.py` & `pyGDM2-1.1.4/pyGDM2/visu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
@@ -87,16 +87,17 @@
 
 
 ########################################################################
 ##                      VISUALIZATION FUNCTIONS
 ########################################################################
 def structure(struct, projection='auto', color='auto', scale=1, 
               borders=3, marker='s', lw=0.1, EACHN=1, tit='',
-              plot_legend=True,
-              ax=None, absscale=False, show=True, **kwargs):
+              colors_multimat=None,
+              plot_legend=True, ax=None, absscale=False, show=True, 
+              **kwargs):
     """plot structure in 2d, projected to e.g. the XY plane
     
     plot the structure `struct` as a scatter projection to a carthesian plane.
     Either from list of coordinates, or using a simulation definition as input.
     
     kwargs are passed to matplotlib's `scatter`
     
@@ -127,14 +128,17 @@
           
     EACHN : int, default: 1 (=all)
           show each `EACHN` points only
     
     tit : str, default: ""
         title for plot (optional)
     
+    colors_multimat : list, default: None
+        optional list of colors (matplotlib compatible) to use for different materials
+    
     plot_legend : bool, default: True
         whether to add a legend if multi-material structure (requires auto-color enabled)
     
     ax : matplotlib `axes`, default: None (=create new)
            axes object (matplotlib) to plot into
            
     absscale : bool, default: False
@@ -216,15 +220,18 @@
         scale = min([scale_w, scale_h])
     
     ## --- if multi-material: set maker colors
     if color != 'auto':
         im = ax.scatter(X,Y, marker=marker, s=scale**2,
                         c=color, edgecolors=color, lw=lw, **kwargs)
     else:
-        colors = ['C{}'.format(i) for i in range(1,10)]*int(2 + len(indices_subsets)/9.)
+        if colors_multimat is None:
+            colors = ['C{}'.format(i) for i in range(1,10)]*int(2 + len(indices_subsets)/9.)
+        else:
+            colors = colors_multimat
         for i, idx in enumerate(indices_subsets):
             col = colors[i]
             if plot_legend:
                 label = different_materials[i]
             else:
                 label = ''
             im = ax.scatter(X[idx],Y[idx], marker=marker, s=scale**2,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2/visu3d.py` & `pyGDM2-1.1.4/pyGDM2/visu3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding: utf-8
 #
-#Copyright (C) 2017-2022, P. R. Wiecha
+#Copyright (C) 2017-2023, P. R. Wiecha
 #
 #This program is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, either version 3 of the License, or
 #(at your option) any later version.
 #
 #This program is distributed in the hope that it will be useful,
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2.egg-info/PKG-INFO` & `pyGDM2-1.1.4/pyGDM2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pyGDM2
-Version: 1.1.3.2
+Version: 1.1.4
 Summary: A python full-field electrodynamical solver, based on the Green dyadic method (volume integral technique in frequency domain).
 Home-page: https://gitlab.com/wiechapeter/pyGDM2
-Download-URL: 
 Author: Peter R. Wiecha
 Author-email: pwiecha@laas.fr
 License: GPLv3+
 Keywords: coupled dipoles method,green dyadic method,electrodynamical simulations,nano optics,frequency-domain
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 ***********************************
 Requirements / Installation
 ***********************************
 
 pyGDM is an open source python toolkit for electro-dynamical simulations, implementing the `Green dyadic method (GDM) <https://doi.org/10.1088/0034-4885/68/8/R05>`_, a volume discretization technique. 
@@ -147,7 +148,9 @@
    - P\. R. Wiecha
 
 
 
    
 
 
+
+
```

### Comparing `pyGDM2-1.1.3.2/pyGDM2.egg-info/SOURCES.txt` & `pyGDM2-1.1.4/pyGDM2.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 examples/04_tutorials/using_callbacks.py
 examples/04_tutorials/visualize_incident_field.py
 pyGDM2/__init__.py
 pyGDM2/core.py
 pyGDM2/electron.py
 pyGDM2/linear.py
 pyGDM2/materials.py
-pyGDM2/multipole.py
 pyGDM2/nonlinear.py
 pyGDM2/structures.py
 pyGDM2/tools.py
 pyGDM2/visu.py
 pyGDM2/visu3d.py
 pyGDM2.egg-info/PKG-INFO
 pyGDM2.egg-info/SOURCES.txt
@@ -69,14 +68,19 @@
 pyGDM2/EO/tools.py
 pyGDM2/fields/__init__.py
 pyGDM2/fields/deprecated.py
 pyGDM2/fields/efield_class.py
 pyGDM2/fields/electron.py
 pyGDM2/fields/focused_beams.py
 pyGDM2/fields/regular.py
+pyGDM2/multipole/__init__.py
+pyGDM2/multipole/main.py
+pyGDM2/multipole/polarizabilities.py
+pyGDM2/multipole/processing.py
+pyGDM2/multipole/propagators.py
 pyGDM2/propagators/__init__.py
 pyGDM2/propagators/propagators.py
 pyGDM2/propagators/propagators_2D.py
 pyGDM2/propagators/propagators_periodic.py
 pyGDM2/propagators/propagators_periodic_slow.py
 tests/basic_tests.py
 tests/tests_propagators.py
```

### Comparing `pyGDM2-1.1.3.2/setup.py` & `pyGDM2-1.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         openmp_linker = ""
 
 
 
 # =============================================================================
 # with or without fortran modules?
 # =============================================================================
+package_list=['pyGDM2', 'pyGDM2.fields', 'pyGDM2.propagators', 'pyGDM2.multipole', 'pyGDM2.EO']
+
 if ("--with-fortran" in sys.argv):
     sys.argv.remove("--with-fortran")
     print ("Compiling fortran module (former implementation).\n"+
            "Accessible under `pyGDM2.f_api`.")
     optional_fortran_extension = \
             [Extension(
                     name = 'pyGDM2.f_api.pyGDMfor', 
@@ -112,19 +114,18 @@
                        'fortranBase/routines_decayrate.f90',
                               ],
                     define_macros = [('F2PY_REPORT_ON_ARRAY_COPY','1')],
                     extra_compile_args = [openmp, '-O3', '-mcmodel=medium'],
                     extra_link_args = [openmp_linker, '-O3'],
                     )
              ]
-    package_list=['pyGDM2', 'pyGDM2.fields', 'pyGDM2.propagators', 
-                  'pyGDM2.EO', 'pyGDM2.f_api']
+    package_list.append('pyGDM2.f_api')
 else:
     optional_fortran_extension = []
-    package_list=['pyGDM2', 'pyGDM2.fields', 'pyGDM2.propagators', 'pyGDM2.EO']
+    
     
 print ("\n" + 60*'#' + 2*"\n")
 
 
 
 # =============================================================================
 # main setup    
@@ -141,20 +142,21 @@
     long_description=read('README.rst'),
     packages=package_list,
     ext_modules=optional_fortran_extension,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Scientific/Engineering :: Physics",
         "Environment :: Console",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Intended Audience :: Science/Research"
     ],
     url = 'https://gitlab.com/wiechapeter/pyGDM2',
     download_url = '',
     keywords = ['coupled dipoles method', 'green dyadic method', 'electrodynamical simulations', 'nano optics', 'frequency-domain'],
     install_requires=['numpy', 'numba'],
-    python_requires='>=3.5',
+    python_requires='>=3.7',
 )
```

### Comparing `pyGDM2-1.1.3.2/tests/basic_tests.py` & `pyGDM2-1.1.4/tests/basic_tests.py`

 * *Files identical despite different names*

### Comparing `pyGDM2-1.1.3.2/tests/tests_propagators.py` & `pyGDM2-1.1.4/tests/tests_propagators.py`

 * *Files identical despite different names*

