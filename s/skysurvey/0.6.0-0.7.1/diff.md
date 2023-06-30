# Comparing `tmp/skysurvey-0.6.0.tar.gz` & `tmp/skysurvey-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey-0.6.0.tar", last modified: Mon Jun 12 09:50:58 2023, max compression
+gzip compressed data, was "skysurvey-0.7.1.tar", last modified: Fri Jun 30 09:22:08 2023, max compression
```

## Comparing `skysurvey-0.6.0.tar` & `skysurvey-0.7.1.tar`

### file list

```diff
@@ -1,35 +1,44 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-12 09:50:58.348226 skysurvey-0.6.0/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.6.0/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-06-12 09:50:58.348282 skysurvey-0.6.0/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.6.0/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)     1169 2023-06-12 09:50:58.348586 skysurvey-0.6.0/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-06-12 09:49:45.000000 skysurvey-0.6.0/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-12 09:50:58.343821 skysurvey-0.6.0/skysurvey/
--rw-r--r--   0 rigault   (2358) staff       (20)       92 2023-06-12 09:46:56.000000 skysurvey-0.6.0/skysurvey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.6.0/skysurvey/config.py
--rw-r--r--   0 rigault   (2358) staff       (20)        0 2023-06-02 08:51:15.000000 skysurvey-0.6.0/skysurvey/dag.py
--rw-r--r--   0 rigault   (2358) staff       (20)    27022 2023-06-09 12:17:31.000000 skysurvey-0.6.0/skysurvey/dataset.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-12 09:50:58.345661 skysurvey-0.6.0/skysurvey/survey/
--rw-r--r--   0 rigault   (2358) staff       (20)      103 2023-06-09 12:36:07.000000 skysurvey-0.6.0/skysurvey/survey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8645 2023-05-02 20:15:06.000000 skysurvey-0.6.0/skysurvey/survey/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10970 2023-06-02 10:03:36.000000 skysurvey-0.6.0/skysurvey/survey/healpix.py
--rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.6.0/skysurvey/survey/polygon.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.6.0/skysurvey/survey/ztf.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-12 09:50:58.348007 skysurvey-0.6.0/skysurvey/target/
--rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.6.0/skysurvey/target/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.6.0/skysurvey/target/collection.py
--rw-r--r--   0 rigault   (2358) staff       (20)    31327 2023-06-02 09:43:01.000000 skysurvey-0.6.0/skysurvey/target/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.6.0/skysurvey/target/environments.py
--rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.6.0/skysurvey/target/kilonova.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2341 2023-06-09 12:22:54.000000 skysurvey-0.6.0/skysurvey/target/sncc.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10070 2023-06-02 09:06:49.000000 skysurvey-0.6.0/skysurvey/target/snia.py
--rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.6.0/skysurvey/target/stars.py
--rw-r--r--   0 rigault   (2358) staff       (20)     6386 2023-06-02 09:51:33.000000 skysurvey-0.6.0/skysurvey/target/timeserie.py
--rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.6.0/skysurvey/template.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-12 09:50:58.344773 skysurvey-0.6.0/skysurvey.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-06-12 09:50:58.000000 skysurvey-0.6.0/skysurvey.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      721 2023-06-12 09:50:58.000000 skysurvey-0.6.0/skysurvey.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-12 09:50:58.000000 skysurvey-0.6.0/skysurvey.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-12 09:47:03.000000 skysurvey-0.6.0/skysurvey.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)      162 2023-06-12 09:50:58.000000 skysurvey-0.6.0/skysurvey.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-06-12 09:50:58.000000 skysurvey-0.6.0/skysurvey.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.109190 skysurvey-0.7.1/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.7.1/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-06-30 09:22:08.109241 skysurvey-0.7.1/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     2136 2023-06-30 08:24:06.000000 skysurvey-0.7.1/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)     1205 2023-06-30 09:22:08.109530 skysurvey-0.7.1/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-06-12 09:49:45.000000 skysurvey-0.7.1/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.104800 skysurvey-0.7.1/skysurvey/
+-rw-r--r--   0 rigault   (2358) staff       (20)       90 2023-06-30 09:21:49.000000 skysurvey-0.7.1/skysurvey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      524 2023-06-27 13:24:20.000000 skysurvey-0.7.1/skysurvey/config.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    27899 2023-06-29 09:38:43.000000 skysurvey-0.7.1/skysurvey/dataset.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.106149 skysurvey-0.7.1/skysurvey/examples/
+-rw-r--r--   0 rigault   (2358) staff       (20)       26 2023-06-29 14:59:14.000000 skysurvey-0.7.1/skysurvey/examples/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2233 2023-06-29 14:59:29.000000 skysurvey-0.7.1/skysurvey/examples/mocksurvey.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.107007 skysurvey-0.7.1/skysurvey/survey/
+-rw-r--r--   0 rigault   (2358) staff       (20)      125 2023-06-28 15:34:39.000000 skysurvey-0.7.1/skysurvey/survey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     9538 2023-06-29 14:45:35.000000 skysurvey-0.7.1/skysurvey/survey/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2849 2023-06-29 07:52:19.000000 skysurvey-0.7.1/skysurvey/survey/des.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    15609 2023-06-29 13:44:29.000000 skysurvey-0.7.1/skysurvey/survey/healpix.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      976 2023-06-30 08:20:21.000000 skysurvey-0.7.1/skysurvey/survey/lsst.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    13238 2023-06-29 13:35:29.000000 skysurvey-0.7.1/skysurvey/survey/polygon.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8955 2023-06-29 09:16:04.000000 skysurvey-0.7.1/skysurvey/survey/survey.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1938 2023-06-29 13:30:27.000000 skysurvey-0.7.1/skysurvey/survey/ztf.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.108790 skysurvey-0.7.1/skysurvey/target/
+-rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.7.1/skysurvey/target/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.7.1/skysurvey/target/collection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    32874 2023-06-29 18:30:17.000000 skysurvey-0.7.1/skysurvey/target/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.7.1/skysurvey/target/environments.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.7.1/skysurvey/target/kilonova.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2341 2023-06-09 12:22:54.000000 skysurvey-0.7.1/skysurvey/target/sncc.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10033 2023-06-28 13:24:24.000000 skysurvey-0.7.1/skysurvey/target/snia.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.7.1/skysurvey/target/stars.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     6428 2023-06-28 13:23:49.000000 skysurvey-0.7.1/skysurvey/target/timeserie.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.7.1/skysurvey/template.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.109100 skysurvey-0.7.1/skysurvey/tools/
+-rw-r--r--   0 rigault   (2358) staff       (20)       64 2023-06-29 10:12:11.000000 skysurvey-0.7.1/skysurvey/tools/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2301 2023-06-27 14:26:14.000000 skysurvey-0.7.1/skysurvey/tools/snana.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2762 2023-06-27 08:23:39.000000 skysurvey-0.7.1/skysurvey/tools/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 09:22:08.105825 skysurvey-0.7.1/skysurvey.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      747 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      922 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-12 09:47:03.000000 skysurvey-0.7.1/skysurvey.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)      194 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-06-30 09:22:08.000000 skysurvey-0.7.1/skysurvey.egg-info/top_level.txt
```

### Comparing `skysurvey-0.6.0/LICENSE` & `skysurvey-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey-0.6.0/PKG-INFO` & `skysurvey-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skysurvey
-Version: 0.6.0
+Version: 0.7.1
 Summary: Simulating Transient in the sky and how to observe them
 Home-page: https://github.com/MickaelRigault/skysurvey
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `skysurvey-0.6.0/README.md` & `skysurvey-0.7.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -20,43 +20,59 @@
 ```bash
 git clone https://github.com/MickaelRigault/skysurvey.git
 cd skysurvey
 python setup.py install
 ```
 
 # Quick Start
-You need to create a `Target` object (or child of) and a `Survey` object (or child of) and then to simulate how your survey would see your targets. This latter is called a `DataSet`. Here is a quick example:
+You need to create a `Target` and a `Survey` and
+then to simulate how your survey would see your targets. 
+This latter is called a `DataSet`. Here is a quick example:
+
 ## Step 1: targets (truth)
 ```python
-from skysurvey import target
-snia = target.SNeIa() # create a pre-defined SN Ia target object
-data = snia.draw(size=5000) # and draw 5000 of them (you have many options)
-data.head(5) # data also stored in snia.data
+import skysurvey
+snia = skysurvey.SNeIa()
+data = snia.draw(size=50_000, tstart=56_000, tstop=56_100) # see options
+data.head(5) # also snia.data
 ```
 
 ## Step 2: Survey (when you pointed and sky conditions)
 ```python
-from skysurvey import survey
-# Say I what a ztf-fields survey, observing 1000 fields per day for 4 years
-# Let get the starting date from the data
-starting_date = snia.data["t0"].min()-50 # 50 days before the first target, no need to simulate a survey before that
-
-# and this is a much-simplified version of ZTF (independent random draws)
-ztf = survey.ZTF.from_random(size=365*4*1000, # number of observation 
-                       bands=["ztfg","ztfr","ztfi"], # band to observed
-                       mjd_range=[starting_date, starting_date+365*4], # timerange of observation
-                       skynoise_range=[10,20], # sky noise
-                     )
-ztf.data.head(5)
+import numpy as np
+from skysurvey.tools import utils
+
+size = 10_000
+
+# footprint
+from shapely import geometry
+sq_footprint = geometry.box(-1, -1, +1, +1)
+
+# Observing data
+ra, dec = utils.random_radec(size=size, ra_range=[200,250], dec_range=[-20,10])
+
+data = {}
+data["ra"] = ra
+data["dec"] = dec
+data["gain"] = 1
+data["zp"] = 30
+data["skynoise"] = np.random.normal(size=size, loc=150, scale=20)
+data["mjd"] = np.random.uniform(56_000-10, 56_100 + 10, size=size)
+data["band"] = np.random.choice(["desg","desr","desi"], size=size)
+
+# Build the survey
+survey = skysurvey.Survey.from_pointings(data, footprint=sq_footprint)
+survey.show()
 ```
 
 ## Step 3: Dataset
 
-And now let's build the dataset (computation split by fieldid)
+And now let's build the dataset. The simulated lightcurves are in
+dset.data, the input survey is stored in dset.survey, the input
+targets is stored in dset.targets
+
 ```python
-from survey import dataset
-dset = dataset.DataSet.from_targets_and_survey(snia, ztf) # this takes ~30s on a laptop for ~5000 targets
+from skysurvey import dataset
+dset = dataset.DataSet.from_targets_and_survey(snia, survey)
 dset.data
-# your survey (here ztf) is stored in dset.survey
-# your targets (here snia) is stored in dset.targets
 ```
```

### Comparing `skysurvey-0.6.0/setup.cfg` & `skysurvey-0.7.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -26,21 +26,24 @@
 install_requires = 
 	importlib_resources; python_version < '3.10'  # not needed from 3.10
 	
 	numpy
 	pandas
 	scipy
 	
+	healpy
+	shapely
+	geopandas
+	
 	astropy
 	sncosmo
-	healpy
 	extinction
 	
-	modeldag
-	ztffields
+	modeldag>=0.3.3
+	ztffields>=0.4.3
 
 [options.package_data]
 
 [options.extras_require]
 docs = nbsphinx
 tests = pytest; coverage
```

### Comparing `skysurvey-0.6.0/skysurvey/dataset.py` & `skysurvey-0.7.1/skysurvey/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from astropy.table import Table
 
 from .template import Template
 
 
 __all__ = ["DataSet", "get_obsdata"]
 
-def get_obsdata(template, observations, parameters, zpsys="ab"):
+def get_obsdata(template, observations, parameters, zpsys="ab", incl_error=True):
     """ get observed data using ``sncosmo.realize_lcs()``
 
     Parameters
     ----------
     template: sncosmo.Model
         an sncosmo model from which we can draw observations
         (passed to 
@@ -27,14 +27,19 @@
         Dataframe containing the observing infortation.
         requested entries: TBD
     
     parameters: pandas.DataFrame
         Dataframe containing the target parameters information.
         These depend on you model. 
 
+    incl_error: bool
+        should the returned flux contain a random gaussian scatter
+        drawn from the flux_err ?
+        If False, lightcurve flux are "perfect".
+
     Returns
     -------
     MultiIndex DataFrame
         all the observations for all targets
 
     See also
     --------
@@ -46,15 +51,17 @@
         
     sncosmo_obs = Table.from_pandas(observations.rename({"mjd":"time"}, axis=1)) # sncosmo format
     
     # sn parameters
     list_of_parameters = [p_.to_dict() for i_,p_ in parameters.iterrows()] # sncosmo format
     
     # realize LC
-    list_of_observations = sncosmo.realize_lcs(sncosmo_obs, template, list_of_parameters)
+    list_of_observations = sncosmo.realize_lcs(sncosmo_obs, template, list_of_parameters,
+                                               scatter=incl_error)
+    
     if len(list_of_observations) == 0:
         return None
     
     return pandas.concat([l.to_pandas().set_index(observations.index) for l in list_of_observations],  keys=parameters.index)
 
 def _get_obsdata_(data, **kwargs):
     """ internal method to simplify get_obsdata using single input (for map)
@@ -104,49 +111,53 @@
         read_parquet: loads a stored dataset
         """
         self.set_data(data)
         self.set_targets(targets)
         self.set_survey(survey)
         
     @classmethod
-    def from_targets_and_survey(cls, targets, survey, template=None, client=None, **kwargs):
+    def from_targets_and_survey(cls, targets, survey, template=None, client=None,
+                                    incl_error=True, **kwargs):
         """ loads a dataset (observed data) given targets and a survey
 
         This first matches the targets (given targets.data[["ra","dec"]]) with the
         survey to find which target has been observed with which field.
         Then simulate the targets lightcurves given the observing data (survey.data).
         
 
         Parameters
         ----------
         targets: skysurvey.Target (or child of)
             target data corresponding to the true target parameters  
             (as given by nature)
             
-        survey: skysurvey.Survey (or child of)
+        survey: skysurvey.Survey, skysurvey.GridSurvey (or child of)
             sky observation (what was observed when with which situation)
 
         client: dask.distributed.Client()
             dask client to use if any. This is used for 
             parallelization of the lc generation per field.
 
+        incl_error: bool
+
         **kwargs goes to realize_survey_target_lcs
 
         Returns
         -------
         class instance
             the observation data have been derived and stored as self.data
 
         See also
         --------
         read_parquet: loads a stored dataset
         """
         lightcurves, fieldids = cls.realize_survey_target_lcs(targets, survey, template=template,
                                                                   client=client,
-                                                 **kwargs)
+                                                                  incl_error=incl_error,
+                                                                  **kwargs)
         data = pandas.concat(lightcurves, keys=fieldids # store fieldid
                                  ).reset_index(survey.fieldids.names)
         return cls(data, targets=targets, survey=survey)
 
     @classmethod
     def read_parquet(cls, parquetfile, survey=None, targets=None, **kwargs):
         """ loads a stored dataset. 
@@ -290,15 +301,15 @@
             if detected:
                 data = data[ data["detection"] ] > detlimit
             else:
                 data = data[ data["detection"] ] <= detlimit
 
         return data
         
-    def get_ndetection(self, detlimit=5, per_band=False):
+    def get_ndetection(self, detlimit=5, per_band=False, data=None):
         """ get the number of detection for each lightcurves
 
         Basically computes the number of datapoints with (flux/fluxerr)>detlimit)
 
         Parameters
         ----------
         detlimit: float, int
@@ -310,15 +321,19 @@
             if true it will then be per target *and* per band.
 
         Returns
         -------
         pandas.Series
             the number of detected point per target (and per band if per_band=True)
         """
-        data = self.data.copy()
+        if data is None:
+            data = self.data.copy()
+        else:
+            data = data.copy()
+            
         data["detected"] = (data["flux"]/data["fluxerr"])>detlimit
         if per_band:
             groupby = ["index","band"]
         else:
             groupby = "index"
         
         ndetection = data.groupby(groupby)["detected"].sum()
@@ -580,14 +595,15 @@
     
     # -------------- #
     #    Statics     #
     # -------------- #
     @classmethod
     def realize_survey_target_lcs(cls, targets, survey, template=None,
                                   template_prop={}, nfirst=None,
+                                  incl_error=True,
                                   client=None):
         """ creates the lightcurve of the input targets as they 
         would be observed by the survey. 
         = These are split per survey fields. =
         
         
         Parameters
@@ -610,14 +626,15 @@
             if given, only the first nfrist entries will be considered.
             This is a debug / test tool.
         
         client: dask.distributed.Client()
             dask client to use if any. This is used for 
             parallelization of the lc generation per field.
         
+        incl_error: bool
             
         Returns
         -------
         list, list
             - list of dataframe (1 per fields, all targets of the field in)
             - list of fields (fieldid)
             
@@ -639,21 +656,23 @@
                 fieldids_indexes = pandas.Index(data=fieldids_indexes, name=survey.fieldids.names[0])
                 
         else: # input is a single-kind target
             lc_out, fieldids_indexes = cls._realize_survey_kindtarget_lcs(targets, survey,
                                                           template=template,
                                                           template_prop=template_prop,
                                                           nfirst=nfirst,
-                                                          client=client)
+                                                          client=client,
+                                                          incl_error=incl_error)
         return lc_out, fieldids_indexes
 
         
     @staticmethod
     def _realize_survey_kindtarget_lcs( targets, survey, template=None,
                                            template_prop={}, nfirst=None,
+                                           incl_error=True,
                                            client=None):
         """ creates the lightcurve of the input single-kind 
         targets as they  would be observed by the survey. 
         = These are split per survey fields. =
         
         
         Parameters
@@ -676,15 +695,16 @@
             if given, only the first nfrist entries will be considered.
             This is a debug / test tool.
         
         client: dask.distributed.Client()
             dask client to use if any. This is used for 
             parallelization of the lc generation per field.
         
-            
+        incl_error: bool
+        
         Returns
         -------
         list, list
             - list of dataframe (1 per fields, all targets of the field in)
             - list of fields (fieldid)
             
         See also
@@ -739,23 +759,24 @@
             # Taking the data we need
             this_target = target_indexed.xs(index_, level=levels)[template_columns].copy()
             return sncosmo_model, this_survey, this_target
 
         data = [get_index_lc_input(index_) for index_ in fieldids_indexes]
         if client is not None:
             big_future = client.scatter(data) # scatter data
-            futures_ = client.map(_get_obsdata_, big_future)
+            futures_ = client.map(_get_obsdata_, big_future, incl_error=incl_error)
             lc_out = client.gather(futures_)
         else:
-            lc_out = [_get_obsdata_(data_) for data_ in data if data_ is not None]
+            lc_out = [_get_obsdata_(data_, incl_error=incl_error)
+                          for data_ in data if data_ is not None]
 
         return lc_out, fieldids_indexes
 
     # ============== #
-    #   Properties   #
+    #   Properties   # 
     # ============== #
     @property
     def data(self):
         """ """
         return self._data
 
     @property
```

### Comparing `skysurvey-0.6.0/skysurvey/survey/core.py` & `skysurvey-0.7.1/skysurvey/survey/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import pandas
 
 __all__ = ["BaseSurvey"] # no import when 'import *'
 
 class BaseSurvey( object ):
     
-    REQUIRED_COLUMNS = ['mjd', 'band', 'skynoise', 'fieldid', "gain", "zp"]
+    REQUIRED_COLUMNS = ['mjd', 'band', 'skynoise', "gain", "zp"]
     
     def __init__(self, data):
         """ 
         See also
         --------
         
         """
@@ -37,25 +37,36 @@
         lower_precision: bool
              change the types from 64 to 32 precision when possible.
 
         Returns
         -------
         None
         """
-        if data is not None and not np.in1d(self.REQUIRED_COLUMNS, data.columns).all():
-            raise ValueError(f"at least one of the following column name if missing {self.REQUIRED_COLUMNS}")
+        if data is None:
+            self._data = None
+            return
+        
+        if not np.in1d(self.REQUIRED_COLUMNS, data.columns).all():
+            warnings.warn(f"at least one of the following column name if missing {self.REQUIRED_COLUMNS}")
 
-        if lower_precision and data is not None:
+        if self.fields is not None and self.fieldids.name is not None:
+            if not np.all([f_name in data for f_name in self.fieldids.names]):
+                warnings.warn(f"fieldid {self.fieldids.names} are not in the input data")
+            
+        if lower_precision:
             data = data.astype( {k: str(v).replace("64","32") for k, v in data.dtypes.to_dict().items()})
             
         self._data = data
-        
     # ------------ #
     #   GETTER     #
     # ------------ #
+    def get_timerange(self, timekey="mjd"):
+        """ """
+        return self.data[timekey].agg([np.min, np.max]).values
+        
     def get_fieldcoverage(self, incl_zeros=False, fillna=np.NaN,
                           **kwargs):
         """ short cut to get_fieldstat('size') 
 
         Parameters
         ----------
         incl_zeros: bool
@@ -116,42 +127,55 @@
         -------
         DataFrame or Serie 
             following groupby.agg()
 
         """
         if data is None:
             data = self.data.copy()
-            
+
+        fieldids = self.fieldids.names
+
+        fieldgrouped = self.data.groupby(fieldids)
         if stat in ["size","value_counts"]:
-            data = data["fieldid"].value_counts()
+            data = fieldgrouped.size()
             
         elif columns is None:
-            data = data.groupby("fieldid").agg(stat)
+            data = fieldgrouped.agg(stat)
         else:
-            data = data.groupby("fieldid")[columns].agg(stat)
+            data = fieldgrouped[columns].agg(stat)
             
         if not incl_zeros:
             return data
-        
-        if type(data) == pandas.Series: # Serie
-            all_data = np.ones(self.nfields)*fillna
-            all_data[data.index] = data.values
-            all_data = pandas.Series(all_data, name=f"fieldid_{stat}")
-            
-        else: # DataFrame
-            all_data = np.ones((self.nfields, data.shape[1]))*fillna
-            all_data[data.index] = data.values
-            all_data = pandas.DataFrame(all_data, columns=data.columns)
-            
-        return all_data
+
+        return data.reindex(self.fieldids, level=0)
         
         
     def radec_to_fieldid(self, radec):
         """ get the fieldid of the given (list of) coordinates """
         raise NotImplementedError("you have not implemented radec_to_fieldid for your survey")
+
+    def get_observations_from_coords(self, radec):
+        """ returns the data associated to the input radec coordinates
+        
+        (calls radec_to_fieldid and select data matching the fieldid)
+
+        Parameters
+        ----------
+        radec: pandas.DataFrame or 2d array
+            coordinates in degree
+            (see format radec_to_fieldid())
+            
+        Returns
+        -------
+        pandas.DataFrame
+            copy of the data observed in the given radec coordinates
+        
+        """
+        fields = self.radec_to_fieldid(radec, observed_fields=True)
+        return self.data[ self.data[self.fieldids.name].isin(fields[self.fieldids.name]) ].copy()
     
     # ----------- #
     #  PLOTTER    #
     # ----------- #        
     def show(self):
         """ shows the sky coverage """
         raise NotImplementedError("you have not implemented show for your survey")
@@ -252,14 +276,22 @@
     def nfields(self):
         """ number of fields """
         if not hasattr(self,"_nfields") or self._nfields is None:
             warnings.warn("no nfields set, so this is assuming max of data['fieldid'].")
             self._nfields =self.data["fieldid"].max()
             
         return self._nfields
+
+    @property
+    def fields(self):
+        """ geodataframe containing the fields coordinates """
+        if not hasattr(self,"_fields"):
+            return None
+        return self._fields
+
     
     @property
     def of_type(self):
         """ kind of survey that is """
         return str(type(self)).split("'")[-2].split(".")[-1]
 
     @property
```

### Comparing `skysurvey-0.6.0/skysurvey/survey/ztf.py` & `skysurvey-0.7.1/skysurvey/survey/ztf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,59 @@
-from .polygon import Survey
+from .survey import GridSurvey
 from ztffields.fields import Fields
 
 __all__ = ["ZTF"]
 
-class ZTF( Survey ):
+class ZTF( GridSurvey ):
 
-    def __init__(self, data=None, level="focalplane", **kwargs):
+    
+    def __init__(self, data=None, level="quadrant", **kwargs):
         """ """
+        
+        footprint = Fields.get_contours(level=level,
+                                              as_polygon=True, allow_multipolygon=True)
         fields = Fields.get_field_geometry(level=level)
-        return super().__init__(data=data, fields=fields)
-
+        
+        super().__init__(data=data, fields=fields, footprint=footprint)
+        self._level = level
+        
     @classmethod
     def from_logs(cls, **kwargs):
         """ """
         from ztfquery.skyvision import get_summary_logs
         logs = get_summary_logs(**kwargs)
         return cls.from_pointings(data=logs, level="quadrant")
         
-        
     @classmethod
     def from_pointings(cls, data, level="quadrant"):
         """ """
         if type(data) is dict:
             data = pandas.DataFrame.from_dict(data)
             
         return cls(data=data, level=level)
 
-
-    @classmethod
-    def from_random(cls, size, bands, mjd_range, skynoise_range,
-                    level="focalplane", **kwargs):
-        """ 
-        fields
-        """
-        this = cls(level=level)
-        this.draw_random(size, bands,  
-                        mjd_range, skynoise_range, 
-                        inplace=True, **kwargs)
-        return this
-
-
-    def show(self, data=None, **kwargs):
+    def show_ztf(self, data=None, fieldstat=None, **kwargs):
         """ shows the sky coverage 
 
+        data: pandas.DataFrame
+            data to be consider to get the field statistics.
+            fieldstat will be derived from that (main grid only) groupby(fieldid).size()
+            = ignored is fieldstat is given = 
+            
+        fieldstat: pandas.Series
+            field statistics.
+
         **kwargs goes to ztffields.skyplot_fields
         """
         import ztffields
-        if data is None:
-            data = self.data
-        
-        datamain = data[data["fieldid"]<1000] # main grid
-        fieldid_s = datamain.groupby("expid").first().groupby("fieldid").size()
+        if fieldstat is None:
+            if data is None:
+                data = self.data
+                
+            datamain = data[data["fieldid"]<1000] # main grid
+            fieldstat = datamain.groupby("expid").first().groupby("fieldid").size()
 
-        fig = ztffields.skyplot_fields(fieldid_s, 
+        fig = ztffields.skyplot_fields(fieldstat, 
                                         label="number of observations (main grid)",
                                            **kwargs)
+        return fig
```

### Comparing `skysurvey-0.6.0/skysurvey/target/collection.py` & `skysurvey-0.7.1/skysurvey/target/collection.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.6.0/skysurvey/target/core.py` & `skysurvey-0.7.1/skysurvey/target/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import warnings
 import numpy as np
 import pandas
 import inspect
 from astropy import cosmology, time
 from astropy.utils.decorators import classproperty
 
 
 from ..template import Template
+from ..tools.utils import parse_skyarea, surface_of_skyarea
 
 
 __all__ = ["Target", "Transient"]
 
 
+
 class Target( object ):
 
     _KIND = "unknow"
     _TEMPLATE = None
     _MODEL = None # dict config 
     
     # - Cosmo
@@ -94,14 +97,15 @@
         this.set_data(data)
         return this
         
     @classmethod
     def from_draw(cls, size=None, model=None, template=None,
                       zmax=None, tstart=None, tstop=None,
                       zmin=0, nyears=None,
+                      skyarea=None,
                       **kwargs):
         """ loads the instance from a random draw of targets given the model 
 
         Parameters
         ----------
         size: int, None
             number of target you want to sample
@@ -140,14 +144,21 @@
         nyears: float
             if given, nyears will set:
             - size: it will be the number of target expected up to zmax 
             in the given  number of years. 
             This uses get_rate(zmax).
             - tstop: tstart+365.25*nyears
 
+        skyarea: None, string, geometry
+            sky area to be considered.
+            - str: full (equivalent to None), ['extra-galactic', not implemented yet]
+            - geometry: shapely.Geometry
+            - None: full sky 
+
+
         **kwargs goes to self.draw()
 
         Returns
         -------
         class instance
             self.data, self.model and self.template will be loaded.
 
@@ -156,18 +167,22 @@
         from_setting:  loads an instance given model parameters (dict)            
         """
         this = cls()
         if model is not None:
             this.set_model(model)
 
         if template is not None:
-            self.set_template(template)
+            this.set_template(template)
             
-        _ = this.draw(size=size, zmax=zmax, tstart=tstart, tstop=tstop,
-                      nyears=nyears, **kwargs)
+        _ = this.draw(size=size,
+                        zmin=zmin, zmax=zmax,
+                        tstart=tstart, tstop=tstop,
+                        nyears=nyears,
+                        skyarea=skyarea,
+                          **kwargs)
         return this
         
     # ------------- # 
     #   Template    #
     # ------------- #
     def set_template(self, template):
         """ set the template 
@@ -283,16 +298,16 @@
         -------
         bandflux : float or `~numpy.ndarray`
             Flux in photons / s /cm^2, unless `zp` and `zpsys` are
             given, in which case flux is scaled so that it corresponds
             to the requested zeropoint. Return value is `float` if all
             input parameters are scalars, `~numpy.ndarray` otherwise.
         """
-        template = self.get_target_template(index)
-        return template.bandflux(band, template.get('t0')+phase, zp=zp, zpsys=zpsys)
+        sncosmo_model = self.get_target_template(index).sncosmo_model
+        return sncosmo_model.bandflux(band, sncosmo_model.get('t0')+phase, zp=zp, zpsys=zpsys)
 
 
     def clone_target_change_entry(self, index, name, values, as_dataframe=False):
         """ get a clone of the given target at the given redshifts.
         This: 
         (1) copies the index entries, 
         (2) sets the `name` to the input `values`
@@ -318,15 +333,15 @@
         Returns
         -------
         instance or DataFrame
         """
         dd = self.data.loc[index].to_frame().T
         dd.loc[index, name] = np.atleast_1d(values)
         dd = dd.explode(name)
-        dd[name] = dd[name].astype(float)
+#        dd[name] = dd[name].convert_dtypes()
         data = self.model.redraw_from(name, dd, incl_name=False)
         if as_dataframe:
             return data
         
         return self.__class__.from_data(data)
     
     # -------------- #
@@ -486,48 +501,15 @@
 
         Returns
         -------
         array
             array of observed magnitude (``distmod(z)+magabs``)
         
         """
-        return cosmology.distmod(np.asarray(z)).value + magabs
-
-    def draw_radec(cls, model="random", size=None, ra_range=[0,360], dec_range=[-90,90]):
-        """ draw the sky positions
-
-        Parameters
-        ----------
-        model: str
-            name of the model. Implemented:
-            - random: random homogeneous 2d-sky distribution
-            (accounts for dec deformation)
-
-        size: int, None
-            number of draw
-
-        ra_range: 2d-array
-            right-accension boundaries (min, max)
-
-        dec_range: 2d-array
-            declination boundaries
-            
-        Returns
-        -------
-        2d-array
-            list of ra, list of dec.
-        """
-        if model == "random":
-            dec_sin_range = np.sin(np.asarray(dec_range)*np.pi/180)
-            ra = np.random.uniform(*ra_range, size=size)
-            dec = np.arcsin( np.random.uniform(*dec_sin_range, size=size) ) / (np.pi/180)
-        else:
-            raise NotImplementedError("Only the 'random' radec model has been implemented. ")
-        
-        return ra, dec
+        return cosmology.distmod(np.asarray(z, dtype="float32")).value + magabs
 
     # -------------- #
     #   Model        #
     # -------------- #
     def set_model(self, model):
         """ set the target model 
 
@@ -627,15 +609,15 @@
         value of the entry parameter
         
         Example
         -------
         >>> self.get_model_parameter('redshift', 'zmax', None)
 
         """
-        return self.model.model[entry]["param"].get(key, default)
+        return self.model.model[entry]["kwargs"].get(key, default)
 
     def change_model_parameter(self, **kwargs):
         """ Change the model parameters
 
         **kwargs will update any model entry parameters (i.e., the "param", e.g. t0["param"]).
 
         Example
@@ -683,18 +665,18 @@
         return fig
             
     # =============== #
     #   Draw Methods  #
     # =============== #
     def draw(self, size=None,
                  zmax=None, zmin=0,
-                 tstart=None, tstop=None,
-                 nyears=None,
+                 tstart=None, tstop=None, nyears=None,
+                 skyarea=None,
                  inplace=True, **kwargs):
-        """ draws the parameter model (using self.model.draw() 
+        """ draws the parameter model (using self.model.draw()) 
 
         Parameters
         ----------
         size: int
             = ignored is nyears is not None =
             number of target you want to draw.
 
@@ -715,64 +697,104 @@
         nyears: float
             if given, nyears will set:
             - size: it will be the number of target expected up to zmax 
             in the given  number of years. 
             This uses ``get_rate(zmax)``.
             - tstop: ``tstart+365.25*nyears``
 
+        skyarea: None, string, geometry
+            sky area to be considered.
+            - str: full (equivalent to None), 'extra-galactic'
+            - geometry: shapely.Geometry
+            - None: full sky
+
         inplace: bool
             sets self.data to the newly drawn dataframe
 
         Returns
         -------
         DataFrame
             the simulated dataframe.
 
         """
+        if nyears is None and (tstart is not None and tstop is not None):
+            nyears = (tstop-tstart)/365.25
+                
+        if nyears is not None and (tstart is not None and tstop is None):
+            tstop = tstart + nyears*365.25
+
+        if nyears is not None and (tstart is  None and tstop is not None):
+            tstart = tstop - nyears*365.25
+                
+        if nyears is None and size is None:
+            raise ValueError(" You must provide either nyears or size")
         
-        # short cut 
-        # -> change the redshift
+        if nyears is not None and size is not None:
+            nyears = None # its job is done.
+
+        #
+        # Redshift
+        #
+        # zmax
         if zmax is not None:
             kwargs.setdefault("redshift",{}).update({"zmax": zmax})
             
         elif nyears is not None:
             zmax = self.get_model_parameter("redshift", "zmax", None)
-
+        # zmin
         if zmin is not None and "redshift" in self.model.model:
             kwargs.setdefault("redshift",{}).update({"zmin": zmin})
             
         elif nyears is not None:
             zmin = self.get_model_parameter("redshift", "zmin", None)
 
         if tstop is not None:
             if type( tstop ) is str:
                 tstop = time.Time(tstop).mjd
 
             kwargs.setdefault("t0",{}).update({"high": tstop})
-            
-        # time range:        
+
+        #
+        # time range
+        #
         if tstart is not None:
             if type( tstart ) is str:
                 tstart = time.Time(tstart).mjd
                 
             kwargs.setdefault("t0",{}).update({"low": tstart})
             if tstop is None and nyears is None: # do 1 year by default
                 kwargs.setdefault("t0",{}).update({"high": tstart+365.25})
         # tstart is None, then what ?
         elif tstop is not None and nyears is not None:
             tstart = tstop - 365.25*nyears # fixed later            
         elif nyears is not None:
             tstart = self.get_model_parameter("t0", "low", None)
 
+        #
+        # Sky area
+        #
+        skyarea = parse_skyarea(skyarea) # shapely.geometry or skyarea
+        if skyarea is not None:
+            param_affected = [k for k, v in self.model.get_func_parameters().items() if "skyarea" in v]
+            if "radec" in self.model.model.keys() and "radec" not in param_affected:
+                warnings.warn("radec in model, skyarea given, but the radec func does not accept skyarea.")
+                
+            for k in param_affected:
+                kwargs.setdefault(k,{}).update({"skyarea": skyarea})
+                
+
+        #
+        # Size
+        #
+        # skyarea affect get_rate
         if nyears is not None:
-            rate_min = self.get_rate(zmin) if (zmin is not None and zmin >0) else 0
+            rate_min = self.get_rate(zmin, skyarea=skyarea) if (zmin is not None and zmin >0) else 0
             kwargs.setdefault("t0",{}).update({"low": tstart, "high": tstart + 365.25*nyears})
-            size = int((self.get_rate(zmax)-rate_min) * nyears)
+            size = int((self.get_rate(zmax, skyarea=skyarea)-rate_min) * nyears)
             
-
         # actually draw the data
         data = self.model.draw(size=size, **kwargs)
         if inplace:
             # lower precision
             data = data.astype( {k: str(v).replace("64","32") for k, v in data.dtypes.to_dict().items()})
             self.set_data(data)
             
@@ -857,21 +879,28 @@
         -------
         1d-array
             pdf of the redshift distribution
         """
         rates = np.diff(self.get_rate(z, **kwargs))
         return rates/np.nansum(rates)
     
-    def get_rate(self, z, **kwargs):
+    def get_rate(self, z, skyarea=None, **kwargs):
         """ number of target (per year) up to the given redshift
 
         Parameters
         ----------
         z: float
             redshift
+        
+        skyarea: None, str, float, geometry
+            sky area (in deg**2).
+            - None or 'full': 4pi
+            - "extra-galactic": 4pi - (milky-way b<5)
+            - float: area in deg**2
+            - geometry: shapely.geometry.area is used (assumed in deg**2)
 
         **wkwargs goes to the rate function (if a function, not a number)
 
         Returns
         -------
         int
         
@@ -880,14 +909,19 @@
         getpdf_redshift: the redshift distribution
         rate: float (volumetric_rate) or func (any)
         """
         if callable(self.rate):
             return self.rate(z, **kwargs)
         
         volume = self.cosmology.comoving_volume(z).to("Gpc**3").value
+        skyarea = surface_of_skyarea(skyarea) # in deg**2 or None
+        if skyarea is not None:
+            full_sky = 4*np.pi * (180/np.pi)**2 # 4pi in deg**2
+            volume *= (skyarea/full_sky)
+            
         z_rate = volume * self.rate
         return z_rate
         
     def get_lightcurve(self, band, times,
                            sncosmo_model=None, index=None,
                            in_mag=False, zp=25, zpsys="ab",
                            **kwargs):
```

### Comparing `skysurvey-0.6.0/skysurvey/target/sncc.py` & `skysurvey-0.7.1/skysurvey/target/sncc.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.6.0/skysurvey/target/snia.py` & `skysurvey-0.7.1/skysurvey/target/snia.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 import numpy as np
 from .core import Transient
 
 from .environments import getpdf_asymetric_gaussian
+from ..tools.utils import random_radec
 
 __all__ = ["SNeIa"]
 
 
 # ================== #
 #                    #
 # Pre-Defined models #
@@ -265,16 +266,16 @@
                              "kwargs": {"z":"@z", "magabs":"@magabs"},
                             },
 
                    x0 = {"func": "magobs_to_amplitude", # defined in Transients
                          "kwargs": {"magobs":"@magobs", "param_name": "x0"},
                         }, #because it needs to call sncosmo_model.get(param_name)
                        
-                   radec = {"func": "random",
-                            "kwargs": {"ra_range":[0, 360], "dec_range":[-30, 90]},
+                   radec = {"func": random_radec,
+                            "kwargs": {},
                             "as": ["ra","dec"]
                            }
                     )
 
 
 class SNeIaHostMass( Transient ):
     
@@ -304,16 +305,16 @@
                              "kwargs": {"z":"@z", "magabs":"@magabs"},
                              },
 
                    x0 = {"func": "magobs_to_amplitude", # defined in Transients
                          "kwargs": {"magobs": "@magobs", "param_name":"x0"}
                         }, #because it needs to call sncosmo_model.get(param_name)
                        
-                   radec = {"func": "random",
-                            "kwargs": dict(ra_range=[0, 360], dec_range=[-30, 90]),
+                   radec = {"func": random_radec,
+                            "kwargs": {},
                             "as": ["ra","dec"]}
                     )
```

### Comparing `skysurvey-0.6.0/skysurvey/target/stars.py` & `skysurvey-0.7.1/skysurvey/target/stars.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.6.0/skysurvey/target/timeserie.py` & `skysurvey-0.7.1/skysurvey/target/timeserie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from .core import Transient
-
+from ..tools.utils import random_radec
 __all__ = ["TSTransient"]
 
 class TSTransient( Transient ):
     """ TimeSerie Transient.
 
     This model will generate a Transient object from
     any TimeSerieSource model from sncosmo.
@@ -30,15 +30,15 @@
                              "kwargs": {"z":"@z", "magabs": "@magabs"}
                             },
                                
                    amplitude = {"func": "magobs_to_amplitude",
                                 "kwargs": {"magobs": "@magobs"}
                             },
                    # This you need to match with the survey
-                   radec = {"func": "random",
+                   radec = {"func": random_radec,
                             "as": ["ra","dec"]
                             }
                  )
     
     @classmethod
     def from_sncosmo(cls, source, rate=1e3, model=None,
                                 magabs=None, magscatter=None):
```

### Comparing `skysurvey-0.6.0/skysurvey/template.py` & `skysurvey-0.7.1/skysurvey/template.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.6.0/skysurvey.egg-info/PKG-INFO` & `skysurvey-0.7.1/skysurvey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skysurvey
-Version: 0.6.0
+Version: 0.7.1
 Summary: Simulating Transient in the sky and how to observe them
 Home-page: https://github.com/MickaelRigault/skysurvey
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `skysurvey-0.6.0/skysurvey.egg-info/SOURCES.txt` & `skysurvey-0.7.1/skysurvey.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 skysurvey/__init__.py
 skysurvey/config.py
-skysurvey/dag.py
 skysurvey/dataset.py
 skysurvey/template.py
 skysurvey.egg-info/PKG-INFO
 skysurvey.egg-info/SOURCES.txt
 skysurvey.egg-info/dependency_links.txt
 skysurvey.egg-info/not-zip-safe
 skysurvey.egg-info/requires.txt
 skysurvey.egg-info/top_level.txt
+skysurvey/examples/__init__.py
+skysurvey/examples/mocksurvey.py
 skysurvey/survey/__init__.py
 skysurvey/survey/core.py
+skysurvey/survey/des.py
 skysurvey/survey/healpix.py
+skysurvey/survey/lsst.py
 skysurvey/survey/polygon.py
+skysurvey/survey/survey.py
 skysurvey/survey/ztf.py
 skysurvey/target/__init__.py
 skysurvey/target/collection.py
 skysurvey/target/core.py
 skysurvey/target/environments.py
 skysurvey/target/kilonova.py
 skysurvey/target/sncc.py
 skysurvey/target/snia.py
 skysurvey/target/stars.py
-skysurvey/target/timeserie.py
+skysurvey/target/timeserie.py
+skysurvey/tools/__init__.py
+skysurvey/tools/snana.py
+skysurvey/tools/utils.py
```

