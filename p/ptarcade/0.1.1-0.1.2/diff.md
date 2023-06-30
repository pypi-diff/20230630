# Comparing `tmp/ptarcade-0.1.1.tar.gz` & `tmp/ptarcade-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptarcade-0.1.1.tar", max compression
+gzip compressed data, was "ptarcade-0.1.2.tar", max compression
```

## Comparing `ptarcade-0.1.1.tar` & `ptarcade-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      673 2023-06-29 23:09:28.232412 ptarcade-0.1.1/README.md
--rw-r--r--   0        0        0     3313 2023-06-29 23:25:57.055952 ptarcade-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      555 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/__init__.py
--rw-r--r--   0        0        0    32466 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/chains_utils.py
--rw-r--r--   0        0        0       23 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/data/__init__.py
--rw-r--r--   0        0        0     1026 2023-06-29 23:54:55.629319 ptarcade-0.1.1/src/ptarcade/data/default_config.py
--rw-r--r--   0        0        0    29964 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/data/g_star.dat
--rw-r--r--   0        0        0     4182 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/fast_interpolate.py
--rw-r--r--   0        0        0    15036 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/input_handler.py
--rw-r--r--   0        0        0    17354 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/models_utils.py
--rw-r--r--   0        0        0    30151 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/plot_utils.py
--rw-r--r--   0        0        0     6906 2023-06-29 05:37:13.771628 ptarcade-0.1.1/src/ptarcade/pta_importer.py
--rw-r--r--   0        0        0    11573 2023-06-29 23:54:58.423893 ptarcade-0.1.1/src/ptarcade/sampler.py
--rw-r--r--   0        0        0    16501 2023-06-29 23:28:26.999901 ptarcade-0.1.1/src/ptarcade/signal_builder.py
--rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ptarcade-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      673 2023-06-29 23:09:28.232412 ptarcade-0.1.2/README.md
+-rw-r--r--   0        0        0     3313 2023-06-30 21:13:19.488677 ptarcade-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/__init__.py
+-rw-r--r--   0        0        0    32466 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/chains_utils.py
+-rw-r--r--   0        0        0       23 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/data/__init__.py
+-rw-r--r--   0        0        0     1026 2023-06-30 21:13:04.270655 ptarcade-0.1.2/src/ptarcade/data/default_config.py
+-rw-r--r--   0        0        0    29964 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/data/g_star.dat
+-rw-r--r--   0        0        0     4182 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/fast_interpolate.py
+-rw-r--r--   0        0        0    15036 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/input_handler.py
+-rw-r--r--   0        0        0    17354 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/models_utils.py
+-rw-r--r--   0        0        0    30151 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/plot_utils.py
+-rw-r--r--   0        0        0     6885 2023-06-30 21:13:19.488677 ptarcade-0.1.2/src/ptarcade/pta_importer.py
+-rw-r--r--   0        0        0    11573 2023-06-29 23:54:58.423893 ptarcade-0.1.2/src/ptarcade/sampler.py
+-rw-r--r--   0        0        0    18088 2023-06-30 21:26:10.379417 ptarcade-0.1.2/src/ptarcade/signal_builder.py
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ptarcade-0.1.2/PKG-INFO
```

### Comparing `ptarcade-0.1.1/README.md` & `ptarcade-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/pyproject.toml` & `ptarcade-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
   "doc/build/*.py",
   "doc/temp/*.py",
   ".eggs/*.py",
 ]
 
 [tool.poetry]
 name = "PTArcade"
-version = "0.1.1"
+version = "0.1.2"
 description = "PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data."
 readme = "README.md"
 authors = ["Andrea Mitridate <andrea.mitridate@nanograv.org>",]
 keywords = ["ptarcade"]
 repository = "https://github.com/andrea-mitridate/PTArcade"
 documentation = "https://andrea-mitridate.github.io/PTArcade/"
 classifiers = [
```

### Comparing `ptarcade-0.1.1/src/ptarcade/__init__.py` & `ptarcade-0.1.2/src/ptarcade/__init__.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/src/ptarcade/chains_utils.py` & `ptarcade-0.1.2/src/ptarcade/chains_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/src/ptarcade/data/default_config.py` & `ptarcade-0.1.2/src/ptarcade/data/default_config.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/src/ptarcade/data/g_star.dat` & `ptarcade-0.1.2/src/ptarcade/data/g_star.dat`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/src/ptarcade/fast_interpolate.py` & `ptarcade-0.1.2/src/ptarcade/fast_interpolate.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/src/ptarcade/input_handler.py` & `ptarcade-0.1.2/src/ptarcade/input_handler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/src/ptarcade/models_utils.py` & `ptarcade-0.1.2/src/ptarcade/models_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/src/ptarcade/plot_utils.py` & `ptarcade-0.1.2/src/ptarcade/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/src/ptarcade/pta_importer.py` & `ptarcade-0.1.2/src/ptarcade/pta_importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,28 +158,32 @@
         If `pta_data` is not str or dict.
 
     """
     if pta_data == "NG15":
         # This returns a path in the astropy cache that points to these files, otherwise
         # it downloads them there and returns the path
 
-        # Temporarily issue error msg and quit if user asks for NG15
-        log.error("The 15yr data is [bold red]not yet[/] publicly available.\n"
-                  "We will update PTArcade in tandem with its release.\n", extra={"markup":True})
-        raise SystemExit
-
         ng15_dic = {
             "psrs_data": download_file(
-                "http://0.0.0.0/ng15_psrs_v1p1.pkl.gz", show_progress=True, cache=True, pkgname="ptarcade",
+                "https://zenodo.org/record/8102748/files/ng15_psrs_v1p1.pkl.gz?download=1",
+                show_progress=True,
+                cache=True,
+                pkgname="ptarcade",
             ),
             "noise_data": download_file(
-                "http://0.0.0.0/ng15_wn_v1p1.json", show_progress=True, cache=True, pkgname="ptarcade",
+                "https://zenodo.org/record/8102748/files/ng15_wn_v1p1.json?download=1",
+                show_progress=True,
+                cache=True,
+                pkgname="ptarcade",
             ),
             "emp_dist": download_file(
-                "http://0.0.0.0/ng15_emp_v1p1.pkl", show_progress=True, cache=True, pkgname="ptarcade",
+                "https://zenodo.org/record/8102748/files/ng15_emp_v1p1.pkl?download=1",
+                show_progress=True,
+                cache=True,
+                pkgname="ptarcade",
             ),
         }
 
         psrs = get_pulsars(ng15_dic["psrs_data"])
         params = get_wn(ng15_dic["noise_data"])
         emp_dist = ng15_dic["emp_dist"]
```

### Comparing `ptarcade-0.1.1/src/ptarcade/sampler.py` & `ptarcade-0.1.2/src/ptarcade/sampler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.1/src/ptarcade/signal_builder.py` & `ptarcade-0.1.2/src/ptarcade/signal_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -413,24 +413,62 @@
             # rename unzipped dir to original zip name
             tempdir.rename(ceffyldl)
         # find ipta data inside dir
         datadir = (ceffyldl / "ipta-dr2_fftkde_10k[94]_epa_sj")
 
 
     elif inputs["config"].pta_data == "NG15":
-        log.error("The 15yr data is [bold red]not yet[/] publicly available.\n"
-                  "We will update PTArcade in tandem with its release.\n"
-                  "At the moment, only IPTA2 is supported in ceffyl mode.\n",
-                  extra={"markup":True})
-        raise SystemExit
 
         if inputs["config"].corr:
-            pass
+            # download from zenodo
+            ceffyldl = download_file(
+                "https://zenodo.org/record/8102748/files/30f_fs%7Bhd%7D_ceffyl.zip?download=1",
+                cache=True,
+                pkgname="ptarcade",
+                )
+            # make a Path object for ease of use
+            ceffyldl = Path(ceffyldl)
+
+            # Check if we've unzipped or not
+            # If not, unzip and name the same as the original download so that astropy can find it again
+            if ceffyldl.is_file():
+                tempdir = (ceffyldl.parent / "temp")
+                # extract
+                with ZipFile(ceffyldl) as zf:
+                    zf.extractall(tempdir)
+                # delete original zip
+                ceffyldl.unlink()
+                # rename unzipped dir to original zip name
+                tempdir.rename(ceffyldl)
+            # find ipta data inside dir
+            datadir = (ceffyldl / "30f_fs{hd}_ceffyl")
         else:
-            pass
+
+            # download from zenodo
+            ceffyldl = download_file(
+                "https://zenodo.org/record/8102748/files/30f_fs%7Bcp%7D_ceffyl.zip?download=1",
+                cache=True,
+                pkgname="ptarcade",
+                )
+            # make a Path object for ease of use
+            ceffyldl = Path(ceffyldl)
+
+            # Check if we've unzipped or not
+            # If not, unzip and name the same as the original download so that astropy can find it again
+            if ceffyldl.is_file():
+                tempdir = (ceffyldl.parent / "temp")
+                # extract
+                with ZipFile(ceffyldl) as zf:
+                    zf.extractall(tempdir)
+                # delete original zip
+                ceffyldl.unlink()
+                # rename unzipped dir to original zip name
+                tempdir.rename(ceffyldl)
+            # find ipta data inside dir
+            datadir = (ceffyldl / "30f_fs{cp}_ceffyl")
 
     elif inputs["config"].pta_data == "NG12":
         # download from zenodo
         ceffyldl = download_file(
             "https://zenodo.org/record/8096699/files/ng12p5_ceffyl.zip?download=1",
             cache=True,
             pkgname="ptarcade",
```

### Comparing `ptarcade-0.1.1/PKG-INFO` & `ptarcade-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptarcade
-Version: 0.1.1
+Version: 0.1.2
 Summary: PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data.
 Home-page: https://github.com/andrea-mitridate/PTArcade
 Keywords: ptarcade
 Author: Andrea Mitridate
 Author-email: andrea.mitridate@nanograv.org
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Developers
```

