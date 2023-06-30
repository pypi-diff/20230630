# Comparing `tmp/pymbd-0.9.2.tar.gz` & `tmp/pymbd-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymbd-0.9.2.tar", last modified: Sat Aug  1 15:24:06 2020, max compression
+gzip compressed data, was "pymbd-0.9.3.tar", last modified: Sun Aug  2 11:11:20 2020, max compression
```

## Comparing `pymbd-0.9.2.tar` & `pymbd-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    16726 2017-12-05 21:59:36.000000 pymbd-0.9.2/LICENSE
--rw-r--r--   0        0        0     4817 2020-08-01 14:48:15.559929 pymbd-0.9.2/README.md
--rw-r--r--   0        0        0      960 2020-06-23 07:45:20.114193 pymbd-0.9.2/build.py
--rw-r--r--   0        0        0     1530 2020-08-01 14:50:42.990647 pymbd-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2209 2020-06-21 10:40:03.771571 pymbd-0.9.2/src/mbd.h
--rw-r--r--   0        0        0      164 2020-06-23 07:45:20.118956 pymbd-0.9.2/src/pymbd/__init__.py
--rw-r--r--   0        0        0    11757 2020-06-28 22:17:29.980014 pymbd-0.9.2/src/pymbd/fortran.py
--rw-r--r--   0        0        0    11370 2020-06-23 07:45:20.120396 pymbd-0.9.2/src/pymbd/pymbd.py
--rw-r--r--   0        0        0     4890 2020-06-23 07:45:20.121046 pymbd-0.9.2/src/pymbd/tensorflow.py
--rw-r--r--   0        0        0     1786 2020-06-23 07:45:20.121502 pymbd-0.9.2/src/pymbd/utils.py
--rw-r--r--   0        0        0    17151 2020-06-23 07:45:20.121991 pymbd-0.9.2/src/pymbd/vdw-params.csv
--rw-r--r--   0        0        0     5799 2020-08-01 15:24:06.499988 pymbd-0.9.2/setup.py
--rw-r--r--   0        0        0     6074 2020-08-01 15:24:06.501103 pymbd-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    16726 2017-12-05 21:59:36.000000 pymbd-0.9.3/LICENSE
+-rw-r--r--   0        0        0     5337 2020-08-02 11:01:19.165948 pymbd-0.9.3/README.md
+-rw-r--r--   0        0        0      960 2020-06-23 07:45:20.114193 pymbd-0.9.3/build.py
+-rw-r--r--   0        0        0     1559 2020-08-02 10:58:34.961879 pymbd-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2209 2020-06-21 10:40:03.771571 pymbd-0.9.3/src/mbd.h
+-rw-r--r--   0        0        0      164 2020-06-23 07:45:20.118956 pymbd-0.9.3/src/pymbd/__init__.py
+-rw-r--r--   0        0        0      658 2020-08-02 10:58:06.436907 pymbd-0.9.3/src/pymbd/__main__.py
+-rw-r--r--   0        0        0    11770 2020-08-01 23:05:34.713598 pymbd-0.9.3/src/pymbd/fortran.py
+-rw-r--r--   0        0        0    11370 2020-06-23 07:45:20.120396 pymbd-0.9.3/src/pymbd/pymbd.py
+-rw-r--r--   0        0        0     4903 2020-08-01 23:04:02.328819 pymbd-0.9.3/src/pymbd/tensorflow.py
+-rw-r--r--   0        0        0     1786 2020-06-23 07:45:20.121502 pymbd-0.9.3/src/pymbd/utils.py
+-rw-r--r--   0        0        0    17151 2020-06-23 07:45:20.121991 pymbd-0.9.3/src/pymbd/vdw-params.csv
+-rw-r--r--   0        0        0     6358 2020-08-02 11:11:21.078938 pymbd-0.9.3/setup.py
+-rw-r--r--   0        0        0     6623 2020-08-02 11:11:21.080291 pymbd-0.9.3/PKG-INFO
```

### Comparing `pymbd-0.9.2/LICENSE` & `pymbd-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymbd-0.9.2/README.md` & `pymbd-0.9.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 # Libmbd
 
-[![build](https://img.shields.io/travis/jhrmnn/libmbd/master.svg)](https://travis-ci.com/jhrmnn/libmbd)
+[![build](https://img.shields.io/travis/com/jhrmnn/libmbd/master.svg)](https://travis-ci.com/jhrmnn/libmbd)
 [![coverage](https://img.shields.io/codecov/c/github/jhrmnn/libmbd.svg)](https://codecov.io/gh/jhrmnn/libmbd)
 ![python](https://img.shields.io/pypi/pyversions/pymbd.svg)
-[![release](https://img.shields.io/github/release/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/releases)
-[![conda](https://img.shields.io/conda/v/libmbd/pymbd.svg)](https://anaconda.org/libmbd/pymbd)
+[![conda](https://img.shields.io/conda/vn/conda-forge/libmbd.svg)](https://anaconda.org/conda-forge/libmbd)
 [![pypi](https://img.shields.io/pypi/v/pymbd.svg)](https://pypi.org/project/pymbd/)
 [![commits since](https://img.shields.io/github/commits-since/jhrmnn/libmbd/latest.svg)](https://github.com/jhrmnn/libmbd/releases)
 [![last commit](https://img.shields.io/github/last-commit/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/commits/master)
 [![license](https://img.shields.io/github/license/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/blob/master/LICENSE)
 [![code style](https://img.shields.io/badge/code%20style-black-202020.svg)](https://github.com/ambv/black)
+[![doi](https://img.shields.io/badge/doi-10.5281%2Fzenodo.594879-blue)](http://doi.org/10.5281/zenodo.594879)
 
 Libmbd implements the [many-body dispersion](http://dx.doi.org/10.1063/1.4865104) (MBD) method in several programming languages and frameworks:
 
 - The Fortran implementation is the reference, most advanced implementation, with support for analytical gradients and distributed parallelism, and additional functionality beyond the MBD method itself. It provides a low-level and a high-level Fortran API, as well as a C API. Furthermore, Python bindings to the C API are provided.
 - The Python/Numpy implementation is intended for prototyping, and as a high-level language reference.
 - The Python/Tensorflow implementation is an experiment that should enable rapid prototyping of machine learning applications with MBD.
 
 The Python-based implementations as well as Python bindings to the Libmbd C API are accessible from the Python package called Pymbd.
 
-## Installing Pymbd
+## Installing
 
-The easiest way to get Pymbd is to install the Pymbd [Conda](https://conda.io/docs/) package, which ships with pre-built Libmbd.
+**TL;DR** Install prebuilt Libmbd binaries via [Conda-forge](https://conda-forge.org) and Pymbd with [Pip](https://pip.pypa.io/en/stable/quickstart/).
 
 ```
-conda install -c libmbd pymbd
+conda install -c conda-forge libmbd
+pip install pymbd
 ```
 
-Alternatively, if you have Libmbd already installed on your system (see below), you can install Pymbd with Pip, in which case it links against the installed Libmbd. To support Libmbd built with ScaLAPACK/MPI, the `mpi` extras is required, which installs `mpi4py` as an extra dependency.
+One can also install the ScaLAPACK/MPI version.
 
 ```
-pip install pymbd  # or pymbd[mpi]
+conda install -c conda-forge 'libmbd=*=mpi_*' mpi4py
+pip install pymbd[mpi]
 ```
 
-If Libmbd is installed in a non-standard location, you can point Pymbd to it with
+Verify installation with
 
 ```
-env LIBMBD_PREFIX=<path to Libmbd> pip install pymbd
-```
-
-If you don’t need the Fortran bindings in Pymbd, you can install it without the C extension, in which case `pymbd.fortran` becomes unimportable:
-
-```
-env LIBMBD_PREFIX= pip install pymbd
+$ python -m pymbd
+Expected energy:   -0.0002462647623815428
+Calculated energy: -0.0002462647623817456
 ```
 
-## Installing Libmbd
+###  Libmbd
 
 Libmbd uses CMake for compiling and installing, and requires a Fortran compiler, LAPACK, and optionally ScaLAPACK/MPI.
 
 On Ubuntu:
 
 ```bash
 apt-get install gfortran libblas-dev liblapack-dev [mpi-default-dev mpi-default-bin libscalapack-mpi-dev]
@@ -69,14 +67,41 @@
 cmake .. [-DENABLE_SCALAPACK_MPI=ON]
 make
 make install
 ```
 
 This installs the Libmbd shared library, C API header file, and high-level Fortran API module file.
 
+### Pymbd
+
+Pymbd can be installed and updated using [Pip](https://pip.pypa.io/en/stable/quickstart/), but requires installed Libmbd as a dependency (see above).
+
+```
+pip install pymbd
+```
+
+To support Libmbd built with ScaLAPACK/MPI, the `mpi` extras is required, which installs `mpi4py` as an extra dependency. In this case one has to make sure that `mpi4py` is linked against the same MPI library as Libmbd (for instance by compiling both manually, or installing both via Conda-forge).
+
+```
+pip install pymbd[mpi]
+```
+
+If Libmbd is installed in a non-standard location, you can point Pymbd to it with
+
+```
+env LIBMBD_PREFIX=<path to Libmbd install prefix> pip install pymbd
+```
+
+If you don’t need the Fortran bindings in Pymbd, you can install it without the C extension, in which case `pymbd.fortran` becomes unimportable:
+
+```
+env LIBMBD_PREFIX= pip install pymbd
+```
+
+
 ## Examples
 
 ```python
 from pymbd import mbd_energy_species, ang
 from pymbd.fortran import MBDCalc
 
 ene_py = mbd_energy_species(  # pure Python implementation
```

### Comparing `pymbd-0.9.2/build.py` & `pymbd-0.9.3/build.py`

 * *Files identical despite different names*

### Comparing `pymbd-0.9.2/pyproject.toml` & `pymbd-0.9.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1", "cffi"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "pymbd"
-version = "0.9.2"
+version = "0.9.3"
 description = "Many-body dispersion library"
 authors = ["Jan Hermann <dev@jan.hermann.name>"]
 readme = "README.md"
 packages = [{ include = "pymbd", from = "src" }]
 repository = "https://github.com/jhrmnn/libmbd"
 documentation = "https://jhrmnn.github.io/libmbd/pymbd"
 license = "MPL-2.0"
@@ -29,28 +29,28 @@
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.5"
 scipy = "^1"
 numpy = "^1"
+cffi = "^1"
 pytest = { version = "^5", optional = true }
 mpi4py = { version = "^3", optional = true }
 
 [tool.poetry.extras]
 mpi = ["mpi4py"]
 test = ["pytest"]
 
 [tool.poetry.dev-dependencies]
-cffi = "^1"
 flake8 = "^3.5"
 flake8-bugbear = "^19"
 flake8-comprehensions = "^2"
 flake8-quotes = "^2"
 black = { version = ">=19-beta.0", python = "^3.6" }
 pydocstyle = "^5"
 pep8-naming = "^0.8"
-isort = "^4.3"
+isort = { version = "^5", python = "^3.6" }
 
 [tool.black]
 target-version = ["py35"]
 skip-string-normalization = true
```

### Comparing `pymbd-0.9.2/src/mbd.h` & `pymbd-0.9.3/src/mbd.h`

 * *Files identical despite different names*

### Comparing `pymbd-0.9.2/src/pymbd/fortran.py` & `pymbd-0.9.3/src/pymbd/fortran.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         return self._lattice.copy()
 
     @lattice.setter
     def lattice(self, lattice):
         _lib.cmbd_update_lattice(self._geom_f, _cast('double*', _array(lattice)))
 
     def has_lattice(self):
-        """True if a crystal."""
+        """Whether structure is a crystal."""
         return self._lattice is not None
 
     @_auto_context
     def ts_energy(self, alpha_0, C6, R_vdw, sR, d=20.0, damping='fermi'):
         """Calculate a TS energy.
 
         :param array-like alpha_0: (a.u.) atomic polarizabilities
```

### Comparing `pymbd-0.9.2/src/pymbd/pymbd.py` & `pymbd-0.9.3/src/pymbd/pymbd.py`

 * *Files identical despite different names*

### Comparing `pymbd-0.9.2/src/pymbd/tensorflow.py` & `pymbd-0.9.3/src/pymbd/tensorflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 from __future__ import division, print_function
 
 from math import pi
 
 import numpy as np
-
 import tensorflow as tf
 
 from .pymbd import freq_grid
 
+__all__ = ()
+
 pi = tf.constant(pi, tf.float64)
 ang = 1 / 0.529177249
 
 
 class MBDEvaluator(object):
     def __init__(self, gradients=False, **kwargs):
         self._inputs = coords, alpha_0, C6, R_vdw, beta = [
```

### Comparing `pymbd-0.9.2/src/pymbd/utils.py` & `pymbd-0.9.3/src/pymbd/utils.py`

 * *Files identical despite different names*

### Comparing `pymbd-0.9.2/src/pymbd/vdw-params.csv` & `pymbd-0.9.3/src/pymbd/vdw-params.csv`

 * *Files identical despite different names*

### Comparing `pymbd-0.9.2/setup.py` & `pymbd-0.9.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 packages = \
 ['pymbd']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1,<2', 'scipy>=1,<2']
+['cffi>=1,<2', 'numpy>=1,<2', 'scipy>=1,<2']
 
 extras_require = \
 {'mpi': ['mpi4py>=3,<4'], 'test': ['pytest>=5,<6']}
 
 setup_kwargs = {
     'name': 'pymbd',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Many-body dispersion library',
-    'long_description': "# Libmbd\n\n[![build](https://img.shields.io/travis/jhrmnn/libmbd/master.svg)](https://travis-ci.com/jhrmnn/libmbd)\n[![coverage](https://img.shields.io/codecov/c/github/jhrmnn/libmbd.svg)](https://codecov.io/gh/jhrmnn/libmbd)\n![python](https://img.shields.io/pypi/pyversions/pymbd.svg)\n[![release](https://img.shields.io/github/release/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/releases)\n[![conda](https://img.shields.io/conda/v/libmbd/pymbd.svg)](https://anaconda.org/libmbd/pymbd)\n[![pypi](https://img.shields.io/pypi/v/pymbd.svg)](https://pypi.org/project/pymbd/)\n[![commits since](https://img.shields.io/github/commits-since/jhrmnn/libmbd/latest.svg)](https://github.com/jhrmnn/libmbd/releases)\n[![last commit](https://img.shields.io/github/last-commit/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/commits/master)\n[![license](https://img.shields.io/github/license/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/blob/master/LICENSE)\n[![code style](https://img.shields.io/badge/code%20style-black-202020.svg)](https://github.com/ambv/black)\n\nLibmbd implements the [many-body dispersion](http://dx.doi.org/10.1063/1.4865104) (MBD) method in several programming languages and frameworks:\n\n- The Fortran implementation is the reference, most advanced implementation, with support for analytical gradients and distributed parallelism, and additional functionality beyond the MBD method itself. It provides a low-level and a high-level Fortran API, as well as a C API. Furthermore, Python bindings to the C API are provided.\n- The Python/Numpy implementation is intended for prototyping, and as a high-level language reference.\n- The Python/Tensorflow implementation is an experiment that should enable rapid prototyping of machine learning applications with MBD.\n\nThe Python-based implementations as well as Python bindings to the Libmbd C API are accessible from the Python package called Pymbd.\n\n## Installing Pymbd\n\nThe easiest way to get Pymbd is to install the Pymbd [Conda](https://conda.io/docs/) package, which ships with pre-built Libmbd.\n\n```\nconda install -c libmbd pymbd\n```\n\nAlternatively, if you have Libmbd already installed on your system (see below), you can install Pymbd with Pip, in which case it links against the installed Libmbd. To support Libmbd built with ScaLAPACK/MPI, the `mpi` extras is required, which installs `mpi4py` as an extra dependency.\n\n```\npip install pymbd  # or pymbd[mpi]\n```\n\nIf Libmbd is installed in a non-standard location, you can point Pymbd to it with\n\n```\nenv LIBMBD_PREFIX=<path to Libmbd> pip install pymbd\n```\n\nIf you don’t need the Fortran bindings in Pymbd, you can install it without the C extension, in which case `pymbd.fortran` becomes unimportable:\n\n```\nenv LIBMBD_PREFIX= pip install pymbd\n```\n\n## Installing Libmbd\n\nLibmbd uses CMake for compiling and installing, and requires a Fortran compiler, LAPACK, and optionally ScaLAPACK/MPI.\n\nOn Ubuntu:\n\n```bash\napt-get install gfortran libblas-dev liblapack-dev [mpi-default-dev mpi-default-bin libscalapack-mpi-dev]\n```\n\nOn macOS:\n\n```bash\nbrew install gcc [open-mpi scalapack]\n```\n\nThe compiling and installation can then proceed with\n\n```\ngit clone https://github.com/jhrmnn/libmbd.git && cd libmbd\nmkdir build && cd build\ncmake .. [-DENABLE_SCALAPACK_MPI=ON]\nmake\nmake install\n```\n\nThis installs the Libmbd shared library, C API header file, and high-level Fortran API module file.\n\n## Examples\n\n```python\nfrom pymbd import mbd_energy_species, ang\nfrom pymbd.fortran import MBDCalc\n\nene_py = mbd_energy_species(  # pure Python implementation\n    [(0, 0, 0), (0, 0, 4*ang)], ['Ar', 'Ar'], [1, 1], 0.83\n)\nwith MBDCalc() as calc:\n    ene_f = calc.mbd_energy_species(  # Fortran implementation\n        [(0, 0, 0), (0, 0, 4*ang)], ['Ar', 'Ar'], [1, 1], 0.83\n    )\nassert abs(ene_f-ene_py) < 1e-15\n```\n\n```fortran\nuse mbd, only: mbd_input_t, mbd_calc_t\n\ntype(mbd_input_t) :: inp\ntype(mbd_calc_t) :: calc\nreal(8) :: energy, gradients(3, 2)\ninteger :: code\ncharacter(200) :: origin, msg\n\ninp%atom_types = ['Ar', 'Ar']\ninp%coords = reshape([0d0, 0d0, 0d0, 0d0, 0d0, 7.5d0], [3, 2])\ninp%xc = 'pbe'\ncall calc%init(inp)\ncall calc%get_exception(code, origin, msg)\nif (code > 0) then\n    print *, msg\n    stop\nend if\ncall calc%update_vdw_params_from_ratios([0.98d0, 0.98d0])\ncall calc%evaluate_vdw_method(energy)\ncall calc%get_gradients(gradients)\ncall calc%destroy()\n```\n\n## Links\n\n- Libmbd documentation: https://jhrmnn.github.io/libmbd\n- Pymbd documentation: https://jhrmnn.github.io/libmbd/pymbd\n\n## Developing\n\nFor development, Libmbd doesn't have to be installed on the system, and Pymbd can be linked against local installation of Libmbd.\n\n```\ngit clone https://github.com/jhrmnn/libmbd.git && cd libmbd\npython3 -m venv venv && source venv/bin/activate\nmake\n# development work...\nmake\n```\n",
+    'long_description': "# Libmbd\n\n[![build](https://img.shields.io/travis/com/jhrmnn/libmbd/master.svg)](https://travis-ci.com/jhrmnn/libmbd)\n[![coverage](https://img.shields.io/codecov/c/github/jhrmnn/libmbd.svg)](https://codecov.io/gh/jhrmnn/libmbd)\n![python](https://img.shields.io/pypi/pyversions/pymbd.svg)\n[![conda](https://img.shields.io/conda/vn/conda-forge/libmbd.svg)](https://anaconda.org/conda-forge/libmbd)\n[![pypi](https://img.shields.io/pypi/v/pymbd.svg)](https://pypi.org/project/pymbd/)\n[![commits since](https://img.shields.io/github/commits-since/jhrmnn/libmbd/latest.svg)](https://github.com/jhrmnn/libmbd/releases)\n[![last commit](https://img.shields.io/github/last-commit/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/commits/master)\n[![license](https://img.shields.io/github/license/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/blob/master/LICENSE)\n[![code style](https://img.shields.io/badge/code%20style-black-202020.svg)](https://github.com/ambv/black)\n[![doi](https://img.shields.io/badge/doi-10.5281%2Fzenodo.594879-blue)](http://doi.org/10.5281/zenodo.594879)\n\nLibmbd implements the [many-body dispersion](http://dx.doi.org/10.1063/1.4865104) (MBD) method in several programming languages and frameworks:\n\n- The Fortran implementation is the reference, most advanced implementation, with support for analytical gradients and distributed parallelism, and additional functionality beyond the MBD method itself. It provides a low-level and a high-level Fortran API, as well as a C API. Furthermore, Python bindings to the C API are provided.\n- The Python/Numpy implementation is intended for prototyping, and as a high-level language reference.\n- The Python/Tensorflow implementation is an experiment that should enable rapid prototyping of machine learning applications with MBD.\n\nThe Python-based implementations as well as Python bindings to the Libmbd C API are accessible from the Python package called Pymbd.\n\n## Installing\n\n**TL;DR** Install prebuilt Libmbd binaries via [Conda-forge](https://conda-forge.org) and Pymbd with [Pip](https://pip.pypa.io/en/stable/quickstart/).\n\n```\nconda install -c conda-forge libmbd\npip install pymbd\n```\n\nOne can also install the ScaLAPACK/MPI version.\n\n```\nconda install -c conda-forge 'libmbd=*=mpi_*' mpi4py\npip install pymbd[mpi]\n```\n\nVerify installation with\n\n```\n$ python -m pymbd\nExpected energy:   -0.0002462647623815428\nCalculated energy: -0.0002462647623817456\n```\n\n###  Libmbd\n\nLibmbd uses CMake for compiling and installing, and requires a Fortran compiler, LAPACK, and optionally ScaLAPACK/MPI.\n\nOn Ubuntu:\n\n```bash\napt-get install gfortran libblas-dev liblapack-dev [mpi-default-dev mpi-default-bin libscalapack-mpi-dev]\n```\n\nOn macOS:\n\n```bash\nbrew install gcc [open-mpi scalapack]\n```\n\nThe compiling and installation can then proceed with\n\n```\ngit clone https://github.com/jhrmnn/libmbd.git && cd libmbd\nmkdir build && cd build\ncmake .. [-DENABLE_SCALAPACK_MPI=ON]\nmake\nmake install\n```\n\nThis installs the Libmbd shared library, C API header file, and high-level Fortran API module file.\n\n### Pymbd\n\nPymbd can be installed and updated using [Pip](https://pip.pypa.io/en/stable/quickstart/), but requires installed Libmbd as a dependency (see above).\n\n```\npip install pymbd\n```\n\nTo support Libmbd built with ScaLAPACK/MPI, the `mpi` extras is required, which installs `mpi4py` as an extra dependency. In this case one has to make sure that `mpi4py` is linked against the same MPI library as Libmbd (for instance by compiling both manually, or installing both via Conda-forge).\n\n```\npip install pymbd[mpi]\n```\n\nIf Libmbd is installed in a non-standard location, you can point Pymbd to it with\n\n```\nenv LIBMBD_PREFIX=<path to Libmbd install prefix> pip install pymbd\n```\n\nIf you don’t need the Fortran bindings in Pymbd, you can install it without the C extension, in which case `pymbd.fortran` becomes unimportable:\n\n```\nenv LIBMBD_PREFIX= pip install pymbd\n```\n\n\n## Examples\n\n```python\nfrom pymbd import mbd_energy_species, ang\nfrom pymbd.fortran import MBDCalc\n\nene_py = mbd_energy_species(  # pure Python implementation\n    [(0, 0, 0), (0, 0, 4*ang)], ['Ar', 'Ar'], [1, 1], 0.83\n)\nwith MBDCalc() as calc:\n    ene_f = calc.mbd_energy_species(  # Fortran implementation\n        [(0, 0, 0), (0, 0, 4*ang)], ['Ar', 'Ar'], [1, 1], 0.83\n    )\nassert abs(ene_f-ene_py) < 1e-15\n```\n\n```fortran\nuse mbd, only: mbd_input_t, mbd_calc_t\n\ntype(mbd_input_t) :: inp\ntype(mbd_calc_t) :: calc\nreal(8) :: energy, gradients(3, 2)\ninteger :: code\ncharacter(200) :: origin, msg\n\ninp%atom_types = ['Ar', 'Ar']\ninp%coords = reshape([0d0, 0d0, 0d0, 0d0, 0d0, 7.5d0], [3, 2])\ninp%xc = 'pbe'\ncall calc%init(inp)\ncall calc%get_exception(code, origin, msg)\nif (code > 0) then\n    print *, msg\n    stop\nend if\ncall calc%update_vdw_params_from_ratios([0.98d0, 0.98d0])\ncall calc%evaluate_vdw_method(energy)\ncall calc%get_gradients(gradients)\ncall calc%destroy()\n```\n\n## Links\n\n- Libmbd documentation: https://jhrmnn.github.io/libmbd\n- Pymbd documentation: https://jhrmnn.github.io/libmbd/pymbd\n\n## Developing\n\nFor development, Libmbd doesn't have to be installed on the system, and Pymbd can be linked against local installation of Libmbd.\n\n```\ngit clone https://github.com/jhrmnn/libmbd.git && cd libmbd\npython3 -m venv venv && source venv/bin/activate\nmake\n# development work...\nmake\n```\n",
     'author': 'Jan Hermann',
     'author_email': 'dev@jan.hermann.name',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/jhrmnn/libmbd',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pymbd-0.9.2/PKG-INFO` & `pymbd-0.9.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymbd
-Version: 0.9.2
+Version: 0.9.3
 Summary: Many-body dispersion library
 Home-page: https://github.com/jhrmnn/libmbd
 License: MPL-2.0
 Author: Jan Hermann
 Author-email: dev@jan.hermann.name
 Requires-Python: >=3.5,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,70 +19,69 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: mpi
 Provides-Extra: test
+Requires-Dist: cffi (>=1,<2)
 Requires-Dist: mpi4py (>=3,<4); extra == "mpi"
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: pytest (>=5,<6); extra == "test"
 Requires-Dist: scipy (>=1,<2)
 Project-URL: Documentation, https://jhrmnn.github.io/libmbd/pymbd
 Project-URL: Repository, https://github.com/jhrmnn/libmbd
 Description-Content-Type: text/markdown
 
 # Libmbd
 
-[![build](https://img.shields.io/travis/jhrmnn/libmbd/master.svg)](https://travis-ci.com/jhrmnn/libmbd)
+[![build](https://img.shields.io/travis/com/jhrmnn/libmbd/master.svg)](https://travis-ci.com/jhrmnn/libmbd)
 [![coverage](https://img.shields.io/codecov/c/github/jhrmnn/libmbd.svg)](https://codecov.io/gh/jhrmnn/libmbd)
 ![python](https://img.shields.io/pypi/pyversions/pymbd.svg)
-[![release](https://img.shields.io/github/release/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/releases)
-[![conda](https://img.shields.io/conda/v/libmbd/pymbd.svg)](https://anaconda.org/libmbd/pymbd)
+[![conda](https://img.shields.io/conda/vn/conda-forge/libmbd.svg)](https://anaconda.org/conda-forge/libmbd)
 [![pypi](https://img.shields.io/pypi/v/pymbd.svg)](https://pypi.org/project/pymbd/)
 [![commits since](https://img.shields.io/github/commits-since/jhrmnn/libmbd/latest.svg)](https://github.com/jhrmnn/libmbd/releases)
 [![last commit](https://img.shields.io/github/last-commit/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/commits/master)
 [![license](https://img.shields.io/github/license/jhrmnn/libmbd.svg)](https://github.com/jhrmnn/libmbd/blob/master/LICENSE)
 [![code style](https://img.shields.io/badge/code%20style-black-202020.svg)](https://github.com/ambv/black)
+[![doi](https://img.shields.io/badge/doi-10.5281%2Fzenodo.594879-blue)](http://doi.org/10.5281/zenodo.594879)
 
 Libmbd implements the [many-body dispersion](http://dx.doi.org/10.1063/1.4865104) (MBD) method in several programming languages and frameworks:
 
 - The Fortran implementation is the reference, most advanced implementation, with support for analytical gradients and distributed parallelism, and additional functionality beyond the MBD method itself. It provides a low-level and a high-level Fortran API, as well as a C API. Furthermore, Python bindings to the C API are provided.
 - The Python/Numpy implementation is intended for prototyping, and as a high-level language reference.
 - The Python/Tensorflow implementation is an experiment that should enable rapid prototyping of machine learning applications with MBD.
 
 The Python-based implementations as well as Python bindings to the Libmbd C API are accessible from the Python package called Pymbd.
 
-## Installing Pymbd
+## Installing
 
-The easiest way to get Pymbd is to install the Pymbd [Conda](https://conda.io/docs/) package, which ships with pre-built Libmbd.
+**TL;DR** Install prebuilt Libmbd binaries via [Conda-forge](https://conda-forge.org) and Pymbd with [Pip](https://pip.pypa.io/en/stable/quickstart/).
 
 ```
-conda install -c libmbd pymbd
+conda install -c conda-forge libmbd
+pip install pymbd
 ```
 
-Alternatively, if you have Libmbd already installed on your system (see below), you can install Pymbd with Pip, in which case it links against the installed Libmbd. To support Libmbd built with ScaLAPACK/MPI, the `mpi` extras is required, which installs `mpi4py` as an extra dependency.
+One can also install the ScaLAPACK/MPI version.
 
 ```
-pip install pymbd  # or pymbd[mpi]
+conda install -c conda-forge 'libmbd=*=mpi_*' mpi4py
+pip install pymbd[mpi]
 ```
 
-If Libmbd is installed in a non-standard location, you can point Pymbd to it with
+Verify installation with
 
 ```
-env LIBMBD_PREFIX=<path to Libmbd> pip install pymbd
-```
-
-If you don’t need the Fortran bindings in Pymbd, you can install it without the C extension, in which case `pymbd.fortran` becomes unimportable:
-
-```
-env LIBMBD_PREFIX= pip install pymbd
+$ python -m pymbd
+Expected energy:   -0.0002462647623815428
+Calculated energy: -0.0002462647623817456
 ```
 
-## Installing Libmbd
+###  Libmbd
 
 Libmbd uses CMake for compiling and installing, and requires a Fortran compiler, LAPACK, and optionally ScaLAPACK/MPI.
 
 On Ubuntu:
 
 ```bash
 apt-get install gfortran libblas-dev liblapack-dev [mpi-default-dev mpi-default-bin libscalapack-mpi-dev]
@@ -102,14 +101,41 @@
 cmake .. [-DENABLE_SCALAPACK_MPI=ON]
 make
 make install
 ```
 
 This installs the Libmbd shared library, C API header file, and high-level Fortran API module file.
 
+### Pymbd
+
+Pymbd can be installed and updated using [Pip](https://pip.pypa.io/en/stable/quickstart/), but requires installed Libmbd as a dependency (see above).
+
+```
+pip install pymbd
+```
+
+To support Libmbd built with ScaLAPACK/MPI, the `mpi` extras is required, which installs `mpi4py` as an extra dependency. In this case one has to make sure that `mpi4py` is linked against the same MPI library as Libmbd (for instance by compiling both manually, or installing both via Conda-forge).
+
+```
+pip install pymbd[mpi]
+```
+
+If Libmbd is installed in a non-standard location, you can point Pymbd to it with
+
+```
+env LIBMBD_PREFIX=<path to Libmbd install prefix> pip install pymbd
+```
+
+If you don’t need the Fortran bindings in Pymbd, you can install it without the C extension, in which case `pymbd.fortran` becomes unimportable:
+
+```
+env LIBMBD_PREFIX= pip install pymbd
+```
+
+
 ## Examples
 
 ```python
 from pymbd import mbd_energy_species, ang
 from pymbd.fortran import MBDCalc
 
 ene_py = mbd_energy_species(  # pure Python implementation
```

