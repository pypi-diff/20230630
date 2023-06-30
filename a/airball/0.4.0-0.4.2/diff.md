# Comparing `tmp/airball-0.4.0.tar.gz` & `tmp/airball-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airball-0.4.0.tar", last modified: Thu Jun 29 09:10:59 2023, max compression
+gzip compressed data, was "airball-0.4.2.tar", last modified: Fri Jun 30 08:24:13 2023, max compression
```

## Comparing `airball-0.4.0.tar` & `airball-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-29 09:10:59.726911 airball-0.4.0/
--rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.4.0/LICENSE
--rw-r--r--   0 zyrxvo     (501) staff       (20)     1023 2023-06-29 09:10:59.726792 airball-0.4.0/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)      472 2023-02-16 19:20:04.000000 airball-0.4.0/README.md
--rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2022-06-02 19:07:19.000000 airball-0.4.0/pyproject.toml
--rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2023-06-29 09:10:59.726954 airball-0.4.0/setup.cfg
--rw-r--r--   0 zyrxvo     (501) staff       (20)      922 2023-06-29 09:03:54.000000 airball-0.4.0/setup.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-29 09:10:59.724420 airball-0.4.0/src/
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-29 09:10:59.725823 airball-0.4.0/src/airball/
--rw-r--r--   0 zyrxvo     (501) staff       (20)      243 2023-06-23 02:16:23.000000 airball-0.4.0/src/airball/__init__.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     8979 2023-06-27 13:19:02.000000 airball-0.4.0/src/airball/analytic.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    43811 2023-06-29 09:01:58.000000 airball-0.4.0/src/airball/environments.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    11157 2023-06-29 08:34:54.000000 airball-0.4.0/src/airball/flybys.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    15000 2023-02-09 02:16:12.000000 airball-0.4.0/src/airball/particle.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     8475 2023-06-29 07:55:57.000000 airball-0.4.0/src/airball/tools.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)      181 2023-06-29 01:38:57.000000 airball-0.4.0/src/airball/units.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-29 09:10:59.726608 airball-0.4.0/src/airball.egg-info/
--rw-r--r--   0 zyrxvo     (501) staff       (20)     1023 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)      379 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/SOURCES.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/dependency_links.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)       35 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/requires.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2023-06-29 09:10:59.000000 airball-0.4.0/src/airball.egg-info/top_level.txt
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-30 08:24:13.230597 airball-0.4.2/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.4.2/LICENSE
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     1023 2023-06-30 08:24:13.230480 airball-0.4.2/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      472 2023-02-16 19:20:04.000000 airball-0.4.2/README.md
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2022-06-02 19:07:19.000000 airball-0.4.2/pyproject.toml
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2023-06-30 08:24:13.230638 airball-0.4.2/setup.cfg
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      922 2023-06-30 08:22:52.000000 airball-0.4.2/setup.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-30 08:24:13.227773 airball-0.4.2/src/
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-30 08:24:13.229484 airball-0.4.2/src/airball/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      334 2023-06-30 08:23:00.000000 airball-0.4.2/src/airball/__init__.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     9107 2023-06-30 08:21:41.000000 airball-0.4.2/src/airball/analytic.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    14527 2023-06-30 08:16:39.000000 airball-0.4.2/src/airball/environments.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    11157 2023-06-29 08:34:54.000000 airball-0.4.2/src/airball/flybys.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     7787 2023-06-30 07:51:03.000000 airball-0.4.2/src/airball/imf.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    15000 2023-02-09 02:16:12.000000 airball-0.4.2/src/airball/particle.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    21713 2023-06-30 06:28:22.000000 airball-0.4.2/src/airball/stars.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     8774 2023-06-30 08:05:48.000000 airball-0.4.2/src/airball/tools.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      181 2023-06-29 01:38:57.000000 airball-0.4.2/src/airball/units.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-30 08:24:13.230320 airball-0.4.2/src/airball.egg-info/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     1023 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      419 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/SOURCES.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/dependency_links.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       35 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/requires.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/top_level.txt
```

### Comparing `airball-0.4.0/LICENSE` & `airball-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airball-0.4.0/PKG-INFO` & `airball-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airball
-Version: 0.4.0
+Version: 0.4.2
 Summary: A package for implementing flybys in hannorein/rebound
 Home-page: https://github.com/zyrxvo/airball/
 Author: Garett Brown
 Author-email: garett.brown@mail.utoronto.ca
 Project-URL: Bug Tracker, https://github.com/zyrxvo/airball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `airball-0.4.0/setup.py` & `airball-0.4.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="airball",
-    version="0.4.0",
+    version="0.4.2",
     author="Garett Brown",
     author_email="garett.brown@mail.utoronto.ca",
     description="A package for implementing flybys in hannorein/rebound",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zyrxvo/airball/",
     project_urls={
```

### Comparing `airball-0.4.0/src/airball/analytic.py` & `airball-0.4.2/src/airball/analytic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 import numpy as _numpy
 import rebound as _rebound
 from scipy.special import j0 as _j0,jv as _jv
 
 from .tools import *
+from . import units
 
 ############################################################
 ################## Analytical Estimates ####################
 ############################################################
 
 def binary_energy(sim):#sun_mass, planet_mass, planet_a):
     '''
         The energy of a binary system, -(G*M*m)/(2*a).
         
         Parameters
         ----------
         sim : REBOUND Simulation
     '''
-    units = rebound_units(sim)
-    G = (sim.G * units['length']**3 / units['mass'] / units['time']**2)
+    unit_set = rebound_units(sim)
+    G = (sim.G * unit_set['length']**3 / unit_set['mass'] / unit_set['time']**2)
     p = sim.particles
-    return (-G * p[0].m * units['mass'] * p[1].m * units['mass'] / (2. * p[1].a * units['length'])).decompose(list(units.values()))
+    return (-G * p[0].m * unit_set['mass'] * p[1].m * unit_set['mass'] / (2. * p[1].a * unit_set['length'])).decompose(list(unit_set.values()))
     
 def energy_change_adiabatic_estimate(sim, star, averaged=True):
     '''
         An analytical estimate for the change in energy of a binary system due to a flyby star.
         
         From the conclusions of Roy & Haddow (2003) https://ui.adsabs.harvard.edu/abs/2003CeMDA..87..411R/abstract and Heggie (2006) https://ui.adsabs.harvard.edu/abs/2006fbp..book...20H/abstract. The orbital element angles of the flyby star are determined with respect to the plane defined by the binary orbit. In REBOUND this is the same as when the inclination of the planet is zero.
         
         Parameters
         ----------
         sim : REBOUND Simulation
         star : AIRBALL Star flyby object
     '''
-    units = rebound_units(sim)
-    t0 = 0*units['time']
-    G = (sim.G * units['length']**3 / units['mass'] / units['time']**2)
+    unit_set = rebound_units(sim)
+    t0 = 0*unit_set['time']
+    G = (sim.G * unit_set['length']**3 / unit_set['mass'] / unit_set['time']**2)
 
     sim = sim.copy()
     sim.rotate(_rebound.Rotation.to_new_axes(newz=sim.angular_momentum()))
     
     p = sim.particles
-    m1, m2, m3 = p[0].m * units['mass'], p[1].m * units['mass'], star.mass # redefine the masses for convenience
+    m1, m2, m3 = p[0].m * unit_set['mass'], p[1].m * unit_set['mass'], star.mass # redefine the masses for convenience
     M12 = m1 + m2 # total mass of the binary system
     M123 = m1 + m2 + m3 # total mass of all the objects involved
     
     mu = G*M123
     es = vinf_and_b_to_e(mu=mu, star_b=star.b, star_vinf=star.v)
     
-    a, e = p[1].a * units['length'], p[1].e # redefine the orbital elements of the planet for convenience
+    a, e = p[1].a * unit_set['length'], p[1].e # redefine the orbital elements of the planet for convenience
     n = _numpy.sqrt(G*M12/a**3) # compute the mean motion of the planet
     
     w, W, i = star.omega, star.Omega, star.inc # redefine the orientation elements of the flyby star for convenience
     V = star.v
     GM123 = G*M123 
     q = (- GM123 + _numpy.sqrt( GM123**2. + star.b**2. * V**4.))/V**2. # compute the periapsis of the flyby star
 
@@ -61,26 +62,26 @@
     e4 = _jv(-1,e) - e*_j0(e) - e*_jv(2,e) + _jv(3,e)
 
     # Calculate a convenient function of the planet's semi-major axis and the flyby star's periapsis.
     k = _numpy.sqrt((2*M12*q**3)/(M123*a**3))
     
     # Calculate convenient functions of the flyby star's eccentricity.
     f1 = ((es + 1.0)**(0.75)) / ((2.0**(0.75)) * (es*es))
-    with u.set_enabled_equivalencies(u.dimensionless_angles()):
+    with units.set_enabled_equivalencies(units.dimensionless_angles()):
         f2 = (3.0/(2.0*_numpy.sqrt(2.0))) * (_numpy.sqrt((es*es) - 1.0) - _numpy.arccos(1.0/es)) / ((es - 1.0)**(1.5))
     
     # Compute the prefactor and terms of the calculation done by Roy & Haddow (2003)
     prefactor = (-_numpy.sqrt(_numpy.pi)/8.0) * ((G*m1*m2*m3)/M12) * ((a*a)/(q*q*q)) * f1 * k**(2.5) * _numpy.exp((-2.0*k/3.0)*f2)
-    with u.set_enabled_equivalencies(u.dimensionless_angles()):
+    with units.set_enabled_equivalencies(units.dimensionless_angles()):
         term1 = e1 * ( _numpy.sin(2.0*w + n*t0)*_numpy.cos(2.0*i - 1.0)- _numpy.sin(2.0*w + n*t0)*_numpy.cos(2.0*i)*_numpy.cos(2.0*W) - 3.0*_numpy.sin(n*t0 + 2.0*w)*_numpy.cos(2.0*W) - 4.0*_numpy.sin(2.0*W)*_numpy.cos(2.0*w + n*t0)*_numpy.cos(i) )
         term2 = e2 * (1.0 - e*e) * ( _numpy.sin(2.0*w + n*t0)*(1.0-_numpy.cos(2.0*i)) - _numpy.sin(2.0*w + n*t0)*_numpy.cos(2.0*i)*_numpy.cos(2.0*W) - 3.0*_numpy.sin(n*t0 +2.0*w)*_numpy.cos(2.0*W) - 4.0*_numpy.cos(n*t0 + 2.0*w)*_numpy.sin(2.0*W)*_numpy.cos(i) )
         term3 = e4 * _numpy.sqrt(1.0 - e*e) * (-2.0*_numpy.cos(2.0*i)*_numpy.cos(2.0*w + n*t0)*_numpy.sin(2.0*W) - 6.0*_numpy.cos(2.0*w + n*t0)*_numpy.sin(2.0*W) - 8.0*_numpy.cos(2.0*W)*_numpy.sin(2.0*w + n*t0)*_numpy.cos(i) )
     
-    if averaged: return (prefactor).decompose(list(units.values()))
-    else: return (prefactor * ( term1 + term2 + term3)).decompose(list(units.values()))
+    if averaged: return (prefactor).decompose(list(unit_set.values()))
+    else: return (prefactor * ( term1 + term2 + term3)).decompose(list(unit_set.values()))
 
 def relative_energy_change(sim, star, averaged=False):
     '''
         An analytical estimate for the relative change in energy of a binary system due to a flyby star.
         
         Combines energy_change_adiabatic_estimate(...) and binary_energy(...) functions.
         
@@ -101,42 +102,42 @@
         Parameters
         ----------
         sim : REBOUND Simulation with two bodies, a central star and a planet
         star : AIRBALL Star flyby object
     '''
 
 
-    units = rebound_units(sim)
-    t0 = 0*units['time']
-    G = (sim.G * units['length']**3 / units['mass'] / units['time']**2)
+    unit_set = rebound_units(sim)
+    t0 = 0*unit_set['time']
+    G = (sim.G * unit_set['length']**3 / unit_set['mass'] / unit_set['time']**2)
     
     p = sim.particles
-    m1, m2, m3 = p[0].m * units['mass'], p[1].m * units['mass'], star.mass # redefine the masses for convenience
+    m1, m2, m3 = p[0].m * unit_set['mass'], p[1].m * unit_set['mass'], star.mass # redefine the masses for convenience
     M12 = m1 + m2 # total mass of the binary system
     M123 = m1 + m2 + m3 # total mass of all the objects involved
     
     mu = G*M123
     es = vinf_and_b_to_e(mu=mu, star_b=star.b, star_vinf=star.v)
     
-    a, e = p[1].a * units['length'], p[1].e # redefine the orbital elements of the planet for convenience
+    a, e = p[1].a * unit_set['length'], p[1].e # redefine the orbital elements of the planet for convenience
     n = _numpy.sqrt(G*M12/a**3) # compute the mean motion of the planet
     
     w, W, i = star.omega, star.Omega, star.inc # redefine the orientation elements of the flyby star for convenience
     V = star.v
     GM123 = G*M123 
     q = (- GM123 + _numpy.sqrt( GM123**2. + star.b**2. * V**4.))/V**2. # compute the periapsis of the flyby star
     
     prefactor = (-15.0/4.0) * m3 / _numpy.sqrt(M12*M123) * ((a/q)**1.5) * ((e * _numpy.sqrt(1.0 - e*e))/((1.0 + es)**1.5))
-    with u.set_enabled_equivalencies(u.dimensionless_angles()):
+    with units.set_enabled_equivalencies(units.dimensionless_angles()):
         t1 = (_numpy.sin(i) * _numpy.sin(i) * _numpy.sin(2.0*W) * ( _numpy.arccos(-1.0/es) + _numpy.sqrt(es*es - 1.0) )).value
         t2 = ((1.0/3.0) * (1.0 + _numpy.cos(i)*_numpy.cos(i)) * _numpy.cos(2.0*w) * _numpy.sin(2.0*W)).value
         t3 = (2.0 * _numpy.cos(i) * _numpy.sin(2.0*w) * _numpy.cos(2.0*W) * ((es*es - 1.0)**1.5)/(es*es)).value
 
-    if averaged: return (prefactor * ( ( _numpy.arccos(-1.0/es).value + _numpy.sqrt(es*es - 1.0) ) + (2.0/3.0) + (2.0 * ((es*es - 1.0)**1.5)/(es*es)) )).decompose(list(units.values()))
-    else: return (prefactor * (t1 + t2 + t3)).decompose(list(units.values()))
+    if averaged: return (prefactor * ( ( _numpy.arccos(-1.0/es).value + _numpy.sqrt(es*es - 1.0) ) + (2.0/3.0) + (2.0 * ((es*es - 1.0)**1.5)/(es*es)) )).decompose(list(unit_set.values()))
+    else: return (prefactor * (t1 + t2 + t3)).decompose(list(unit_set.values()))
 
 def energy_change_close_encounters_sim(sim):
     '''
         An analytical estimate for the change in energy of a binary system due to a flyby star.
         
         From the conclusions of Roy & Haddow (2003) https://ui.adsabs.harvard.edu/abs/2003CeMDA..87..411R/abstract and Heggie (2006) https://ui.adsabs.harvard.edu/abs/2006fbp..book...20H/abstract. The orbital element angles of the flyby star are determined with respect to the plane defined by the binary orbit. In REBOUND this is the same as when the inclination of the planet is zero.
```

### Comparing `airball-0.4.0/src/airball/flybys.py` & `airball-0.4.2/src/airball/flybys.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.0/src/airball/particle.py` & `airball-0.4.2/src/airball/particle.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.0/src/airball.egg-info/PKG-INFO` & `airball-0.4.2/src/airball.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airball
-Version: 0.4.0
+Version: 0.4.2
 Summary: A package for implementing flybys in hannorein/rebound
 Home-page: https://github.com/zyrxvo/airball/
 Author: Garett Brown
 Author-email: garett.brown@mail.utoronto.ca
 Project-URL: Bug Tracker, https://github.com/zyrxvo/airball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

