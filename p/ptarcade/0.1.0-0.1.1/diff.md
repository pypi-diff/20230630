# Comparing `tmp/ptarcade-0.1.0.tar.gz` & `tmp/ptarcade-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptarcade-0.1.0.tar", max compression
+gzip compressed data, was "ptarcade-0.1.1.tar", max compression
```

## Comparing `ptarcade-0.1.0.tar` & `ptarcade-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      448 2023-06-29 05:38:20.259917 ptarcade-0.1.0/README.md
--rw-r--r--   0        0        0     3313 2023-06-29 05:49:51.982661 ptarcade-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      555 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/__init__.py
--rw-r--r--   0        0        0    32466 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/chains_utils.py
--rw-r--r--   0        0        0       23 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/data/__init__.py
--rw-r--r--   0        0        0     1026 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/data/default_config.py
--rw-r--r--   0        0        0    29964 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/data/g_star.dat
--rw-r--r--   0        0        0     4182 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/fast_interpolate.py
--rw-r--r--   0        0        0    15036 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/input_handler.py
--rw-r--r--   0        0        0    17354 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/models_utils.py
--rw-r--r--   0        0        0    30151 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/plot_utils.py
--rw-r--r--   0        0        0     6906 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/pta_importer.py
--rw-r--r--   0        0        0    11573 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/sampler.py
--rw-r--r--   0        0        0    15944 2023-06-29 05:37:13.771628 ptarcade-0.1.0/src/ptarcade/signal_builder.py
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 ptarcade-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      673 2023-06-29 23:09:28.232412 ptarcade-0.1.1/README.md
+-rw-r--r--   0        0        0     3313 2023-06-29 23:25:57.055952 ptarcade-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/__init__.py
+-rw-r--r--   0        0        0    32466 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/chains_utils.py
+-rw-r--r--   0        0        0       23 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/data/__init__.py
+-rw-r--r--   0        0        0     1026 2023-06-29 23:54:55.629319 ptarcade-0.1.1/src/ptarcade/data/default_config.py
+-rw-r--r--   0        0        0    29964 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/data/g_star.dat
+-rw-r--r--   0        0        0     4182 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/fast_interpolate.py
+-rw-r--r--   0        0        0    15036 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/input_handler.py
+-rw-r--r--   0        0        0    17354 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/models_utils.py
+-rw-r--r--   0        0        0    30151 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/plot_utils.py
+-rw-r--r--   0        0        0     6906 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/pta_importer.py
+-rw-r--r--   0        0        0    11573 2023-06-29 23:54:58.423893 ptarcade-0.1.1/src/ptarcade/sampler.py
+-rw-r--r--   0        0        0    16501 2023-06-29 23:28:26.999901 ptarcade-0.1.1/src/ptarcade/signal_builder.py
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ptarcade-0.1.1/PKG-INFO
```

### Comparing `ptarcade-0.1.0/pyproject.toml` & `ptarcade-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
   "doc/build/*.py",
   "doc/temp/*.py",
   ".eggs/*.py",
 ]
 
 [tool.poetry]
 name = "PTArcade"
-version = "0.1.0"
+version = "0.1.1"
 description = "PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data."
 readme = "README.md"
 authors = ["Andrea Mitridate <andrea.mitridate@nanograv.org>",]
 keywords = ["ptarcade"]
 repository = "https://github.com/andrea-mitridate/PTArcade"
 documentation = "https://andrea-mitridate.github.io/PTArcade/"
 classifiers = [
```

### Comparing `ptarcade-0.1.0/src/ptarcade/__init__.py` & `ptarcade-0.1.1/src/ptarcade/__init__.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/chains_utils.py` & `ptarcade-0.1.1/src/ptarcade/chains_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/data/default_config.py` & `ptarcade-0.1.1/src/ptarcade/data/default_config.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/data/g_star.dat` & `ptarcade-0.1.1/src/ptarcade/data/g_star.dat`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/fast_interpolate.py` & `ptarcade-0.1.1/src/ptarcade/fast_interpolate.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/input_handler.py` & `ptarcade-0.1.1/src/ptarcade/input_handler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/models_utils.py` & `ptarcade-0.1.1/src/ptarcade/models_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/plot_utils.py` & `ptarcade-0.1.1/src/ptarcade/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/pta_importer.py` & `ptarcade-0.1.1/src/ptarcade/pta_importer.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/sampler.py` & `ptarcade-0.1.1/src/ptarcade/sampler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.0/src/ptarcade/signal_builder.py` & `ptarcade-0.1.1/src/ptarcade/signal_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -425,34 +425,51 @@
 
         if inputs["config"].corr:
             pass
         else:
             pass
 
     elif inputs["config"].pta_data == "NG12":
-        log.error("The 12yr data needed for ceffyl is [bold red]not yet[/] publicly available.\n"
-                  "We will update PTArcade in tandem with its release.\n"
-                  "At the moment, only IPTA2 is supported in ceffyl mode.\n",
-                  extra={"markup":True})
-        raise SystemExit
+        # download from zenodo
+        ceffyldl = download_file(
+            "https://zenodo.org/record/8096699/files/ng12p5_ceffyl.zip?download=1",
+            cache=True,
+            pkgname="ptarcade",
+            )
+        # make a Path object for ease of use
+        ceffyldl = Path(ceffyldl)
+
+        # Check if we've unzipped or not
+        # If not, unzip and name the same as the original download so that astropy can find it again
+        if ceffyldl.is_file():
+            tempdir = (ceffyldl.parent / "temp")
+            # extract
+            with ZipFile(ceffyldl) as zf:
+                zf.extractall(tempdir)
+            # delete original zip
+            ceffyldl.unlink()
+            # rename unzipped dir to original zip name
+            tempdir.rename(ceffyldl)
+        # find ipta data inside dir
+        datadir = (ceffyldl / "ng12p5_ceffyl")
 
     ceffyl_pta = Ceffyl.ceffyl(datadir)
 
     params = list(inputs["model"].parameters.values())
 
     model = []
 
     model.append(Ceffyl.signal(N_freqs=inputs["config"].gwb_components,
                           psd=aux.omega2cross(inputs["model"].spectrum, ceffyl=True),  
                           params=params,
                           name=''))
     
     
     if inputs["model"].smbhb:
-        mu, sigma = bhb_priors.get(inputs["config"].pta_data, [False, False])
+        mu, sigma = bhb_priors.get(inputs["config"].pta_data, np.array([False, False]))
 
         if mu.all() and inputs["config"].bhb_th_prior:
             bhb_params = [parameter.Normal(mu=mu, sigma=sigma, size=2)("gw_bhb")]
             bhb_signal = powerlaw2_ceffyl
 
         else:
             if inputs["config"].A_bhb_logmin:
```

### Comparing `ptarcade-0.1.0/PKG-INFO` & `ptarcade-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptarcade
-Version: 0.1.0
+Version: 0.1.1
 Summary: PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data.
 Home-page: https://github.com/andrea-mitridate/PTArcade
 Keywords: ptarcade
 Author: Andrea Mitridate
 Author-email: andrea.mitridate@nanograv.org
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Developers
@@ -39,14 +39,16 @@
 Requires-Dist: tables (>=3.8.0,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/andrea-mitridate/PTArcade/issues
 Project-URL: Documentation, https://andrea-mitridate.github.io/PTArcade/
 Project-URL: Repository, https://github.com/andrea-mitridate/PTArcade
 Description-Content-Type: text/markdown
 
 # PTArcade
+[![PyPI version](https://badge.fury.io/py/ptarcade.svg)](https://badge.fury.io/py/ptarcade) [<img src="https://img.shields.io/badge/dockerhub-ptarcade-important.svg?logo=Docker">](https://hub.docker.com/r/ngnewphy/ptarcade)
+
 
 PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data. 
 
 The user can specify a new physics signal (either deterministic or stochastic), and the code will output Monte Carlo chains that can be used to reconstruct the model's parameter posterior distributions. 
 
 Please see our detailed documentation [here](https://andrea-mitridate.github.io/PTArcade/)
```

