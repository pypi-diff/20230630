# Comparing `tmp/orthosnap-0.1.1.tar.gz` & `tmp/orthosnap-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthosnap-0.1.1.tar", last modified: Tue Jul 26 16:57:07 2022, max compression
+gzip compressed data, was "orthosnap-1.0.0.tar", last modified: Fri Jun 30 00:34:46 2023, max compression
```

## Comparing `orthosnap-0.1.1.tar` & `orthosnap-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2022-07-26 16:57:07.688746 orthosnap-0.1.1/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1078 2021-03-03 18:43:45.000000 orthosnap-0.1.1/LICENSE.md
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     5210 2022-07-26 16:57:07.688401 orthosnap-0.1.1/PKG-INFO
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     4510 2022-07-26 09:53:38.000000 orthosnap-0.1.1/README.md
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2022-07-26 16:57:07.685364 orthosnap-0.1.1/orthosnap/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)        0 2021-02-27 00:52:54.000000 orthosnap-0.1.1/orthosnap/__init__.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      131 2022-06-30 02:34:29.000000 orthosnap-0.1.1/orthosnap/__main__.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2421 2022-07-26 16:39:58.000000 orthosnap-0.1.1/orthosnap/args_processing.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)    10045 2022-07-26 16:40:21.000000 orthosnap-0.1.1/orthosnap/helper.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     3974 2022-07-26 16:37:45.000000 orthosnap-0.1.1/orthosnap/orthosnap.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     7516 2022-07-26 16:18:15.000000 orthosnap-0.1.1/orthosnap/parser.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)       22 2022-07-26 16:49:25.000000 orthosnap-0.1.1/orthosnap/version.py
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     2366 2022-07-26 16:37:25.000000 orthosnap-0.1.1/orthosnap/writer.py
-drwxr-xr-x   0 jlsteenwyk   (501) staff       (20)        0 2022-07-26 16:57:07.687886 orthosnap-0.1.1/orthosnap.egg-info/
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     5210 2022-07-26 16:57:07.000000 orthosnap-0.1.1/orthosnap.egg-info/PKG-INFO
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)      406 2022-07-26 16:57:07.000000 orthosnap-0.1.1/orthosnap.egg-info/SOURCES.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)        1 2022-07-26 16:57:07.000000 orthosnap-0.1.1/orthosnap.egg-info/dependency_links.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)       56 2022-07-26 16:57:07.000000 orthosnap-0.1.1/orthosnap.egg-info/entry_points.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)       43 2022-07-26 16:57:07.000000 orthosnap-0.1.1/orthosnap.egg-info/requires.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)       10 2022-07-26 16:57:07.000000 orthosnap-0.1.1/orthosnap.egg-info/top_level.txt
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)       38 2022-07-26 16:57:07.688881 orthosnap-0.1.1/setup.cfg
--rw-r--r--   0 jlsteenwyk   (501) staff       (20)     1317 2021-11-01 18:17:07.000000 orthosnap-0.1.1/setup.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2023-06-30 00:34:46.927183 orthosnap-1.0.0/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1078 2022-07-26 18:51:33.000000 orthosnap-1.0.0/LICENSE.md
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5010 2023-06-30 00:34:46.927027 orthosnap-1.0.0/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4310 2023-06-23 16:07:59.000000 orthosnap-1.0.0/README.md
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2023-06-30 00:34:46.925976 orthosnap-1.0.0/orthosnap/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        0 2021-02-27 00:52:54.000000 orthosnap-1.0.0/orthosnap/__init__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      131 2022-06-30 02:34:29.000000 orthosnap-1.0.0/orthosnap/__main__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2512 2023-06-23 15:27:02.000000 orthosnap-1.0.0/orthosnap/args_processing.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)    10524 2023-06-23 15:29:58.000000 orthosnap-1.0.0/orthosnap/helper.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4031 2023-06-23 15:27:02.000000 orthosnap-1.0.0/orthosnap/orthosnap.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     7516 2022-07-26 16:18:15.000000 orthosnap-1.0.0/orthosnap/parser.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       22 2023-06-23 15:27:42.000000 orthosnap-1.0.0/orthosnap/version.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2383 2023-06-23 15:27:01.000000 orthosnap-1.0.0/orthosnap/writer.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2023-06-30 00:34:46.926813 orthosnap-1.0.0/orthosnap.egg-info/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5010 2023-06-30 00:34:46.000000 orthosnap-1.0.0/orthosnap.egg-info/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      406 2023-06-30 00:34:46.000000 orthosnap-1.0.0/orthosnap.egg-info/SOURCES.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        1 2023-06-30 00:34:46.000000 orthosnap-1.0.0/orthosnap.egg-info/dependency_links.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       56 2023-06-30 00:34:46.000000 orthosnap-1.0.0/orthosnap.egg-info/entry_points.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       43 2023-06-30 00:34:46.000000 orthosnap-1.0.0/orthosnap.egg-info/requires.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       10 2023-06-30 00:34:46.000000 orthosnap-1.0.0/orthosnap.egg-info/top_level.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       38 2023-06-30 00:34:46.927232 orthosnap-1.0.0/setup.cfg
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1316 2023-06-30 00:34:16.000000 orthosnap-1.0.0/setup.py
```

### Comparing `orthosnap-0.1.1/LICENSE.md` & `orthosnap-1.0.0/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2020 Jacob L. Steenwyk and contributors
+Copyright (c) 2022 Jacob L. Steenwyk and contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `orthosnap-0.1.1/PKG-INFO` & `orthosnap-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthosnap
-Version: 0.1.1
+Version: 1.0.0
 Summary: orthosnap, identify orthologous subgroups of genes in large orthologous groups of genes.
 Home-page: https://github.com/jlsteenwyk/orthosnap
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
     ·
     <a href="https://github.com/jlsteenwyk/orthosnap/issues">Report Bug</a>
     ·
     <a href="https://github.com/jlsteenwyk/orthosnap/issues">Request Feature</a>
   </p>
     <p align="center">
         <a href="https://github.com/JLSteenwyk/orthosnap/actions" alt="Build">
-            <img src="https://img.shields.io/github/workflow/status/jlsteenwyk/orthosnap/CI/master">
+            <img src="https://img.shields.io/github/actions/workflow/status/JLSteenwyk/orthosnap/ci.yml?branch=master">
         </a>
         <a href="https://codecov.io/gh/JLSteenwyk/orthosnap">
           <img src="https://codecov.io/gh/JLSteenwyk/orthosnap/branch/master/graph/badge.svg?token=FX66FUET0L"/>
         </a>
         <a href="https://github.com/jlsteenwyk/orthosnap/graphs/contributors" alt="Contributors">
             <img src="https://img.shields.io/github/contributors/jlsteenwyk/orthosnap">
         </a>
@@ -48,24 +48,21 @@
         </a>
         <a href="https://lbesson.mit-license.org/" alt="License">
             <img src="https://img.shields.io/badge/License-MIT-blue.svg">
         </a>
         <a href="https://pypi.org/project/orthosnap/" alt="PyPI - Python Version">
             <img src="https://img.shields.io/pypi/pyversions/orthosnap">
         </a>
-        <br />
-        <a href="https://www.biorxiv.org/content/10.1101/2021.10.30.466607">
-          <img src="https://zenodo.org/badge/DOI/10.1101/2021.10.30.466607.svg">
-        </a>
-        <a href="https://patreon.com/jlsteenwyk"><img src="https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Djlsteenwyk%26type%3Dpatrons&style=flat" alt="Support me on Patreon" /></a>
+        <a href="https://jlsteenwyk.com/publication_pdfs/2022_Steenwyk_etal_PLoS_Biology.pdf">
+          <img src="https://zenodo.org/badge/DOI/10.1371/journal.pbio.3001827.svg">
     </p>
 </p>
 
-orthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees.<br /><br />
-If you found orthosnap useful, please cite *orthosnap: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees*. Steenwyk et al. 2021, bioRxiv. doi: [10.1101/2021.10.30.466607](https://www.biorxiv.org/content/10.1101/2021.10.30.466607v1).
+OrthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees.<br /><br />
+If you found orthosnap useful, please cite *OrthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees*. Steenwyk et al. 2022, PLOS Biology. doi: [10.1371/journal.pbio.3001827](https://jlsteenwyk.com/publication_pdfs/2022_Steenwyk_etal_PLoS_Biology.pdf).
 <br /><br />
 
 ---
 
 <br />
 
 This documentation covers downloading and installing orthosnap. Details about orthosnap usage including a tutorial are available on our [online documentation](https://jlsteenwyk.com/orthosnap/).
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: orthosnap Version: 0.1.1 Summary: orthosnap,
+Metadata-Version: 2.1 Name: orthosnap Version: 1.0.0 Summary: orthosnap,
 identify orthologous subgroups of genes in large orthologous groups of genes.
 Home-page: https://github.com/jlsteenwyk/orthosnap Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com License: UNKNOWN Platform: UNKNOWN
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Scientific/Engineering Description-Content-Type: text/markdown
 License-File: LICENSE.md
                                     [Logo]
                      Docs Â· Report_Bug Â· Request_Feature
-[https://img.shields.io/github/workflow/status/jlsteenwyk/orthosnap/CI/master]
-       [https://codecov.io/gh/JLSteenwyk/orthosnap/branch/master/graph/
-   badge.svg?token=FX66FUET0L] [https://img.shields.io/github/contributors/
-                  jlsteenwyk/orthosnap] [follow_on_Twitter]
+ [https://img.shields.io/github/actions/workflow/status/JLSteenwyk/orthosnap/
+   ci.yml?branch=master] [https://codecov.io/gh/JLSteenwyk/orthosnap/branch/
+   master/graph/badge.svg?token=FX66FUET0L] [https://img.shields.io/github/
+            contributors/jlsteenwyk/orthosnap] [follow_on_Twitter]
                  [https://static.pepy.tech/personalized-badge/
 orthosnap?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPi%20Downloads]
  [https://img.shields.io/badge/License-MIT-blue.svg] [https://img.shields.io/
-                          pypi/pyversions/orthosnap]
-  [https://zenodo.org/badge/DOI/10.1101/2021.10.30.466607.svg] [Support_me_on
-                                   Patreon]
-orthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy
+       pypi/pyversions/orthosnap] [https://zenodo.org/badge/DOI/10.1371/
+                           journal.pbio.3001827.svg]
+OrthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy
 orthologs from gene family trees.
 
-If you found orthosnap useful, please cite *orthosnap: a tree splitting and
+If you found orthosnap useful, please cite *OrthoSNAP: a tree splitting and
 pruning algorithm for retrieving single-copy orthologs from gene family trees*.
-Steenwyk et al. 2021, bioRxiv. doi: [10.1101/2021.10.30.466607](https://
-www.biorxiv.org/content/10.1101/2021.10.30.466607v1).
+Steenwyk et al. 2022, PLOS Biology. doi: [10.1371/journal.pbio.3001827](https:/
+/jlsteenwyk.com/publication_pdfs/2022_Steenwyk_etal_PLoS_Biology.pdf).
 
 ---
 This documentation covers downloading and installing orthosnap. Details about
 orthosnap usage including a tutorial are available on our [online
 documentation](https://jlsteenwyk.com/orthosnap/).
 **Installation** **If you are having trouble installing orthosnap, please
 contact the lead developer, Jacob L. Steenwyk, via [email](https://
```

### Comparing `orthosnap-0.1.1/README.md` & `orthosnap-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ·
     <a href="https://github.com/jlsteenwyk/orthosnap/issues">Report Bug</a>
     ·
     <a href="https://github.com/jlsteenwyk/orthosnap/issues">Request Feature</a>
   </p>
     <p align="center">
         <a href="https://github.com/JLSteenwyk/orthosnap/actions" alt="Build">
-            <img src="https://img.shields.io/github/workflow/status/jlsteenwyk/orthosnap/CI/master">
+            <img src="https://img.shields.io/github/actions/workflow/status/JLSteenwyk/orthosnap/ci.yml?branch=master">
         </a>
         <a href="https://codecov.io/gh/JLSteenwyk/orthosnap">
           <img src="https://codecov.io/gh/JLSteenwyk/orthosnap/branch/master/graph/badge.svg?token=FX66FUET0L"/>
         </a>
         <a href="https://github.com/jlsteenwyk/orthosnap/graphs/contributors" alt="Contributors">
             <img src="https://img.shields.io/github/contributors/jlsteenwyk/orthosnap">
         </a>
@@ -29,24 +29,21 @@
         </a>
         <a href="https://lbesson.mit-license.org/" alt="License">
             <img src="https://img.shields.io/badge/License-MIT-blue.svg">
         </a>
         <a href="https://pypi.org/project/orthosnap/" alt="PyPI - Python Version">
             <img src="https://img.shields.io/pypi/pyversions/orthosnap">
         </a>
-        <br />
-        <a href="https://www.biorxiv.org/content/10.1101/2021.10.30.466607">
-          <img src="https://zenodo.org/badge/DOI/10.1101/2021.10.30.466607.svg">
-        </a>
-        <a href="https://patreon.com/jlsteenwyk"><img src="https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Djlsteenwyk%26type%3Dpatrons&style=flat" alt="Support me on Patreon" /></a>
+        <a href="https://jlsteenwyk.com/publication_pdfs/2022_Steenwyk_etal_PLoS_Biology.pdf">
+          <img src="https://zenodo.org/badge/DOI/10.1371/journal.pbio.3001827.svg">
     </p>
 </p>
 
-orthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees.<br /><br />
-If you found orthosnap useful, please cite *orthosnap: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees*. Steenwyk et al. 2021, bioRxiv. doi: [10.1101/2021.10.30.466607](https://www.biorxiv.org/content/10.1101/2021.10.30.466607v1).
+OrthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees.<br /><br />
+If you found orthosnap useful, please cite *OrthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees*. Steenwyk et al. 2022, PLOS Biology. doi: [10.1371/journal.pbio.3001827](https://jlsteenwyk.com/publication_pdfs/2022_Steenwyk_etal_PLoS_Biology.pdf).
 <br /><br />
 
 ---
 
 <br />
 
 This documentation covers downloading and installing orthosnap. Details about orthosnap usage including a tutorial are available on our [online documentation](https://jlsteenwyk.com/orthosnap/).
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
                                     [Logo]
                      Docs Â· Report_Bug Â· Request_Feature
-[https://img.shields.io/github/workflow/status/jlsteenwyk/orthosnap/CI/master]
-       [https://codecov.io/gh/JLSteenwyk/orthosnap/branch/master/graph/
-   badge.svg?token=FX66FUET0L] [https://img.shields.io/github/contributors/
-                  jlsteenwyk/orthosnap] [follow_on_Twitter]
+ [https://img.shields.io/github/actions/workflow/status/JLSteenwyk/orthosnap/
+   ci.yml?branch=master] [https://codecov.io/gh/JLSteenwyk/orthosnap/branch/
+   master/graph/badge.svg?token=FX66FUET0L] [https://img.shields.io/github/
+            contributors/jlsteenwyk/orthosnap] [follow_on_Twitter]
                  [https://static.pepy.tech/personalized-badge/
 orthosnap?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPi%20Downloads]
  [https://img.shields.io/badge/License-MIT-blue.svg] [https://img.shields.io/
-                          pypi/pyversions/orthosnap]
-  [https://zenodo.org/badge/DOI/10.1101/2021.10.30.466607.svg] [Support_me_on
-                                   Patreon]
-orthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy
+       pypi/pyversions/orthosnap] [https://zenodo.org/badge/DOI/10.1371/
+                           journal.pbio.3001827.svg]
+OrthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy
 orthologs from gene family trees.
 
-If you found orthosnap useful, please cite *orthosnap: a tree splitting and
+If you found orthosnap useful, please cite *OrthoSNAP: a tree splitting and
 pruning algorithm for retrieving single-copy orthologs from gene family trees*.
-Steenwyk et al. 2021, bioRxiv. doi: [10.1101/2021.10.30.466607](https://
-www.biorxiv.org/content/10.1101/2021.10.30.466607v1).
+Steenwyk et al. 2022, PLOS Biology. doi: [10.1371/journal.pbio.3001827](https:/
+/jlsteenwyk.com/publication_pdfs/2022_Steenwyk_etal_PLoS_Biology.pdf).
 
 ---
 This documentation covers downloading and installing orthosnap. Details about
 orthosnap usage including a tutorial are available on our [online
 documentation](https://jlsteenwyk.com/orthosnap/).
 **Installation** **If you are having trouble installing orthosnap, please
 contact the lead developer, Jacob L. Steenwyk, via [email](https://
```

### Comparing `orthosnap-0.1.1/orthosnap/args_processing.py` & `orthosnap-1.0.0/orthosnap/args_processing.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,22 +45,23 @@
         sys.exit()
 
     rooted = args.rooted
     snap_trees = args.snap_trees
 
     if args.output_path:
         output_path = args.output_path
+        if not output_path.endswith("/"):
+            output_path = output_path + "/"
     else:
-        output_path = re.sub("/[^/]+$", '', fasta)
-        if not output_path:
-            output_path = "."
+        output_path = re.sub("/[^/]+$", "", fasta)
+        if output_path == fasta:
+            output_path = "./"
         elif not output_path.endswith("/"):
             output_path = output_path + "/"
 
-
     if args.inparalog_to_keep:
         inparalog_to_keep = InparalogToKeep(args.inparalog_to_keep)
     else:
         inparalog_to_keep = InparalogToKeep.longest_seq_len
 
     return dict(
         tree=tree,
```

### Comparing `orthosnap-0.1.1/orthosnap/helper.py` & `orthosnap-1.0.0/orthosnap/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,28 +24,37 @@
     """
 
     newtree.collapse_all(lambda c: c.confidence is not None and c.confidence < support)
 
     return newtree
 
 
-def determine_if_dups_are_sister(subtree_tips: list):
+def determine_if_dups_are_sister(subtree_tips: list, newtree):
     """
     determine if dups are sister to one another
     """
     # get first set of subtree tips
-    first_set_of_subtree_tips = subtree_tips[0]
+    # first_set_of_subtree_tips = subtree_tips[0]
+    # first_set_of_subtree_tips = subtree_tips
     # set if duplicate sequences are sister as True
     are_sisters = True
-    # check if duplicate sequences are sister
-    for set_of_subtree_tips in subtree_tips[1:]:
-        if first_set_of_subtree_tips != set_of_subtree_tips:
-            are_sisters = False
-        if not are_sisters:
-            break
+    # create a copy of the tree
+    dup_tree = copy.deepcopy(newtree)
+
+    dup_tree = dup_tree.common_ancestor(subtree_tips)
+    _, all_tips = get_all_tips_and_taxa_names(dup_tree)
+    if set(all_tips) != set(subtree_tips):
+        are_sisters = False
+
+    # # check if duplicate sequences are sister
+    # for set_of_subtree_tips in subtree_tips[1:]:
+    #     if first_set_of_subtree_tips != set_of_subtree_tips:
+    #         are_sisters = False
+    #     if not are_sisters:
+    #         break
 
     return are_sisters
 
 
 def get_all_tips_and_taxa_names(tree):
     """
     get all taxa and tip names in a phylogeny
@@ -150,18 +159,19 @@
 
     # remove duplicate sequences if they are sister to one another
     # following the approach in PhyloTreePruner
     for name in counts_of_taxa_from_terms:
         # if the taxon is represented by more than one sequence
         if counts_of_taxa_from_terms[name] > 1:
             # get subtree tips
-            subtree_tips, dups = get_subtree_tips(terms, name, tree)
+            _, dups = get_subtree_tips(terms, name, tree)
 
             # check if subtrees are sister to one another
-            are_sisters = determine_if_dups_are_sister(subtree_tips)
+            # are_sisters = determine_if_dups_are_sister(subtree_tips)
+            are_sisters = determine_if_dups_are_sister(dups, newtree)
 
             # if duplicate sequences are sister, get the longest sequence
             if are_sisters:
                 # trim short sequences and keep long sequences in newtree
                 newtree, terms = inparalog_to_keep_determination(
                     newtree, fasta_dict, dups, terms, inparalog_to_keep
                 )
@@ -210,15 +220,22 @@
 
     # add list of terms to assigned_tips list
     # and create subgroup fasta files
     (
         subgroup_counter,
         assigned_tips,
     ) = write_output_fasta_and_account_for_assigned_tips_single_copy_case(
-        fasta, subgroup_counter, terms, fasta_dict, assigned_tips, snap_trees, newtree, output_path
+        fasta,
+        subgroup_counter,
+        terms,
+        fasta_dict,
+        assigned_tips,
+        snap_trees,
+        newtree,
+        output_path,
     )
 
     return subgroup_counter, assigned_tips
 
 
 def inparalog_to_keep_determination(
     newtree,
@@ -226,15 +243,14 @@
     dups: list,
     terms: list,
     inparalog_to_keep: InparalogToKeep,
 ):
     """
     remove_short_sequences_among_duplicates_that_are_sister
     """
-
     lengths = dict()
     # keep inparalog based on sequence length
     if inparalog_to_keep.value in [
         "shortest_seq_len",
         "median_seq_len",
         "longest_seq_len",
     ]:
@@ -309,23 +325,26 @@
     terms: list,
     fasta_dict: dict,
     assigned_tips: list,
     snap_tree: bool,
     newtree,
     output_path: str,
 ):
-
     # write output
-    fasta_path_stripped = re.sub("^.*/", '', fasta)
-    output_file_name = f"{output_path}/{fasta_path_stripped}.orthosnap.{subgroup_counter}.fa"
+    fasta_path_stripped = re.sub("^.*/", "", fasta)
+    output_file_name = (
+        f"{output_path}/{fasta_path_stripped}.orthosnap.{subgroup_counter}.fa"
+    )
     with open(output_file_name, "w") as output_handle:
         for term in terms:
             SeqIO.write(fasta_dict[term], output_handle, "fasta")
             assigned_tips.append(term)
 
     if snap_tree:
-        output_file_name = f"{output_path}/{fasta_path_stripped}.orthosnap.{subgroup_counter}.tre"
+        output_file_name = (
+            f"{output_path}/{fasta_path_stripped}.orthosnap.{subgroup_counter}.tre"
+        )
         Phylo.write(newtree, output_file_name, "newick")
 
     subgroup_counter += 1
 
     return subgroup_counter, assigned_tips
```

### Comparing `orthosnap-0.1.1/orthosnap/orthosnap.py` & `orthosnap-1.0.0/orthosnap/orthosnap.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,22 @@
     Master execute Function
     -----------------------
     This function executes the main functions and calls other subfunctions
     """
 
     # write user args to stdout
     write_user_args(
-        tree, fasta, support, occupancy, rooted, snap_trees, inparalog_to_keep, output_path
+        tree,
+        fasta,
+        support,
+        occupancy,
+        rooted,
+        snap_trees,
+        inparalog_to_keep,
+        output_path,
     )
 
     # create start time logger
     start_time = time.time()
 
     # read input files and midpoint root tree
     tree, fasta_dict = read_input_files(tree, fasta, rooted)
```

### Comparing `orthosnap-0.1.1/orthosnap/parser.py` & `orthosnap-1.0.0/orthosnap/parser.py`

 * *Files identical despite different names*

### Comparing `orthosnap-0.1.1/orthosnap/writer.py` & `orthosnap-1.0.0/orthosnap/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,24 @@
     Taxon occupancy threshold: {occupancy}
     Output newick of SNAP-OGs: {snap_trees}
     Output directory: {output_path}
     """
         )
     )
 
+
 def write_output_stats(fasta, subgroup_counter, start_time, snap_trees, output_path):
     """
     Function to print out output statistics
     """
 
-    fasta_path_stripped = re.sub("^.*/", '', fasta)
-    output_file_name = f"{output_path}/{fasta_path_stripped}.orthosnap.{subgroup_counter}.fa"
+    fasta_path_stripped = re.sub("^.*/", "", fasta)
+    output_file_name = (
+        f"{output_path}/{fasta_path_stripped}.orthosnap.{subgroup_counter}.fa"
+    )
 
     if subgroup_counter > 0:
         print(
             textwrap.dedent(
                 f"""\
 
             ---------------------
```

### Comparing `orthosnap-0.1.1/orthosnap.egg-info/PKG-INFO` & `orthosnap-1.0.0/orthosnap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthosnap
-Version: 0.1.1
+Version: 1.0.0
 Summary: orthosnap, identify orthologous subgroups of genes in large orthologous groups of genes.
 Home-page: https://github.com/jlsteenwyk/orthosnap
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
     ·
     <a href="https://github.com/jlsteenwyk/orthosnap/issues">Report Bug</a>
     ·
     <a href="https://github.com/jlsteenwyk/orthosnap/issues">Request Feature</a>
   </p>
     <p align="center">
         <a href="https://github.com/JLSteenwyk/orthosnap/actions" alt="Build">
-            <img src="https://img.shields.io/github/workflow/status/jlsteenwyk/orthosnap/CI/master">
+            <img src="https://img.shields.io/github/actions/workflow/status/JLSteenwyk/orthosnap/ci.yml?branch=master">
         </a>
         <a href="https://codecov.io/gh/JLSteenwyk/orthosnap">
           <img src="https://codecov.io/gh/JLSteenwyk/orthosnap/branch/master/graph/badge.svg?token=FX66FUET0L"/>
         </a>
         <a href="https://github.com/jlsteenwyk/orthosnap/graphs/contributors" alt="Contributors">
             <img src="https://img.shields.io/github/contributors/jlsteenwyk/orthosnap">
         </a>
@@ -48,24 +48,21 @@
         </a>
         <a href="https://lbesson.mit-license.org/" alt="License">
             <img src="https://img.shields.io/badge/License-MIT-blue.svg">
         </a>
         <a href="https://pypi.org/project/orthosnap/" alt="PyPI - Python Version">
             <img src="https://img.shields.io/pypi/pyversions/orthosnap">
         </a>
-        <br />
-        <a href="https://www.biorxiv.org/content/10.1101/2021.10.30.466607">
-          <img src="https://zenodo.org/badge/DOI/10.1101/2021.10.30.466607.svg">
-        </a>
-        <a href="https://patreon.com/jlsteenwyk"><img src="https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Djlsteenwyk%26type%3Dpatrons&style=flat" alt="Support me on Patreon" /></a>
+        <a href="https://jlsteenwyk.com/publication_pdfs/2022_Steenwyk_etal_PLoS_Biology.pdf">
+          <img src="https://zenodo.org/badge/DOI/10.1371/journal.pbio.3001827.svg">
     </p>
 </p>
 
-orthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees.<br /><br />
-If you found orthosnap useful, please cite *orthosnap: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees*. Steenwyk et al. 2021, bioRxiv. doi: [10.1101/2021.10.30.466607](https://www.biorxiv.org/content/10.1101/2021.10.30.466607v1).
+OrthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees.<br /><br />
+If you found orthosnap useful, please cite *OrthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy orthologs from gene family trees*. Steenwyk et al. 2022, PLOS Biology. doi: [10.1371/journal.pbio.3001827](https://jlsteenwyk.com/publication_pdfs/2022_Steenwyk_etal_PLoS_Biology.pdf).
 <br /><br />
 
 ---
 
 <br />
 
 This documentation covers downloading and installing orthosnap. Details about orthosnap usage including a tutorial are available on our [online documentation](https://jlsteenwyk.com/orthosnap/).
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: orthosnap Version: 0.1.1 Summary: orthosnap,
+Metadata-Version: 2.1 Name: orthosnap Version: 1.0.0 Summary: orthosnap,
 identify orthologous subgroups of genes in large orthologous groups of genes.
 Home-page: https://github.com/jlsteenwyk/orthosnap Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com License: UNKNOWN Platform: UNKNOWN
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Science/Research Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Scientific/Engineering Description-Content-Type: text/markdown
 License-File: LICENSE.md
                                     [Logo]
                      Docs Â· Report_Bug Â· Request_Feature
-[https://img.shields.io/github/workflow/status/jlsteenwyk/orthosnap/CI/master]
-       [https://codecov.io/gh/JLSteenwyk/orthosnap/branch/master/graph/
-   badge.svg?token=FX66FUET0L] [https://img.shields.io/github/contributors/
-                  jlsteenwyk/orthosnap] [follow_on_Twitter]
+ [https://img.shields.io/github/actions/workflow/status/JLSteenwyk/orthosnap/
+   ci.yml?branch=master] [https://codecov.io/gh/JLSteenwyk/orthosnap/branch/
+   master/graph/badge.svg?token=FX66FUET0L] [https://img.shields.io/github/
+            contributors/jlsteenwyk/orthosnap] [follow_on_Twitter]
                  [https://static.pepy.tech/personalized-badge/
 orthosnap?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPi%20Downloads]
  [https://img.shields.io/badge/License-MIT-blue.svg] [https://img.shields.io/
-                          pypi/pyversions/orthosnap]
-  [https://zenodo.org/badge/DOI/10.1101/2021.10.30.466607.svg] [Support_me_on
-                                   Patreon]
-orthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy
+       pypi/pyversions/orthosnap] [https://zenodo.org/badge/DOI/10.1371/
+                           journal.pbio.3001827.svg]
+OrthoSNAP: a tree splitting and pruning algorithm for retrieving single-copy
 orthologs from gene family trees.
 
-If you found orthosnap useful, please cite *orthosnap: a tree splitting and
+If you found orthosnap useful, please cite *OrthoSNAP: a tree splitting and
 pruning algorithm for retrieving single-copy orthologs from gene family trees*.
-Steenwyk et al. 2021, bioRxiv. doi: [10.1101/2021.10.30.466607](https://
-www.biorxiv.org/content/10.1101/2021.10.30.466607v1).
+Steenwyk et al. 2022, PLOS Biology. doi: [10.1371/journal.pbio.3001827](https:/
+/jlsteenwyk.com/publication_pdfs/2022_Steenwyk_etal_PLoS_Biology.pdf).
 
 ---
 This documentation covers downloading and installing orthosnap. Details about
 orthosnap usage including a tutorial are available on our [online
 documentation](https://jlsteenwyk.com/orthosnap/).
 **Installation** **If you are having trouble installing orthosnap, please
 contact the lead developer, Jacob L. Steenwyk, via [email](https://
```

### Comparing `orthosnap-0.1.1/setup.py` & `orthosnap-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,11 +32,11 @@
     classifiers=CLASSIFIERS,
     entry_points={"console_scripts": ["orthosnap = orthosnap.orthosnap:main"]},
     version=__version__,
     include_package_data=True,
     install_requires=REQUIRES,
 )
 
-## push new version to pypi
+# push new version to pypi
 # rm -rf dist
 # python3 setup.py sdist bdist_wheel --universal
 # twine upload dist/* -r pypi
```

