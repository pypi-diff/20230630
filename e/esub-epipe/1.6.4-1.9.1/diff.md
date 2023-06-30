# Comparing `tmp/esub-epipe-1.6.4.tar.gz` & `tmp/esub-epipe-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esub-epipe-1.6.4.tar", last modified: Wed Jun 24 05:56:30 2020, max compression
+gzip compressed data, was "esub-epipe-1.9.1.tar", last modified: Fri Jun  3 10:26:35 2022, max compression
```

## Comparing `esub-epipe-1.6.4.tar` & `esub-epipe-1.9.1.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2020-06-24 05:56:30.896273 esub-epipe-1.6.4/
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)      244 2020-06-16 10:17:30.000000 esub-epipe-1.6.4/AUTHORS.rst
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)     1560 2020-06-16 10:17:30.000000 esub-epipe-1.6.4/CONTRIBUTING.rst
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)       97 2020-06-24 05:56:16.000000 esub-epipe-1.6.4/HISTORY.rst
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)     1115 2020-06-16 10:17:30.000000 esub-epipe-1.6.4/LICENSE
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)      100 2020-06-16 10:17:30.000000 esub-epipe-1.6.4/MANIFEST.in
--rw-r--r--   0 dominik   (1000) dominik   (1000)     4153 2020-06-24 05:56:30.896273 esub-epipe-1.6.4/PKG-INFO
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)     3024 2020-06-24 05:56:07.000000 esub-epipe-1.6.4/README.rst
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2020-06-24 05:56:30.876273 esub-epipe-1.6.4/esub/
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)      276 2020-06-16 10:17:30.000000 esub-epipe-1.6.4/esub/__init__.py
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)    11116 2020-06-18 07:52:56.000000 esub-epipe-1.6.4/esub/epipe.py
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)    17551 2020-06-18 11:38:40.000000 esub-epipe-1.6.4/esub/esub.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2020-06-24 05:56:30.886273 esub-epipe-1.6.4/esub/scripts/
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2020-06-16 10:17:30.000000 esub-epipe-1.6.4/esub/scripts/__init__.py
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)     2375 2020-06-18 08:05:27.000000 esub-epipe-1.6.4/esub/scripts/check_logs.py
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)     2376 2020-06-18 08:04:40.000000 esub-epipe-1.6.4/esub/scripts/send_cmd.py
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)     9234 2020-06-23 12:18:29.000000 esub-epipe-1.6.4/esub/submit_jobarray.py
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)     2071 2020-06-23 12:18:34.000000 esub-epipe-1.6.4/esub/submit_mpi.py
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)    27786 2020-06-18 11:35:59.000000 esub-epipe-1.6.4/esub/utils.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2020-06-24 05:56:30.889606 esub-epipe-1.6.4/esub_epipe.egg-info/
--rw-r--r--   0 dominik   (1000) dominik   (1000)     4153 2020-06-24 05:56:30.000000 esub-epipe-1.6.4/esub_epipe.egg-info/PKG-INFO
--rw-r--r--   0 dominik   (1000) dominik   (1000)      597 2020-06-24 05:56:30.000000 esub-epipe-1.6.4/esub_epipe.egg-info/SOURCES.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)        1 2020-06-24 05:56:30.000000 esub-epipe-1.6.4/esub_epipe.egg-info/dependency_links.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)       65 2020-06-24 05:56:30.000000 esub-epipe-1.6.4/esub_epipe.egg-info/entry_points.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)        1 2020-06-24 05:56:30.000000 esub-epipe-1.6.4/esub_epipe.egg-info/not-zip-safe
--rw-r--r--   0 dominik   (1000) dominik   (1000)       39 2020-06-24 05:56:30.000000 esub-epipe-1.6.4/esub_epipe.egg-info/requires.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)       11 2020-06-24 05:56:30.000000 esub-epipe-1.6.4/esub_epipe.egg-info/top_level.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)       38 2020-06-24 05:56:30.896273 esub-epipe-1.6.4/setup.cfg
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)     1340 2020-06-18 07:22:45.000000 esub-epipe-1.6.4/setup.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2020-06-24 05:56:30.896273 esub-epipe-1.6.4/tests/
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2020-06-16 10:17:30.000000 esub-epipe-1.6.4/tests/__init__.py
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)      987 2020-06-16 10:17:30.000000 esub-epipe-1.6.4/tests/test_epipe.py
--rwxr-xr-x   0 dominik   (1000) dominik   (1000)     5048 2020-06-18 08:10:49.000000 esub-epipe-1.6.4/tests/test_esub.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2964 2020-06-18 07:37:43.000000 esub-epipe-1.6.4/tests/test_scripts.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2839 2020-06-18 08:17:05.000000 esub-epipe-1.6.4/tests/test_submit.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-06-03 10:26:35.239106 esub-epipe-1.9.1/
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)      244 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/AUTHORS.rst
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)     1560 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/CONTRIBUTING.rst
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)      580 2022-06-03 10:22:47.000000 esub-epipe-1.9.1/HISTORY.rst
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)     1115 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/LICENSE
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)      100 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/MANIFEST.in
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     3780 2022-06-03 10:26:35.239106 esub-epipe-1.9.1/PKG-INFO
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)     3175 2022-06-03 10:21:42.000000 esub-epipe-1.9.1/README.rst
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-06-03 10:26:35.235772 esub-epipe-1.9.1/esub/
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)      276 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/esub/__init__.py
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)    11966 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/esub/epipe.py
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)    24586 2022-05-19 05:56:39.000000 esub-epipe-1.9.1/esub/esub.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-06-03 10:26:35.235772 esub-epipe-1.9.1/esub/scripts/
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/esub/scripts/__init__.py
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)     2269 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/esub/scripts/check_logs.py
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)     2306 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/esub/scripts/send_cmd.py
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)    11490 2022-06-03 10:21:17.000000 esub-epipe-1.9.1/esub/submit.py
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)    36356 2022-05-19 05:47:04.000000 esub-epipe-1.9.1/esub/utils.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-06-03 10:26:35.235772 esub-epipe-1.9.1/esub_epipe.egg-info/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     3780 2022-06-03 10:26:34.000000 esub-epipe-1.9.1/esub_epipe.egg-info/PKG-INFO
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      573 2022-06-03 10:26:35.000000 esub-epipe-1.9.1/esub_epipe.egg-info/SOURCES.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)        1 2022-06-03 10:26:34.000000 esub-epipe-1.9.1/esub_epipe.egg-info/dependency_links.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)       64 2022-06-03 10:26:34.000000 esub-epipe-1.9.1/esub_epipe.egg-info/entry_points.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)        1 2022-06-03 10:26:34.000000 esub-epipe-1.9.1/esub_epipe.egg-info/not-zip-safe
+-rw-r--r--   0 dominik   (1000) dominik   (1000)       39 2022-06-03 10:26:35.000000 esub-epipe-1.9.1/esub_epipe.egg-info/requires.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)       11 2022-06-03 10:26:35.000000 esub-epipe-1.9.1/esub_epipe.egg-info/top_level.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)       38 2022-06-03 10:26:35.239106 esub-epipe-1.9.1/setup.cfg
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)     1335 2022-06-03 10:22:19.000000 esub-epipe-1.9.1/setup.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-06-03 10:26:35.235772 esub-epipe-1.9.1/tests/
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/tests/__init__.py
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)      962 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/tests/test_epipe.py
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)     6631 2022-05-19 05:47:04.000000 esub-epipe-1.9.1/tests/test_esub.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     3202 2022-05-19 05:47:04.000000 esub-epipe-1.9.1/tests/test_esub_slurm.py
+-rwxr-xr-x   0 dominik   (1000) dominik   (1000)     2964 2022-04-26 07:39:22.000000 esub-epipe-1.9.1/tests/test_scripts.py
```

### Comparing `esub-epipe-1.6.4/CONTRIBUTING.rst` & `esub-epipe-1.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `esub-epipe-1.6.4/LICENSE` & `esub-epipe-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esub-epipe-1.6.4/PKG-INFO` & `esub-epipe-1.9.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,86 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: esub-epipe
-Version: 1.6.4
+Version: 1.9.1
 Summary: Easy-to-use job Scheduler for Python code
-Home-page: https://cosmo-docs.phys.ethz.ch/esub-epipe
+Home-page: https://cosmo-docs.phys.ethz.ch/esub
 Author: Dominik Zuercher
 Author-email: dominik.zuercher@phys.ethz.ch
 License: MIT License
-Description: =================================
-        esub-epipe - Version 1.6.4 STABLE
-        =================================
-        
-        .. image:: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe/badges/master/coverage.svg
-          		:target: https://cosmo-gitlab.phys.ethz.ch/esub-epipe/NGSF
-        
-        .. image:: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe/badges/master/pipeline.svg
-                :target: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe
-        
-        
-        .. image:: http://img.shields.io/badge/arXiv-2006.12506-orange.svg?style=flat
-                :target: https://arxiv.org/abs/2006.12506
-        
-        
-        
-        esub-epipe is part of the Non-Gaussian Statistics Framework (`NGSF <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/NGSF>`_).
-        
-        If you use this package in your research please cite Zuercher et al. 2020. (`arXiv-2006.12506 <https://arxiv.org/abs/2006.12506>`_).
-        
-        `Source <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe>`_
-        
-        `Documentation <http://cosmo-docs.phys.ethz.ch/esub-epipe>`_
-        
-        Introduction
-        ============
-        
-        - Are you tired of rewriting the same kind of submission scripts to sumbit your code to a computer cluster?
-        
-        - Do you not want to rewrite different versions of your code for serial, parallel or MPI execution?
-        
-        - Do you wish there would be an easy way to submit large numbers of dependent jobs to a computer cluster without writing the same kind of pipeline scripts and worrying about resource allocation every time?
-        
-        If any of these points applies to you, you have come to the right place!
-        
-        When using this package you will only need to write a single python executable file. The same file can then be used to run your code
-        serially, in parallel or in an MPI environement on your local machine. You can also use the same file to submit your code to a
-        computer cluster.
-        
-        Even more, if you are building large pipelines with many dependent jobs, or even tasks which have to be executed multiple times
-        you will just have to write a single YAML file in which you state what you want to run and esub will submit all those
-        jobs to the computer cluster such that you can continue working on your amazing projects while waiting for the results :)
-        
-        Getting Started
-        ===============
-        
-        The easiest and fastest way to learn about esub is to have a look at the Examples Section in the documentation.
-        If you wish to learn more also have a look at the Usage Section in the documenation in which we documented all the things you can do with esub.
-        
-        Disclaimer
-        ==========
-        
-        At the moment only IBMs bsub system is supported but we hope to include other queing systems in the future.
-        
-        Credits
-        =======
-        
-        This package was created on May 12 2019 by Dominik Zuercher (PhD student at ETH Zurich in Alexandre Refregiers `Comsology Research Group <https://cosmology.ethz.ch/>`_)
-        It is inspired by the jobchainer code written by Tomasz Kacprzak.
-        
-        The package is maintained by Dominik Zuercher dominik.zuercher@phys.ethz.ch.
-        
-        Contributing
-        ============
-        
-        Contributions are welcome, and they are greatly appreciated! Every
-        little bit helps, and credit will always be given.
-        
 Keywords: esub,epipe
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+==================================
+esub-epipe - Version 1.9.1 STABLE
+==================================
+
+.. image:: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe/badges/master/pipeline.svg
+        :target: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe
+
+
+.. image:: http://img.shields.io/badge/arXiv-2006.12506-orange.svg?style=flat
+        :target: https://arxiv.org/abs/2006.12506
+
+.. image:: http://img.shields.io/badge/arXiv-2110.10135-orange.svg?style=flat
+        :target: https://arxiv.org/abs/arXiv:2110.10135
+
+
+
+esub-epipe is part of the Non-Gaussian Statistics Framework (`NGSF <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/NGSF>`_).
+
+If you use this package in your research please cite Zuercher et al. 2020 (`arXiv-2006.12506 <https://arxiv.org/abs/2006.12506>`_)
+and Zuercher et al. 2021 (`arXiv-2110.10135 <https://arxiv.org/abs/2110.10135>`_).
+
+`Source <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe>`_
+
+`Documentation <http://cosmo-docs.phys.ethz.ch/esub>`_
+
+Introduction
+============
+
+- Are you tired of rewriting the same kind of submission scripts to sumbit your code to a computer cluster?
+
+- Do you not want to rewrite different versions of your code for serial, parallel or MPI execution, but instead use the same executable everytime?
+
+- Do you wish there would be an easy way to submit large numbers of dependent jobs to a computer cluster without writing the same kind of pipeline scripts and worrying about resource allocation every time?
+
+If any of these points applies to you, you have come to the right place :)
+
+When using this package you will only need to write a single python executable file. The same file can then be used to run your code
+serially, in parallel or in an MPI environement on your local machine. You can also use the same file to submit your code to a
+computer cluster that runs IBMs LSF system or SLURM (experimental).
+
+Even more, if you are building large pipelines with many dependent jobs, or even tasks which have to be executed multiple times
+you will just have to write a single YAML file in which you state what you want to run and esub will submit all those
+jobs to the computer cluster such that you can continue working on your amazing projects while waiting for the results :)
+
+Getting Started
+===============
+
+The easiest and fastest way to learn about esub is to have a look at the Examples Section in the documentation.
+If you wish to learn more also have a look at the Usage Section in the documenation in which we documented all the things you can do with esub.
+
+Disclaimer
+==========
+
+At the moment only IBMs bsub system is supported but we hope to include other queing systems in the future.
+
+Credits
+=======
+
+This package was created on May 12 2019 by Dominik Zuercher (PhD student at ETH Zurich in Alexandre Refregiers `Comsology Research Group <https://cosmology.ethz.ch/>`_)
+It is inspired by the jobchainer code written by Tomasz Kacprzak.
+
+The package is maintained by Dominik Zuercher dominik.zuercher@phys.ethz.ch.
+
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every
+little bit helps, and credit will always be given.
```

### Comparing `esub-epipe-1.6.4/README.rst` & `esub-epipe-1.9.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-=================================
-esub-epipe - Version 1.6.4 STABLE
-=================================
-
-.. image:: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe/badges/master/coverage.svg
-  		:target: https://cosmo-gitlab.phys.ethz.ch/esub-epipe/NGSF
+==================================
+esub-epipe - Version 1.9.1 STABLE
+==================================
 
 .. image:: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe/badges/master/pipeline.svg
         :target: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe
 
 
 .. image:: http://img.shields.io/badge/arXiv-2006.12506-orange.svg?style=flat
         :target: https://arxiv.org/abs/2006.12506
 
+.. image:: http://img.shields.io/badge/arXiv-2110.10135-orange.svg?style=flat
+        :target: https://arxiv.org/abs/arXiv:2110.10135
+
 
 
 esub-epipe is part of the Non-Gaussian Statistics Framework (`NGSF <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/NGSF>`_).
 
-If you use this package in your research please cite Zuercher et al. 2020. (`arXiv-2006.12506 <https://arxiv.org/abs/2006.12506>`_).
+If you use this package in your research please cite Zuercher et al. 2020 (`arXiv-2006.12506 <https://arxiv.org/abs/2006.12506>`_)
+and Zuercher et al. 2021 (`arXiv-2110.10135 <https://arxiv.org/abs/2110.10135>`_).
 
 `Source <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe>`_
 
-`Documentation <http://cosmo-docs.phys.ethz.ch/esub-epipe>`_
+`Documentation <http://cosmo-docs.phys.ethz.ch/esub>`_
 
 Introduction
 ============
 
 - Are you tired of rewriting the same kind of submission scripts to sumbit your code to a computer cluster?
 
-- Do you not want to rewrite different versions of your code for serial, parallel or MPI execution?
+- Do you not want to rewrite different versions of your code for serial, parallel or MPI execution, but instead use the same executable everytime?
 
 - Do you wish there would be an easy way to submit large numbers of dependent jobs to a computer cluster without writing the same kind of pipeline scripts and worrying about resource allocation every time?
 
-If any of these points applies to you, you have come to the right place!
+If any of these points applies to you, you have come to the right place :)
 
 When using this package you will only need to write a single python executable file. The same file can then be used to run your code
 serially, in parallel or in an MPI environement on your local machine. You can also use the same file to submit your code to a
-computer cluster.
+computer cluster that runs IBMs LSF system or SLURM (experimental).
 
 Even more, if you are building large pipelines with many dependent jobs, or even tasks which have to be executed multiple times
 you will just have to write a single YAML file in which you state what you want to run and esub will submit all those
 jobs to the computer cluster such that you can continue working on your amazing projects while waiting for the results :)
 
 Getting Started
 ===============
```

### Comparing `esub-epipe-1.6.4/esub/epipe.py` & `esub-epipe-1.9.1/esub/epipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,35 +10,34 @@
 
 # package imports
 import sys
 import argparse
 import subprocess
 import shlex
 import yaml
-from ekit.logger import vprint
 from ekit import logger as logger_utils
 
 from esub import esub
 
 
-LOGGER = logger_utils.init_logger(__file__)
+LOGGER = logger_utils.init_logger(__name__)
 
 
 def starter_message():
-    print()
-    print(' ______   ______   __    ______   ______  ')
-    print('| _____| |   _  | |  |  |   _  | | _____| ')
-    print('| |___   |  |_| | |  |  |  |_| | | |___   ')
-    print('|  ___|  | _____| |  |  | _____| |  ___|  ')
-    print('| |____  | |      |  |  | |      | |____  ')
-    print('|______| |_|      |__|  |_|      |______| ')
-    print()
+    print(' ')
+    print("             _____               ")
+    print("________________(_)____________  ")
+    print("_  _ \\__  __ \\_  /___  __ \\  _ \\ ")
+    print("/  __/_  /_/ /  / __  /_/ /  __/ ")
+    print("\\___/_  .___//_/  _  .___/\\___/  ")
+    print("     /_/          /_/            ")
+    print(' ')
 
 
-def format_loop_cmd(command, index):
+def format_loop_cmd(command, index, entry):
     """
     Inserts a loop index into a command if specified by eg. "{}"
     inside the command. Then evaluates the command
     as an f-string to resolve possible (e.g. mathematical) expressions.
 
     :param command: command string
     :param index: loop index
@@ -54,15 +53,15 @@
         try:
             # if this fails, there are more places where the index
             # should be inserted than we currently have items in
             # the list
             command_formatted = command.format(*index_repeated)
             break
         except IndexError:
-            index_repeated.append(index)
+            index_repeated.append(entry)
 
     # evaluate as f-string
     command_formatted = eval('f"{}"'.format(command_formatted))
 
     return command_formatted
 
 
@@ -97,18 +96,17 @@
     dep_string = ''
     for dep in deps:
         if represents_int(dep):
             job_ids = [dep]
         elif dep in job_dict.keys():
             job_ids = job_dict[dep]
         else:
-            vprint(
+            LOGGER.warning(
                 "Did not find a job named {}. \
-                 Ignoring dependencies on it".format(dep),
-                logger=LOGGER, verbose=True)
+                 Ignoring dependencies on it".format(dep))
             continue
         for job_id in job_ids:
             dep_string += 'ended({}) && '.format(int(job_id))
     dep_string = dep_string[:-4]
     dep_string = '"' + dep_string + '"'
 
     cmd = base_cmd + \
@@ -132,60 +130,57 @@
     which gets added to the dependency list.
 
     :param cmd: Command string to submit
     :param assert_ids: whether to check that job ids were successfully obtained
     :return: The ids of the just submitted jobs
     """
 
-    vprint('Running {}'.format(cmd),
-           logger=LOGGER, verbose=True)
-
     stdout_lines = []
     with subprocess.Popen(shlex.split(cmd),
                           stdout=subprocess.PIPE,
                           stderr=subprocess.PIPE,
                           bufsize=1,
                           universal_newlines=True) as proc:
 
         # read stdout
         for line in proc.stdout:
             stdout_lines.append(line)
 
             if esub.TIMEOUT_MESSAGE in line:
-                vprint(esub.TIMEOUT_MESSAGE,
-                       logger=LOGGER, verbose=True)
+                LOGGER.warning(esub.TIMEOUT_MESSAGE)
+        # read stderr
+        for line in proc.stdout:
+            stdout_lines.append(line)
+
+            if esub.TIMEOUT_MESSAGE in line:
+                LOGGER.warning(esub.TIMEOUT_MESSAGE)
 
         # read stderr
         stderr = '\n'.join(proc.stderr)
 
     # raise an exception in case the process did not terminate successfully
     if proc.returncode != 0:
         raise RuntimeError('Running the command \"{}\" failed with\
-                            exit code {}. Error: \n{}'. format(cmd,
-                                                               proc.returncode,
-                                                               stderr))
+                            exit code {}. Error: \n{}'. format(
+            cmd, proc.returncode, stderr))
 
     # get ids of newly submitted jobs
     last_line = stdout_lines[-1]
 
     ids = []
-    for string in last_line.split(' '):
+    for string in last_line.split('Submitted job ids:')[-1].split(' '):
         try:
             int(string)
             ids.append(string)
         except ValueError:
             pass
 
     if assert_ids:
-        assert len(
-            ids) > 0, 'Something went wrong, did not manage\
-                       to get any job ids from stdout'
-
-    print()
-
+        assert len(ids) > 0, 'Something went wrong, did not manage ' \
+                             'to get any job ids from stdout'
     return ids
 
 
 def get_parameters(step):
     """
     Extracts and stores global variables from the\
     parameter object in epipe file
@@ -198,18 +193,22 @@
     for element in param_list:
         key = list(element.keys())[0]
         parameters[key] = element[key]
 
     parameter_dict = {}
     for par_key in parameters.keys():
         parameter_dict[par_key] = parameters[par_key]
+
+    for key in parameter_dict.keys():
+        LOGGER.debug(f"Setting parameter {key} -> {parameter_dict[key]}")
     return parameter_dict
 
 
-def process_item(step, job_dict, index=-1, loop_dependence=None,
+def process_item(step, job_dict, index=-1, loop_entry=None,
+                 loop_dependence=None,
                  parameters=None, assert_ids=True):
     """
     Processes one of the epipe items in the pipeline
 
     :param step: The job item
     :param job_dict: The previous job id dictionary
     :param index: Loop index if within a loop
@@ -236,32 +235,33 @@
             deps.append(dep)
 
         # if we are inside a loop, then format the
         # loop-internal dependencies as necessary
         if in_loop:
             for ii, dep in enumerate(deps):
                 if not represents_int(dep):
-                    deps[ii] = '{}__{}'.format(dep, index)
+                    deps[ii] = '{}__{}'.format(dep, loop_entry)
 
     # add the global dependencies of the loop
     if loop_dependence is not None:
         for lp in loop_dependence:
             deps.append(lp)
 
     # get the job name and the job command
     job_name = step['name']
     base_cmd = step['cmd']
     if in_loop:
-        job_name = '{}__{}'.format(job_name, index)
-        base_cmd = format_loop_cmd(base_cmd, index)
+        job_name = '{}__{}'.format(job_name, loop_entry)
+        base_cmd = format_loop_cmd(base_cmd, index, loop_entry)
 
     # submit the job
-    vprint('Submitting job {}'.format(job_name),
-           logger=LOGGER, verbose=True)
+    LOGGER.debug(f"Propagating dependencies {deps} to job {job_name}")
+    LOGGER.info('Submitting job {}'.format(job_name))
     cmd = make_submit_command(base_cmd, job_name, deps, job_dict, parameters)
+    print(cmd)
     new_ids = submit(cmd, assert_ids=assert_ids)
     job_dict[job_name] = new_ids
 
 
 def main(args=None):
     """
     epipe main function. Accepts a epipe yaml
@@ -274,65 +274,82 @@
         args = sys.argv[1:]
 
     description = "This is epipe a tool to easily submit\
                    pipelines to a clusters queing system"
     parser = argparse.ArgumentParser(description=description, add_help=True)
     # parse all the submitter arguments
     parser.add_argument('pipeline', type=str, action='store',
-                        help='Path to the pipeline file. Format should be as\
-                              specified in the epipe example. Check\
-                              Documentations')
+                        help='Path to the pipeline file. Format should be as '
+                        'specified in the epipe example. Check '
+                        'documentations')
     parser.add_argument('--ignore_jobid_errors', action='store_true',
-                        help='Switches off check whether ids of submitted\
-                              jobs were successfully obtained, useful for\
-                              testing')
+                        help='Switches off checks checking '
+                        'wheter ids of submitted '
+                        'jobs were successfully obtained, useful for '
+                        'testing')
+    parser.add_argument('--epipe_verbosity', type=int,
+                        default=3, choices=(0, 1, 2, 3, 4),
+                        help='epipe verbosity. From 0-4 with 4 being '
+                        'the most verbose. Default is 3 (info).')
+
     args = parser.parse_args(args)
+    logger_utils.set_logger_level(LOGGER, args.epipe_verbosity)
+
     pipeline = args.pipeline
+    LOGGER.debug(f"Using pipeline in file {pipeline}")
+
     assert_ids = not args.ignore_jobid_errors
 
     # read pipeline file
     with open(pipeline, 'r') as f:
-        pipeline = yaml.load(f)
+        pipeline = yaml.load(f, yaml.FullLoader)
 
     starter_message()
 
     # parse all the jobs and their dependencies from the pipeline string
     job_dict = {}
 
-    vprint('Starting submission \n',
-           logger=LOGGER, verbose=True)
+    LOGGER.info('Starting submission')
 
     parameters = None
 
     for step in pipeline:
+        LOGGER.debug(f"Processing item {step}")
         if 'parameters' in step.keys():
-            vprint("Found parameter object",
-                   logger=LOGGER, verbose=True)
+            LOGGER.debug("Found parameter object")
             parameters = get_parameters(step)
-            vprint("Have set global parameters as {}".format(parameters),
-                   logger=LOGGER, verbose=True)
             continue
 
         if 'loop' in step.keys():
+            LOGGER.debug("Found loop object")
 
-            loop_indices = list(step['loop'])
+            loop_entries = list(step['loop'])
+            if len(loop_entries) == 2:
+                if isinstance(loop_entries[0], int) & isinstance(
+                   loop_entries[1], int):
+                    LOGGER.warning(
+                        "Loop object has structure "
+                        "[int1, int2] -> Intrepreting as a range!")
+                    loop_entries = [x for x in range(
+                        loop_entries[0], loop_entries[1])]
+            LOGGER.info(f"Submitting loop indices {loop_entries}")
             deps = []
             # get the names of all jobs that have been
             # submitted before the loop
             submitted_jobs = set(job_dict.keys())
 
             if 'dep' in step.keys():
                 step['dep'] = str(step['dep'])
                 dependencies = step['dep'].replace(' ', '').split(',')
                 for dep in dependencies:
                     deps.append(dep)
 
-            for index in range(loop_indices[0], loop_indices[1]):
+            for index, entry in enumerate(loop_entries):
                 for item in step['items']:
-                    process_item(item, job_dict, index=index,
+                    process_item(item, job_dict, index=index, loop_entry=entry,
                                  loop_dependence=deps, parameters=parameters,
                                  assert_ids=assert_ids)
 
             # find the names of the newly submitted jobs
             loop_jobs = set(job_dict.keys()) - submitted_jobs
 
             # add the loop as a whole to the job dictionary
@@ -340,13 +357,12 @@
             for loop_job in loop_jobs:
                 job_dict[step['name']] += job_dict[loop_job]
 
         else:
             process_item(step, job_dict, parameters=parameters,
                          assert_ids=assert_ids)
 
-    vprint('Submission finished',
-           logger=LOGGER, verbose=True)
+    LOGGER.info('Submission finished')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `esub-epipe-1.6.4/esub/esub.py` & `esub-epipe-1.9.1/esub/esub.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,404 +11,544 @@
 # package import
 import argparse
 import math
 import os
 import sys
 import collections
 from esub import utils
-from ekit.logger import vprint
 from ekit import logger as logger_utils
 
 
-LOGGER = logger_utils.init_logger(__file__)
+LOGGER = logger_utils.init_logger(__name__)
 TIMEOUT_MESSAGE = 'Maximum number of pending jobs reached, ' \
                   'will sleep for 30 minutes and retry'
 
 
 def starter_message():
-    print()
-    print(' ______   _______   _    _   _______ ')
-    print('|  ____| |  _____| | |  | | |  _    |')
-    print('| |___   | |_____  | |  | | | |_|  _|')
-    print('|  ___|  |_____  | | |  | | |  _  |_ ')
-    print('| |____   _____| | | |__| | | |_|   |')
-    print('|______| |_______| \\______/ |_______|')
-    print()
+    print(' ')
+    print("                   ______   ")
+    print("________________  ____  /_  ")
+    print("_  _ \\_  ___/  / / /_  __ \\ ")
+    print("/  __/(__  )/ /_/ /_  /_/ / ")
+    print("\\___//____/ \\__,_/ /_.___/  ")
+    print(' ')
 
 
 def main(args=None):
     """
     Main function of esub.
 
-    :param args: Command line arguments are parsed
+    :param args: Command line arguments that are parsed
     """
 
     if args is None:
         args = sys.argv[1:]
 
-    # Make log directory if non existing
-    log_dir = os.path.join(os.getcwd(), 'esub_logs')
-    if not os.path.isdir(log_dir):
-        os.makedirs(log_dir)
-        vprint('Created directory {}'.format(log_dir),
-               logger=LOGGER, verbose=True)
-
     # initializing parser
     description = "This is esub an user friendly and flexible tool to " \
                   "submit jobs to a cluster or run them locally"
     parser = argparse.ArgumentParser(description=description, add_help=True)
 
+    # deault for resources
     resources = dict(main_memory=1000,
                      main_time=4,
                      main_time_per_index=None,
                      main_scratch=2000,
                      watchdog_memory=1000,
                      watchdog_time=4,
                      watchdog_scratch=2000,
                      merge_memory=1000,
                      merge_time=4,
                      merge_scratch=2000)
 
     # parse all the submitter arguments
-    parser.add_argument(
-        'exec', type=str, help='path to the executable (python file '
-                               'containing functions main, watchdog, merge)')
+    parser.add_argument('exec', type=str,
+                        help='path to the executable (python file '
+                        'containing functions main, watchdog, merge)')
     parser.add_argument('--mode', type=str, default='run',
                         choices=('run', 'jobarray', 'mpi',
                                  'run-mpi', 'run-tasks'),
                         help='The mode in which to operate. '
                         'Choices: run, jobarray, mpi, run-mpi, '
                         'run-tasks')
     parser.add_argument('--job_name', type=str, default='job',
                         help='Individual name for this job. CAUTION: '
                              'Multiple jobs with same name'
                              'can confuse system!')
     parser.add_argument('--source_file', type=str, default='source_esub.sh',
                         help='Optionally provide a source file which '
-                        'gets executed first (loading modules, '
+                        'gets executed on the computing '
+                        'node before your jobs are started.'
+                        'Useful for loading modules, '
                         'declaring environemental variables and so on')
     parser.add_argument('--main_memory', type=float,
                         default=resources['main_memory'],
-                        help='Memory allocated per core for main job in MB')
+                        help='Memory allocated per core for main '
+                        'job in MB. Default: 1000 MB')
     parser.add_argument('--main_time', type=float,
                         default=resources['main_time'],
-                        help='Job run time limit in hours for main job')
+                        help='Job run time limit in hours for'
+                        ' main job. Default 4h')
     parser.add_argument('--main_time_per_index', type=float,
                         default=resources['main_time_per_index'],
                         help='Job run time limit in hours for main '
-                             'job per index, overwrites main_time if set')
+                             'job per index, overwrites main_time if set.')
     parser.add_argument('--main_scratch', type=float,
                         default=resources['main_scratch'],
-                        help='Local scratch for allocated for main job')
+                        help='Local scratch memory allocated '
+                        'for main job in MB. Default 2000 MB')
     parser.add_argument('--watchdog_memory', type=float,
                         default=resources['watchdog_memory'],
                         help='Memory allocated per core '
-                             'for watchdog job in MB')
+                             'for watchdog job in MB. Default: 1000 MB')
     parser.add_argument('--watchdog_time', type=float,
                         default=resources['watchdog_time'],
-                        help='Job run time limit in hours for watchdog job')
+                        help='Job run time limit in hours '
+                        'for watchdog job. Default: 4h')
     parser.add_argument('--watchdog_scratch', type=float,
                         default=resources['watchdog_scratch'],
-                        help='Local scratch for allocated for watchdog job')
+                        help='Local scratch memory allocated '
+                        'for watchdog job. Default: 2000 MB')
     parser.add_argument('--merge_memory', type=float,
                         default=resources['merge_memory'],
-                        help='Memory allocated per core for merge job in MB')
+                        help='Memory allocated per core for '
+                        'merge job in MB. Default: 1000 MB')
     parser.add_argument('--merge_time', type=float,
                         default=resources['merge_time'],
-                        help='Job run time limit in hours for merge job')
+                        help='Job run time limit in hours '
+                        'for merge job. Default: 4h')
     parser.add_argument('--merge_scratch', type=float,
                         default=resources['merge_scratch'],
-                        help='Local scratch for allocated for merge job')
-    parser.add_argument('--function', type=str, default=['main'], nargs='+',
-                        choices=('main', 'watchdog', 'merge', 'rerun_missing',
-                                 'all'),
+                        help='Local scratch memory allocated '
+                        'for merge job. Default: 2000 MB')
+    parser.add_argument('--function', type=str, default='main',
                         help='The functions that should be executed. '
-                        'Choices: main, watchdog, merge, rerun_missing, all')
+                        'Choices: main, watchdog, merge, '
+                        'rerun_missing, check_missing, all, '
+                        'or a list separated by whitespaces.')
     parser.add_argument('--main_name', type=str, default='main',
-                        help='Name of the main function in the executable')
+                        help='Name of the main function in the executable.')
     parser.add_argument('--tasks', type=str, default='0',
                         help='Task string from which the indices are parsed. '
-                             'Either single index, list of indices or range '
-                             'looking like int1 > int2')
-    parser.add_argument('--n_cores', type=int, default=1,
-                        help='The number of cores to request')
+                             'Either single index, list of '
+                             'indices (format 0,1,2 ), a range '
+                             'looking like int1 > int2 or path '
+                             'to a text file that holds '
+                             'a string in the format of the '
+                             'beforementioned formats.')
+    parser.add_argument('--n_cores', type=int, default=-1,
+                        help='The number of cores to '
+                        'request for the main function (DEPRECATED).')
+    parser.add_argument('--n_jobs', type=int, default=1,
+                        help='The number of jobs to '
+                        'request for the main function.')
+    parser.add_argument('--max_njobs', type=int, default=-1,
+                        help='The maximal number of jobs that are allowed '
+                        'to run at the same time.')
     parser.add_argument('--dependency', type=str, default='',
                         help='A dependency string that gets added to the '
-                             'dependencies (meant for pipelining)')
+                             'dependencies (example after(<jobid>).')
     parser.add_argument('--system', type=str, default='bsub',
-                        choices=('bsub',),
-                        help='Type of the queing system '
-                             '(so far only know bsub)')
+                        choices=('bsub', 'slurm'),
+                        help='Type of the system. '
+                        'Default is bsub (IBMs LSF system).'
+                        'Support for slurm is expermimental!')
+    parser.add_argument('--log_dir', type=str,
+                        default=os.path.join(os.getcwd(), 'esub_logs'),
+                        help='Directory where to write the logs to. '
+                        'By default uses the current working directory.')
     parser.add_argument('--test', action='store_true',
-                        default=False, help='Test mode')
+                        default=False,
+                        help='Test mode. Will not submit '
+                        'the jobs but only print.')
+    parser.add_argument('--discard_output', action='store_true',
+                        default=False,
+                        help='If True all stdout/stderr is '
+                        'written to /dev/null.')
+    parser.add_argument('--batchsize', type=int,
+                        default=100000,
+                        help='The maximum length of a jobarray. If requesting'
+                        ' a larger jobarray it will automatically get '
+                        'split into smaller ones. Default: 100000')
+    parser.add_argument('--additional_args', type=str, default='',
+                        help='Can pass comma-separated, additional, '
+                        'cluster-specific arguemnts. e.g. '
+                        '--additional_args="-C knl,--exclusive" to request '
+                        'only KNL nodes and to not share nodes with other '
+                        'users. The availablility of such arguments depends '
+                        'on the cluster you are using.')
+    parser.add_argument('--additional_bsub_args', type=str, default='',
+                        help='Additional arguments for the LSF system. '
+                        'Example: \'-R "span[ptile=100]"\' to request that '
+                        'all 100 cores are on the same computing node')
+    parser.add_argument('--esub_verbosity', type=int,
+                        default=3, choices=(0, 1, 2, 3, 4),
+                        help='esub verbosity. From 0-4 with 4 being '
+                        'the most verbose. Default is 3 (info).')
+    parser.add_argument('--main_n_cores_per_job', type=int,
+                        default=1,
+                        help='Number of cores per job for the main function. '
+                        'Default: 1')
+    parser.add_argument('--watchdog_n_cores', type=int,
+                        default=1,
+                        help='Number of cores per job for the watchdog. '
+                        'fuction. Default: 1')
+    parser.add_argument('--merge_n_cores', type=int,
+                        default=1,
+                        help='Number of cores per job for the merge. '
+                        'Default: 1')
+    parser.add_argument('--mpi_merge', action='store_true',
+                        default=False,
+                        help='If True merge function is run as an MPI job. '
+                        'Otherwise as a normal job with merge_cores.')
+    parser.add_argument('--mpi_watchdog', action='store_true',
+                        default=False,
+                        help='If True watchdog function is run as an MPI job. '
+                        'Otherwise as a normal job with watchdog_cores.')
 
     args, function_args = parser.parse_known_args(args)
 
+    logger_utils.set_logger_level(LOGGER, args.esub_verbosity)
+
+    if args.n_cores > -1:
+        LOGGER.warning(
+            "DEPRECATION WARNING: The n_cores option will be dropped in a "
+            "future version. Use n_jobs instead.")
+        args.n_jobs = args.n_cores
+
+    # Make log directory if non existing
+    log_dir = args.log_dir
+    if not os.path.isdir(log_dir):
+        os.makedirs(log_dir)
+        LOGGER.debug('Created log directory {}'.format(log_dir))
+
     mode = args.mode
+    add_args = args.additional_args
     main_name = args.main_name
     job_name = args.job_name
     source_file = args.source_file
     tasks = args.tasks
     exe = args.exec
-    n_cores = args.n_cores
+    n_jobs = args.n_jobs
+    main_n_cores = args.main_n_cores_per_job
+    watchdog_n_cores = args.watchdog_n_cores
+    merge_n_cores = args.merge_n_cores
     function = args.function
     system = args.system
+    if system == 'slurm':
+        LOGGER.warning(
+            "Support for slurm is experimental and only some basic features "
+            "of esub-epipe are supported!")
     ext_dependencies = args.dependency
 
-    if len(function) == 1 and function[0] == 'all':
-        function = 'all'
-
     # Make sure that executable exits
     if os.path.isfile(exe):
         if not os.path.isabs(exe):
             exe = os.path.join(os.getcwd(), exe)
+            LOGGER.debug(f"Using executable file at {exe}")
     else:
         raise FileNotFoundError(
             'Did not find {}. Please specify a valid path for '
             'executable'.format(exe))
 
     starter_message()
 
     # Set path to log file and to file storing finished main job ids
     path_log = utils.get_path_log(log_dir, job_name)
+    LOGGER.debug(f"Using log file at {path_log}")
+
     path_finished = utils.get_path_finished_indices(log_dir, job_name)
-    vprint("Using log file {}".format(path_log),
-           logger=LOGGER, verbose=True)
-    vprint("Storing finished indices in file {}".format(path_finished),
-           logger=LOGGER, verbose=True)
-    vprint("Running in mode {}".format(mode),
-           logger=LOGGER, verbose=True)
+    LOGGER.debug(f"Storing finished indices at {path_finished}")
+    LOGGER.info("Running in run mode {}".format(mode))
 
     # importing the functions from the executable
     executable = utils.import_executable(exe)
 
     # check if required function exists. Otherwise skip it
+    if ',' in function:
+        function = function.split(',')
+    else:
+        function = [function]
+    if (len(function) == 1) and (function[0] == 'all'):
+        function = 'all'
     if function == 'all':
         function = ['main', 'rerun_missing', 'watchdog', 'merge']
     for func in function:
         if func == 'rerun_missing':
             continue
         elif func == 'main':
             if not hasattr(executable, main_name):
-                vprint(
+                LOGGER.warning(
                     "Did not find main function {} in the executable. "
-                    "Skipping it...".format(main_name),
-                    logger=LOGGER, verbose=True)
+                    "Skipping it...".format(main_name))
                 function.remove(func)
         else:
             if not hasattr(executable, func):
-                vprint(
+                LOGGER.warning(
                     "Did not find function {} in the executable. "
-                    "Skipping it...".format(func),
-                    logger=LOGGER, verbose=True)
+                    "Skipping it...".format(func))
                 function.remove(func)
     if len(function) == 0:
-        vprint("No function to run found. Exiting...",
-               logger=LOGGER, verbose=True)
+        LOGGER.warning("No function to run found. Exiting.")
         sys.exit(0)
 
     # run setup if implemented
     if hasattr(executable, 'setup'):
-        vprint('Running setup from executable',
-               logger=LOGGER, verbose=True)
+        LOGGER.info('Running setup function from executable')
         getattr(executable, 'setup')(function_args)
 
     # get resources from executable if implemented
     res_update = dict()
     if hasattr(executable, 'resources'):
-        vprint('Getting cluster resources from executable',
-               logger=LOGGER, verbose=True)
+        LOGGER.info(
+            'Running resources function from executable. '
+            'Updating resource requirements.')
         res_update = getattr(executable, 'resources')(function_args)
 
     # overwrite with non-default command-line input
     for res_name, res_default_val in resources.items():
         res_cmd_line = getattr(args, res_name)
         if res_cmd_line != res_default_val:
             res_update[res_name] = res_cmd_line
-
+            LOGGER.debug(
+                f'Overriding default resource {res_name}: '
+                f'{res_default_val} -> {res_cmd_line}')
     resources.update(res_update)
 
     if resources['main_time_per_index'] is not None:
         n_indices = len(utils.get_indices(tasks))
         resources['main_time'] = resources['main_time_per_index'] * \
-            math.ceil(n_indices / n_cores)
-
+            math.ceil(n_indices / n_jobs)
+        LOGGER.debug(
+            f"main_time_per_index is set -> Overriding "
+            f"main_time to {resources['main_time']}h")
     del resources['main_time_per_index']
 
     # check if log files should be overwritten
-    overwrite_log = function == 'all'
+    overwrite_log = (function == 'all') | (function == 'main')
 
     # CASE 1 : run locally
     if (mode == 'run') | (mode == 'run-mpi') | (mode == 'run-tasks'):
+        LOGGER.info("Running locally!")
+
         # adding function and tasks arguments
         if function == 'all':
-            vprint("Running all functions specified in executable",
-                   logger=LOGGER, verbose=True)
+            LOGGER.debug("Running all functions sspecified in executable")
         else:
-            vprint("Running the function(s) {} "
-                   "specified in executable".format(
-                       ', '.join(function)),
-                   logger=LOGGER, verbose=True)
+            LOGGER.debug(
+                "Running the function(s) {} "
+                "specified in executable".format(', '.join(function)))
 
         # getting index list
         indices = utils.get_indices(tasks)
-        vprint("Running on tasks: {}".format(indices),
-               logger=LOGGER, verbose=True)
+        LOGGER.info("Running on tasks: {}".format(indices))
 
         # loop over functions
         for f in function:
 
+            LOGGER.info(f"Running function {f}")
             indices_use = indices
 
             # check if function is specified
             if f == 'main' or f == 'rerun_missing':
                 function_found = hasattr(executable, main_name)
             else:
                 function_found = hasattr(executable, f)
 
             if not function_found:
-                vprint(
+                LOGGER.warning(
                     "The requested function {} is missing in the executable. "
-                    "Skipping...".format(f),
-                    logger=LOGGER, verbose=True)
+                    "Skipping...".format(f))
                 continue
 
             if f == 'main':
                 # resetting missing file
-                vprint("Resetting file holding finished indices",
-                       logger=LOGGER, verbose=True)
+                LOGGER.debug("Resetting file holding finished indices")
                 utils.robust_remove(path_finished)
 
             if f == 'rerun_missing':
                 indices_use = utils.check_indices(
-                    indices, path_finished, executable, function_args, LOGGER)
+                    indices, path_finished, executable,
+                    function_args, verbosity=args.esub_verbosity)
                 if len(indices_use) > 0:
-                    vprint("Rerunning tasks: {}".format(indices_use),
-                           logger=LOGGER, verbose=True)
+                    LOGGER.info("Rerunning tasks: {}".format(indices_use))
                     f = 'main'
                 else:
-                    vprint('All indices are finished, nothing to re-run.',
-                           logger=LOGGER, verbose=True)
+                    LOGGER.info('All indices are finished, nothing to re-run.')
                     continue
 
-            if f == 'main':
+            if f == 'check_missing':
+                indices_use = utils.check_indices(
+                    indices, path_finished, executable, function_args,
+                    check_indices_file=False, verbosity=args.esub_verbosity)
+                if len(indices_use) > 0:
+                    LOGGER.info("Rerunning tasks: {}".format(indices_use))
+                    f = 'main'
+                else:
+                    LOGGER.info('All indices are finished, nothing to re-run.')
+                    continue
 
+            if f == 'main':
                 if mode == 'run':
                     for index in getattr(executable, main_name)(indices,
                                                                 function_args):
+                        LOGGER.info(
+                            "##################### Starting Task {} "
+                            "#####################".format(index))
                         utils.write_index(index, path_finished)
-                        vprint(
+                        LOGGER.info(
                             "##################### Finished Task {} "
-                            "#####################".format(index),
-                            logger=LOGGER, verbose=True)
+                            "#####################".format(index))
 
                 elif mode == 'run-mpi':
+                    LOGGER.info(
+                        "##################### Starting MPI job"
+                        "#####################")
                     utils.run_local_mpi_job(
-                        exe, n_cores, function_args, LOGGER, main_name)
-                    vprint(
-                        "##################### Finished "
-                        "#####################",
-                        logger=LOGGER, verbose=True)
+                        exe, main_n_cores, function_args, LOGGER,
+                        main_name, args.esub_verbosity)
+                    LOGGER.info(
+                        "##################### Finished MPI job"
+                        "#####################")
 
                 elif mode == 'run-tasks':
-                    dones = utils.run_local_mpi_tasks(
-                        executable, n_cores, function_args, tasks, main_name,
-                        LOGGER)
+                    LOGGER.info(
+                        "##################### Starting parallel tasks {} "
+                        "#####################".format(tasks))
+                    dones = utils.run_local_tasks(
+                        executable, n_jobs, function_args, tasks, main_name)
                     for index in dones:
                         utils.write_index(index, path_finished)
-                        vprint(
+                        LOGGER.info(
                             "##################### Finished Task {} "
-                            "#####################".format(index),
-                            logger=LOGGER, verbose=True)
+                            "#####################".format(index))
 
             else:
                 getattr(executable, f)(indices_use, function_args)
 
     # CASE 2 and 3 : running jobs on cluster (MPI or jobarray)
-    elif (mode == 'jobarray') | (mode == 'mpi'):
+    elif (mode == 'jobarray') | (mode == 'mpi') | (mode == 'tasks'):
         # Add dependencies to functions
         if (function == 'all') & (mode == 'jobarray'):
             function = ['main', 'watchdog', 'rerun_missing', 'merge']
-            vprint("Submitting all functions specified in executable "
-                   "to queuing system. Watchdog running along "
-                   "main. Trying to rerun jobs after main finished. "
-                   "Merge running at the end.",
-                   logger=LOGGER, verbose=True)
-        elif (function == 'all') & (mode == 'mpi'):
+            LOGGER.info(
+                "Submitting all functions specified in executable "
+                "to queuing system. Watchdog running along "
+                "main. Trying to rerun jobs after main finished. "
+                "Merge running at the end.")
+        elif (function == 'all') & ((mode == 'mpi') | (mode == 'tasks')):
             function = ['main', 'watchdog', 'merge']
-            vprint("Submitting all functions specified in executable "
-                   "to queuing system. Watchdog running along "
-                   "main. Merge running at the end.",
-                   logger=LOGGER, verbose=True)
+            LOGGER.info(
+                "Submitting all functions specified in executable "
+                "to queuing system. Watchdog running along "
+                "main. Merge running at the end.")
         else:
-            vprint("Submitting the function(s) {} specified in "
-                   "executable to queuing system".
-                   format(', '.join(function)),
-                   logger=LOGGER, verbose=True)
+            LOGGER.info(
+                "Submitting the function(s) {} specified in "
+                "executable to queuing system".
+                format(', '.join(function)))
 
         jobids = collections.OrderedDict()
         for ii, f in enumerate(function):
-
-            if f == 'main' or f == 'rerun_missing':
+            if (f == 'main') or (f == 'rerun_missing') or (
+                    f == 'check_missing'):
                 function_found = hasattr(executable, main_name)
             else:
                 function_found = hasattr(executable, f)
 
             if not function_found:
-                vprint(
+                LOGGER.warning(
                     "The requested function {} is missing in the executable. "
-                    "Skipping...".format(f),
-                    logger=LOGGER, verbose=True)
+                    "Skipping...".format(f))
                 continue
 
             if f == 'main':
                 # resetting missing file
-                vprint("Resetting file holding finished indices",
-                       logger=LOGGER, verbose=True)
+                LOGGER.debug("Resetting file holding finished indices")
                 utils.robust_remove(path_finished)
-                n_cores_use = n_cores
+                n_jobs_use = n_jobs
+                n_cores_use = main_n_cores
+                mode_ = mode
+            elif f == 'watchdog':
+                n_jobs_use = 1
+                n_cores_use = watchdog_n_cores
+                if args.mpi_watchdog:
+                    mode_ = 'mpi'
+                else:
+                    mode_ = 'jobarray'
+            elif f == 'merge':
+                n_jobs_use = 1
+                n_cores_use = merge_n_cores
+                if args.mpi_merge:
+                    mode_ = 'mpi'
+                else:
+                    mode_ = 'jobarray'
             else:
-                n_cores_use = 1
-
-            vprint(
-                "Submitting {} job to {} core(s)".format(f, n_cores_use),
-                logger=LOGGER, verbose=True)
+                # reruns
+                n_jobs_use = 1
+                n_cores_use = main_n_cores
+                mode_ = mode
+
+            LOGGER.debug(
+                f"Submitting function {f} broken down "
+                f"into {n_jobs_use} job(s)")
 
             # reset logs
-            vprint('Resetting log files',
-                   logger=LOGGER, verbose=True)
+            LOGGER.debug('Resetting log files')
             stdout_log, stderr_log = utils.get_log_filenames(
                 log_dir, job_name, f)
             utils.robust_remove(stdout_log)
             utils.robust_remove(stderr_log)
 
             # the current job depends at most on the previous one
             # (e.g., rerun_missing does not need to wait for the
             # watchdog to finish)
             dependency = utils.get_dependency_string(
-                f, jobids, ext_dependencies, system)
+                f, jobids, ext_dependencies, system,
+                verbosity=args.esub_verbosity)
 
-            jobid = utils.submit_job(tasks, mode, exe, log_dir, function_args,
+            jobid = utils.submit_job(tasks, mode_, exe, log_dir, function_args,
                                      function=f,
                                      source_file=source_file,
+                                     n_jobs=n_jobs_use,
                                      n_cores=n_cores_use,
                                      job_name=job_name,
                                      dependency=dependency,
                                      system=system,
                                      main_name=main_name,
                                      test=args.test,
+                                     add_args=add_args,
+                                     batchsize=args.batchsize,
+                                     max_njobs=args.max_njobs,
+                                     add_bsub=args.additional_bsub_args,
+                                     discard_output=args.discard_output,
+                                     verbosity=args.esub_verbosity,
+                                     main_mode=mode,
+                                     main_n_cores=main_n_cores,
                                      **resources)
             jobids[f] = jobid
-            vprint(
-                "Submitted job for function {} as jobid {}".format(f, jobid),
-                logger=LOGGER, verbose=True)
-
-        vprint("Submitted jobids: {}".format(
-            ' '.join([str(jobid) for jobid in jobids.values()])),
-            logger=LOGGER, verbose=True)
+
+            LOGGER.info(
+                "Submitted job for function {}. "
+                "Got jobid(s) {}".format(f, jobid))
+
+        jobid_str = ''
+        for jobid_list in jobids.values():
+            if isinstance(jobid_list, int):
+                jobid_str += f'{str(jobid_list)} '
+            elif isinstance(jobid_list, list):
+                for id in jobid_list:
+                    jobid_str += f'{str(id)} '
+            else:
+                pass
+        if len(jobid_str) == 0:
+            jobid_str = 'None'
+
+        LOGGER.info("Submission finished")
+        print(f"Submitted jobids: {jobid_str}")
 
         # write to log
         if overwrite_log:
             utils.write_to_log(
                 path_log, 'esub arguments: \n{}'.format(args), mode='w')
             utils.write_to_log(
                 path_log, 'function arguments: \n{}'.format(function_args))
```

### Comparing `esub-epipe-1.6.4/esub/scripts/check_logs.py` & `esub-epipe-1.9.1/esub/scripts/check_logs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Copyright (C) 2019 ETH Zurich,
 # Institute for Particle Physics and Astrophysics
 # Author: Joerg Herbel
 
 import os
 import argparse
 
-from ekit.logger import vprint
 from ekit import logger as logger_utils
 
-LOGGER = logger_utils.init_logger(__file__)
+LOGGER = logger_utils.init_logger(__name__)
 
 
 def main(dirpath_logs):
 
     # Get all log files in directory
     filenames_logs = filter(lambda fn: not fn.startswith('.') and
                             os.path.splitext(fn)[1] == '.log',
@@ -51,20 +50,18 @@
         for exp_cont in expected_content:
             if exp_cont not in log:
                 unfinished_logs.append(filename)
                 break
 
     # Report
     if len(unfinished_logs) == 0:
-        vprint('No unfinished jobs found',
-               logger=LOGGER, verbose=True)
+        LOGGER.info('No unfinished jobs found')
     else:
-        vprint('Logs containing unfinished jobs:\n{}'.format(
-            '\n'.join(unfinished_logs)),
-            logger=LOGGER, verbose=True)
+        LOGGER.info('Logs containing unfinished jobs:\n{}'.format(
+            '\n'.join(unfinished_logs)))
 
 
 if __name__ == '__main__':
     description = "Send a command to all jobs logged in " \
                   "esub logfiles in a given directory"
     parser = argparse.ArgumentParser(description=description, add_help=True)
     parser.add_argument('--dirpath_logs', type=str,
```

### Comparing `esub-epipe-1.6.4/esub/scripts/send_cmd.py` & `esub-epipe-1.9.1/esub/scripts/send_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 # Institute for Particle Physics and Astrophysics
 # Author: Joerg Herbel
 
 import os
 import shlex
 import subprocess
 import argparse
-from ekit.logger import vprint
 from ekit import logger as logger_utils
 
-LOGGER = logger_utils.init_logger(__file__)
+LOGGER = logger_utils.init_logger(__name__)
 
 
 def get_job_ids(path_log):
 
     # Read file
     with open(path_log, 'r') as f:
         lines = f.readlines()
@@ -56,16 +55,15 @@
     # Extract job ids from files
     job_ids = []
     for filename in filenames_logs:
         job_ids += get_job_ids(os.path.join(dirpath_logs, filename))
 
     # Modify jobs
     for job_id in job_ids:
-        vprint('Sending cmd {} to job {}'.format(cmd, job_id),
-               logger=LOGGER, verbose=True)
+        LOGGER.info('Sending cmd {} to job {}'.format(cmd, job_id))
         send_to_job(cmd, job_id)
 
 
 if __name__ == '__main__':
     description = "Send a command to all jobs logged in esub " \
                   "logfiles in a given directory"
     parser = argparse.ArgumentParser(description=description, add_help=True)
```

### Comparing `esub-epipe-1.6.4/esub/submit_jobarray.py` & `esub-epipe-1.9.1/esub/submit.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,228 +11,274 @@
 # package imports
 import os
 import argparse
 import time
 from esub import utils
 import subprocess
 import shlex
-from ekit.logger import vprint
 from ekit import logger as logger_utils
 
-LOGGER = logger_utils.init_logger(__file__)
-
+LOGGER = logger_utils.init_logger(__name__)
 
 # parse all the submitter arguments
 parser = argparse.ArgumentParser()
 parser.add_argument('--job_name', type=str, required=True)
 parser.add_argument('--source_file', type=str, required=True)
 parser.add_argument('--main_memory', type=float, required=True)
 parser.add_argument('--main_time', type=float, required=True)
 parser.add_argument('--main_scratch', type=float, required=True)
 parser.add_argument('--function', type=str, required=True)
 parser.add_argument('--executable', type=str, required=True)
 parser.add_argument('--tasks', type=str, required=True)
-parser.add_argument('--n_cores', type=int, required=True)
+parser.add_argument('--n_jobs', type=int, required=True)
+parser.add_argument('--main_n_cores', type=int, required=True)
 parser.add_argument('--log_dir', type=str, required=True)
 parser.add_argument('--system', type=str, required=True)
 parser.add_argument('--main_name', type=str, required=True)
+parser.add_argument('--mode', type=str, required=True)
+parser.add_argument('--main_mode', type=str, required=True)
+parser.add_argument('--batchsize', type=int, required=True)
+parser.add_argument('--max_njobs', type=int, required=True)
+parser.add_argument('--discard_output', action='store_true', default=False)
+parser.add_argument('--esub_verbosity', type=int, default=3)
 
 args, function_args = parser.parse_known_args()
 function = args.function
 source_file = args.source_file
 job_name = args.job_name
 log_dir = args.log_dir
 exe = args.executable
 tasks = args.tasks
-n_cores = args.n_cores
+n_jobs = args.n_jobs
+main_n_cores = args.main_n_cores
 main_memory = args.main_memory
 main_time = args.main_time
 main_scratch = args.main_scratch
 system = args.system
 main_name = args.main_name
+mode = args.mode
+main_mode = args.main_mode
+
+if mode == 'mpi':
+    try:
+        from mpi4py import MPI
+        is_master = MPI.COMM_WORLD.rank == 0
+    except ImportError:
+        if args.test:
+            is_master = False
+        else:
+            raise ImportError(
+                "You are attempting to run a MPI job. This requires a local "
+                "MPI environement as well as the mpi4py package")
+else:
+    is_master = True
+
+logger_utils.set_logger_level(LOGGER, args.esub_verbosity)
 
 # get path of log file and of file containing finished indices
 path_log = utils.get_path_log(log_dir, job_name)
 path_finished = utils.get_path_finished_indices(log_dir, job_name)
 
 TIMEOUT_MESSAGE = 'Maximum number of pending jobs reached, ' \
                   'will sleep for 30 minutes and retry'
 
 # get rank of the processor
-if system == 'bsub':
-    try:
-        msg_limit_reached = 'Pending job threshold reached.'
-        pipe_limit_reached = 'stderr'
+try:
+    msg_limit_reached = 'Pending job threshold reached.'
+    pipe_limit_reached = 'stderr'
+    if system == 'bsub':
         rank = int(os.environ['LSB_JOBINDEX'])
-        rank -= 1
-    except KeyError:
-        vprint(
-            "Environment variable LSB_JOBINDEX not set. Setting rank to 1. "
-            "Are you in a bsub system?", level='warning', verbose=True,
-            logger=LOGGER)
-        rank = 1
+    elif system == 'slurm':
+        rank = int(os.environ['SLURM_ARRAY_TASK_ID'])
+    rank -= 1
+except KeyError:
+    LOGGER.warning(
+        "Unable to get current Job array index. Are you on a slurm or bsub "
+        "system? Setting it to 1")
+    rank = 1
+
+is_first = rank == 1
 
 # Import the executable
 executable = utils.import_executable(exe)
 
-if function == 'main':
-    vprint(
-        'Running the function {} specified in executable'.format(main_name),
-        logger=LOGGER, verbose=True)
-else:
-    vprint(
-        'Running the function {} specified in executable'.format(function),
-        logger=LOGGER, verbose=True)
-
-if function == 'rerun_missing':
-    vprint('Checking if all main jobs terminated correctly...',
-           logger=LOGGER, verbose=True)
-    indices_all = utils.get_indices(tasks)
+if is_master:
+    if function == 'main':
+        LOGGER.info(
+            f'Running the function {main_name} specified in executable')
+    else:
+        LOGGER.info(
+            'Running the function {} specified in executable'.format(function))
 
-    indices_missing = utils.check_indices(
-        indices_all, path_finished, executable, function_args, LOGGER)
+if (function == 'rerun_missing') | (function == 'check_missing'):
+    if system == 'slurm':
+        raise Exception("rerun_missing not implemented for slurm. Aborting")
+    if is_master:
+        LOGGER.info('Checking if all main jobs terminated correctly...')
 
-    utils.write_to_log(
-        path_log, 'Found {} missing indices'.format(len(indices_missing)))
+    indices_all = utils.get_indices(tasks)
+    if function == 'rerun_missing':
+        indices_missing = utils.check_indices(
+            indices_all, path_finished, executable, function_args,
+            verbosity=args.esub_verbosity)
+    elif function == 'check_missing':
+        indices_missing = utils.check_indices(
+            indices_all, path_finished, executable, function_args,
+            check_indices_file=False, verbosity=args.esub_verbosity)
 
-    if len(indices_missing) == 0:
-        vprint('Nothing to resubmit. All jobs ended.',
-               logger=LOGGER, verbose=True)
-    else:
-        if len(indices_missing) > 1:
-            tasks = ','.join(map(str, indices_missing[:-1]))
-            n_cores = len(indices_missing) - 1
-            vprint(
-                'Re-Submitting tasks {} to {} cores'.format(tasks, n_cores),
-                logger=LOGGER, verbose=True)
-            jobid = utils.submit_job(tasks=tasks, mode='jobarray',
-                                     exe=args.executable, log_dir=log_dir,
-                                     function_args=function_args,
-                                     function='main', source_file=source_file,
-                                     n_cores=n_cores, job_name=job_name,
-                                     main_memory=main_memory,
-                                     main_time=main_time,
-                                     main_scratch=main_scratch, dependency='',
-                                     system=system, main_name=main_name)
+    if is_master:
+        utils.write_to_log(
+            path_log, 'Found {} missing indices'.format(len(indices_missing)))
 
-            utils.write_to_log(
-                path_log, 'Job id rerun_missing extended: {}'.format(jobid))
+        if len(indices_missing) == 0:
+            LOGGER.info('Nothing to resubmit. All jobs ended.')
         else:
-            jobid = None
-
-        # Change to local scratch if set; this has to be done after submission,
-        # s.t. that the pwd at submission time is
-        # the original directory where the submission starts
-        utils.cd_local_scratch()
-
-        # run last job locally to not waste any resources
-        index = indices_missing[-1]
-        vprint(
-            '##################### Starting Task {}\
-             #####################'.format(index),
-            logger=LOGGER, verbose=True)
-        for index in getattr(executable, main_name)([index], function_args):
-            utils.write_index(index, path_finished)
-        vprint(
-            '##################### Finished Task {}\
-             #####################'.format(index),
-            logger=LOGGER, verbose=True)
-
-        if len(indices_missing) == 1:
-            utils.write_to_log(path_log, 'First index is done')
-
-        # wait until all jobs are done
-        if jobid is not None:
-            while True:
-                while True:
-                    output = dict(stdout=[], stderr=[])
-                    with subprocess.Popen(
-                            shlex.split('bjobs {}'.format(jobid)),
-                            stdout=subprocess.PIPE,
-                            stderr=subprocess.PIPE,
-                            bufsize=1,
-                            universal_newlines=True) as proc:
+            if len(indices_missing) > 1:
+                # submit jobs
+                tasks = ','.join(map(str, indices_missing[:-1]))
+                n_jobs = len(indices_missing) - 1
+                LOGGER.info(
+                    'Re-Submitting tasks {} as {} jobs'.format(tasks, n_jobs))
+                jobid = utils.submit_job(tasks=tasks, mode=main_mode,
+                                         exe=args.executable, log_dir=log_dir,
+                                         function_args=function_args,
+                                         function='main',
+                                         source_file=source_file,
+                                         n_jobs=n_jobs, n_cores=main_n_cores,
+                                         job_name=job_name,
+                                         main_memory=main_memory,
+                                         main_time=main_time,
+                                         main_scratch=main_scratch,
+                                         dependency='',
+                                         system=system, main_name=main_name,
+                                         batchsize=args.batchsize,
+                                         discard_output=args.discard_output,
+                                         max_njobs=args.max_njobs,
+                                         verbosity=args.esub_verbosity)
+
+                utils.write_to_log(
+                    path_log,
+                    'Job id rerun_missing extended: {}'.format(jobid[0]))
+            else:
+                jobid = None
+
+            # Change to local scratch if set; this has to be done
+            # after submission,
+            # s.t. that the pwd at submission time is
+            # the original directory where the submission starts
+            utils.cd_local_scratch(args.esub_verbosity)
+
+            # run last job locally to not waste any resources
+            index = indices_missing[-1]
+            if is_master:
+                LOGGER.info(
+                    '##################### Starting Task {}\
+                    #####################'.format(index))
+            for index in getattr(
+                    executable, main_name)([index], function_args):
+                if is_master:
+                    utils.write_index(index, path_finished)
+            if is_master:
+                LOGGER.info(
+                    '##################### Finished Task {}\
+                    #####################'.format(index))
+
+            if is_master:
+                if len(indices_missing) == 1:
+                    utils.write_to_log(path_log, 'First index is done')
+
+            if is_master:
+                # wait until all jobs are done
+                if jobid is not None:
+                    while True:
+                        while True:
+                            output = dict(stdout=[], stderr=[])
+                            with subprocess.Popen(
+                                    shlex.split('bjobs {}'.format(jobid[0])),
+                                    stdout=subprocess.PIPE,
+                                    stderr=subprocess.PIPE,
+                                    bufsize=1,
+                                    universal_newlines=True) as proc:
+
+                                # check for limit for maximum number
+                                # of pending jobs
+                                pending_limit_reached = False
+                                for line in getattr(proc, pipe_limit_reached):
+
+                                    pending_limit_reached = \
+                                        msg_limit_reached in line
+                                    if pending_limit_reached:
+                                        break
+                                    else:
+                                        output[pipe_limit_reached].append(line)
+
+                                # if the limit has been reached,
+                                # kill process and sleep
+                                if pending_limit_reached:
+                                    proc.kill()
+                                    LOGGER.warning(TIMEOUT_MESSAGE)
+                                    time.sleep(60 * 30)
+                                    continue
+
+                                # read rest of the output
+                                for line in proc.stdout:
+                                    output['stdout'].append(line)
+                                for line in proc.stderr:
+                                    output['stderr'].append(line)
 
-                        # check for limit for maximum number of pending jobs
-                        for line in getattr(proc, pipe_limit_reached):
-
-                            pending_limit_reached = msg_limit_reached in line
-                            if pending_limit_reached:
                                 break
-                            else:
-                                output[pipe_limit_reached].append(line)
-
-                        # if the limit has been reached, kill process and sleep
-                        if pending_limit_reached:
-                            proc.kill()
-                            vprint(TIMEOUT_MESSAGE,
-                                   logger=LOGGER, verbose=True)
-                            time.sleep(60 * 30)
-                            continue
-
-                        # read rest of the output
-                        for line in proc.stdout:
-                            output['stdout'].append(line)
-                        for line in proc.stderr:
-                            output['stderr'].append(line)
-
-                        break
-
-                # check if process terminated successfully
-                if proc.returncode != 0:
-                    raise RuntimeError('Running the command \"{}\" failed with'
-                                       'exit code {}. Error: \n{}'.
-                                       format('bjobs {}'.format(jobid),
-                                              proc.returncode,
-                                              '\n'.join(output['stderr'])))
-
-                # check jobstate
-                jobstate = output['stdout'][-1].split()[2]
-                if (jobstate == 'DONE') | (jobstate == 'EXIT'):
-                    break
-                time.sleep(60)
 
-        indices_missing = utils.check_indices(
-            indices_all, path_finished, executable, function_args, LOGGER)
+                        # check if process terminated successfully
+                        if proc.returncode != 0:
+                            raise RuntimeError(
+                                'Running the command \"{}\" failed with'
+                                'exit code {}. Error: \n{}'.format(
+                                    'bjobs {}'.format(jobid[0]),
+                                    proc.returncode,
+                                    '\n'.join(output['stderr'])))
+
+                        # check jobstate
+                        jobstate = output['stdout'][-1].split()[2]
+                        # for slurm either COMPLETED or FAILED?
+                        if (jobstate == 'DONE') | (jobstate == 'EXIT'):
+                            break
+                        time.sleep(60)
+
+                indices_missing = utils.check_indices(
+                    indices_all, path_finished, executable, function_args,
+                    verbosity=args.esub_verbosity)
 
-    if len(indices_missing) == 0:
-        vprint('All indices finished',
-               logger=LOGGER, verbose=True)
-        utils.write_to_log(path_log, 'All indices finished')
-    else:
-        vprint('Even after rerun not all indices finished sucessfully',
-               logger=LOGGER, verbose=True)
-        utils.write_to_log(
-            path_log, 'Even after rerun not all indices finished sucessfully')
 else:
     # Change to local scratch if set
-    utils.cd_local_scratch()
+    utils.cd_local_scratch(args.esub_verbosity)
 
     # getting index list based on jobid
-    indices = utils.get_indices_splitted(tasks, n_cores, rank)
+    indices = utils.get_indices_splitted(tasks, n_jobs, rank)
 
     if function == 'main':
 
-        vprint('Running on tasks: {}'.format(indices),
-               logger=LOGGER, verbose=True)
+        if is_master:
+            LOGGER.info('Running on tasks: {}'.format(indices))
 
         is_first = rank == 0
 
         for index in getattr(executable, main_name)(indices, function_args):
-            utils.write_index(index, path_finished)
-            vprint(
-                '##################### Finished Task {}\
-                 #####################'.format(index),
-                logger=LOGGER, verbose=True)
+            if is_master:
+                utils.write_index(index, path_finished)
+                LOGGER.info(
+                    '##################### Finished Task {}\
+                    #####################'.format(index))
 
             if is_first:
                 utils.write_to_log(path_log, 'First index is done')
                 is_first = False
 
     else:
-        utils.write_to_log(path_log, 'Running {}'.format(function))
-        vprint('Running {}, {} task(s), \
-                    first: {}, last: {}'.format(function, len(indices),
-                                                indices[0], indices[-1]),
-               logger=LOGGER, verbose=True)
+        if is_master:
+            utils.write_to_log(path_log, 'Running {}'.format(function))
+            LOGGER.info('Running {}, {} task(s), \
+                        first: {}, last: {}'.format(function, len(indices),
+                                                    indices[0], indices[-1]))
         getattr(executable, function)(indices, function_args)
-        utils.write_to_log(path_log, 'Finished running {}'.format(function))
+        if is_master:
+            utils.write_to_log(
+                path_log, 'Finished running {}'.format(function))
```

### Comparing `esub-epipe-1.6.4/esub_epipe.egg-info/PKG-INFO` & `esub-epipe-1.9.1/esub_epipe.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,86 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: esub-epipe
-Version: 1.6.4
+Version: 1.9.1
 Summary: Easy-to-use job Scheduler for Python code
-Home-page: https://cosmo-docs.phys.ethz.ch/esub-epipe
+Home-page: https://cosmo-docs.phys.ethz.ch/esub
 Author: Dominik Zuercher
 Author-email: dominik.zuercher@phys.ethz.ch
 License: MIT License
-Description: =================================
-        esub-epipe - Version 1.6.4 STABLE
-        =================================
-        
-        .. image:: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe/badges/master/coverage.svg
-          		:target: https://cosmo-gitlab.phys.ethz.ch/esub-epipe/NGSF
-        
-        .. image:: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe/badges/master/pipeline.svg
-                :target: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe
-        
-        
-        .. image:: http://img.shields.io/badge/arXiv-2006.12506-orange.svg?style=flat
-                :target: https://arxiv.org/abs/2006.12506
-        
-        
-        
-        esub-epipe is part of the Non-Gaussian Statistics Framework (`NGSF <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/NGSF>`_).
-        
-        If you use this package in your research please cite Zuercher et al. 2020. (`arXiv-2006.12506 <https://arxiv.org/abs/2006.12506>`_).
-        
-        `Source <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe>`_
-        
-        `Documentation <http://cosmo-docs.phys.ethz.ch/esub-epipe>`_
-        
-        Introduction
-        ============
-        
-        - Are you tired of rewriting the same kind of submission scripts to sumbit your code to a computer cluster?
-        
-        - Do you not want to rewrite different versions of your code for serial, parallel or MPI execution?
-        
-        - Do you wish there would be an easy way to submit large numbers of dependent jobs to a computer cluster without writing the same kind of pipeline scripts and worrying about resource allocation every time?
-        
-        If any of these points applies to you, you have come to the right place!
-        
-        When using this package you will only need to write a single python executable file. The same file can then be used to run your code
-        serially, in parallel or in an MPI environement on your local machine. You can also use the same file to submit your code to a
-        computer cluster.
-        
-        Even more, if you are building large pipelines with many dependent jobs, or even tasks which have to be executed multiple times
-        you will just have to write a single YAML file in which you state what you want to run and esub will submit all those
-        jobs to the computer cluster such that you can continue working on your amazing projects while waiting for the results :)
-        
-        Getting Started
-        ===============
-        
-        The easiest and fastest way to learn about esub is to have a look at the Examples Section in the documentation.
-        If you wish to learn more also have a look at the Usage Section in the documenation in which we documented all the things you can do with esub.
-        
-        Disclaimer
-        ==========
-        
-        At the moment only IBMs bsub system is supported but we hope to include other queing systems in the future.
-        
-        Credits
-        =======
-        
-        This package was created on May 12 2019 by Dominik Zuercher (PhD student at ETH Zurich in Alexandre Refregiers `Comsology Research Group <https://cosmology.ethz.ch/>`_)
-        It is inspired by the jobchainer code written by Tomasz Kacprzak.
-        
-        The package is maintained by Dominik Zuercher dominik.zuercher@phys.ethz.ch.
-        
-        Contributing
-        ============
-        
-        Contributions are welcome, and they are greatly appreciated! Every
-        little bit helps, and credit will always be given.
-        
 Keywords: esub,epipe
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+==================================
+esub-epipe - Version 1.9.1 STABLE
+==================================
+
+.. image:: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe/badges/master/pipeline.svg
+        :target: https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe
+
+
+.. image:: http://img.shields.io/badge/arXiv-2006.12506-orange.svg?style=flat
+        :target: https://arxiv.org/abs/2006.12506
+
+.. image:: http://img.shields.io/badge/arXiv-2110.10135-orange.svg?style=flat
+        :target: https://arxiv.org/abs/arXiv:2110.10135
+
+
+
+esub-epipe is part of the Non-Gaussian Statistics Framework (`NGSF <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/NGSF>`_).
+
+If you use this package in your research please cite Zuercher et al. 2020 (`arXiv-2006.12506 <https://arxiv.org/abs/2006.12506>`_)
+and Zuercher et al. 2021 (`arXiv-2110.10135 <https://arxiv.org/abs/2110.10135>`_).
+
+`Source <https://cosmo-gitlab.phys.ethz.ch/cosmo_public/esub-epipe>`_
+
+`Documentation <http://cosmo-docs.phys.ethz.ch/esub>`_
+
+Introduction
+============
+
+- Are you tired of rewriting the same kind of submission scripts to sumbit your code to a computer cluster?
+
+- Do you not want to rewrite different versions of your code for serial, parallel or MPI execution, but instead use the same executable everytime?
+
+- Do you wish there would be an easy way to submit large numbers of dependent jobs to a computer cluster without writing the same kind of pipeline scripts and worrying about resource allocation every time?
+
+If any of these points applies to you, you have come to the right place :)
+
+When using this package you will only need to write a single python executable file. The same file can then be used to run your code
+serially, in parallel or in an MPI environement on your local machine. You can also use the same file to submit your code to a
+computer cluster that runs IBMs LSF system or SLURM (experimental).
+
+Even more, if you are building large pipelines with many dependent jobs, or even tasks which have to be executed multiple times
+you will just have to write a single YAML file in which you state what you want to run and esub will submit all those
+jobs to the computer cluster such that you can continue working on your amazing projects while waiting for the results :)
+
+Getting Started
+===============
+
+The easiest and fastest way to learn about esub is to have a look at the Examples Section in the documentation.
+If you wish to learn more also have a look at the Usage Section in the documenation in which we documented all the things you can do with esub.
+
+Disclaimer
+==========
+
+At the moment only IBMs bsub system is supported but we hope to include other queing systems in the future.
+
+Credits
+=======
+
+This package was created on May 12 2019 by Dominik Zuercher (PhD student at ETH Zurich in Alexandre Refregiers `Comsology Research Group <https://cosmology.ethz.ch/>`_)
+It is inspired by the jobchainer code written by Tomasz Kacprzak.
+
+The package is maintained by Dominik Zuercher dominik.zuercher@phys.ethz.ch.
+
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every
+little bit helps, and credit will always be given.
```

### Comparing `esub-epipe-1.6.4/esub_epipe.egg-info/SOURCES.txt` & `esub-epipe-1.9.1/esub_epipe.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 esub/__init__.py
 esub/epipe.py
 esub/esub.py
-esub/submit_jobarray.py
-esub/submit_mpi.py
+esub/submit.py
 esub/utils.py
 esub/scripts/__init__.py
 esub/scripts/check_logs.py
 esub/scripts/send_cmd.py
 esub_epipe.egg-info/PKG-INFO
 esub_epipe.egg-info/SOURCES.txt
 esub_epipe.egg-info/dependency_links.txt
 esub_epipe.egg-info/entry_points.txt
 esub_epipe.egg-info/not-zip-safe
 esub_epipe.egg-info/requires.txt
 esub_epipe.egg-info/top_level.txt
 tests/__init__.py
 tests/test_epipe.py
 tests/test_esub.py
-tests/test_scripts.py
-tests/test_submit.py
+tests/test_esub_slurm.py
+tests/test_scripts.py
```

### Comparing `esub-epipe-1.6.4/setup.py` & `esub-epipe-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,33 +16,33 @@
     history = history_file.read().replace(".. :changelog", "")
 
 
 PACKAGE_PATH = os.path.abspath(os.path.join(__file__, os.pardir))
 
 setup(
     name="esub-epipe",
-    version="1.6.4",
+    version="1.9.1",
     description=("Easy-to-use job Scheduler for Python code"),
     long_description=open('README.rst').read(),
     author='Dominik Zuercher',
     author_email='dominik.zuercher@phys.ethz.ch',
-    url='https://cosmo-docs.phys.ethz.ch/esub-epipe',
+    url='https://cosmo-docs.phys.ethz.ch/esub',
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     license="MIT License",
     zip_safe=False,
     keywords="esub, epipe",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.10",
     ],
     entry_points={
         'console_scripts': [
             "esub = esub.esub:main", "epipe = esub.epipe:main"
         ]
     }
 )
```

### Comparing `esub-epipe-1.6.4/tests/test_epipe.py` & `esub-epipe-1.9.1/tests/test_epipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright (C) 2019 ETH Zurich, Institute for Particle Physics and Astrophysics
+# Copyright (C) 2019 ETH Zurich,
+# Institute for Particle Physics and Astrophysics
 # Author: Joerg Herbel
 
 import os
 import shutil
 import shlex
 import subprocess
 
@@ -11,26 +12,25 @@
 
     # create directory for test output
     path_testdir = os.path.join(os.getcwd(), 'esub_test_dir')
     if not os.path.isdir(path_testdir):
         os.mkdir(path_testdir)
 
     # run epipe
-    cmd = 'epipe tests/pipe.yaml --ignore_jobid_errors'
+    cmd = 'epipe tests/pipe.yaml --ignore_jobid_errors --epipe_verbosity=4'
     subprocess.call(shlex.split(cmd))
 
     # remove directory for test output
     shutil.rmtree(path_testdir)
 
     # check that log files were created and remove them
     log_dir = 'esub_logs'
     job_files = ['job1_done.dat',
                  'loopjob1__0_done.dat',
                  'loopjob1__1_done.dat',
                  'loopjob2__0_done.dat',
                  'loopjob2__1_done.dat']
 
     for job_file in job_files:
-        print(os.path.join(log_dir, job_file))
         assert os.path.isfile(os.path.join(log_dir, job_file))
 
     shutil.rmtree(log_dir)
```

### Comparing `esub-epipe-1.6.4/tests/test_scripts.py` & `esub-epipe-1.9.1/tests/test_scripts.py`

 * *Files identical despite different names*

