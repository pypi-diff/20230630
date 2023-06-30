# Comparing `tmp/resonances-0.2.6.tar.gz` & `tmp/resonances-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resonances-0.2.6.tar", max compression
+gzip compressed data, was "resonances-0.2.7.tar", max compression
```

## Comparing `resonances-0.2.6.tar` & `resonances-0.2.7.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     1071 2023-01-21 08:32:40.950152 resonances-0.2.6/LICENSE
--rw-r--r--   0        0        0     6451 2023-05-12 15:05:24.085106 resonances-0.2.6/README.md
--rw-r--r--   0        0        0     2059 2023-05-12 15:05:24.086018 resonances-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      417 2023-03-10 09:50:28.272800 resonances-0.2.6/resonances/__init__.py
--rw-r--r--   0        0        0      115 2023-01-21 08:32:40.952434 resonances-0.2.6/resonances/__main__.py
--rw-r--r--   0        0        0     1725 2023-01-21 08:32:40.952516 resonances-0.2.6/resonances/body.py
--rw-r--r--   0        0        0     1447 2023-01-21 08:32:40.952591 resonances-0.2.6/resonances/config.json
--rw-r--r--   0        0        0     1320 2023-02-18 10:50:00.878029 resonances-0.2.6/resonances/config.py
--rw-r--r--   0        0        0        0 2023-01-21 08:32:40.952748 resonances-0.2.6/resonances/data/__init__.py
--rw-r--r--   0        0        0     3435 2023-05-12 15:05:24.086311 resonances-0.2.6/resonances/data/astdys.py
--rw-r--r--   0        0        0     1120 2023-01-21 08:32:40.952931 resonances-0.2.6/resonances/data/const.py
--rw-r--r--   0        0        0      192 2023-01-21 08:32:40.953006 resonances-0.2.6/resonances/data/util.py
--rw-r--r--   0        0        0     4402 2023-01-21 08:32:40.953136 resonances-0.2.6/resonances/experiment/console.py
--rw-r--r--   0        0        0     1313 2023-03-10 15:42:06.867976 resonances-0.2.6/resonances/experiment/finder.py
--rw-r--r--   0        0        0     1209 2023-01-21 08:32:40.953297 resonances-0.2.6/resonances/experiment/loader.py
--rw-r--r--   0        0        0     1904 2023-01-21 08:32:40.953382 resonances-0.2.6/resonances/experiment/shape.py
--rw-r--r--   0        0        0     1377 2023-02-18 11:14:33.313263 resonances-0.2.6/resonances/logger.py
--rw-r--r--   0        0        0      745 2023-05-12 15:05:24.086551 resonances-0.2.6/resonances/matrix/matrix.py
--rw-r--r--   0        0        0     2350 2023-03-10 15:42:06.868386 resonances-0.2.6/resonances/matrix/three_body_matrix.py
--rw-r--r--   0        0        0     1911 2023-05-12 15:05:24.086782 resonances-0.2.6/resonances/matrix/two_body_matrix.py
--rw-r--r--   0        0        0        0 2023-01-21 08:32:40.953829 resonances-0.2.6/resonances/resonance/__init__.py
--rw-r--r--   0        0        0     1213 2023-01-21 08:32:40.953932 resonances-0.2.6/resonances/resonance/factory.py
--rw-r--r--   0        0        0    11846 2023-01-21 08:32:40.954070 resonances-0.2.6/resonances/resonance/libration.py
--rw-r--r--   0        0        0     1925 2023-05-12 15:05:24.086983 resonances-0.2.6/resonances/resonance/mmr.py
--rw-r--r--   0        0        0     3533 2023-03-10 15:42:06.868737 resonances-0.2.6/resonances/resonance/plot.py
--rw-r--r--   0        0        0     6300 2023-05-12 15:05:24.087224 resonances-0.2.6/resonances/resonance/three_body.py
--rw-r--r--   0        0        0     2303 2023-05-12 15:05:24.087456 resonances-0.2.6/resonances/resonance/two_body.py
--rw-r--r--   0        0        0    11551 2023-05-12 15:05:24.087675 resonances-0.2.6/resonances/simulation.py
--rw-r--r--   0        0        0      263 2023-05-12 15:05:24.087848 resonances-0.2.6/resonances/util.py
--rw-r--r--   0        0        0     8449 1970-01-01 00:00:00.000000 resonances-0.2.6/setup.py
--rw-r--r--   0        0        0     7731 1970-01-01 00:00:00.000000 resonances-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-21 08:32:40.950152 resonances-0.2.7/LICENSE
+-rw-r--r--   0        0        0     6451 2023-05-12 15:05:24.085106 resonances-0.2.7/README.md
+-rw-r--r--   0        0        0     2059 2023-06-30 12:16:00.407014 resonances-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      417 2023-03-10 09:50:28.272800 resonances-0.2.7/resonances/__init__.py
+-rw-r--r--   0        0        0      115 2023-01-21 08:32:40.952434 resonances-0.2.7/resonances/__main__.py
+-rw-r--r--   0        0        0     1725 2023-01-21 08:32:40.952516 resonances-0.2.7/resonances/body.py
+-rw-r--r--   0        0        0     1447 2023-01-21 08:32:40.952591 resonances-0.2.7/resonances/config.json
+-rw-r--r--   0        0        0     1320 2023-02-18 10:50:00.878029 resonances-0.2.7/resonances/config.py
+-rw-r--r--   0        0        0        0 2023-01-21 08:32:40.952748 resonances-0.2.7/resonances/data/__init__.py
+-rw-r--r--   0        0        0     3435 2023-05-12 15:05:24.086311 resonances-0.2.7/resonances/data/astdys.py
+-rw-r--r--   0        0        0     1120 2023-01-21 08:32:40.952931 resonances-0.2.7/resonances/data/const.py
+-rw-r--r--   0        0        0      192 2023-01-21 08:32:40.953006 resonances-0.2.7/resonances/data/util.py
+-rw-r--r--   0        0        0     4402 2023-01-21 08:32:40.953136 resonances-0.2.7/resonances/experiment/console.py
+-rw-r--r--   0        0        0     1313 2023-03-10 15:42:06.867976 resonances-0.2.7/resonances/experiment/finder.py
+-rw-r--r--   0        0        0     1209 2023-01-21 08:32:40.953297 resonances-0.2.7/resonances/experiment/loader.py
+-rw-r--r--   0        0        0     1904 2023-01-21 08:32:40.953382 resonances-0.2.7/resonances/experiment/shape.py
+-rw-r--r--   0        0        0     1377 2023-02-18 11:14:33.313263 resonances-0.2.7/resonances/logger.py
+-rw-r--r--   0        0        0      745 2023-05-12 15:05:24.086551 resonances-0.2.7/resonances/matrix/matrix.py
+-rw-r--r--   0        0        0     2350 2023-03-10 15:42:06.868386 resonances-0.2.7/resonances/matrix/three_body_matrix.py
+-rw-r--r--   0        0        0     1911 2023-05-12 15:05:24.086782 resonances-0.2.7/resonances/matrix/two_body_matrix.py
+-rw-r--r--   0        0        0        0 2023-01-21 08:32:40.953829 resonances-0.2.7/resonances/resonance/__init__.py
+-rw-r--r--   0        0        0     1213 2023-01-21 08:32:40.953932 resonances-0.2.7/resonances/resonance/factory.py
+-rw-r--r--   0        0        0    11846 2023-01-21 08:32:40.954070 resonances-0.2.7/resonances/resonance/libration.py
+-rw-r--r--   0        0        0     1925 2023-05-12 15:05:24.086983 resonances-0.2.7/resonances/resonance/mmr.py
+-rw-r--r--   0        0        0     3533 2023-03-10 15:42:06.868737 resonances-0.2.7/resonances/resonance/plot.py
+-rw-r--r--   0        0        0     6300 2023-05-12 15:05:24.087224 resonances-0.2.7/resonances/resonance/three_body.py
+-rw-r--r--   0        0        0     2303 2023-05-12 15:05:24.087456 resonances-0.2.7/resonances/resonance/two_body.py
+-rw-r--r--   0        0        0    11551 2023-05-12 15:05:24.087675 resonances-0.2.7/resonances/simulation.py
+-rw-r--r--   0        0        0      263 2023-05-12 15:05:24.087848 resonances-0.2.7/resonances/util.py
+-rw-r--r--   0        0        0     7683 1970-01-01 00:00:00.000000 resonances-0.2.7/PKG-INFO
```

### Comparing `resonances-0.2.6/LICENSE` & `resonances-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/README.md` & `resonances-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/pyproject.toml` & `resonances-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resonances"
-version = "0.2.6"
+version = "0.2.7"
 description = "Identification of mean-motion resonances"
 authors = ["Evgeny Smirnov <smirik@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://smirik.github.io/resonances/"
 repository = "https://github.com/smirik/resonances"
 documentation = "http://smirik.github.io/resonances/"
```

### Comparing `resonances-0.2.6/resonances/body.py` & `resonances-0.2.7/resonances/body.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/config.json` & `resonances-0.2.7/resonances/config.json`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/config.py` & `resonances-0.2.7/resonances/config.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/data/astdys.py` & `resonances-0.2.7/resonances/data/astdys.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/data/const.py` & `resonances-0.2.7/resonances/data/const.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/experiment/console.py` & `resonances-0.2.7/resonances/experiment/console.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/experiment/finder.py` & `resonances-0.2.7/resonances/experiment/finder.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/experiment/loader.py` & `resonances-0.2.7/resonances/experiment/loader.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/experiment/shape.py` & `resonances-0.2.7/resonances/experiment/shape.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/logger.py` & `resonances-0.2.7/resonances/logger.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/matrix/matrix.py` & `resonances-0.2.7/resonances/matrix/matrix.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/matrix/three_body_matrix.py` & `resonances-0.2.7/resonances/matrix/three_body_matrix.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/matrix/two_body_matrix.py` & `resonances-0.2.7/resonances/matrix/two_body_matrix.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/resonance/factory.py` & `resonances-0.2.7/resonances/resonance/factory.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/resonance/libration.py` & `resonances-0.2.7/resonances/resonance/libration.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/resonance/mmr.py` & `resonances-0.2.7/resonances/resonance/mmr.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/resonance/plot.py` & `resonances-0.2.7/resonances/resonance/plot.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/resonance/three_body.py` & `resonances-0.2.7/resonances/resonance/three_body.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/resonance/two_body.py` & `resonances-0.2.7/resonances/resonance/two_body.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/resonances/simulation.py` & `resonances-0.2.7/resonances/simulation.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.6/setup.py` & `resonances-0.2.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['resonances',
- 'resonances.data',
- 'resonances.experiment',
- 'resonances.matrix',
- 'resonances.resonance']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['astropy>=5.2.1,<6.0.0',
- 'matplotlib>=3.6.3,<4.0.0',
- 'numpy>=1.24.1,<2.0.0',
- 'pandas>=1.5.3,<2.0.0',
- 'rebound>=3.23.2,<4.0.0',
- 'scipy>=1.10.0,<2.0.0',
- 'seaborn>=0.12.2,<0.13.0']
-
-entry_points = \
-{'console_scripts': ['ain = '
-                     'resonances.experiment.console:asteroids_in_resonance',
-                     'asteroids-in-resonance = '
-                     'resonances.experiment.console:asteroids_in_resonance',
-                     'ia = resonances.experiment.console:asteroids',
-                     'identify-asteroids = '
-                     'resonances.experiment.console:asteroids',
-                     'identify-quick = resonances.experiment.console:quick',
-                     'identify-resonances = '
-                     'resonances.experiment.console:identifier',
-                     'iq = resonances.experiment.console:quick',
-                     'ir = resonances.experiment.console:identifier',
-                     'simulation-shape = '
-                     'resonances.experiment.console:calc_shape',
-                     'ss = resonances.experiment.console:calc_shape']}
-
-setup_kwargs = {
-    'name': 'resonances',
-    'version': '0.2.6',
-    'description': 'Identification of mean-motion resonances',
-    'long_description': '# Mean-Motion Resonances\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Resonances](https://github.com/smirik/resonances/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/smirik/resonances/actions/workflows/ci.yml)\n\n`resonances` is an open-source package dedicated to the identification of mean-motion resonances of small bodies. Many examples are for the Solar system; however, you might use the package for any possible planetary system, including exoplanets.\n\nFor more information, [read the documentation](https://smirik.github.io/resonances/).\n\n**Note:** while this app has many functional and integration tests built in, it is still in the dev stage. Hence, it might include some inconsistencies. So, any community help is appreciated!\n\n## Features\n\nThe package:\n\n- can automatically identify two-body and three-body mean-motion resonance in the Solar system,\n- accurately differentiates different types of resonances (pure, transient, uncertain),\n- provides an interface for mass tasks (i.e. find resonant areas in a planetary system),\n- can plot time series and periodograms,\n- and, yeah, it is well tested ;)\n\nIt actively uses [REBOUND integrator](https://rebound.readthedocs.io) maintained by Hanno Rein and others.\n\n## Installation\n\nTo install resonances on your system, follow the instructions on the appropriate [installation guide](https://smirik.github.io/resonances/install/)\n\n## Mean-motion resonances\n\nFor those who are not familiar with the mean-motion resonances, here is the list of papers used to develop this package:\n\n### Papers about the automatic identification of resonant asteroids\n\n1. Smirnov, E. A. & Dovgalev, I. S. Identification of Asteroids in Two-Body Resonances. Solar System Research 52, 347–354 (2018).\n2. Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707\n3. Smirnov, E. A. & Shevchenko, I. I. Massive identification of asteroids in three-body resonances. Icarus 222, 220–228 (2013).\n4. Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.\n5. Nesvorný, D. & Morbidelli, A. Three-Body Mean Motion Resonances and the Chaotic Structure of the Asteroid Belt. The Astronomical Journal 116, 3029–3037 (1998).\n\n### Papers about mean-motion resonances\n\n1. Chirikov, B. V. A universal instability of many-dimensional oscillator systems. Physics reports 52, 263–379 (1979).\n1. Gallardo, T. Strength, stability and three dimensional structure of mean motion resonances in the solar system. Icarus 317, 121–134 (2019).\n1. Gallardo, T. Atlas of the mean motion resonances in the Solar System. Icarus 184, 29–38 (2006).\n1. Gallardo, T., Coito, L. & Badano, L. Planetary and satellite three body mean motion resonances. Icarus 274, 83–98 (2016).\n1. Milani, A., Cellino, A., Knezevic, Z., Novaković, B. & Spoto, F. Asteroid families classification: Exploiting very large datasets. Icarus 239, 46–73 (2014).\n1. Murray, N. & Holman, M. Diffusive chaos in the outer asteroid belt. The Astronomical Journal 114, 1246 (1997).\n1. Murray, N., Holman, M. & Potter, M. On the Origin of Chaos in the Asteroid Belt. The Astronomical Journal 116, 2583–2589 (1998).\n1. Shevchenko, I. I. On the Lyapunov exponents of the asteroidal motion subject to resonances and encounters. Proc. IAU 2, 15–30 (2006).\n\n### Books\n\n1. Murray, C. D. & Dermott, S. F. Solar system dynamics. (Cambridge Univ. Press, 2012).\n1. Morbidelli, A. Modern celestial mechanics: aspects of solar system dynamics. (2002).\n\n## References\n\nWhenever you use this package, we are kindly asking you to refer to one of the following papers (please choose the appropriate):\n\n1. **The package itself**: \n\n* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing. https://doi.org/10.1016/j.ascom.2023.100707\n\n```tex\n@article{Smirnov2023,\n  title    = {A new python package for identifying celestial bodies trapped in mean-motion resonances},\n  journal  = {Astronomy and Computing},\n  year     = {2023},\n  issn     = {2213-1337},\n  doi      = {https://doi.org/10.1016/j.ascom.2023.100707},\n  url      = {https://www.sciencedirect.com/science/article/pii/S2213133723000227},\n  author   = {E.A. Smirnov},\n  keywords = {Mean-motion resonances, Python, Identification, Asteroids},\n  abstract = {In this paper, a new open-source package ‘resonances’ written in python is introduced. It allows to find, analyse, and plot two-body and three-body mean-motion eccentricity-type resonances in the Solar and other planetary systems. The package has a better accuracy of the automatic identification procedure for resonant objects compared to previous studies. Furthermore, it has built-in integrations with AstDyS and NASA JPL catalogues. The code is extensively documented and tested with automatic tests. The package is available on GitHub under MIT Licence.}\n}\n```\n\n2. **The Libration module and automatic identification of librations**: \n\n* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707\n\n3. **Mass identification of mean-motion resonances:** \n\n* Smirnov, E. A., & Dovgalev, I. S. (2018). Identification of Asteroids in Two-Body Resonances. Solar System Research, 52(4), 347–354. https://doi.org/10.1134/S0038094618040056 \n* Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.\n\n## Authors\n\nThe authors of the package:\n\n- [Evgeny Smirnov](https://github.com/smirik) ([FB](https://facebook.com/smirik), [Telegram](https://t.me/smirik))\n\n## Acknowledgement\n\n- Many thanks to the co-authors of the papers (prof. I.\xa0I. Shevchenko, I.\xa0Dovgalev, and Dr.\xa0E.\xa0Popova).\n- The creators of [REBOUND integrator](https://rebound.readthedocs.io).\n- The creators of [Astropy](http://astropy.org).\n- The creators of `numpy`, `scipy`, `pandas`, and `matplotlib`.\n\n## Contributing\n\nFeel free to contribute to the code by sending pull requests [to the repository](https://github.com/smirik/resonances).\n\n## License\n\nMIT\n',
-    'author': 'Evgeny Smirnov',
-    'author_email': 'smirik@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'http://smirik.github.io/resonances/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<3.12',
+Metadata-Version: 2.1
+Name: resonances
+Version: 0.2.7
+Summary: Identification of mean-motion resonances
+Home-page: http://smirik.github.io/resonances/
+License: MIT
+Keywords: astronomy,nbody,resonance,mmr
+Author: Evgeny Smirnov
+Author-email: smirik@gmail.com
+Requires-Python: >=3.8.1,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Dist: astropy (>=5.2.1,<6.0.0)
+Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
+Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: rebound (>=3.23.2,<4.0.0)
+Requires-Dist: scipy (>=1.10.0,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Project-URL: Documentation, http://smirik.github.io/resonances/
+Project-URL: Repository, https://github.com/smirik/resonances
+Description-Content-Type: text/markdown
+
+# Mean-Motion Resonances
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Resonances](https://github.com/smirik/resonances/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/smirik/resonances/actions/workflows/ci.yml)
+
+`resonances` is an open-source package dedicated to the identification of mean-motion resonances of small bodies. Many examples are for the Solar system; however, you might use the package for any possible planetary system, including exoplanets.
+
+For more information, [read the documentation](https://smirik.github.io/resonances/).
+
+**Note:** while this app has many functional and integration tests built in, it is still in the dev stage. Hence, it might include some inconsistencies. So, any community help is appreciated!
+
+## Features
+
+The package:
+
+- can automatically identify two-body and three-body mean-motion resonance in the Solar system,
+- accurately differentiates different types of resonances (pure, transient, uncertain),
+- provides an interface for mass tasks (i.e. find resonant areas in a planetary system),
+- can plot time series and periodograms,
+- and, yeah, it is well tested ;)
+
+It actively uses [REBOUND integrator](https://rebound.readthedocs.io) maintained by Hanno Rein and others.
+
+## Installation
+
+To install resonances on your system, follow the instructions on the appropriate [installation guide](https://smirik.github.io/resonances/install/)
+
+## Mean-motion resonances
+
+For those who are not familiar with the mean-motion resonances, here is the list of papers used to develop this package:
+
+### Papers about the automatic identification of resonant asteroids
+
+1. Smirnov, E. A. & Dovgalev, I. S. Identification of Asteroids in Two-Body Resonances. Solar System Research 52, 347–354 (2018).
+2. Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707
+3. Smirnov, E. A. & Shevchenko, I. I. Massive identification of asteroids in three-body resonances. Icarus 222, 220–228 (2013).
+4. Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
+5. Nesvorný, D. & Morbidelli, A. Three-Body Mean Motion Resonances and the Chaotic Structure of the Asteroid Belt. The Astronomical Journal 116, 3029–3037 (1998).
+
+### Papers about mean-motion resonances
+
+1. Chirikov, B. V. A universal instability of many-dimensional oscillator systems. Physics reports 52, 263–379 (1979).
+1. Gallardo, T. Strength, stability and three dimensional structure of mean motion resonances in the solar system. Icarus 317, 121–134 (2019).
+1. Gallardo, T. Atlas of the mean motion resonances in the Solar System. Icarus 184, 29–38 (2006).
+1. Gallardo, T., Coito, L. & Badano, L. Planetary and satellite three body mean motion resonances. Icarus 274, 83–98 (2016).
+1. Milani, A., Cellino, A., Knezevic, Z., Novaković, B. & Spoto, F. Asteroid families classification: Exploiting very large datasets. Icarus 239, 46–73 (2014).
+1. Murray, N. & Holman, M. Diffusive chaos in the outer asteroid belt. The Astronomical Journal 114, 1246 (1997).
+1. Murray, N., Holman, M. & Potter, M. On the Origin of Chaos in the Asteroid Belt. The Astronomical Journal 116, 2583–2589 (1998).
+1. Shevchenko, I. I. On the Lyapunov exponents of the asteroidal motion subject to resonances and encounters. Proc. IAU 2, 15–30 (2006).
+
+### Books
+
+1. Murray, C. D. & Dermott, S. F. Solar system dynamics. (Cambridge Univ. Press, 2012).
+1. Morbidelli, A. Modern celestial mechanics: aspects of solar system dynamics. (2002).
+
+## References
+
+Whenever you use this package, we are kindly asking you to refer to one of the following papers (please choose the appropriate):
+
+1. **The package itself**: 
+
+* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing. https://doi.org/10.1016/j.ascom.2023.100707
+
+```tex
+@article{Smirnov2023,
+  title    = {A new python package for identifying celestial bodies trapped in mean-motion resonances},
+  journal  = {Astronomy and Computing},
+  year     = {2023},
+  issn     = {2213-1337},
+  doi      = {https://doi.org/10.1016/j.ascom.2023.100707},
+  url      = {https://www.sciencedirect.com/science/article/pii/S2213133723000227},
+  author   = {E.A. Smirnov},
+  keywords = {Mean-motion resonances, Python, Identification, Asteroids},
+  abstract = {In this paper, a new open-source package ‘resonances’ written in python is introduced. It allows to find, analyse, and plot two-body and three-body mean-motion eccentricity-type resonances in the Solar and other planetary systems. The package has a better accuracy of the automatic identification procedure for resonant objects compared to previous studies. Furthermore, it has built-in integrations with AstDyS and NASA JPL catalogues. The code is extensively documented and tested with automatic tests. The package is available on GitHub under MIT Licence.}
 }
+```
+
+2. **The Libration module and automatic identification of librations**: 
+
+* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707
+
+3. **Mass identification of mean-motion resonances:** 
+
+* Smirnov, E. A., & Dovgalev, I. S. (2018). Identification of Asteroids in Two-Body Resonances. Solar System Research, 52(4), 347–354. https://doi.org/10.1134/S0038094618040056 
+* Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
+
+## Authors
+
+The authors of the package:
+
+- [Evgeny Smirnov](https://github.com/smirik) ([FB](https://facebook.com/smirik), [Telegram](https://t.me/smirik))
+
+## Acknowledgement
+
+- Many thanks to the co-authors of the papers (prof. I. I. Shevchenko, I. Dovgalev, and Dr. E. Popova).
+- The creators of [REBOUND integrator](https://rebound.readthedocs.io).
+- The creators of [Astropy](http://astropy.org).
+- The creators of `numpy`, `scipy`, `pandas`, and `matplotlib`.
+
+## Contributing
+
+Feel free to contribute to the code by sending pull requests [to the repository](https://github.com/smirik/resonances).
+
+## License
 
+MIT
 
-setup(**setup_kwargs)
```

