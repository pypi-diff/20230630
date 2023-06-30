# Comparing `tmp/riptide-3.4.81.tar.gz` & `tmp/riptide-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riptide-3.4.81.tar", last modified: Fri Jun 30 12:58:48 2023, max compression
+gzip compressed data, was "riptide-3.4.9.tar", last modified: Tue Dec  6 17:57:22 2022, max compression
```

## Comparing `riptide-3.4.81.tar` & `riptide-3.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mjenior    (503) staff       (20)        0 2023-06-30 12:58:48.167519 riptide-3.4.81/
--rwxrwxrwx   0 mjenior    (503) staff       (20)     1071 2022-09-29 21:58:44.000000 riptide-3.4.81/LICENSE.txt
--rwxrwxrwx   0 mjenior    (503) staff       (20)       28 2022-09-29 21:58:44.000000 riptide-3.4.81/MANIFEST.in
--rw-r--r--   0 mjenior    (503) staff       (20)    12295 2023-06-30 12:58:48.167043 riptide-3.4.81/PKG-INFO
--rwxrwxrwx   0 mjenior    (503) staff       (20)    11750 2023-06-30 12:44:25.000000 riptide-3.4.81/README.md
--rwxrwxrwx   0 mjenior    (503) staff       (20)      683 2023-06-30 12:44:04.000000 riptide-3.4.81/pyproject.toml
--rw-r--r--   0 mjenior    (503) staff       (20)       38 2023-06-30 12:58:48.167682 riptide-3.4.81/setup.cfg
-drwxr-xr-x   0 mjenior    (503) staff       (20)        0 2023-06-30 12:58:48.162917 riptide-3.4.81/src/
--rwxrwxrwx   0 mjenior    (503) staff       (20)       80 2022-09-29 21:58:44.000000 riptide-3.4.81/src/__init__.py
-drwxr-xr-x   0 mjenior    (503) staff       (20)        0 2023-06-30 12:58:48.166393 riptide-3.4.81/src/riptide.egg-info/
--rw-r--r--   0 mjenior    (503) staff       (20)    12295 2023-06-30 12:58:48.000000 riptide-3.4.81/src/riptide.egg-info/PKG-INFO
--rw-r--r--   0 mjenior    (503) staff       (20)      219 2023-06-30 12:58:48.000000 riptide-3.4.81/src/riptide.egg-info/SOURCES.txt
--rw-r--r--   0 mjenior    (503) staff       (20)        1 2023-06-30 12:58:48.000000 riptide-3.4.81/src/riptide.egg-info/dependency_links.txt
--rw-r--r--   0 mjenior    (503) staff       (20)       17 2023-06-30 12:58:48.000000 riptide-3.4.81/src/riptide.egg-info/top_level.txt
--rwxrwxrwx   0 mjenior    (503) staff       (20)    55250 2023-06-30 12:43:38.000000 riptide-3.4.81/src/riptide.py
+drwxr-xr-x   0 mjenior    (502) staff       (20)        0 2022-12-06 17:57:22.920498 riptide-3.4.9/
+-rw-r--r--   0 mjenior    (502) staff       (20)     1071 2022-09-29 21:58:44.000000 riptide-3.4.9/LICENSE.txt
+-rw-r--r--   0 mjenior    (502) staff       (20)       28 2022-09-29 21:58:44.000000 riptide-3.4.9/MANIFEST.in
+-rw-r--r--   0 mjenior    (502) staff       (20)    12304 2022-12-06 17:57:22.920147 riptide-3.4.9/PKG-INFO
+-rw-r--r--   0 mjenior    (502) staff       (20)    11760 2022-12-05 23:22:50.000000 riptide-3.4.9/README.md
+-rw-r--r--   0 mjenior    (502) staff       (20)      682 2022-12-06 17:57:13.000000 riptide-3.4.9/pyproject.toml
+-rw-r--r--   0 mjenior    (502) staff       (20)       38 2022-12-06 17:57:22.920603 riptide-3.4.9/setup.cfg
+drwxr-xr-x   0 mjenior    (502) staff       (20)        0 2022-12-06 17:57:22.918229 riptide-3.4.9/src/
+-rw-r--r--   0 mjenior    (502) staff       (20)       80 2022-09-29 21:58:44.000000 riptide-3.4.9/src/__init__.py
+drwxr-xr-x   0 mjenior    (502) staff       (20)        0 2022-12-06 17:57:22.919698 riptide-3.4.9/src/riptide.egg-info/
+-rw-r--r--   0 mjenior    (502) staff       (20)    12304 2022-12-06 17:57:22.000000 riptide-3.4.9/src/riptide.egg-info/PKG-INFO
+-rw-r--r--   0 mjenior    (502) staff       (20)      219 2022-12-06 17:57:22.000000 riptide-3.4.9/src/riptide.egg-info/SOURCES.txt
+-rw-r--r--   0 mjenior    (502) staff       (20)        1 2022-12-06 17:57:22.000000 riptide-3.4.9/src/riptide.egg-info/dependency_links.txt
+-rw-r--r--   0 mjenior    (502) staff       (20)       17 2022-12-06 17:57:22.000000 riptide-3.4.9/src/riptide.egg-info/top_level.txt
+-rw-r--r--   0 mjenior    (502) staff       (20)    49922 2022-12-06 17:56:41.000000 riptide-3.4.9/src/riptide.py
```

### Comparing `riptide-3.4.81/LICENSE.txt` & `riptide-3.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `riptide-3.4.81/PKG-INFO` & `riptide-3.4.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riptide
-Version: 3.4.81
+Version: 3.4.9
 Summary: Reaction Inclusion by Parsimony and Transcript Distribution (RIPTiDe)
 Author-email: Matthew Jenior <mattjenior@gmail.com>
 Project-URL: Homepage, https://github.com/mjenior/riptide
 Project-URL: Bug Tracker, https://github.com/mjenior/riptide/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # RIPTiDe
 
 **R**eaction **I**nclusion by **P**arsimony and **T**ranscript **D**istribution
 
-v3.4.81
+v3.4.2
+----
 
 Transcriptomic analyses of bacteria have become instrumental to our understanding of their responses to changes in their environment. While traditional analyses have been informative, leveraging these datasets within genome-scale metabolic network reconstructions (GENREs) can provide greatly improved context for shifts in pathway utilization and downstream/upstream ramifications for changes in metabolic regulation. Many previous techniques for GENRE transcript integration have focused on creating maximum consensus with input datasets, but these approaches have been shown to generate less accurate metabolic predictions than a transcript-agnostic method of flux minimization (pFBA), which identifies the most efficient/economic patterns of metabolism given certain growth constraints. Despite this success, growth conditions are not always easily quantifiable and highlights the need for novel platforms that build from these findings. This method, known as RIPTiDe, combines these concepts and utilizes overall minimization of flux weighted by transcriptomic analysis to identify the most energy efficient pathways to achieve growth that include more highly transcribed enzymes, without previous insight into extracellular conditions. This platform could be important for revealing context-specific bacterial phenotypes in line with governing principles of adaptive evolution, that drive disease manifestation or interactions between microbes.
 
 Please cite when using:
 ```
 Jenior ML, Moutinho Jr TJ, Dougherty BV, & Papin JA. (2020). Transcriptome-guided parsimonious flux analysis improves predictions with metabolic networks in complex environments. PLOS Comp Biol. https://doi.org/10.1371/journal.pcbi.1007099.
 ```
@@ -43,15 +44,15 @@
 
 ### Arguments for core RIPTiDe functions:
 
 **riptide.read_transcription_file() - Generates dictionary of transcriptomic abundances from a file**
 ```
 REQUIRED
 file : string
-    User-provided file name which contains gene IDs as rows and associated transcription values as columns per replicate
+    User-provided file name which contains gene IDs and associated transcription values
 
 OPTIONAL
 header : boolean
     Defines if read abundance file has a header that needs to be ignored
     Default is no header
 sep: string
     Defines what character separates entries on each line
@@ -77,40 +78,34 @@
     Default is 0.125
 norm : bool
     Normalize transcript abundances using RPM calculation
     Performed by default
 factor : numeric
     Denominator for read normalization calculation
     Default is 1e6 (RPM)
-silent  : bool
-    Silences std out 
-    Default is False
 ```
 
-**riptide.maxfit() - Create context-specific model based on transcript distribution with maximum fit of flux distribution to input transctiptome**
+**riptide.contextualize() - Create context-specific model based on transcript distribution with maximum fit of flux distribution to input transctiptome**
 ```
 REQUIRED
 model : cobra.Model
     The model to be contextualized
 transcriptome : dictionary
     Dictionary of transcript abundances, output of read_transcription_file()
 
 OPTIONAL
+cpus  : int
+    CPUs number for parallelization
+    Default is all available 
 frac_min : float
     Lower bound for range of minimal fractions to test
     Default is 0.25
 frac_max : float
     Upper bound for range of minimal fractions to test
     Default is 0.85
-frac_step : float
-    Starting interval size within fraction range
-    Default is 0.1
-prune : bool
-    Perform pruning step
-    Default is True
 samples : int 
     Number of flux samples to collect
     Default is 500
 silent  : bool
     Silences std out 
     Default is False
 minimum : float
@@ -121,40 +116,46 @@
     Default is False
 objective : bool
     Sets previous objective function as a constraint with minimum flux equal to user input fraction
     Default is True
 additive : bool
     Pool transcription abundances for reactions with multiple contributing gene products
     Default is False
+important : list
+    List of gene or reaction ID strings for which the highest weights are assigned regardless of transcription
+    Default is False
 direct : bool
     Assigns both minimization and maximization step coefficents directly, instead of relying on abundance distribution
     Default is False
 set_bounds : bool
     Uses flux variability analysis results from constrained model to set new bounds for all reactions
     Default is True
 tasks : list
     List of gene or reaction ID strings for forced inclusion in final model (metabolic tasks or essential genes)
-task_lb : float
-    Minimum flux bound for metabolic task reactions during pruning
-    Default is equal to threshold var
 exclude : list
     List of reaction ID strings for forced exclusion from final model
 gpr : bool
     Determines if GPR rules will be considered during coefficient assignment
     Default is False
 threshold : float
     Minimum flux a reaction must acheive in order to avoid pruning during flux sum minimization step
-    Default is 1e-8
+    Default is 1e-6
 defined : False or list
     User defined range of linear coeffients, needs to be defined in a list like [1, 0.5, 0.1, 0.01, 0.001]
     Works best paired with binned abundance catagories from riptide.read_transcription_file()
     Default is False
+open_exchanges : bool
+    Sets all exchange reactions bounds to (-1000., 1000.)
+    Default is False
+skip_fva : bool
+    Skips final flux variability analysis
+    Default is False
 ```
 
-**riptide.contextualize() - Create context-specific model based on transcript distribution with user-defined objective flux minimum**
+**riptide.single_contextualize() - Create context-specific model based on transcript distribution with user-defined objective flux minimum**
 ```
 REQUIRED
 model : cobra.Model
     The model to be contextualized
 
 OPTIONAL
 transcriptome : dictionary
@@ -176,17 +177,14 @@
 OPTIONAL
 path : str
     New directory to write output files
 file_type : str
     Type of output file for RIPTiDe model
     Accepts either sbml or json
     Default is JSON
-silent  : bool
-    Silences std out 
-    Default is False
 ```
 
 ## Usage
 
 **Comments before starting:** 
 - Make sure that genes in the transcriptome file matches those that are in your model.
 - Check the example files for proper data formatting
@@ -264,11 +262,10 @@
 context_specific_flux_samples = riptide_object.flux_samples
 ```
 
 ## Additional Information
 
 Thank you for your interest in RIPTiDe!
 
-
 If you encounter any problems, please [file an issue](https://github.com/mjenior/riptide/issues) along with a detailed description.
 
 Distributed under the terms of the [MIT](http://opensource.org/licenses/MIT) license, "riptide" is free and open source software
```

### Comparing `riptide-3.4.81/README.md` & `riptide-3.4.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # RIPTiDe
 
 **R**eaction **I**nclusion by **P**arsimony and **T**ranscript **D**istribution
 
-v3.4.81
+v3.4.2
+----
 
 Transcriptomic analyses of bacteria have become instrumental to our understanding of their responses to changes in their environment. While traditional analyses have been informative, leveraging these datasets within genome-scale metabolic network reconstructions (GENREs) can provide greatly improved context for shifts in pathway utilization and downstream/upstream ramifications for changes in metabolic regulation. Many previous techniques for GENRE transcript integration have focused on creating maximum consensus with input datasets, but these approaches have been shown to generate less accurate metabolic predictions than a transcript-agnostic method of flux minimization (pFBA), which identifies the most efficient/economic patterns of metabolism given certain growth constraints. Despite this success, growth conditions are not always easily quantifiable and highlights the need for novel platforms that build from these findings. This method, known as RIPTiDe, combines these concepts and utilizes overall minimization of flux weighted by transcriptomic analysis to identify the most energy efficient pathways to achieve growth that include more highly transcribed enzymes, without previous insight into extracellular conditions. This platform could be important for revealing context-specific bacterial phenotypes in line with governing principles of adaptive evolution, that drive disease manifestation or interactions between microbes.
 
 Please cite when using:
 ```
 Jenior ML, Moutinho Jr TJ, Dougherty BV, & Papin JA. (2020). Transcriptome-guided parsimonious flux analysis improves predictions with metabolic networks in complex environments. PLOS Comp Biol. https://doi.org/10.1371/journal.pcbi.1007099.
 ```
@@ -29,15 +30,15 @@
 
 ### Arguments for core RIPTiDe functions:
 
 **riptide.read_transcription_file() - Generates dictionary of transcriptomic abundances from a file**
 ```
 REQUIRED
 file : string
-    User-provided file name which contains gene IDs as rows and associated transcription values as columns per replicate
+    User-provided file name which contains gene IDs and associated transcription values
 
 OPTIONAL
 header : boolean
     Defines if read abundance file has a header that needs to be ignored
     Default is no header
 sep: string
     Defines what character separates entries on each line
@@ -63,40 +64,34 @@
     Default is 0.125
 norm : bool
     Normalize transcript abundances using RPM calculation
     Performed by default
 factor : numeric
     Denominator for read normalization calculation
     Default is 1e6 (RPM)
-silent  : bool
-    Silences std out 
-    Default is False
 ```
 
-**riptide.maxfit() - Create context-specific model based on transcript distribution with maximum fit of flux distribution to input transctiptome**
+**riptide.contextualize() - Create context-specific model based on transcript distribution with maximum fit of flux distribution to input transctiptome**
 ```
 REQUIRED
 model : cobra.Model
     The model to be contextualized
 transcriptome : dictionary
     Dictionary of transcript abundances, output of read_transcription_file()
 
 OPTIONAL
+cpus  : int
+    CPUs number for parallelization
+    Default is all available 
 frac_min : float
     Lower bound for range of minimal fractions to test
     Default is 0.25
 frac_max : float
     Upper bound for range of minimal fractions to test
     Default is 0.85
-frac_step : float
-    Starting interval size within fraction range
-    Default is 0.1
-prune : bool
-    Perform pruning step
-    Default is True
 samples : int 
     Number of flux samples to collect
     Default is 500
 silent  : bool
     Silences std out 
     Default is False
 minimum : float
@@ -107,40 +102,46 @@
     Default is False
 objective : bool
     Sets previous objective function as a constraint with minimum flux equal to user input fraction
     Default is True
 additive : bool
     Pool transcription abundances for reactions with multiple contributing gene products
     Default is False
+important : list
+    List of gene or reaction ID strings for which the highest weights are assigned regardless of transcription
+    Default is False
 direct : bool
     Assigns both minimization and maximization step coefficents directly, instead of relying on abundance distribution
     Default is False
 set_bounds : bool
     Uses flux variability analysis results from constrained model to set new bounds for all reactions
     Default is True
 tasks : list
     List of gene or reaction ID strings for forced inclusion in final model (metabolic tasks or essential genes)
-task_lb : float
-    Minimum flux bound for metabolic task reactions during pruning
-    Default is equal to threshold var
 exclude : list
     List of reaction ID strings for forced exclusion from final model
 gpr : bool
     Determines if GPR rules will be considered during coefficient assignment
     Default is False
 threshold : float
     Minimum flux a reaction must acheive in order to avoid pruning during flux sum minimization step
-    Default is 1e-8
+    Default is 1e-6
 defined : False or list
     User defined range of linear coeffients, needs to be defined in a list like [1, 0.5, 0.1, 0.01, 0.001]
     Works best paired with binned abundance catagories from riptide.read_transcription_file()
     Default is False
+open_exchanges : bool
+    Sets all exchange reactions bounds to (-1000., 1000.)
+    Default is False
+skip_fva : bool
+    Skips final flux variability analysis
+    Default is False
 ```
 
-**riptide.contextualize() - Create context-specific model based on transcript distribution with user-defined objective flux minimum**
+**riptide.single_contextualize() - Create context-specific model based on transcript distribution with user-defined objective flux minimum**
 ```
 REQUIRED
 model : cobra.Model
     The model to be contextualized
 
 OPTIONAL
 transcriptome : dictionary
@@ -162,17 +163,14 @@
 OPTIONAL
 path : str
     New directory to write output files
 file_type : str
     Type of output file for RIPTiDe model
     Accepts either sbml or json
     Default is JSON
-silent  : bool
-    Silences std out 
-    Default is False
 ```
 
 ## Usage
 
 **Comments before starting:** 
 - Make sure that genes in the transcriptome file matches those that are in your model.
 - Check the example files for proper data formatting
@@ -250,11 +248,10 @@
 context_specific_flux_samples = riptide_object.flux_samples
 ```
 
 ## Additional Information
 
 Thank you for your interest in RIPTiDe!
 
-
 If you encounter any problems, please [file an issue](https://github.com/mjenior/riptide/issues) along with a detailed description.
 
 Distributed under the terms of the [MIT](http://opensource.org/licenses/MIT) license, "riptide" is free and open source software
```

### Comparing `riptide-3.4.81/pyproject.toml` & `riptide-3.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "riptide"
-version = "3.4.81"
+version = "3.4.9"
 authors = [
   { name="Matthew Jenior", email="mattjenior@gmail.com" },
 ]
 description = "Reaction Inclusion by Parsimony and Transcript Distribution (RIPTiDe)"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `riptide-3.4.81/src/riptide.egg-info/PKG-INFO` & `riptide-3.4.9/src/riptide.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riptide
-Version: 3.4.81
+Version: 3.4.9
 Summary: Reaction Inclusion by Parsimony and Transcript Distribution (RIPTiDe)
 Author-email: Matthew Jenior <mattjenior@gmail.com>
 Project-URL: Homepage, https://github.com/mjenior/riptide
 Project-URL: Bug Tracker, https://github.com/mjenior/riptide/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # RIPTiDe
 
 **R**eaction **I**nclusion by **P**arsimony and **T**ranscript **D**istribution
 
-v3.4.81
+v3.4.2
+----
 
 Transcriptomic analyses of bacteria have become instrumental to our understanding of their responses to changes in their environment. While traditional analyses have been informative, leveraging these datasets within genome-scale metabolic network reconstructions (GENREs) can provide greatly improved context for shifts in pathway utilization and downstream/upstream ramifications for changes in metabolic regulation. Many previous techniques for GENRE transcript integration have focused on creating maximum consensus with input datasets, but these approaches have been shown to generate less accurate metabolic predictions than a transcript-agnostic method of flux minimization (pFBA), which identifies the most efficient/economic patterns of metabolism given certain growth constraints. Despite this success, growth conditions are not always easily quantifiable and highlights the need for novel platforms that build from these findings. This method, known as RIPTiDe, combines these concepts and utilizes overall minimization of flux weighted by transcriptomic analysis to identify the most energy efficient pathways to achieve growth that include more highly transcribed enzymes, without previous insight into extracellular conditions. This platform could be important for revealing context-specific bacterial phenotypes in line with governing principles of adaptive evolution, that drive disease manifestation or interactions between microbes.
 
 Please cite when using:
 ```
 Jenior ML, Moutinho Jr TJ, Dougherty BV, & Papin JA. (2020). Transcriptome-guided parsimonious flux analysis improves predictions with metabolic networks in complex environments. PLOS Comp Biol. https://doi.org/10.1371/journal.pcbi.1007099.
 ```
@@ -43,15 +44,15 @@
 
 ### Arguments for core RIPTiDe functions:
 
 **riptide.read_transcription_file() - Generates dictionary of transcriptomic abundances from a file**
 ```
 REQUIRED
 file : string
-    User-provided file name which contains gene IDs as rows and associated transcription values as columns per replicate
+    User-provided file name which contains gene IDs and associated transcription values
 
 OPTIONAL
 header : boolean
     Defines if read abundance file has a header that needs to be ignored
     Default is no header
 sep: string
     Defines what character separates entries on each line
@@ -77,40 +78,34 @@
     Default is 0.125
 norm : bool
     Normalize transcript abundances using RPM calculation
     Performed by default
 factor : numeric
     Denominator for read normalization calculation
     Default is 1e6 (RPM)
-silent  : bool
-    Silences std out 
-    Default is False
 ```
 
-**riptide.maxfit() - Create context-specific model based on transcript distribution with maximum fit of flux distribution to input transctiptome**
+**riptide.contextualize() - Create context-specific model based on transcript distribution with maximum fit of flux distribution to input transctiptome**
 ```
 REQUIRED
 model : cobra.Model
     The model to be contextualized
 transcriptome : dictionary
     Dictionary of transcript abundances, output of read_transcription_file()
 
 OPTIONAL
+cpus  : int
+    CPUs number for parallelization
+    Default is all available 
 frac_min : float
     Lower bound for range of minimal fractions to test
     Default is 0.25
 frac_max : float
     Upper bound for range of minimal fractions to test
     Default is 0.85
-frac_step : float
-    Starting interval size within fraction range
-    Default is 0.1
-prune : bool
-    Perform pruning step
-    Default is True
 samples : int 
     Number of flux samples to collect
     Default is 500
 silent  : bool
     Silences std out 
     Default is False
 minimum : float
@@ -121,40 +116,46 @@
     Default is False
 objective : bool
     Sets previous objective function as a constraint with minimum flux equal to user input fraction
     Default is True
 additive : bool
     Pool transcription abundances for reactions with multiple contributing gene products
     Default is False
+important : list
+    List of gene or reaction ID strings for which the highest weights are assigned regardless of transcription
+    Default is False
 direct : bool
     Assigns both minimization and maximization step coefficents directly, instead of relying on abundance distribution
     Default is False
 set_bounds : bool
     Uses flux variability analysis results from constrained model to set new bounds for all reactions
     Default is True
 tasks : list
     List of gene or reaction ID strings for forced inclusion in final model (metabolic tasks or essential genes)
-task_lb : float
-    Minimum flux bound for metabolic task reactions during pruning
-    Default is equal to threshold var
 exclude : list
     List of reaction ID strings for forced exclusion from final model
 gpr : bool
     Determines if GPR rules will be considered during coefficient assignment
     Default is False
 threshold : float
     Minimum flux a reaction must acheive in order to avoid pruning during flux sum minimization step
-    Default is 1e-8
+    Default is 1e-6
 defined : False or list
     User defined range of linear coeffients, needs to be defined in a list like [1, 0.5, 0.1, 0.01, 0.001]
     Works best paired with binned abundance catagories from riptide.read_transcription_file()
     Default is False
+open_exchanges : bool
+    Sets all exchange reactions bounds to (-1000., 1000.)
+    Default is False
+skip_fva : bool
+    Skips final flux variability analysis
+    Default is False
 ```
 
-**riptide.contextualize() - Create context-specific model based on transcript distribution with user-defined objective flux minimum**
+**riptide.single_contextualize() - Create context-specific model based on transcript distribution with user-defined objective flux minimum**
 ```
 REQUIRED
 model : cobra.Model
     The model to be contextualized
 
 OPTIONAL
 transcriptome : dictionary
@@ -176,17 +177,14 @@
 OPTIONAL
 path : str
     New directory to write output files
 file_type : str
     Type of output file for RIPTiDe model
     Accepts either sbml or json
     Default is JSON
-silent  : bool
-    Silences std out 
-    Default is False
 ```
 
 ## Usage
 
 **Comments before starting:** 
 - Make sure that genes in the transcriptome file matches those that are in your model.
 - Check the example files for proper data formatting
@@ -264,11 +262,10 @@
 context_specific_flux_samples = riptide_object.flux_samples
 ```
 
 ## Additional Information
 
 Thank you for your interest in RIPTiDe!
 
-
 If you encounter any problems, please [file an issue](https://github.com/mjenior/riptide/issues) along with a detailed description.
 
 Distributed under the terms of the [MIT](http://opensource.org/licenses/MIT) license, "riptide" is free and open source software
```

### Comparing `riptide-3.4.81/src/riptide.py` & `riptide-3.4.9/src/riptide.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#!/usr/bin/env python3
+#!/usr/bin/python
 
 import os
 import sys
+import copy
 import time
 import numpy
+import cobra
 import bisect
 import pandas
 import warnings
-from random import seed
-from copy import deepcopy
-from datetime import datetime
-
-import cobra
 import symengine
+import concurrent.futures
+from concurrent.futures import ProcessPoolExecutor
+from random import seed
 from cobra.util import solver
 from scipy.stats import spearmanr
 from numpy.random import permutation
 from cobra.flux_analysis import flux_variability_analysis
 
 
 # Create a class to house riptide output data
@@ -24,68 +24,57 @@
     def __init__(self):
         self.model = 'NULL'
         self.transcriptome = 'NULL'
         self.minimization_coefficients = 'NULL'
         self.maximization_coefficients = 'NULL'
         self.pruned = 'NULL'
         self.flux_samples = 'NULL'
+        self.flux_variability = 'NULL'
         self.fraction_of_optimum = 'NULL'
         self.metabolic_tasks = 'NULL'
         self.concordance = 'NULL'
         self.gpr_integration = 'NULL'
         self.percent_of_mapping = 'NULL'
+        self.included_important = 'NULL'
         self.additional_parameters = 'NULL'
         self.fraction_bounds = 'NULL'
         self.maxfit = False
 
 
 # Save the output of RIPTiDe in a newly created directory
-def save_output(riptide_obj='NULL', path='NULL', file_type='JSON', silent=False):
+def save_output(riptide_obj='NULL', path='NULL', file_type='JSON'):
     '''Writes RIPTiDe results to files in a new directory
     
     Parameters
     ----------
 
     REQUIRED
     riptide_obj : RIPTiDe object
-        Class object created by riptide.contextualize() or riptide.maxfit()
+        Class object created by riptide.contextualize()
 
     OPTIONAL
     path : str
         New directory to write output files
     file_type : str
         Type of output file for RIPTiDe model
         Accepts either sbml or json
         Default is JSON
-    silent : bool
-        Silences std out 
-        Default is False
     '''
 
     if riptide_obj == 'NULL':
         raise ValueError('ERROR: Did not provide a RIPTiDe object')
     
-    curr_wd = str(os.getcwd())
     if path == 'NULL':
-        if silent == False:
-            print('WARNING: Did not provide an output directory. Using default riptide_files in working directory')
-        path = curr_wd + '/' + riptide_obj.model.id + '_' + riptide_obj.run_start
-    else:
-        path = path + '_' + riptide_obj.run_start
+        print('WARNING: Did not provide an output directory. Using default riptide_files in working directory')
+        path = 'riptide_files'
     try:
-        # Recursively build dirs if possible
         os.mkdir(path)
-        if silent == False: print('Saving results to', path)
     except:
-        if silent == False:
-            print('WARNING: Output path already exists, overwriting previous files')
+        print('WARNING: Output path already exists, overwriting previous files')
         pass
-    
-    if silent == False:
-        print('Saving results to', path)
 
     # Write model to file
     if file_type.upper() == 'JSON':
         outFile = path + '/model.json'
         cobra.io.save_json_model(riptide_obj.model, outFile)
     else:
         outFile = path + '/model.sbml'
@@ -101,14 +90,17 @@
                 abund = '\t'.join([str(x) for x in riptide_obj.transcriptome[gene]])
                 transcription.write(gene + '\t' + abund + '\n')
 
     # Write flux samples and FVA to a tsv
     if isinstance(riptide_obj.flux_samples, str) == False:
         outFile = path + '/flux_samples.tsv'
         riptide_obj.flux_samples.to_csv(outFile, sep='\t')
+    if isinstance(riptide_obj.flux_variability, str) == False:
+        outFile = path + '/flux_variability.tsv'
+        riptide_obj.flux_variability.to_csv(outFile, sep='\t')
 
     # Write coefficient dictionaries to tsvs
     outFile = path + '/flux_minimization_coefficients.tsv'
     with open(outFile, 'w') as min_coefficients:
         min_coefficients.write('reaction\tlinear_coefficient\n')
         for rxn in riptide_obj.minimization_coefficients.keys():
             min_coefficients.write(rxn + '\t' + str(riptide_obj.minimization_coefficients[rxn]) + '\n')
@@ -128,21 +120,17 @@
 
     # Save some information from all results from maxfit iterations
     if riptide_obj.maxfit == True:
         outFile = path + '/maxfit_iters.tsv'
         with open(outFile, 'w') as maxfit:
             maxfit.write('opt_fraction\tR_value\tp_value\n')
             for index in riptide_obj.maxfit_report.keys():
-                try:
-                    line = str(index) + '\t' + str(riptide_obj.maxfit_report[index]['r']) + '\t' + str(riptide_obj.maxfit_report[index]['p']) + '\n'
-                except:
-                    line = str(index) + '\t' + str(riptide_obj.maxfit_report[index]) + '\t' '\n'
+                line = str(index) + '\t' + str(riptide_obj.maxfit_report[index]['r']) + '\t' + str(riptide_obj.maxfit_report[index]['p']) + '\n'
                 maxfit.write(line)
 
-
     # Assemble parameters and output metrics text file
     outFile = path + '/parameters.txt'
     with open(outFile, 'w') as parameters:
         # Parameters
         parameters.write('Fraction of optimum objective value: ' + str(riptide_obj.fraction_of_optimum) + '\n')
         parameters.write('Percent of genes in mapping found in model: ' + str(riptide_obj.percent_of_mapping) + '\n')
         parameters.write('Minimum flux to avoid pruning: ' + str(riptide_obj.additional_parameters['threshold']) + '\n')
@@ -167,14 +155,18 @@
             parameters.write('Conservative pruning based on GPR: Yes\n')
         else:
             parameters.write('Conservative pruning based on GPR: No\n')
         if riptide_obj.additional_parameters['additive'] == True:
             parameters.write('Pooled transcript based on GPR: Yes\n')
         else:
             parameters.write('Pooled transcript based on GPR: No\n')
+        if riptide_obj.additional_parameters['open_exchanges'] == True:
+            parameters.write('Exchange reactions switched open: Yes\n')
+        else:
+            parameters.write('Exchange reactions switched open: No\n')
         if riptide_obj.additional_parameters['silent'] == True:
             parameters.write('Run in silent mode: Yes\n')
         else:
             parameters.write('Run in silent mode: No\n\n')
         if riptide_obj.fraction_bounds != 'NULL':
              parameters.write('Max fit optimal fraction lower bound: ' + str(riptide_obj.fraction_bounds[0]) + '\n')
              parameters.write('Max fit optimal fraction upper bound: ' + str(riptide_obj.fraction_bounds[1]) + '\n')
@@ -190,15 +182,15 @@
                 p_val = round(riptide_obj.concordance['p'], 4)
                 parameters.write('Correlation between activity and transcriptome: R=' + str(r_val) + ', p-value=' + str(p_val) + '\n')
         parameters.write('RIPTiDe run time: ' + str(riptide_obj.additional_parameters['operation']['run_time']) + ' seconds\n')
         
 
 # Read in transcriptomic read abundances, default is tsv with no header 
 def read_transcription_file(file, header = False, sep = '\t', rarefy = False, level = 'default',
-    binning = False, quant_max = 0.9, quant_min = 0.5, step = 0.125, norm = True, factor = 1e6, silent=False):
+    binning = False, quant_max = 0.9, quant_min = 0.5, step = 0.125, norm = True, factor = 1e6):
     '''Generates dictionary of transcriptomic abundances from a file
     
     Parameters
     ----------
 
     REQUIRED
     file : string
@@ -232,17 +224,14 @@
         Default is 0.125
     norm : bool
         Normalize transcript abundances using RPM calculation
         Performed by default
     factor : numeric
         Denominator for read normalization calculation
         Default is 1e6 (RPM)
-    silent : bool
-        Silences std out 
-        Default is False
     '''
 
     # Correct some possible user error
     if quant_max >= 1.0 or quant_max <= 0.0: quant_max = 0.99
     if quant_min <= 0.0 or quant_min >= 1.0: quant_min = 0.01
     if step <= 0.0 or step >= 1.0: step = 0.125
     if factor < 1: factor = 1e3
@@ -252,22 +241,20 @@
     reps = 1
     total_transcript = 0
     min_transcript = 0
     with open(file, 'r') as transcription:
         if header == True: header_line = transcription.readline()
 
         for line in transcription:
-            line = line.strip().split(sep)
-            abundances = line[1:]
-            if len(abundances) > 0:
-                abundances = [float(x) for x in abundances]
-                abund_dict[str(line[0])] = abundances
-                total_transcript += float(numpy.median(abundances))
-                min_transcript += float(min(abundances))
-                if reps < len(abundances): reps = len(abundances)
+            line = line.split(sep)
+            abundances = [float(x) for x in line[1:]]
+            abund_dict[str(line[0])] = abundances
+            total_transcript += float(numpy.median(abundances))
+            min_transcript += float(min(abundances))
+            if reps < len(abundances): reps = len(abundances)
 
         abund_dict['replicates'] = reps
 
     # Rarefy abundances
     if level == 'default': 
         level = int(min_transcript)
     else:
@@ -290,16 +277,15 @@
                 if gene == 'replicates':
                     continue
                 else:
                     abund_dict[gene][x] = (abund_dict[gene][x] / total_transcript) * float(factor)
 
     # If user-defined, perform abundance binning by quantile
     if binning == True:
-        if silent == False:
-            print('Performing transcript abundance binning by quantile...')
+        print('Performing transcript abundance binning by quantile...')
         abund_dict = _assign_quantiles(abund_dict, quant_max, quant_min, step)
 
     return abund_dict
 
 
 # Creates transcription abundances catagories based on quantiles - optional
 def _assign_quantiles(transcription, quant_max, quant_min, step):
@@ -347,148 +333,90 @@
     result = numpy.zeros(len(counts))
     for p in permuted:
         result[p] += 1
 
     return list(result)
 
 
-# Simplified to run in parallel
-def _multi_contextualize(args, frac):
-    current_fit = contextualize(model=args['model'], transcriptome=args['transcriptome'], fraction=frac, samples=args['samples'], 
-                         minimum=args['minimum'], conservative=args['conservative'], objective=args['objective'], prune=args['prune'], 
-                         additive=args['additive'], set_bounds=args['set_bounds'], task_frac=args['task_frac'],
-                         tasks=args['tasks'], exclude=args['exclude'], gpr=args['gpr'], threshold=args['threshold'], 
-                         phase=2, silent=True)
-
-    return current_fit
-
+# Version of riptide.contextualize compatible with multiprocessing
+def _iter_riptide(frac, argDict):
+    
+    iter = single_contextualize(model=argDict['model'], transcriptome=argDict['transcriptome'], fraction=frac, 
+                         silent=argDict['silent'], samples=argDict['samples'], 
+                         minimum=argDict['minimum'], conservative=argDict['conservative'], objective=argDict['objective'], 
+                         additive=argDict['additive'], important=argDict['important'], set_bounds=argDict['set_bounds'], 
+                         tasks=argDict['tasks'], exclude=argDict['exclude'], gpr=argDict['gpr'], threshold=argDict['threshold'], 
+                         open_exchanges=argDict['open_exchanges'])
+    return iter
+    
 
 # Finds the best Rho value from a list of riptide objects
-def _find_best_fit(frac_range, argDict, prev_best=None):
-    increment = 100.0 / float(len(frac_range)+1)
+def _find_best_fit(frac_range, argDict):
+    increment = 100.0 / float(len(frac_range))
     progress = 0.0
-
-    if prev_best == None:
-        best_fit_concordance = 0.
-        if argDict['silent'] == False:
-            print('Analyzing context-specific subnetwork flux ranges...')
-    else:
-        best_fit_concordance = prev_best.concordance
-        if argDict['silent'] == False:
-            print('Testing local objective fractions to ' + str(prev_best.fraction_of_optimum) + '...')
-
-    if argDict['silent'] == False: sys.stdout.write('\rProgress: 0%')
-
-    maxfit_report = {}
-    best_fit = _multi_contextualize(argDict, frac_range[0])
-    maxfit_report[best_fit.fraction_of_optimum] = best_fit.concordance
+    if argDict['silent'] == False:
+        sys.stdout.write('\rProgress: 0%')
     
-    progress += increment
-    improved = 0
-    best_fit_concordance = 0.
-    if isinstance(best_fit.concordance, str) == True:
-        if argDict['silent'] == False: sys.stdout.write('\rProgress: ' + str(float("%.2f" % progress)) + '%')
-    elif best_fit.concordance['r'] > best_fit_concordance:
-        best_fit_concordance = best_fit.concordance['r']
-        improved += 1
-        if argDict['silent'] == False: sys.stdout.write('\rProgress: ' + str(float("%.2f" % progress)) + '%  -  improved fit identified (' + str(improved) + ')        ')
-    else:
-        if argDict['silent'] == False: sys.stdout.write('\rProgress: ' + str(float("%.2f" % progress)) + '%')
-        
-    # Identify best fit of flux sample to transcriptome
-    for frac in frac_range[1:]:
-        improvement = False
-        try:
-            fit = _multi_contextualize(argDict, frac)
-        except:
+    maxfit_report = {}
+    with concurrent.futures.ProcessPoolExecutor(max_workers=argDict['cpus']) as executor:
+
+        maxfit_jobs = [executor.submit(_iter_riptide, frac, argDict) for frac in frac_range]
+        first_iter = 1
+        for job in concurrent.futures.as_completed(maxfit_jobs):
+            result = job.result()
             progress += increment
+            progress = float("%.3f" % progress)
             if argDict['silent'] == False:
-                sys.stdout.write('\rProgress: ' + str(float("%.2f" % progress)) + '% ')
-            continue
-            
-        maxfit_report[fit.fraction_of_optimum] = fit.concordance
-        if isinstance(fit.concordance, str) != True:
-            if fit.concordance['r'] > best_fit_concordance: 
-                improvement = True
-                best_fit = fit
-                best_fit_concordance = fit.concordance['r']
-        
-        progress += increment
-        if argDict['silent'] == False:
-            if improvement == False and improved == 0:
-                sys.stdout.write('\rProgress: ' + str(float("%.2f" % progress)) + '% ')
-            elif improved == 0 and prev_best == None:
-                improved += 1
-                sys.stdout.write('\rProgress: ' + str(float("%.2f" % progress)) + '%  -  fit identified                     ')
-            else:
-                improved += 1
-                sys.stdout.write('\rProgress: ' + str(float("%.2f" % progress)) + '%  -  improved fit identified (' + str(improved) + ')        ')
+                sys.stdout.write('\rProgress: ' + str(progress) + '%')
+                sys.stdout.flush()
 
-    if argDict['silent'] == False:
-        if improvement == False and improved == 0:
-            sys.stdout.write('\rProgress: 100%        \n\n')
-            sys.stdout.flush()
-        elif improved == 0 and prev_best == None:
-            sys.stdout.write('\rProgress: 100%  -  fit identified                       \n\n')
-            sys.stdout.flush()
-        else:
-            improved += 1
-            sys.stdout.write('\rProgress: 100%  -  improved fit identified (' + str(improved) + ')         \n\n')
-            sys.stdout.flush()
-    
-    # Check if metabolic tasks can carry flux in the best fit model
-    tasks = argDict['tasks']
-    if argDict['silent'] == False and len(tasks) >= 1:
-        obj_ID = str(best_fit.model.objective.expression).split()[0].split('*')[-1]
-        for task in tasks:
-            best_fit.model.objective = task
-            task_flux = best_fit.model.slim_optimize(error_value=0.)
-            if task_flux <= argDict['threshold']:
-                print('WARNING:', task, 'carries no flux in best fitting model')
-        best_fit.model.objective = obj_ID
+            maxfit_report[result.fraction_of_optimum] = result.concordance
+
+            if first_iter == 1:
+                best_fit = result
+                first_iter = 0
+            elif result.concordance['r'] > best_fit.concordance['r']:
+                best_fit = result
 
+    if argDict['silent'] == False:
+        sys.stdout.write('\rProgress: 100%      \n\n')
     best_fit.maxfit_report = maxfit_report
 
     return best_fit
 
 
 # Iteratively run RIPTiDe over a range of objective minimum fractions
-def maxfit(model, transcriptome = 'none', frac_min = 0.1, frac_max = 0.9, frac_step = 0.1, prune = True,
-    samples = 1000, minimum = False, conservative = False, objective = True, additive = False, 
-    set_bounds = True, silent = False, tasks = [], task_frac = 0.01, exclude = [], gpr = False, threshold = 1e-8):
+def contextualize(model, transcriptome = 'none', frac_min = 0.25, frac_max = 0.85, 
+    samples = 500, cpus = 'all', minimum = False, conservative = False, objective = True, additive = False, 
+    important = [], set_bounds = True, silent = False, tasks = [], exclude = [], gpr = False, threshold = 1e-6, open_exchanges = False):
 
-    '''
-    Iterative RIPTiDe for a range of minimum objective fluxes, returns model with best correlation 
-    with flux sampling results to transcriptome abundances.
+    '''Iterative RIPTiDe for a range of minimum objective fluxes, returns model with best fit to transcriptome
     
     Parameters
     ----------
 
     REQUIRED
     model : cobra.Model
         The model to be contextualized
     transcriptome : dictionary
         Dictionary of transcript abundances, output of read_transcription_file()
     
     OPTIONAL
+    cpus : int
+        CPUs number for parallelization
+        Default is all available 
     frac_min : float
         Lower bound for range of minimal fractions to test
         Default is 0.25
     frac_max : float
         Upper bound for range of minimal fractions to test
         Default is 0.85
-    frac_step : float
-        Starting interval size within fraction range
-        Default is 0.1
-    prune : bool
-        Perform pruning step
-        Default is True
     samples : int 
         Number of flux samples to collect
-        Default is 1000
+        Default is 500
     silent : bool
         Silences std out 
         Default is False
     minimum : float
         Minimum linear coefficient allowed during weight calculation for pFBA
         Default is False
     conservative : bool
@@ -496,156 +424,118 @@
         Default is False
     objective : bool
         Sets previous objective function as a constraint with minimum flux equal to user input fraction
         Default is True
     additive : bool
         Pool transcription abundances for reactions with multiple contributing gene products
         Default is False
+    important : list
+        List of gene or reaction ID strings for which the highest weights are assigned regardless of transcription
+        Default is False
     direct : bool
         Assigns both minimization and maximization step coefficents directly, instead of relying on abundance distribution
         Default is False
     set_bounds : bool
         Uses flux variability analysis results from constrained model to set new bounds for all reactions
         Default is True
     tasks : list
         List of gene or reaction ID strings for forced inclusion in final model (metabolic tasks or essential genes)
-    task_frac : float
-        Minimum fraction of optimal flux for metabolic task reactions given preceeding constraints
-        Default is 0.01
     exclude : list
         List of reaction ID strings for forced exclusion from final model
     gpr : bool
         Determines if GPR rules will be considered during coefficient assignment
         Default is False
     threshold : float
         Minimum flux a reaction must acheive in order to avoid pruning during flux sum minimization step
-        Default is 1e-8
+        Default is 1e-6
+    open_exchanges : bool
+        Sets all exchange reactions bounds to (-1000., 1000)
+        Default is False
+    skip_fva : bool
+        Skip final flux variability analysis step
+        Default is False
     '''
 
     iter_start = time.time()
-    curr_run = str(datetime.now()).replace(' ','_').replace('-','').replace(':','').split('.')[0].replace(' ','_')
+    print('\nInitializing model and integrating transcriptomic data...')
+    print('Pruning zero flux subnetworks...')
+    print('Analyzing context-specific flux distributions...\n')
     seed(937162211)
 
     if samples <= 100:
         raise ValueError('ERROR: Iterative RIPTiDe requires >100 flux sampling depth')
     if transcriptome == 'none':
         raise ValueError('ERROR: Iterative RIPTiDe requires an input transcriptome')
-
-    if _test_exchange_space(model, minimum=1e5):
-        raise ValueError('ERROR: Solution space is too constrained to analyze by current exchange bounds')
+    if cpus == 'all':
+        cpus = os.cpu_count()
+    elif isinstance(cpus, int) == False:
+        raise ValueError('ERROR: Invalid number of threads provided')
 
     if frac_min < 0. or frac_min > 1.:
-        if silent == False:
-            print('WARNING: Improper minimum fraction provided, setting to default value')
+        print('WARNING: Improper minimum fraction provided, setting to default value')
         frac_min = 0.25
     elif frac_min > frac_max:
-        if silent == False:
-            print('WARNING: Improper minimum fraction provided, setting to default value')
+        print('WARNING: Improper minimum fraction provided, setting to default value')
         frac_min = 0.25
 
     if frac_max < 0. or frac_max > 1.:
         print('WARNING: Improper maximum fraction provided, setting to default value')
         frac_max = 0.85
     elif frac_max < frac_min:
-        if silent == False:
-            print('WARNING: Improper maximum fraction provided, setting to default value')
+        print('WARNING: Improper maximum fraction provided, setting to default value')
         frac_max = 0.85
 
-    if threshold+1e-6 < 1e-6:
-        threshold = abs(threshold)
-
-    if task_frac <= 0. or task_frac > 1.:
-        task_frac = 0.01
-    if isinstance(tasks, str) == True: tasks = [tasks]
-
+    frac_step = 0.1
     frac_range = [round(x, 3) for x in list(numpy.arange(frac_min, frac_max+frac_step, frac_step))]
     if len(frac_range) == 1:
-        if silent == False:
-            print('WARNING: Only a single fraction is possible in the input bounds and fraction')
+        print('WARNING: Only a single fraction is possible in the input bounds and fraction')
 
     if silent == False:
-        print('Running max fit RIPTiDe for objective fraction range:', frac_min, 'to', str(frac_max) + '...')
+        print('\nRunning max fit RIPTiDe for objective fraction range:', frac_min, 'to', frac_max, '...')
 
-    argDict = {'model':model, 'transcriptome':transcriptome, 'silent':silent, 
-               'samples':samples, 'minimum':minimum, 'task_frac':task_frac, 'prune':prune,
+    argDict = {'model':model, 'transcriptome':transcriptome, 'silent':silent, 'cpus':cpus,
+               'samples':samples, 'minimum':minimum, 
                'conservative':conservative, 'objective':objective, 'additive':additive, 
-               'set_bounds':set_bounds, 'tasks':tasks, 'exclude':exclude, 
-               'gpr':gpr, 'threshold':threshold, 'phase':2}
-    
-    warnings.filterwarnings('ignore', category=UserWarning)
+               'important':important, 'set_bounds':set_bounds, 'tasks':tasks, 'exclude':exclude, 
+               'gpr':gpr, 'threshold':threshold, 'open_exchanges':open_exchanges}
+
     top_fit = _find_best_fit(frac_range, argDict)
     all_maxfit = top_fit.maxfit_report
     
-    if isinstance(top_fit.concordance, str) != True:
-        small_frac_range = []
-        while frac_step >= 0.025:
-            frac_step = round(frac_step / 2.0, 3)
-            small_frac_range += [round(top_fit.fraction_of_optimum - frac_step, 3), round(top_fit.fraction_of_optimum + frac_step, 3)]
-
-        if len(set(small_frac_range)) >= 1:
-            new_fit = _find_best_fit(list(set(small_frac_range)), argDict, top_fit)
-            if isinstance(new_fit.concordance, str) != True:
-                if new_fit.concordance['r'] > top_fit.concordance['r']:
-                    top_fit = new_fit
-                    for frac in new_fit.maxfit_report.keys():
-                        all_maxfit[frac] = new_fit.maxfit_report[frac]
-    
-    warnings.filterwarnings('default', category=UserWarning)
+    if silent == False:
+        print('Testing local objective fractions to ' + str(top_fit.fraction_of_optimum) + '...')
+    small_frac_range = []
+    while frac_step >= 0.025:
+        frac_step = round(frac_step / 2.0, 3)
+        small_frac_range += [round(top_fit.fraction_of_optimum - frac_step, 3), round(top_fit.fraction_of_optimum + frac_step, 3)]
+    
+    new_fit = _find_best_fit(list(set(small_frac_range)), argDict)
+    if new_fit.concordance['r'] >= top_fit.concordance['r']:
+        top_fit = new_fit
+        for frac in new_fit.maxfit_report.keys():
+             all_maxfit[frac] = new_fit.maxfit_report[frac]
+
     top_fit.maxfit_report = all_maxfit
     top_fit.fraction_bounds = [frac_min, frac_max]
     top_fit.transcriptome = transcriptome
-    
-    # Check best fit
     if silent == False:
-        if top_fit.concordance == 'Not performed':
-            print('No level of optimal objective flux correlated with transcriptome')
-            print(top_fit.fraction_of_optimum, 'of optimum-associated model returned')
-        else:
-            print('Context-specific metabolism fit with', top_fit.fraction_of_optimum, 'of optimal objective flux')
+        print('\nContext-specific metabolism fit with', top_fit.fraction_of_optimum, 'of optimal objective flux')
 
     # Analyze changes introduced by RIPTiDe and return results
-    report_dict = _operation_report(iter_start, model, top_fit.model, top_fit.concordance, silent, phase=1)
+    report_dict = _operation_report(iter_start, model, top_fit.model, top_fit.concordance, silent, mf=True)
     top_fit.additional_parameters['operation'] = report_dict
     top_fit.maxfit = True
-    top_fit.run_start = curr_run
 
     return top_fit
 
 
-# Assemble a corrected list of metabolic tasks based on user
-def _screen_tasks(model, tasks, silent):
-    # Check that each task is in the model
-    screened_tasks = []
-    for x in tasks:
-        # Genes
-        try:
-            rxns = list(model.genes.get_by_id(x).reactions)
-            rxns = [y.id for y in rxns]
-            screened_tasks += rxns
-        except:
-            # Reactions
-            try:
-                rxn = model.reactions.get_by_id(x)
-                screened_tasks.append(rxn.id)
-            except:
-                continue
-
-    # Check if any reactions were found in the model that correspond with supplied IDs
-    screened_tasks = set(screened_tasks)
-    if len(screened_tasks) == 0:
-        if silent == False:
-            print('WARNING: No reactions found associated with provided task IDs')
-    
-    return screened_tasks
-
-
 # Create context-specific model based on transcript distribution
-def contextualize(model, transcriptome = 'none', samples = 1000, silent = False, prune = True,
-    fraction = 0.8, minimum = False, conservative = False, objective = True, additive = False, direct = False,
-    set_bounds = True, tasks = [], task_frac = 0.01, exclude = [], gpr = False, threshold = 1e-8, phase=1):
+def single_contextualize(model, transcriptome = 'none', samples = 500, silent = False, 
+    fraction = 0.8, minimum = False, conservative = False, objective = True, additive = False, important = [], direct = False,
+    set_bounds = True, tasks = [], exclude = [], gpr = False, threshold = 1e-6, open_exchanges = False, skip_fva = False):
 
     '''Reaction Inclusion by Parsimony and Transcriptomic Distribution or RIPTiDe
     
     Creates a contextualized metabolic model based on parsimonious usage of reactions defined
     by their associated transcriptomic abundances. Returns a pruned, context-specific cobra.Model 
     and associated flux analyses along with parameters used in a riptide class object
 
@@ -660,62 +550,53 @@
     transcriptome : dictionary
         Dictionary of transcript abundances, output of read_transcription_file()
         With default, an artifical transcriptome is generated where all abundances equal 1.0
     fraction : float
         Minimum objective fraction used during single run setting
         Default is 0.8
 
-    * Other arguments from iterative implementation are carried over
+    * Most other arguments from iterative implementation are carried over
     '''
 
     start_time = time.time()
-    curr_run = str(datetime.now()).replace(' ','_').replace('-','').replace(':','').split('.')[0]
-    
     seed(937162211)
 
-    if _test_exchange_space(model, minimum=1e5):
-        raise ValueError('ERROR: Solution space is too constrained to analyze by current exchange bounds')
-
     riptide_object = riptideClass()
     riptide_object.additional_parameters = {}
     riptide_object.additional_parameters['threshold'] = threshold
     riptide_object.additional_parameters['silent'] = silent
     riptide_object.additional_parameters['conservative'] = conservative
     riptide_object.additional_parameters['objective'] = objective
     riptide_object.additional_parameters['additive'] = additive
     riptide_object.additional_parameters['set_bounds'] = set_bounds
-    riptide_object.start_time = str(start_time)
-    riptide_object.run_start = curr_run
+    riptide_object.additional_parameters['open_exchanges'] = open_exchanges
 
     # Correct some possible user error
     samples = int(samples)
     if samples < 1: samples = 500
+    if len(important) > 0: samples = 1
     riptide_object.additional_parameters['samples'] = samples
     fraction = float(fraction)
     if fraction <= 0.0: 
         fraction = 0.01
     elif fraction >= 1.0: 
         fraction = 0.99
-    if threshold+1e-6 < 1e-6:
-        threshold = abs(threshold)
-    if task_frac <= 0. or task_frac > 1. or task_frac > fraction:
-        task_frac = fraction
     if minimum != False:
         if minimum <= 0.0: 
             minimum = 0.0001
         elif minimum > 1.0: 
             minimum = 0.0001
     elif minimum == False:
         minimum = None
     riptide_object.additional_parameters['minimum'] = minimum
-    solution = model.slim_optimize(error_value=0.)
-    if solution < 1e-6:
+    solution = model.slim_optimize()
+    if model.slim_optimize() < 1e-6 or str(model.slim_optimize()) == 'nan':
         raise ValueError('ERROR: Provided model objective cannot carry flux! Please correct')
     minimum_threshold = threshold
-    if isinstance(tasks, str) == True: tasks = [tasks]
+    if isinstance(tasks, list) == False: tasks = [tasks]
 
     # Creates artificial transcriptome to identify most parsimonious patterns of metabolism
     if transcriptome == 'none':
         if silent == False:
             print('WARNING: No transcriptome provided. Analyzing most parsimonious state')
         transcriptome = {}
         transcriptome['replicates'] = 1
@@ -738,119 +619,95 @@
     # Save parameters as part of the output object
     riptide_object.fraction_of_optimum = fraction
     riptide_object.transcriptome = transcriptome
     riptide_object.gpr_integration = gpr
 
     # Check original model functionality
     # Partition reactions based on transcription percentile intervals, assign corresponding reaction coefficients
-    if phase == 1:
-        if silent == False: 
-            print('\nInitializing model and integrating transcriptomic data...')
-    
+    if silent == False: print('\nInitializing model and integrating transcriptomic data...')
+    riptide_model = copy.deepcopy(model)
+    riptide_model.id = str(riptide_model.id) + '_riptide'
+    riptide_object.metabolic_tasks = tasks
+
+    # Open exchange reactions
+    if open_exchanges == True:
+        for rxn in riptide_model.exchanges: rxn.bounds = (-1000., 1000.)
+
+    # Remove totally blocked reactions to speed up subsequent sections
+    rm_rxns = list(set(exclude).difference(set(tasks)))
+    if len(rm_rxns) > 0:
+        riptide_model = _prune_model(riptide_model, rm_rxns, conservative)
+
     # Define linear coefficients for both steps
-    rxn_transcriptome, gene_hits = _transcript_to_reactions(transcriptome, model, gpr, additive)
+    rxn_transcriptome, gene_hits = _transcript_to_reactions(transcriptome, riptide_model, gpr, additive)
+    keep_rxns = set()
     all_min_coefficient_dict = {}
-    all_max_coefficient_dict = {}
-    riptide_object.percent_of_mapping = gene_hits
-    
-    if silent == False:
-        if phase == 1:
-            print('Pruning zero flux subnetworks...')
-            
-    inactive_rxns = set(exclude)
+    if silent == False: print('Pruning zero flux subnetworks...')
     for x in range(0, transcriptome['replicates']):
         current_rxn_transcriptome = {}
         for index in rxn_transcriptome.keys():
             if index == 'replicates':
                 continue
             else:
                 current_rxn_transcriptome[index] = rxn_transcriptome[index][x]
-        min_coefficient_dict, max_coefficient_dict = _assign_coefficients(current_rxn_transcriptome, model, direct)
+        min_coefficient_dict, max_coefficient_dict, important_type = _assign_coefficients(current_rxn_transcriptome, riptide_model, important, direct)
         for x in min_coefficient_dict.keys():
             try:
                 all_min_coefficient_dict[x].append(min_coefficient_dict[x])
-                all_max_coefficient_dict[x].append(max_coefficient_dict[x])
             except KeyError:
                 all_min_coefficient_dict[x] = [min_coefficient_dict[x]]
-                all_max_coefficient_dict[x] = [max_coefficient_dict[x]]
-        min_coefficient = min(list(min_coefficient_dict.values()))
-        max_coefficient = max(list(max_coefficient_dict.values()))
         
-        # Correct task coefficients
-        if objective == True: 
-            objective = str(model.objective.expression).split()[0].split('*')[-1]
-            min_coefficient_dict[objective] = min_coefficient
-            max_coefficient_dict[objective] = max_coefficient
-            try:
-                all_min_coefficient_dict[objective].append(min_coefficient_dict[objective])
-                all_max_coefficient_dict[objective].append(max_coefficient_dict[objective])
-            except KeyError:
-                all_min_coefficient_dict[objective] = [min_coefficient_dict[objective]]
-                all_max_coefficient_dict[objective] = [max_coefficient_dict[objective]]
-        if len(tasks) >= 1: 
-            riptide_object.metabolic_tasks = tasks
-            for task in tasks:
-                min_coefficient_dict[task] = min_coefficient
-                max_coefficient_dict[task] = max_coefficient
-                try:
-                    all_min_coefficient_dict[task].append(min_coefficient_dict[task])
-                    all_max_coefficient_dict[task].append(max_coefficient_dict[task])
-                except KeyError:
-                    all_min_coefficient_dict[task] = [min_coefficient_dict[task]]
-                    all_max_coefficient_dict[task] = [max_coefficient_dict[task]]
-        else:
-            tasks = []
-            
-        # Determine inactive network sections based on coefficients
-        inactive_rxns |= _constrain_for_pruning(model=model, min_coefficients=min_coefficient_dict, 
-                                             objective=objective, obj_fraction=fraction, tasks=tasks, task_fraction=task_frac, 
-                                             minimum_flux=minimum_threshold, silent=silent)
-    
-    # Prune inactive model components
+        # Determine active network sections based on coefficients
+        active_rxns = _constrain_and_analyze_model(model=riptide_model, coefficient_dict=min_coefficient_dict, fraction=fraction, sampling_depth=0, 
+            objective=objective, tasks=tasks, minimum_threshold=minimum_threshold, skip_fva=skip_fva)
+        keep_rxns = keep_rxns.union(active_rxns)
+
+    # Determine inactive reactions and prune model
+    rm_rxns = set([x.id for x in riptide_model.reactions]).difference(keep_rxns)
+    riptide_model = _prune_model(riptide_model, rm_rxns, conservative)
+    riptide_object.pruned = _record_pruned_elements(model, riptide_model)
     riptide_object.minimization_coefficients = all_min_coefficient_dict
-    if len(inactive_rxns) > 0 and prune == True:
-        riptide_model = _prune_model(model, inactive_rxns, conservative)
-        riptide_object.pruned = _record_pruned_elements(model, riptide_model)
-    else:
-        riptide_model = deepcopy(model)
-         
-    # Find optimal solution space based on transcription and final constraints
-    if silent == False:
-        if phase == 1:
-            print('Analyzing context-specific flux distributions...')
+    riptide_object.percent_of_mapping = gene_hits
 
-    # Find best sampling weights
-    for x in all_max_coefficient_dict.keys():
-        max_coefficient_dict[x] = max(all_max_coefficient_dict[x])
+    # Find optimal solution space based on transcription and final constraints
+    if silent == False: print('Analyzing context-specific flux distributions...')
+    median_rxn_transcriptome = {}
+    for x in rxn_transcriptome.keys(): 
+        if x == 'replicates':
+            continue
+        else:
+            median_rxn_transcriptome[x] = numpy.median(rxn_transcriptome[x])
+    min_coefficient_dict, max_coefficient_dict, important_type = _assign_coefficients(median_rxn_transcriptome, riptide_model, important, direct)
+    flux_samples, fva_result, concordance = _constrain_and_analyze_model(model=riptide_model, coefficient_dict=max_coefficient_dict, fraction=fraction, 
+        sampling_depth=samples, objective=objective, tasks=tasks, minimum_threshold=minimum_threshold, skip_fva=skip_fva)
     riptide_object.maximization_coefficients = max_coefficient_dict
-
-    # Sample weighted flux distributions
-    flux_samples, concordance = _constrain_for_sampling(model=riptide_model, max_coefficients=max_coefficient_dict, sampling_depth=samples,
-                                                        objective=objective, obj_frac=fraction,  tasks=tasks, task_frac=task_frac, 
-                                                        min_flux=minimum_threshold,silent=silent)
     riptide_object.flux_samples = flux_samples
+    riptide_object.flux_variability = fva_result
     riptide_object.concordance = concordance
-        
+
     # Assign new reaction bounds
-    if set_bounds == True and isinstance(flux_samples, str) == False:
+    if set_bounds == True and skip_fva == False: 
         for rxn in riptide_model.reactions:
-            current_dist = list(flux_samples[rxn.id])
-
-            try:
-                old_bounds = rxn.bounds
-                rxn.lower_bound = min(current_dist)
-                rxn.upper_bound = max(current_dist)
-                if riptide_model.slim_optimize(error_value=0.) == 0.:
-                    rxn.bounds = old_bounds
-            except:
-                continue
+            current_fva = list(fva_result.loc[rxn.id])
+            rxn.bounds = (min(current_fva), max(current_fva))
     riptide_object.model = riptide_model
 
+    # Report on included subset of user-defined important genes
+    if len(important) > 0:
+        if important_type == 'genes':
+            curr_list = set([x.id for x in riptide_model.genes])
+        elif important_type == 'reactions':
+            curr_list = set([y.id for y in riptide_model.reactions])
+        included_important = set(important).intersection(curr_list)
+        riptide_object.included_important = included_important
+    else:
+        riptide_object.included_important = important
+
     # Analyze changes introduced by RIPTiDe and return results
-    report_dict = _operation_report(start_time, model, riptide_model, concordance, silent, phase)
+    report_dict = _operation_report(start_time, model, riptide_model, concordance, silent, mf=False)
     riptide_object.additional_parameters['operation'] = report_dict
 
     return riptide_object
  
 
 # Converts a dictionary of transcript abundances to reaction linear coefficients
 def _transcript_to_reactions(reps_transcription_dict, model, gpr, additive):
@@ -935,15 +792,15 @@
                 rxn_transcript_dict[rxn.id].append(nogene_abund)
     
     return rxn_transcript_dict, gene_hits
 
 
 
 # Converts a dictionary of transcript abundances to reaction linear coefficients
-def _assign_coefficients(rxn_transcript_dict, model, direct):
+def _assign_coefficients(rxn_transcript_dict, model, important, direct):
     
     # Calculate coefficients
     all_abundances = list(rxn_transcript_dict.values())
     denom = max(all_abundances)
     all_abundances.sort()
     max_coefficients = [x / denom for x in all_abundances]
     if direct == True:
@@ -958,150 +815,176 @@
     # Assign coefficients to reactions
     rxn_min_coefficient_dict = {}         
     rxn_max_coefficient_dict = {}
     for rxn in rxn_transcript_dict.keys():
         rxn_min_coefficient_dict[rxn] = coefficient_dict[rxn_transcript_dict[rxn]][0]
         rxn_max_coefficient_dict[rxn] = coefficient_dict[rxn_transcript_dict[rxn]][1]
 
-    return rxn_min_coefficient_dict, rxn_max_coefficient_dict
+    # If user has defined important genes/reactions, integrate new weights here
+    important_type = 'NULL'
+    if len(important) > 0: 
+        rxn_min_coefficient_dict, important_type = _integrate_important(model, important, rxn_min_coefficient_dict)
 
+    return rxn_min_coefficient_dict, rxn_max_coefficient_dict, important_type
 
-# Constrain task minimum flux
-def _constrain_task(model, task, frac, min_flux, silent):
-    
-    model.objective = task
-    model.objective.direction = 'max'
-    
-    task_name = task + '_constraint'
-    task_bound = model.slim_optimize(error_value=0.)
-    if silent == False and task_bound <= min_flux:
-        print('WARNING:', task, 'minimum flux infeasible')
-        task_bounds = [min_flux, model.reactions.get_by_id(task).upper_bound]
-    else:
-        task_bounds = [task_bound, task_bound * frac]
-        
-    task_expression = model.reactions.get_by_id(task).flux_expression
-    task_constraint = model.problem.Constraint(task_expression, name=task_name, ub=max(task_bounds), lb=min(task_bounds))
-    model.add_cons_vars(task_constraint)
-    model.solver.update()
+
+# Assemble a corrected list of metabolic tasks based on user
+def _integrate_tasks(model, tasks):
+    # Check that each task is in the model
+    screened_tasks = []
+    for x in set(tasks):
+        # Genes
+        try:
+            rxns = list(model.genes.get_by_id(x).reactions)
+            rxns = [y.id for y in rxns]
+            screened_tasks += rxns
+        except:
+            pass
+        # Reactions
+        try:
+            rxn = model.reactions.get_by_id(x)
+            screened_tasks.append(rxn.id)
+        except:
+            continue
+
+    # Check if any reactions were found in the model that correspond with supplied IDs
+    if len(screened_tasks) == 0:
+        print('WARNING: No reactions found associated with provided task IDs')
+
+    # Iteratively set each as the objective and find new bounds
+    for rxn in screened_tasks:
+        model.objective = rxn
+        task_obj_val = model.slim_optimize()
+        # Check sign of objective value, just in case
+        if task_obj_val > 0.0:
+            task_constraint = model.problem.Constraint(model.objective.expression, lb=task_obj_val*0.01, ub=task_obj_val)
+            model.add_cons_vars(task_constraint)
+            model.solver.update()
+        elif task_obj_val < 0.0:
+            task_constraint = model.problem.Constraint(model.objective.expression, lb=task_obj_val, ub=task_obj_val*0.01)
+            model.add_cons_vars(task_constraint)
+            model.solver.update()
     
     return model
 
 
-# Create weighted expression - default is pFBA
-def _weighted_expression(model, coefficients={}):
-    
-    if len(list(coefficients.keys())) == 0:
-        for rxn in model.reactions: 
-            coefficients[rxn.id] = 1.0
-    
-    new_expr = symengine.RealDouble(0)
-    for rxn in model.reactions:
+# Assign heaviest weight during pruning to user-defined important genes
+def _integrate_important(model, important, coefficient_dict):
+
+    #weight = numpy.quantile(list(coefficient_dict.values()), 0.25)
+    weight = min(list(coefficient_dict.values()))
+
+    # Check if reactions or genes, get reaction IDs
+    rxn_ids = []
+    for x in important:
+        # Genes
         try:
-            new_expr += coefficients[rxn.id] * rxn.forward_variable
-            new_expr += coefficients[rxn.id] * rxn.reverse_variable
-        except KeyError:
+            rxns = list(model.genes.get_by_id(x).reactions)
+            rxn_ids += [y.id for y in rxns]
+            important_type = 'genes'
+        except:
+            pass
+        # Reactions
+        try:
+            rxn = model.reactions.get_by_id(x)
+            rxn_ids.append(rxn.id)
+            important_type = 'reactions'
+        except:
             continue
-            
-    return new_expr
 
+    # Correct weight in coefficient dictionary
+    for rxn in set(rxn_ids): coefficient_dict[rxn] = weight
 
-# Determine those reactions that carry flux in a pFBA objective set to a threshold of maximum
-def _constrain_for_pruning(model, min_coefficients, objective, obj_fraction, tasks, task_fraction, minimum_flux, silent):
-    
-    constrained_model = deepcopy(model)
-    
-    # Add objective/task constraints
-    min_coefficient = min(list(min_coefficients.values()))
-    if isinstance(objective, str) == True:
-        min_coefficients[objective] = min_coefficient
-        constrained_model = _constrain_task(constrained_model, objective, obj_fraction, minimum_flux, silent)
-
-    # metabolic task constraints
-    if len(tasks) >= 1:
-        for task in tasks:
-            min_coefficients[task] = min_coefficient
-            constrained_model = _constrain_task(constrained_model, task, task_fraction, minimum_flux, silent)
-    
-    pruning_expr = _weighted_expression(model=constrained_model, coefficients=min_coefficients)
-    constrained_model.objective = model.problem.Objective(pruning_expr, direction='min', sloppy=True)
-    constrained_model.solver.update()
-    
-    constrained_fluxes = constrained_model.optimize().fluxes
-    inactive_rxns = set([rxn.id for rxn in constrained_model.reactions if abs(constrained_fluxes[rxn.id]) == 0.]) 
-    
-    return inactive_rxns
+    return coefficient_dict, important_type
 
 
 # Determine those reactions that carry flux in a pFBA objective set to a threshold of maximum
-def _constrain_for_sampling(model, max_coefficients, sampling_depth, objective, obj_frac, tasks, task_frac, min_flux, silent):
-    
-    constrained_model = deepcopy(model)
+def _constrain_and_analyze_model(model, coefficient_dict, fraction, sampling_depth, objective, tasks, minimum_threshold, skip_fva):
     
-    # Apply weigths to new expression, allow deviation
-    if isinstance(objective, str) == True:
-        constrained_model = _constrain_task(constrained_model, objective, obj_frac, min_flux, silent)
-    if len(tasks) >= 1:
-        for task in tasks:
-            constrained_model = _constrain_task(constrained_model, task, task_frac, min_flux, silent)
-
-    sampling_expr = _weighted_expression(model=constrained_model, coefficients=max_coefficients)
-    constrained_model.objective = model.problem.Objective(sampling_expr, direction='max', sloppy=True)
-    constrained_model.solver.update()
-    
-    flux_sum = constrained_model.slim_optimize(error_value=0.)
-    if flux_sum <= min_flux:
-        flux_samples = 'Not performed'
-        concordance = 'Not performed'
-    else:
-        flux_sum_constraint = constrained_model.problem.Constraint(sampling_expr, lb=min_flux, ub=flux_sum)
-        constrained_model.add_cons_vars(flux_sum_constraint)
+    constrained_model = copy.deepcopy(model)
+
+    # Set previous objective as a constraint, allow deviation
+    if objective == True:
+        prev_obj_val = constrained_model.slim_optimize()
+        prev_obj_constraint = constrained_model.problem.Constraint(constrained_model.objective.expression, lb=prev_obj_val*fraction, ub=prev_obj_val)
+        constrained_model.add_cons_vars([prev_obj_constraint])
+        constrained_model.solver.update()
+
+    # Apply weigths to new expression
+    pfba_expr = symengine.RealDouble(0)
+    for rxn in constrained_model.reactions:
+        try:
+            pfba_expr += coefficient_dict[rxn.id] * rxn.forward_variable
+            pfba_expr += coefficient_dict[rxn.id] * rxn.reverse_variable
+        except KeyError:
+            continue
+
+    if sampling_depth == 0:
+        # Include metabolic task constraints
+        if len(tasks) >= 1:
+            constrained_model = _integrate_tasks(constrained_model, tasks)
+
+        # Determine reactions that do not carry any flux in highly constrained solution space
+        constrained_model.objective = constrained_model.problem.Objective(pfba_expr, direction='min', sloppy=True)
         constrained_model.solver.update()
+        solution = constrained_model.optimize()
+        active_rxns = set([rxn.id for rxn in constrained_model.reactions if abs(solution.fluxes[rxn.id]) > minimum_threshold])
+            
+        return active_rxns
         
+    else:
+        # Explore solution space of constrained model with flux sampling, allow deviation
+        constrained_model.objective = constrained_model.problem.Objective(pfba_expr, direction='max', sloppy=True)
+        constrained_model.solver.update()
+        flux_sum_obj_val = constrained_model.slim_optimize()
+        flux_sum_constraint = constrained_model.problem.Constraint(pfba_expr, lb=flux_sum_obj_val*fraction, ub=flux_sum_obj_val)
+        constrained_model.add_cons_vars([flux_sum_constraint])
+        constrained_model.solver.update()
+            
         # Analyze flux ranges and calculate concordance
-        try:
+        if sampling_depth != 1:
+            warnings.filterwarnings('ignore') # Handle possible infeasible warnings
             flux_samples = _gapsplit(constrained_model, depth=sampling_depth)
-            concordance = _calc_concordance(flux_samples, max_coefficients)
-        except:
+            warnings.filterwarnings('default')
+            concordance = _calc_concordance(flux_samples, coefficient_dict)
+        else:
             flux_samples = 'Not performed'
             concordance = 'Not performed'
+        
+        if skip_fva == False:
+            fva = flux_variability_analysis(constrained_model, fraction_of_optimum=fraction)
+        else:
+            fva = 'Not performed'
+
+        return flux_samples, fva, concordance
 
-    return flux_samples, concordance
 
-    
 # Find level of concordance between contextualized flux and assigned coefficients
 def _calc_concordance(flux_samples, coefficient_dict):
-    warnings.filterwarnings('ignore', category=RuntimeWarning)
+    warnings.filterwarnings('ignore') # Handle RuntimeWarning
 
     flux_medians = []
     coefficients = []
 
     for rxn in coefficient_dict.keys():
         try:
             flux_medians.append(abs(numpy.median(list(flux_samples[rxn]))))
             coefficients.append(coefficient_dict[rxn])
         except:
             continue
         
     r_val, p_val = spearmanr(coefficients, flux_medians)
     concordance_dict = {'r':r_val, 'p':p_val}
     
-    warnings.filterwarnings('default', category=RuntimeWarning)
+    warnings.filterwarnings('default')
     return concordance_dict
 
 
 # Prune model based on blocked reactions from minimization as well as user-defined reactions
-def _prune_model(model, rm_rxns, conserve):
-    
-    new_model = deepcopy(model)
-    
-    if str(new_model.id).strip() == '':
-        new_model.id = 'model_riptide'
-    else:
-        new_model.id = str(new_model.id) + '_riptide'
+def _prune_model(new_model, rm_rxns, conserve):
     
     # Parse elements highlighted for pruning based on GPRs
     if conserve == True:
         final_rm_rxns = []
         for rxn in rm_rxns:
             test = 'pass'
             current_genes = list(new_model.reactions.get_by_id(rxn).genes)
@@ -1116,17 +999,17 @@
     else:
         final_rm_rxns = rm_rxns
     
     # Screen for duplicates
     final_rm_rxns = list(set(final_rm_rxns))
     
     # Prune inactive reactions
-    warnings.filterwarnings('ignore', category=UserWarning)
+    warnings.filterwarnings('ignore') # Handle UserWarning
     for rxn in final_rm_rxns: new_model.reactions.get_by_id(rxn).remove_from_model(remove_orphans=True)
-    warnings.filterwarnings('default', category=UserWarning)
+    warnings.filterwarnings('default')
 
     # Prune orphaned nodes
     new_model = _complete_orphan_prune(new_model)
 
     return new_model
 
 
@@ -1169,129 +1052,103 @@
             if len(rxn.metabolites) == 0: 
                 rxn.remove_from_model(); removed = 1
 
     return model
 
 
 # Reports how long RIPTiDe took to run
-def _operation_report(start_time, model, riptide, concordance, silent, phase):
+def _operation_report(start_time, model, riptide, concordance, silent, mf):
     report_dict = {}
 
     # Pruning
     perc_removal = 100.0 - ((float(len(riptide.reactions)) / float(len(model.reactions))) * 100.0)
     perc_removal = round(perc_removal, 2)
     if silent == False:
-        if phase == 1:
-            print('\nReactions pruned to ' + str(len(riptide.reactions)) + ' from ' + str(len(model.reactions)) + ' (' + str(perc_removal) + '% change)')
+        print('\nReactions pruned to ' + str(len(riptide.reactions)) + ' from ' + str(len(model.reactions)) + ' (' + str(perc_removal) + '% change)')
     report_dict['reactions'] = perc_removal
     perc_removal = 100.0 - ((float(len(riptide.metabolites)) / float(len(model.metabolites))) * 100.0)
     perc_removal = round(perc_removal, 2)
     if silent == False:
-        if phase == 1:
-            print('Metabolites pruned to ' + str(len(riptide.metabolites)) + ' from ' + str(len(model.metabolites)) + ' (' + str(perc_removal) + '% change)')
+        print('Metabolites pruned to ' + str(len(riptide.metabolites)) + ' from ' + str(len(model.metabolites)) + ' (' + str(perc_removal) + '% change)')
     report_dict['metabolites'] = perc_removal
 
     # Flux through objective
     model_check = 'works'
     # Check that prune model can still achieve flux through the objective (just in case)
     try:
-        if riptide.slim_optimize(error_value=0.) < 1e-6:
+        if riptide.slim_optimize() < 1e-6 or str(riptide.slim_optimize()) == 'nan':
+            if silent == False:
+                print('WARNING: Contextualized model objective can no longer carry flux')
             model_check = 'broken'
     except:
         pass
 
     if model_check == 'works':
-        new_ov = round(riptide.slim_optimize(error_value=0.), 4)
-        old_ov = round(model.slim_optimize(error_value=0.), 4)
+        new_ov = round(riptide.slim_optimize(), 2)
+        old_ov = round(model.slim_optimize(), 2)
         perc_shift = 100.0 - ((float(new_ov) / float(old_ov)) * 100.0)
         report_dict['obj_change'] = round(perc_shift, 2)
         if perc_shift == 0.0:
-            if silent == False:
-                print('No change in objective flux of ~' + str(new_ov))
+            pass
         elif perc_shift > 0.0:
             perc_shift = round(abs(perc_shift), 2)
             if silent == False:
-                if phase == 1:
-                    print('Flux through the objective DECREASED to ~' + str(new_ov) + ' from ~' + str(old_ov) + ' (' + str(perc_shift) + '% change)')
+                print('Flux through the objective DECREASED to ~' + str(new_ov) + ' from ~' + str(old_ov) + ' (' + str(perc_shift) + '% change)')
         elif perc_shift < 0.0:
             perc_shift = round(abs(perc_shift), 2)
             if silent == False:
-                if phase == 1:
-                    print('Flux through the objective INCREASED to ~' + str(new_ov) + ' from ' + str(old_ov) + ' (' + str(perc_shift) + '% change)')
+                print('Flux through the objective INCREASED to ~' + str(new_ov) + ' from ' + str(old_ov) + ' (' + str(perc_shift) + '% change)')
     else:
         report_dict['obj_change'] = 'fails'
-        if silent == False:
-            print('WARNING: Context-specific model has no objective flux.')
 
     # Report concordance
     if concordance != 'Not performed':
         rho = 'r=' + str(round(concordance['r'], 3))
         if concordance['p'] <= 0.05:
             p_val = round(concordance['p'], 3)
             if p_val == 0.0:
                 p_val = 'p<0.001 *'
             else:
                 p_val = 'p=' + str(p_val) + ' *'
             if silent == False:
-                if phase == 1:
-                    print('Context-specific metabolism correlates with transcriptome (' + rho + ', ' + p_val + ')')
+                print('Context-specific metabolism correlates with transcriptome (' + rho + ', ' + p_val + ')')
         else:
             if silent == False:
-                if phase == 1:
-                    print('Context-specific metabolism does not correlate with transcriptome (' + rho + ', n.s.)')
+                print('Context-specific metabolism does not correlate with transcriptome (' + rho + ', n.s.)')
 
     # Run time
     raw_seconds = int(round(time.time() - start_time))
     report_dict['run_time'] = raw_seconds
     if silent == False:
         if raw_seconds < 60:
-            if phase == 1:
-                print('\nRIPTiDe completed in ' + str(raw_seconds) + ' seconds\n')
+            print('\nRIPTiDe completed in ' + str(raw_seconds) + ' seconds\n')
         else:
             minutes, seconds = divmod(raw_seconds, 60)
             mins = 'minute'
             if minutes > 1:
                 mins = 'minutes'
             secs = 'second'
             if seconds > 1:
                 secs = 'seconds'
             
-            if phase == 1:
+            if mf == False:
                 print('\nRIPTiDe completed in,', str(minutes), mins, 'and', str(int(seconds)), secs, '\n')
-            
-    return report_dict
-
-
-# Calculate rough estimate of solution space based on uptake exchange bounds
-def _test_exchange_space(model, minimum=1e5):
-    
-    with model as m:
-        curr_medium = model.medium
-        lbs = list(curr_medium.values())
-        lbs.sort(reverse=True)
-        
-        space = numpy.prod(lbs[:3])
-
-    if space >= minimum and len(lbs) < 4:
-        return True
-    else:
-        return False
+            else:
+                print('\nMaxfit RIPTiDe completed in,', str(minutes), mins, 'and', str(int(seconds)), secs, '\n')
 
+    return report_dict
 
 #-----------------------------------------------------------------#
 
 # gapsplit flux sampler
-# Adapted from:
 # Keaty TC & Jensen PA (2019). gapsplit: Efficient random sampling for non-convex constraint-based models.
 # bioRxiv 652917; doi: https://doi.org/10.1101/652917 
 
 def _gapsplit(model, depth):
-    warnings.filterwarnings('ignore') # Handle some infeasible warnings
-
-    fva = flux_variability_analysis(model, list(model.reactions), fraction_of_optimum=0.001, processes=1)
+    fva = flux_variability_analysis(model, model.reactions, fraction_of_optimum=0.001)
 
     # only split reactions with feasible range >= min_range
     idxs = (fva.maximum - fva.minimum >= 1e-5).to_numpy().nonzero()[0]
     weights = (1.0 / (fva.maximum - fva.minimum) ** 2).to_numpy()
     samples = numpy.zeros((depth, len(model.reactions)))
     k = 0
     for try_ in range(1000):
@@ -1309,15 +1166,14 @@
             k += 1
         if k >= depth: break
 
     if k < depth:
         # max_tries reached; return fewer samples
         samples = samples[:k,:]
 
-    warnings.filterwarnings('default')
     return pandas.DataFrame(data=samples, columns=fva.maximum.index)
 
 def _generate_sample(model, primary_var, primary_lb, primary_ub):
     
     # Formulate a [MI]QP to find a single solution
     with model:
         model.reactions[primary_var].lower_bound = primary_lb
@@ -1341,7 +1197,8 @@
     for i in range(width.size):
         left[i] = points[loc[i],i]
 
     relative = width / (points[-1,:] - points[0,:])
     target = left + width / 2.0
 
     return relative, target, width
+
```

