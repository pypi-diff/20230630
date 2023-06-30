# Comparing `tmp/superposed-pulses-1.1.tar.gz` & `tmp/superposed-pulses-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superposed-pulses-1.1.tar", last modified: Fri Feb 11 10:14:48 2022, max compression
+gzip compressed data, was "superposed-pulses-1.3.tar", last modified: Fri Jun 30 08:39:46 2023, max compression
```

## Comparing `superposed-pulses-1.1.tar` & `superposed-pulses-1.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 sosno     (1000) sosno     (1000)        0 2022-02-11 10:14:48.087880 superposed-pulses-1.1/
--rw-rw-r--   0 sosno     (1000) sosno     (1000)     1066 2021-01-15 08:33:08.000000 superposed-pulses-1.1/LICENSE
--rw-rw-r--   0 sosno     (1000) sosno     (1000)      902 2022-02-11 10:14:48.087880 superposed-pulses-1.1/PKG-INFO
--rw-rw-r--   0 sosno     (1000) sosno     (1000)      165 2022-02-09 13:05:46.000000 superposed-pulses-1.1/README.md
-drwxrwxr-x   0 sosno     (1000) sosno     (1000)        0 2022-02-11 10:14:48.087880 superposed-pulses-1.1/model/
--rw-rw-r--   0 sosno     (1000) sosno     (1000)       75 2022-02-11 10:10:31.000000 superposed-pulses-1.1/model/__init__.py
--rw-rw-r--   0 sosno     (1000) sosno     (1000)     3069 2022-02-11 10:11:47.000000 superposed-pulses-1.1/model/example.py
--rw-rw-r--   0 sosno     (1000) sosno     (1000)     3736 2021-11-10 09:03:43.000000 superposed-pulses-1.1/model/forcing.py
--rw-rw-r--   0 sosno     (1000) sosno     (1000)     5606 2022-02-11 10:11:47.000000 superposed-pulses-1.1/model/fpp_model.py
--rw-rw-r--   0 sosno     (1000) sosno     (1000)     7800 2021-11-10 09:03:43.000000 superposed-pulses-1.1/model/pulse_shape.py
--rw-rw-r--   0 sosno     (1000) sosno     (1000)       38 2022-02-11 10:14:48.087880 superposed-pulses-1.1/setup.cfg
--rw-rw-r--   0 sosno     (1000) sosno     (1000)     1145 2022-02-11 10:14:45.000000 superposed-pulses-1.1/setup.py
-drwxrwxr-x   0 sosno     (1000) sosno     (1000)        0 2022-02-11 10:14:48.087880 superposed-pulses-1.1/superposed_pulses.egg-info/
--rw-rw-r--   0 sosno     (1000) sosno     (1000)      902 2022-02-11 10:14:48.000000 superposed-pulses-1.1/superposed_pulses.egg-info/PKG-INFO
--rw-rw-r--   0 sosno     (1000) sosno     (1000)      362 2022-02-11 10:14:48.000000 superposed-pulses-1.1/superposed_pulses.egg-info/SOURCES.txt
--rw-rw-r--   0 sosno     (1000) sosno     (1000)        1 2022-02-11 10:14:48.000000 superposed-pulses-1.1/superposed_pulses.egg-info/dependency_links.txt
--rw-rw-r--   0 sosno     (1000) sosno     (1000)        1 2022-02-11 09:47:56.000000 superposed-pulses-1.1/superposed_pulses.egg-info/not-zip-safe
--rw-rw-r--   0 sosno     (1000) sosno     (1000)       58 2022-02-11 10:14:48.000000 superposed-pulses-1.1/superposed_pulses.egg-info/requires.txt
--rw-rw-r--   0 sosno     (1000) sosno     (1000)        6 2022-02-11 10:14:48.000000 superposed-pulses-1.1/superposed_pulses.egg-info/top_level.txt
+drwxrwxr-x   0 sosno     (1000) sosno     (1000)        0 2023-06-30 08:39:46.536316 superposed-pulses-1.3/
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)     1066 2021-01-15 08:33:08.000000 superposed-pulses-1.3/LICENSE
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)     1738 2023-06-30 08:39:46.536316 superposed-pulses-1.3/PKG-INFO
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)     1001 2023-06-30 08:35:55.000000 superposed-pulses-1.3/README.md
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)       38 2023-06-30 08:39:46.536316 superposed-pulses-1.3/setup.cfg
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)     1127 2023-06-30 08:39:39.000000 superposed-pulses-1.3/setup.py
+drwxrwxr-x   0 sosno     (1000) sosno     (1000)        0 2023-06-30 08:39:46.536316 superposed-pulses-1.3/superposed_pulses.egg-info/
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)     1738 2023-06-30 08:39:46.000000 superposed-pulses-1.3/superposed_pulses.egg-info/PKG-INFO
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)      457 2023-06-30 08:39:46.000000 superposed-pulses-1.3/superposed_pulses.egg-info/SOURCES.txt
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)        1 2023-06-30 08:39:46.000000 superposed-pulses-1.3/superposed_pulses.egg-info/dependency_links.txt
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)        1 2022-02-11 09:47:56.000000 superposed-pulses-1.3/superposed_pulses.egg-info/not-zip-safe
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)       40 2023-06-30 08:39:46.000000 superposed-pulses-1.3/superposed_pulses.egg-info/requires.txt
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)       17 2023-06-30 08:39:46.000000 superposed-pulses-1.3/superposed_pulses.egg-info/top_level.txt
+drwxrwxr-x   0 sosno     (1000) sosno     (1000)        0 2023-06-30 08:39:46.536316 superposed-pulses-1.3/superposedpulses/
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)      110 2023-06-30 08:35:55.000000 superposed-pulses-1.3/superposedpulses/__init__.py
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)     3653 2023-06-30 08:35:55.000000 superposed-pulses-1.3/superposedpulses/example.py
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)     3737 2023-06-30 08:35:55.000000 superposed-pulses-1.3/superposedpulses/forcing.py
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)     9713 2023-06-30 08:35:55.000000 superposed-pulses-1.3/superposedpulses/point_model.py
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)    10461 2023-06-30 08:35:55.000000 superposed-pulses-1.3/superposedpulses/pulse_shape.py
+-rw-rw-r--   0 sosno     (1000) sosno     (1000)     4251 2023-06-30 08:35:55.000000 superposed-pulses-1.3/superposedpulses/two_point_forcing.py
```

### Comparing `superposed-pulses-1.1/LICENSE` & `superposed-pulses-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `superposed-pulses-1.1/model/example.py` & `superposed-pulses-1.3/superposedpulses/example.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-import model.forcing as frc
-import model.fpp_model as fpp
-import model.pulse_shape as ps
+import superposedpulses.forcing as frc
+import superposedpulses.point_model as pm
+import superposedpulses.pulse_shape as ps
 
 # Simplest case, using defaults: exponential pulse shape, exponentially distributed amplitudes, constant duration times.
 
-model = fpp.Model(gamma=0.1, total_duration=100, dt=0.01)
+model = pm.PointModel(gamma=0.1, total_duration=100, dt=0.01)
 times, signal = model.make_realization()
 
 plt.plot(times, signal)
 plt.show()
 
 # Double exponential shape
 
-model = fpp.Model(gamma=0.1, total_duration=100, dt=0.01)
+model = pm.PointModel(gamma=0.1, total_duration=100, dt=0.01)
 model.set_pulse_shape(ps.StandardPulseGenerator("2-exp", lam=0.35))
 times, signal = model.make_realization()
 
 plt.plot(times, signal)
 plt.show()
 
+# Adding noise to the signal
+
+model = pm.PointModel(gamma=0.1, total_duration=100, dt=0.01)
+model.add_noise(noise_to_signal_ratio=0.01, noise_type="additive", seed=None)
+times, signal = model.make_realization()
+
+plt.plot(times, signal)
+plt.show()
 
 # Say you want to customise your model a bit: use constant amplitude distribution, and box pulse shapes
 
-model = fpp.Model(gamma=0.1, total_duration=100, dt=0.01)
+model = pm.PointModel(gamma=0.1, total_duration=100, dt=0.01)
 model.set_amplitude_distribution("deg")
 model.set_pulse_shape(ps.BoxShortPulseGenerator())
 
 times, signal = model.make_realization()
 
 plt.plot(times, signal)
 plt.show()
 
 # If you want to implement your own distributions, you can do so by setting a custom ForcingGenerator. Say you want half
 # of your pulses to have amplitude 1, and the other half to have amplitude 2.
 
-model = fpp.Model(gamma=0.1, total_duration=100, dt=0.01)
+model = pm.PointModel(gamma=0.1, total_duration=100, dt=0.01)
 my_forcing_gen = frc.StandardForcingGenerator()
 my_forcing_gen.set_amplitude_distribution(
     lambda k: np.random.randint(low=1, high=3, size=k)
 )
 
 model.set_custom_forcing_generator(my_forcing_gen)
 times, s = model.make_realization()
@@ -76,21 +84,30 @@
     ):
         pass
 
     def set_duration_distribution(self, duration_distribution_function):
         pass
 
 
-model = fpp.Model(gamma=10, total_duration=1000, dt=0.01)
+model = pm.PointModel(gamma=10, total_duration=1000, dt=0.01)
 model.set_custom_forcing_generator(MyFancyForcingGenerator())
 
 times, s = model.make_realization()
 
 plt.plot(times, s)
 plt.show()
 
 # You might also want to get the actual pulse parameters that were used in the realization, this can be done by getting
 # the forcing, which is the set of amplitudes, arrival times and durations for each pulse.
 
 forcing = model.get_last_used_forcing()
 plt.hist(forcing.durations)
 plt.show()
+
+# Two point model example
+model = pm.TwoPointModel(gamma=0.1, total_duration=100, dt=0.01)
+model.set_pulse_shape(ps.ExponentialShortPulseGenerator(tolerance=1e-50))
+times, signal_a, signal_b = model.make_realization()
+
+plt.plot(times, signal_a)
+plt.plot(times, signal_b)
+plt.show()
```

### Comparing `superposed-pulses-1.1/model/forcing.py` & `superposed-pulses-1.3/superposedpulses/forcing.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             self.arrival_times[pulse_index],
             self.amplitudes[pulse_index],
             self.durations[pulse_index],
         )
 
 
 class ForcingGenerator(ABC):
-    """Abstract class used by FPPModels to generate forcing.
+    """Abstract class used by PointModel to generate forcing.
 
     Implementations of this class should have a get_forcing method,
     returning a forcing with arrival times, amplitudes and durations for
     all pulses.
     """
 
     @abstractmethod
```

### Comparing `superposed-pulses-1.1/model/pulse_shape.py` & `superposed-pulses-1.3/superposedpulses/pulse_shape.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABC, abstractmethod
-
 import numpy as np
 from typing import Callable
 import warnings
 
 
 class PulseGenerator(ABC):
     """Abstract pulse shape, implementations should return a pulse shape vector
@@ -30,25 +29,25 @@
         """
         raise NotImplementedError
 
 
 class StandardPulseGenerator(PulseGenerator):
     """Generates all pulse shapes previously supported."""
 
-    __SHAPE_NAMES__ = {"1-exp", "lorentz", "2-exp"}
+    __SHAPE_NAMES__ = {"1-exp", "lorentz", "2-exp", "gaussian"}
     # TODO: Implement the others
 
     def __init__(self, shape_name: str = "1-exp", **kwargs):
         """
         Parameters
         ----------
         shape_name Should be one of StandardPulseShapeGenerator.__SHAPE_NAMES__
         kwargs Additional arguments to be passed to special shapes:
             - "2-exp":
-                - "lam" parameter for the asymmetry parameter
+            - "lam" parameter for the asymmetry parameter
         """
         assert (
             shape_name in StandardPulseGenerator.__SHAPE_NAMES__
         ), "Invalid shape_name"
         self._shape_name: str = shape_name
         self._kwargs = kwargs
 
@@ -68,14 +67,16 @@
     ) -> Callable[[np.ndarray, float, dict], np.ndarray]:
         if shape_name == "1-exp":
             return StandardPulseGenerator._get_exponential_shape
         if shape_name == "2-exp":
             return StandardPulseGenerator._get_double_exponential_shape
         if shape_name == "lorentz":
             return StandardPulseGenerator._get_lorentz_shape
+        if shape_name == "gaussian":
+            return StandardPulseGenerator._get_gaussian_shape
 
     @staticmethod
     def _get_exponential_shape(
         times: np.ndarray, duration: float, kwargs
     ) -> np.ndarray:
         kern = np.zeros(len(times))
         kern[times >= 0] = np.exp(-times[times >= 0] / duration)
@@ -92,14 +93,18 @@
         lam = kwargs["lam"]
         assert (lam > 0.0) & (lam < 1.0)
         kern = np.zeros(len(times))
         kern[times < 0] = np.exp(times[times < 0] / lam / duration)
         kern[times >= 0] = np.exp(-times[times >= 0] / (1 - lam) / duration)
         return kern
 
+    @staticmethod
+    def _get_gaussian_shape(times: np.ndarray, duration: float, kwargs) -> np.ndarray:
+        return np.exp(-((times / duration) ** 2) / 2) / np.sqrt(2 * np.pi)
+
 
 class ShortPulseGenerator(ABC):
     """Abstract pulse shape, implementations should return a pulse shape vector
     with (possibly) different durations.
 
     The length of the returned array is not restricted, this is useful
     for pulse shapes such as the exponential or the box pulse, for which
@@ -180,14 +185,72 @@
         return kern
 
     def get_cutoff(self, duration: float) -> float:
         cutoff = -duration * np.log(self.tolerance)
         return min(cutoff, self._max_cutoff)
 
 
+class LorentzShortPulseGenerator(ShortPulseGenerator):
+    def __init__(self, tolerance: float = 1e-50, max_cutoff: float = 1e50):
+        """Lorentz pulse generator, the length of the returned array is
+        dynamically set to be the shortest to reach a pulse value under the
+        given tolerance. That is, if the pulse shape is p(t), the returned
+        array will be p(t) with t in [-T, T] such that p(-T), p(T) < tolerance.
+
+        p(t) = 1/ (pi (t^2 + 1)).
+
+        A max_cutoff is provided to avoid returning pulse arrays of arbitrarily long lengths.
+        Parameters
+        ----------
+        tolerance Maximum error when cutting the pulse.
+        max_cutoff
+        """
+        super(LorentzShortPulseGenerator, self).__init__(tolerance)
+        self._max_cutoff = max_cutoff
+
+    def get_pulse(self, times: np.ndarray, duration: float) -> np.ndarray:
+        kern = np.zeros(len(times))
+        kern = (np.pi * (1 + (times / duration) ** 2)) ** (-1)
+        return kern
+
+    def get_cutoff(self, duration: float) -> float:
+        cutoff = duration * np.sqrt(1.0 / (self.tolerance * np.pi) - 1)
+        return min(cutoff, self._max_cutoff)
+
+
+class GaussianShortPulseGenerator(ShortPulseGenerator):
+    def __init__(self, tolerance: float = 1e-50, max_cutoff: float = 1e50):
+        """
+        Gaussian pulse generator. The length of the returned array is
+        dynamically set to be the shortest to reach a pulse value under the
+        given tolerance. That is, if the pulse shape is p(t), the returned
+        array will be p(t) with t in [-T, T] such that p(-T), p(T) < tolerance.
+
+        p(t) = exp(-(t)^2 / 2) / sqrt(2*pi).
+
+        A max_cutoff is provided to avoid returning pulse arrays of arbitrarily long lengths.
+        Parameters
+        ----------
+        tolerance Maximum error when cutting the pulse.
+        max_cutoff
+
+        """
+        super(GaussianShortPulseGenerator, self).__init__(tolerance)
+        self._max_cutoff = max_cutoff
+
+    def get_pulse(self, times: np.ndarray, duration: float) -> np.ndarray:
+        kern = np.zeros(len(times))
+        kern = np.exp(-((times / duration) ** 2) / 2) / np.sqrt(2 * np.pi)
+        return kern
+
+    def get_cutoff(self, duration: float) -> float:
+        cutoff = duration * np.sqrt(-2 * np.log(np.sqrt(2 * np.pi) * self.tolerance))
+        return min(cutoff, self._max_cutoff)
+
+
 class BoxShortPulseGenerator(ShortPulseGenerator):
     """Box shape p(t, tau):
 
     p(t, tau) = 1, for |t| < tau / 2
     p(t, tau) = 0, otherwise
     """
```

### Comparing `superposed-pulses-1.1/setup.py` & `superposed-pulses-1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,21 @@
     author="Juan Manuel Losada",
     author_email="juan.m.losada@uit.no",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uit-cosmo/filtered-point-process",
     download_url="https://github.com/uit-cosmo/3ppy/archive/refs/tags/1.1.tar.gz",
     license="MiT",
-    version="1.1",
-    packages=["model"],
+    version="1.3",
+    packages=["superposedpulses"],
     python_requires=">=3.0",
     install_requires=[
         "numpy>=1.15.0",
         "scipy>=1.4.0",
         "tqdm>=4.50.2",
-        "matplotlib>=3.2.0",
     ],
     classifiers=[
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Scientific/Engineering :: Visualization",
```

