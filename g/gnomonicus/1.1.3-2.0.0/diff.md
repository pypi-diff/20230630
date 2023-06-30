# Comparing `tmp/gnomonicus-1.1.3.tar.gz` & `tmp/gnomonicus-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnomonicus-1.1.3.tar", last modified: Wed Mar 22 12:14:55 2023, max compression
+gzip compressed data, was "gnomonicus-2.0.0.tar", last modified: Fri Jun 30 10:10:09 2023, max compression
```

## Comparing `gnomonicus-1.1.3.tar` & `gnomonicus-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 12:14:55.256965 gnomonicus-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-03-22 12:14:14.000000 gnomonicus-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-03-22 12:14:55.256965 gnomonicus-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-03-22 12:14:14.000000 gnomonicus-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 12:14:55.252965 gnomonicus-1.1.3/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-22 12:14:14.000000 gnomonicus-1.1.3/bin/gbkToPkl
--rwxr-xr-x   0 runner    (1001) docker     (123)     7359 2023-03-22 12:14:14.000000 gnomonicus-1.1.3/bin/gnomonicus
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 12:14:55.252965 gnomonicus-1.1.3/gnomonicus/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-22 12:14:14.000000 gnomonicus-1.1.3/gnomonicus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40507 2023-03-22 12:14:14.000000 gnomonicus-1.1.3/gnomonicus/gnomonicus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 12:14:55.256965 gnomonicus-1.1.3/gnomonicus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-03-22 12:14:55.000000 gnomonicus-1.1.3/gnomonicus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-22 12:14:55.000000 gnomonicus-1.1.3/gnomonicus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 12:14:55.000000 gnomonicus-1.1.3/gnomonicus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 12:14:18.000000 gnomonicus-1.1.3/gnomonicus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 12:14:55.000000 gnomonicus-1.1.3/gnomonicus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 12:14:55.000000 gnomonicus-1.1.3/gnomonicus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-22 12:14:14.000000 gnomonicus-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-22 12:14:55.256965 gnomonicus-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:10:09.293426 gnomonicus-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-30 10:10:09.293426 gnomonicus-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:10:09.289426 gnomonicus-2.0.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/bin/gbkToPkl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8844 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/bin/gnomonicus
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:10:09.289426 gnomonicus-2.0.0/gnomonicus/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/gnomonicus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/gnomonicus/gnomonicus_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:10:09.293426 gnomonicus-2.0.0/gnomonicus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:09:20.000000 gnomonicus-2.0.0/gnomonicus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 10:10:09.000000 gnomonicus-2.0.0/gnomonicus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 10:09:11.000000 gnomonicus-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-30 10:10:09.293426 gnomonicus-2.0.0/setup.cfg
```

### Comparing `gnomonicus-1.1.3/LICENSE` & `gnomonicus-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gnomonicus-1.1.3/PKG-INFO` & `gnomonicus-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: gnomonicus
-Version: 1.1.3
+Version: 2.0.0
 Summary: Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 Home-page: https://github.com/oxfordmmm/gnomonicus
 Author: Philip W Fowler, Jeremy Westhead
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford License, see LICENSE
 Keywords: gnomonicus,piezo,lodestone,clockwork,TB
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Tests](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml) [![Build and release Docker](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml) [![Build and release PyPI](https://github.com/oxfordmmm/gnomonicus/actions/workflows/pypi.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/pypi.yaml) [![PyPI version](https://badge.fury.io/py/gnomonicus.svg)](https://badge.fury.io/py/gnomonicus)
+[![Tests](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml) 
+[![Build and release Docker](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml) 
+[![PyPI version](https://badge.fury.io/py/gnomonicus.svg)](https://badge.fury.io/py/gnomonicus)
+[![Docs](https://github.com/oxfordmmm/gnomonicus/actions/workflows/docs.yaml/badge.svg)](https://oxfordmmm.github.io/gnomonicus/)
 
 # gnomonicus
 Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variations
 
 Provides a library of functions for use within scripts, as well as a CLI tool for linking the functions together to produce output
 
+## Documentation
+API reference for developers, and CLI instructions can be found here: https://oxfordmmm.github.io/gnomonicus/ 
 ## Usage
 ```
-usage: gnomonicus [-h] --vcf_file VCF_FILE --genome_object GENOME_OBJECT [--catalogue_file CATALOGUE_FILE] [--ignore_vcf_filter] [--progress] [--output_dir OUTPUT_DIR] [--json] [--alt_json] [--fasta FASTA]
-                  [--minor_populations MINOR_POPULATIONS]
+usage: gnomonicus [-h] --vcf_file VCF_FILE --genome_object GENOME_OBJECT [--catalogue_file CATALOGUE_FILE] [--ignore_vcf_filter] [--progress] [--output_dir OUTPUT_DIR] [--json] [--fasta FASTA] [--minor_populations MINOR_POPULATIONS]
 
 options:
   -h, --help            show this help message and exit
   --vcf_file VCF_FILE   the path to a single VCF file
   --genome_object GENOME_OBJECT
                         the path to a compressed gumpy Genome object or a genbank file
   --catalogue_file CATALOGUE_FILE
                         the path to the resistance catalogue
   --ignore_vcf_filter   whether to ignore the FILTER field in the vcf (e.g. necessary for some versions of Clockwork VCFs)
   --progress            whether to show progress using tqdm
   --output_dir OUTPUT_DIR
                         Directory to save output files to. Defaults to wherever the script is run from.
   --json                Flag to create a single JSON output as well as the CSVs
-  --alt_json            Whether to produce the alternate JSON format. Requires the --json flag too
   --fasta FASTA         Use to output a FASTA file of the resultant genome. Specify either 'fixed' or 'variable' for fixed length and variable length FASTA respectively.
   --minor_populations MINOR_POPULATIONS
                         Path to a line separated file containing genome indices of minor populations.
 ```
 
 ## Helper usage
 As the main script can utilise pickled `gumpy.Genome` objects, there is a supplied helper script. This converts a Genbank file into a pickled gumpy.Genome for significant time saving.
```

### Comparing `gnomonicus-1.1.3/README.md` & `gnomonicus-2.0.0/gnomonicus.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,49 @@
-[![Tests](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml) [![Build and release Docker](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml) [![Build and release PyPI](https://github.com/oxfordmmm/gnomonicus/actions/workflows/pypi.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/pypi.yaml) [![PyPI version](https://badge.fury.io/py/gnomonicus.svg)](https://badge.fury.io/py/gnomonicus)
+Metadata-Version: 2.1
+Name: gnomonicus
+Version: 2.0.0
+Summary: Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
+Home-page: https://github.com/oxfordmmm/gnomonicus
+Author: Philip W Fowler, Jeremy Westhead
+Author-email: philip.fowler@ndm.ox.ac.uk
+License: University of Oxford License, see LICENSE
+Keywords: gnomonicus,piezo,lodestone,clockwork,TB
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Tests](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml) 
+[![Build and release Docker](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml) 
+[![PyPI version](https://badge.fury.io/py/gnomonicus.svg)](https://badge.fury.io/py/gnomonicus)
+[![Docs](https://github.com/oxfordmmm/gnomonicus/actions/workflows/docs.yaml/badge.svg)](https://oxfordmmm.github.io/gnomonicus/)
 
 # gnomonicus
 Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variations
 
 Provides a library of functions for use within scripts, as well as a CLI tool for linking the functions together to produce output
 
+## Documentation
+API reference for developers, and CLI instructions can be found here: https://oxfordmmm.github.io/gnomonicus/ 
 ## Usage
 ```
-usage: gnomonicus [-h] --vcf_file VCF_FILE --genome_object GENOME_OBJECT [--catalogue_file CATALOGUE_FILE] [--ignore_vcf_filter] [--progress] [--output_dir OUTPUT_DIR] [--json] [--alt_json] [--fasta FASTA]
-                  [--minor_populations MINOR_POPULATIONS]
+usage: gnomonicus [-h] --vcf_file VCF_FILE --genome_object GENOME_OBJECT [--catalogue_file CATALOGUE_FILE] [--ignore_vcf_filter] [--progress] [--output_dir OUTPUT_DIR] [--json] [--fasta FASTA] [--minor_populations MINOR_POPULATIONS]
 
 options:
   -h, --help            show this help message and exit
   --vcf_file VCF_FILE   the path to a single VCF file
   --genome_object GENOME_OBJECT
                         the path to a compressed gumpy Genome object or a genbank file
   --catalogue_file CATALOGUE_FILE
                         the path to the resistance catalogue
   --ignore_vcf_filter   whether to ignore the FILTER field in the vcf (e.g. necessary for some versions of Clockwork VCFs)
   --progress            whether to show progress using tqdm
   --output_dir OUTPUT_DIR
                         Directory to save output files to. Defaults to wherever the script is run from.
   --json                Flag to create a single JSON output as well as the CSVs
-  --alt_json            Whether to produce the alternate JSON format. Requires the --json flag too
   --fasta FASTA         Use to output a FASTA file of the resultant genome. Specify either 'fixed' or 'variable' for fixed length and variable length FASTA respectively.
   --minor_populations MINOR_POPULATIONS
                         Path to a line separated file containing genome indices of minor populations.
 ```
 
 ## Helper usage
 As the main script can utilise pickled `gumpy.Genome` objects, there is a supplied helper script. This converts a Genbank file into a pickled gumpy.Genome for significant time saving.
@@ -93,8 +110,8 @@
 
 3. In general, I would also like the option to output fixed- and variable-length FASTA files (the latter takes into account insertions and deletions described in any input VCF file).
 
 ## Unit testing
 
 For speed, rather than use NC_000962.3 (i.e. H37Rv *M. tuberculosis*), we shall use SARS-CoV-2 and have created a fictious drug resistance catalogue, along with some `vcf` files and the expected outputs in `tests/`.
 
-These can be run with `pytest -vv`
+These can be run with `pytest -vv`
```

### Comparing `gnomonicus-1.1.3/bin/gbkToPkl` & `gnomonicus-2.0.0/bin/gbkToPkl`

 * *Files 22% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 Designed to be run once on the host to provide significant speed up for containerised
 workflows. Resultant pickles should not be sent/recieved!!
 '''
 import sys
 import pickle
 import gzip
 import gumpy
+import argparse
 
 if __name__ == "__main__":
-    if len(sys.argv) < 2:
-        print("Usage: gbkToPkl <genbank path> [--compress]")
+    parser = argparse.ArgumentParser()
+    parser.add_argument("genbank_file", help="Path to a genbank file")
+    parser.add_argument("--compress", required=False, action='store_true', default=False, help="Whether to gzip compress the output pickle.")
+    options = parser.parse_args()
+    
+    g = gumpy.Genome(options.genbank_file, show_progress_bar=True)
+    if options.compress:
+        #Save as gzipped version
+        print("Compressing with gzip...")
+        f = gzip.open(sys.argv[1]+".pkl", 'wb', compresslevel=2)
     else:
-        g = gumpy.Genome(sys.argv[1], show_progress_bar=True)
-        if len(sys.argv) == 3 and sys.argv[2] == '--compress':
-            #Save as gzipped version
-            print("Compressing with gzip...")
-            f = gzip.open(sys.argv[1]+".pkl", 'wb', compresslevel=2)
-        else:
-            #Save without gzip
-            f = open(sys.argv[1]+".pkl", 'wb')
-        pickle.dump(g, f)
-        f.close()
+        #Save without gzip
+        f = open(sys.argv[1]+".pkl", 'wb')
+    pickle.dump(g, f)
+    f.close()
```

### Comparing `gnomonicus-1.1.3/bin/gnomonicus` & `gnomonicus-2.0.0/bin/gnomonicus`

 * *Files 12% similar despite different names*

```diff
@@ -7,45 +7,72 @@
 import logging
 import os
 import time
 
 import gumpy
 import piezo
 
-from gnomonicus import loadGenome, NoVariantsException, populateVariants, populateMutations, populateEffects, saveJSON, toAltJSON
+from gnomonicus import loadGenome, populateVariants, populateMutations, populateEffects, saveJSON
 import gnomonicus
 
 if __name__ == "__main__":
     start = time.time()
     #Argparser setup
     parser = argparse.ArgumentParser()
     parser.add_argument("--vcf_file",required=True,help="the path to a single VCF file")
     parser.add_argument("--genome_object",required=True,help="the path to a compressed gumpy Genome object or a genbank file")
     parser.add_argument("--catalogue_file",default=None,required=False,help="the path to the resistance catalogue")
     parser.add_argument("--ignore_vcf_filter",action='store_true',default=False,help="whether to ignore the FILTER field in the vcf (e.g. necessary for some versions of Clockwork VCFs)")
     parser.add_argument("--progress",action='store_true',default=False,help="whether to show progress using tqdm")
     parser.add_argument("--output_dir", required=False, default=".", help="Directory to save output files to. Defaults to wherever the script is run from.")
     parser.add_argument("--json", required=False, action='store_true', default=False, help="Flag to create a single JSON output as well as the CSVs")
-    parser.add_argument("--alt_json", required=False, default=False, action='store_true', help="Whether to produce the alternate JSON format. Requires the --json flag too")
-    parser.add_argument("--fasta", required=False, default=None, help="Use to output a FASTA file of the resultant genome. Specify either 'fixed' or 'variable' for fixed length and variable length FASTA respectively.")
+    parser.add_argument("--fasta", required=False, default=None, help="Use to output a FASTA file of the resultant genome. Specify either 'fixed' or 'variable' for fixed length and variable length FASTA respectively. Alternatively, use 'both' to produce both")
     parser.add_argument("--minor_populations", required=False, default=None, help="Path to a line separated file containing genome indices of minor populations.")
+    parser.add_argument("--csvs", required=False, nargs="+", help="Types of CSV to produce. Accepted values are [variants, mutations, effects, predictions, all]. `all` produces all of the CSVs")
+    parser.add_argument("--debug", default=False, action='store_true', help='Whether to log debugging messages to the log. Defaults to False')
     options = parser.parse_args()
 
     options.output_dir = os.path.realpath(options.output_dir)
 
     #Make the output directory if it doesn't already exist
     os.makedirs(options.output_dir, exist_ok=True)
 
     #Get the stem of the VCF filename for use as a unique ID
-    vcfStem = os.path.split(options.vcf_file)[-1].split(".")[0]
+    vcfStem = os.path.split(options.vcf_file)[-1].replace(".vcf", "")
 
     #Logging setup
-    logging.basicConfig(filename=os.path.join(options.output_dir, f'{vcfStem}.gnomonicus.log'), filemode='w', format='%(asctime)s -  %(levelname)s - %(message)s', datefmt='%d-%b-%y %H:%M:%S', level=logging.DEBUG)
+    if options.debug:
+        LOG_LEVEL = logging.DEBUG
+    else:
+        LOG_LEVEL = logging.WARNING
+    logging.basicConfig(filename=os.path.join(options.output_dir, f'{vcfStem}.gnomonicus.log'), filemode='w', format='%(asctime)s -  %(levelname)s - %(message)s', datefmt='%d-%b-%y %H:%M:%S', level=LOG_LEVEL)
     logging.info(f"gnomonicus starting with output directory {options.output_dir}")
 
+    #Figure out which CSVs should be produced
+    if options.csvs is None:
+        make_variants_csv = False
+        make_mutations_csv = False
+        make_effects_csv = False
+        make_prediction_csv = False
+    elif "all" in options.csvs:
+        make_variants_csv = True
+        make_mutations_csv = True
+        make_effects_csv = True
+        make_prediction_csv = True
+    else:
+        make_variants_csv = "variants" in options.csvs
+        make_mutations_csv = "mutations" in options.csvs
+        make_effects_csv = "effects" in options.csvs
+        make_prediction_csv = "predictions" in options.csvs
+    
+    if options.csvs is None and options.json is False and options.fasta is None:
+        #No files will be created so warn the user
+        print("[WARNING]: No outputs selected. No files will be created. For help, try `gnomonicus --help`")
+        logging.warning("No outputs selected. No files will be created")
+
 
     #Get reference genome
     reference = loadGenome(options.genome_object, options.progress)
     logging.debug("Loaded reference genome")
 
     #Check if we have minor population indices
     if options.minor_populations is not None:
@@ -81,30 +108,30 @@
     #Get the GenomeDifference for extracting genome level mutations
     diff = reference - sample
     logging.debug("Got the genome difference")
 
     #Complain if there are no variants
     if diff.variants is None:
         logging.error("No variants detected!")
-        raise NoVariantsException()
+        raise Exception("No variants detected!")
 
     #Get the variations and mutations
-    variants = populateVariants(vcfStem, options.output_dir, diff, catalogue=resistanceCatalogue)
+    variants = populateVariants(vcfStem, options.output_dir, diff, make_variants_csv, catalogue=resistanceCatalogue)
     logging.debug("Populated and saved variants.csv")
 
     mutations, referenceGenes = populateMutations(vcfStem, options.output_dir, diff, 
-                        reference, sample, resistanceCatalogue)
+                        reference, sample, resistanceCatalogue, make_mutations_csv)
     if mutations is None:
         logging.info("No mutations found - probably due to exclusively inter-gene variation or no variation.\n\t\t\t\t\t\t\t No effects.csv written")
     else:
         logging.debug("Populated and saved mutatons.csv")
 
     #Get the effects of the mutations
     if resistanceCatalogue is not None and mutations is not None:
-        effects, metadata = populateEffects(options.output_dir, resistanceCatalogue, mutations, referenceGenes, vcfStem)
+        effects, metadata = populateEffects(options.output_dir, resistanceCatalogue, mutations, referenceGenes, vcfStem, make_effects_csv, make_prediction_csv)
         logging.debug("Populated and saved effects.csv")
     else:
         metadata = {}
         effects = None
         logging.info("Skipped effects.csv due to lack of resistance catalogue or mutations")
 
     #Add data to the log
@@ -122,21 +149,20 @@
         logging.info(f"Catalogue path: {options.catalogue_file}")
     for drug in sorted(metadata.keys()):
         logging.info(f"{drug} {metadata[drug]}")
     logging.info(f"Completed in {time.time()-start}s")
 
     if options.json:
         #Default prediction values are RFUS but use piezo catalogue's values if existing
-        values = resistanceCatalogue.catalogue.values
-        if not values:
+        values = resistanceCatalogue.catalogue.values if resistanceCatalogue is not None else None
+        if values is None:
             values = list("RFUS")
         logging.info(f"Saving a JSON... See {options.output_dir}/gnomonicus-out.json")
-        saveJSON(variants, mutations, effects, options.output_dir, vcfStem, values, gnomonicus.__version__)
-        if options.alt_json:
-            logging.info(f"Saving the alternate JSON too... See {options.output_dir}/alt-gnomonicus-out.json")
-            toAltJSON(options.output_dir, reference, vcfStem, resistanceCatalogue.catalogue.name)
+        saveJSON(variants, mutations, effects, options.output_dir, vcfStem, resistanceCatalogue, gnomonicus.__version__, time.time()-start, reference, options.vcf_file, options.genome_object, options.catalogue_file)
 
     if options.fasta and options.fasta.lower() in ['fixed', 'variable']:
         fixed = options.fasta.lower() == 'fixed'
         #Write the resultant fasta file
         sample.save_fasta(os.path.join(options.output_dir, vcfStem+"-"+options.fasta+".fasta"), fixed_length=fixed)
-        
+    elif options.fasta and options.fasta.lower() == 'both':
+        sample.save_fasta(os.path.join(options.output_dir, vcfStem+"-fixed.fasta"), fixed_length=True)
+        sample.save_fasta(os.path.join(options.output_dir, vcfStem+"-variable.fasta"), fixed_length=False)
```

### Comparing `gnomonicus-1.1.3/gnomonicus/__init__.py` & `gnomonicus-2.0.0/gnomonicus/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-'''gnomonicus.py is a library providing functions which pull together output VCF of the Lodestone TB pipeline
+'''gnomonicus is a library providing functions which pull together output VCF of the Lodestone TB pipeline
     with a reference genome and a resistance catalogue, and utilise gumpy and
     piezo to produce variants, mutations and an antibiogram.
 
 Provides a CLI script (bin/gnomonicus) which links these functions together to produce all outputs from the inputs.
 Makes the assumption that VCF files are named `<GUID>.vcf`
 
 Classes:
-    MissingFieldException
-    NoVariantsException
-    InvalidMutationException
+    * MissingFieldException
+    * InvalidMutationException
 
 Functions:
-    loadGenome
-    populateVariants
-    populateMutations
-    populateEffects
-    assignMutationBools
-    countNucleotideChanges
-    saveJSON
+    * loadGenome
+    * populateVariants
+    * populateMutations
+    * populateEffects
+    * assignMutationBools
+    * countNucleotideChanges
+    * saveJSON
 '''
 import importlib.metadata
 
 __version__ = importlib.metadata.version("gnomonicus")
 
-from .gnomonicus import (loadGenome, populateVariants, populateMutations, populateEffects, assignMutationBools,
-                        countNucleotideChanges, NoVariantsException, InvalidMutationException,
-                        saveJSON, toAltJSON, handleIndels)
+from .gnomonicus_lib import (loadGenome, populateVariants, populateMutations, populateEffects,
+                        minority_population_variants, InvalidMutationException,
+                        saveJSON)
```

### Comparing `gnomonicus-1.1.3/gnomonicus/gnomonicus.py` & `gnomonicus-2.0.0/gnomonicus/gnomonicus_lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 '''gnomonicus.py is a library providing functions which pull together output VCF of the Lodestone TB pipeline
     with a reference genome and a resistance catalogue, and utilise gumpy and
     piezo to produce variants, mutations and an antibiogram.
 
 Based on sp3predict
 '''
+import copy
 import datetime
 import gzip
 import json
 import logging
 import os
 import pickle
 import re
@@ -16,34 +17,14 @@
 
 import gumpy
 import numpy as np
 import pandas as pd
 import piezo
 from tqdm import tqdm
 
-
-# class MissingFieldException(Exception):
-#     '''Custom exception for when required fields are missing from a given table
-#     '''
-#     def __init__(self, field: str, table: str) -> None:
-#         '''Raise this exception
-
-#         Args:
-#             field (str): Field name missing
-#             table (str): Table which the field is missing from
-#         '''
-#         self.message = f"Field: {field} is not in the {table} table!"
-#         super().__init__(self.message)
-
-class NoVariantsException(Exception):
-    '''Custom exception raised when there are no variants detected
-    '''
-    def __init__(self):
-        super().__init__("No variants were detected!")
-
 class InvalidMutationException(Exception):
     '''Custom exception raised when an invalid mutation is detected
     '''
     def __init__(self, gene: str, mutation: str):
         '''Raise this exception
 
         Args:
@@ -116,64 +97,53 @@
         logging.info(f"No pickled version of genome object, instanciating and dumping. Error: {e}")
     
     #Create new gumpy.Genome and pickle dump for speed later
     reference = gumpy.Genome(path, show_progress_bar=progress)
     pickle.dump(reference, open(path+'.pkl', 'wb'))
     return reference
 
-def populateVariants(vcfStem: str, outputDir: str, diff: gumpy.GenomeDifference, catalogue: piezo.ResistanceCatalogue=None) -> pd.DataFrame:
+def populateVariants(vcfStem: str, outputDir: str, diff: gumpy.GenomeDifference, make_csv: bool, catalogue: piezo.ResistanceCatalogue=None) -> pd.DataFrame:
     '''Populate and save the variants DataFrame as a CSV
 
     Args:
         vcfStem (str): The stem of the filename for the VCF file. Used as a uniqueID
         outputDir (str): Path to the desired output directory
         diff (gumpy.GenomeDifference): GenomeDifference object between reference and the sample
+        make_csv (bool): Whether to write the CSV of the dataframe
         catalogue (piezo.ResistanceCatalogue, optional): Catalogue for determining FRS or COV for minority populations. If None is given, FRS is assumed. Defaults to None
     
     Returns:
         pd.DataFrame: DataFrame of the variants
     '''
     #Populate variants table directly from GenomeDifference
     vals = {
-            'VARIANT': diff.variants, 
-            'NUCLEOTIDE_INDEX': diff.nucleotide_index,
-            'IS_INDEL': diff.is_indel,
-            'IS_NULL': diff.is_null,
-            'IS_HET': diff.is_het,
-            'IS_SNP': diff.is_snp,
-            'INDEL_LENGTH': diff.indel_length,
-            'INDEL_NUCLEOTIDES': diff.indel_nucleotides
+            'variant': diff.variants, 
+            'nucleotide_index': diff.nucleotide_index,
+            'indel_length': diff.indel_length,
+            'indel_nucleotides': diff.indel_nucleotides,
+            'vcf_evidence': [json.dumps(x) for x in diff.vcf_evidences],
+            'vcf_idx': diff.vcf_idx,
+            'gene_name': diff.gene_name,
+            'gene_position': diff.gene_pos,
+            'codon_idx': diff.codon_idx
             }
-    vals = handleIndels(vals)
     variants = pd.DataFrame(vals)
-    variants = variants.astype({
-                                    'IS_INDEL': 'bool',
-                                    'IS_NULL': 'bool',
-                                    'IS_HET': 'bool',
-                                    'IS_SNP': 'bool'
-                                })
     if diff.genome1.minor_populations or diff.genome2.minor_populations:
         variants = pd.concat([variants, minority_population_variants(diff, catalogue)])
 
     #If there are variants, save them to a csv
     if not variants.empty:
         #Add unique ID to each record
-        variants['UNIQUEID'] = vcfStem
-
-        #Double check for required fields
-        #I don't think these can ever be reached... Commenting out for now
-        # if 'VARIANT' not in variants.columns:
-        #     logging.error("VARIANT not in variant table!")
-        #     raise MissingFieldException('VARIANT', 'variant')
-        # if 'IS_SNP' not in variants.columns:
-        #     logging.error("IS_SNP not in variant table!")
-        #     raise MissingFieldException('IS_SNP', 'variant')
+        variants['uniqueid'] = vcfStem
 
-        #Save CSV
-        variants.to_csv(os.path.join(outputDir, f'{vcfStem}.variants.csv'), header=True, index=False)
+        variants = variants[['uniqueid', 'variant', 'gene_name', 'gene_position', 'codon_idx', 'nucleotide_index', 'indel_length', 'indel_nucleotides', 'vcf_evidence', 'vcf_idx']]
+        variants = variants.drop_duplicates()
+        if make_csv:
+            #Save CSV
+            variants.to_csv(os.path.join(outputDir, f'{vcfStem}.variants.csv'), header=True, index=False)
     variants.reset_index(inplace=True)
     return variants
 
 def get_minority_population_type(catalogue: piezo.ResistanceCatalogue) -> str:
     '''Figure out if a catalogue uses FRS or COV. If neither or both, default to FRS
 
     Args:
@@ -202,24 +172,25 @@
     if cov > 0 and frs == 0:
         return 'reads'
     #We have anything else
     return 'percentage'
 
 def populateMutations(
         vcfStem: str, outputDir: str, diff: gumpy.GenomeDifference, reference: gumpy.Genome,
-        sample: gumpy.Genome, resistanceCatalogue: piezo.ResistanceCatalogue) -> (pd.DataFrame, dict):
+        sample: gumpy.Genome, resistanceCatalogue: piezo.ResistanceCatalogue, make_csv: bool) -> (pd.DataFrame, dict):
     '''Popuate and save the mutations DataFrame as a CSV, then return it for use in predictions
 
     Args:
         vcfStem (str): The stem of the filename of the VCF file. Used as a uniqueID
         outputDir (str): Path to the desired output directory
         diff (gumpy.GenomeDifference): GenomeDifference object between reference and this sample
         reference (gumpy.Genome): Reference genome
         sample (gumpy.Genome): Sample genome
         resistanceCatalogue (piezo.ResistanceCatalogue): Resistance catalogue (used to find which genes to check)
+        make_csv (bool): Whether to write the CSV of the dataframe
 
     Raises:
         MissingFieldException: Raised when the mutations DataFrame does not contain the required fields
 
     Returns:
         pd.DataFrame: The mutations DataFrame
         dict: Dictionary mapping gene name --> reference gumpy.Gene object
@@ -234,14 +205,21 @@
         #Make sure minority population mutations are also picked up
         minor_genes = set()
         for population in sample.minor_populations:
             for gene in reference.stacked_gene_name[reference.stacked_nucleotide_index == population[0]]:
                 if gene:
                     minor_genes.add(gene)
         genesWithMutations += minor_genes
+
+        deletions = []
+        #Make sure large deletions are picked up too
+        for name in reference.stacked_gene_name:
+            deletions += np.unique(name[sample.is_deleted]).tolist()
+        genesWithMutations = set(genesWithMutations + deletions)
+
     else:
         #No catalogue, so just stick to genes in the sample
         genesWithMutations = sample.genes
 
     #Iter resistance genes with variation to produce gene level mutations - concating into a single dataframe
     mutations = None
     referenceGenes = {}
@@ -258,108 +236,100 @@
             referenceGenes[gene] = refGene
             #Get gene difference
             diff = refGene - sample.build_gene(gene)
             diffs.append(diff)
 
             #Pull the data out of the gumpy object
             vals = {
-                'MUTATION': diff.mutations,
-                'NUCLEOTIDE_NUMBER': diff.nucleotide_number,
-                'NUCLEOTIDE_INDEX': diff.nucleotide_index,
-                'GENE_POSITION': diff.gene_position,
-                'ALT': diff.alt_nucleotides,
-                'REF': diff.ref_nucleotides,
-                'CODES_PROTEIN': diff.codes_protein,
-                'INDEL_LENGTH': diff.indel_length,
-                'INDEL_NUCLEOTIDES': diff.indel_nucleotides,
-                'IS_CDS': diff.is_cds,
-                'IS_HET': diff.is_het,
-                'IS_NULL': diff.is_null,
-                'IS_PROMOTER': diff.is_promoter,
-                'IS_SNP': diff.is_snp,
+                'mutation': diff.mutations,
+                'nucleotide_number': diff.nucleotide_number,
+                'nucleotide_index': diff.nucleotide_index,
+                'gene_position': diff.gene_position,
+                'alt': diff.alt_nucleotides,
+                'ref': diff.ref_nucleotides,
+                'codes_protein': [diff.codes_protein and pos > 0 if pos is not None else diff.codes_protein for pos in diff.gene_position],
+                'indel_length': diff.indel_length,
+                'indel_nucleotides': diff.indel_nucleotides,
                 }
             #As diff does not populate amino acid items for non-coding genes,
             #pull out the sequence or default to None
             if refGene.codes_protein:
-                vals['AMINO_ACID_NUMBER'] = diff.amino_acid_number
+                vals['amino_acid_number'] = diff.amino_acid_number
                 aa_seq = []
                 #Pull out the amino acid sequence from the alt codons
                 for idx, num in enumerate(diff.amino_acid_number):
                     if num is not None:
                         aa_seq.append(refGene.codon_to_amino_acid[diff.alt_nucleotides[idx]])
                     else:
                         aa_seq.append(None)
-                vals['AMINO_ACID_SEQUENCE'] = np.array(aa_seq)
+                vals['amino_acid_sequence'] = np.array(aa_seq)
             else:
-                vals['AMINO_ACID_NUMBER'] = None
-                vals['AMINO_ACID_SEQUENCE'] = None
-            vals = handleIndels(vals)
+                vals['amino_acid_number'] = None
+                vals['amino_acid_sequence'] = None
+            
+            vals['number_nucleotide_changes'] = [sum(i!=j for (i,j) in zip(r, a)) if r is not None and a is not None else None for r, a in zip(vals['ref'], vals['alt'])]
             
             geneMutations = pd.DataFrame(vals)
             #Add gene name
-            geneMutations['GENE'] = gene
+            geneMutations['gene'] = gene
 
             #Add this gene's mutations to the total dataframe
             if not geneMutations.empty:
                 if mutations is not None:
                     mutations = pd.concat([mutations, geneMutations])
                 else:
                     mutations = geneMutations
     if mutations is not None:
         #Ensure correct datatypes
-        mutations = mutations.astype({'MUTATION': 'str',
-                                    'GENE': 'str',
-                                    'NUCLEOTIDE_NUMBER': 'float',
-                                    'NUCLEOTIDE_INDEX': 'float',
-                                    'GENE_POSITION': 'float',
-                                    'ALT': 'str',
-                                    'REF': 'str',
-                                    'CODES_PROTEIN': 'bool',
-                                    'INDEL_LENGTH': 'float',
-                                    'INDEL_NUCLEOTIDES': 'str',
-                                    'IS_CDS': 'bool',
-                                    'IS_HET': 'bool',
-                                    'IS_NULL': 'bool',
-                                    'IS_PROMOTER': 'bool',
-                                    'IS_SNP': 'bool',
-                                    'AMINO_ACID_NUMBER': 'float',
-                                    'AMINO_ACID_SEQUENCE': 'str'
+        mutations = mutations.astype({'mutation': 'str',
+                                    'gene': 'str',
+                                    'nucleotide_number': 'float',
+                                    'nucleotide_index': 'float',
+                                    'gene_position': 'float',
+                                    'alt': 'str',
+                                    'ref': 'str',
+                                    'codes_protein': 'bool',
+                                    'indel_length': 'float',
+                                    'indel_nucleotides': 'str',
+                                    'amino_acid_number': 'float',
+                                    'amino_acid_sequence': 'str',
                                 })
     #Add minor mutations (these are stored separately)
     if reference.minor_populations or sample.minor_populations:
         #Only do this if they exist
-        mutations = pd.concat([mutations, minority_population_mutations(diffs, resistanceCatalogue)])
-
+        x = minority_population_mutations(diffs, resistanceCatalogue)
+        mutations = pd.concat([mutations, x])
     #If there were mutations, write them to a CSV
     if mutations is not None:
-        #Add synonymous booleans for analysis later
-        mutations[['IS_SYNONYMOUS','IS_NONSYNONYMOUS']] = mutations.apply(assignMutationBools, axis=1)
 
         #Add the number of mutations which occured for this mutation
-        mutations['NUMBER_NUCLEOTIDE_CHANGES'] = mutations.apply(countNucleotideChanges, axis=1)
 
         #Add VCF stem as the uniqueID
-        mutations['UNIQUEID'] = vcfStem
-
-
-        #Raise errors if required fields are missing
-        #I'm pretty sure these are unreachable... commenting out for now
-        # if 'GENE' not in mutations.columns:
-        #     logging.error("GENE is not in the mutations table")
-        #     raise MissingFieldException('GENE', 'mutations')
-        # if 'MUTATION' not in mutations.columns:
-        #     logging.error("MUTATION is not in the mutations table")
-        #     raise MissingFieldException('MUTATION', 'mutations')
+        mutations['uniqueid'] = vcfStem
 
+        if make_csv:
+            #Reorder the columns
+            mutations = mutations[['uniqueid', 'gene', 'mutation', 'ref', 'alt', 'nucleotide_number', 'nucleotide_index', 'gene_position', 'codes_protein', 'indel_length', 'indel_nucleotides', 'amino_acid_number', 'amino_acid_sequence', 'number_nucleotide_changes']]
+            
+            #As we have concated several dataframes, the index is 0,1,2,0,1...
+            #Reset it so that we can use it to delete
+            mutations.reset_index(drop=True, inplace=True)
+            #Filter out nucleotide variants from synonymous mutations to avoid duplication of data
+            mutations_ = copy.deepcopy(mutations)
+            to_drop = []
+            for idx, row in mutations_.iterrows():
+                if row['codes_protein'] and row['ref'] is not None and row['alt'] is not None:
+                    #Protein coding so check if nucleotide within coding region
+                    if len(row['ref']) == 1:
+                        #Nucleotide SNP
+                        to_drop.append(idx)
+            mutations_.drop(index=to_drop, inplace=True)
+            #Save it as CSV
+            mutations_.to_csv(os.path.join(outputDir, f'{vcfStem}.mutations.csv'), index=False)
 
-        #Save it as CSV
-        mutations.to_csv(os.path.join(outputDir, f'{vcfStem}.mutations.csv'), index=False)
-
-        #Remove index to return
-        mutations.reset_index(inplace=True)
     return mutations, referenceGenes
 
 def minority_population_variants(diff: gumpy.GenomeDifference, catalogue: piezo.ResistanceCatalogue) -> pd.DataFrame:
     '''Handle the logic for pulling out minority population calls for genome level variants
 
     Args:
         diff: (gumpy.GenomeDifference): GenomeDifference object for this comparison
@@ -369,37 +339,179 @@
         pd.DataFrame: DataFrame containing the minority population data
     '''
     #Determine if FRS or COV should be used
     minor_type = get_minority_population_type(catalogue)
 
     #Get the variants in GARC
     variants_ = diff.minor_populations(interpretation=minor_type)
-    variants = [v.split(":")[0] for v in variants_]
+
+    nucleotide_indices = []
+    indel_lengths = []
+    indel_nucleotides = []
+    vcf_evidences = []
+    vcf_idx = []
+    gene_name = []
+    gene_pos = []
+    codon_idx = []
+    variants = []
+
+    for variant_ in variants_:
+        variant, evidence = variant_.split(":")
+        variants.append(variant_)
+        
+        if ">" in variant:
+            idx = int(variant.split(">")[0][:-1])
+            nucleotide_indices.append(idx)
+            vcf = diff.genome2.vcf_evidence.get(int(variant.split(">")[0][:-1]))
+            vcf_evidences.append(json.dumps(vcf))
+            
+            ref = variant.split(">")[0][-1]
+            alt = variant.split(">")[-1]
+
+            if ref == alt:
+                #Wildtype call so return 0 as it isn't an ALT
+                vcf_idx.append(0)
+            else:
+                #Simple SNP so check for presence in alts + right COV
+                ev = float(evidence)
+                if ev < 1:
+                    #We have FRS so (due to rounding) convert the VCF's COV to FRS
+                    cov = [round(x/vcf['DP'], 3) for x in vcf["COV"]]
+                else:
+                    cov = vcf['COV']
+                minor_call = variant.split(">")[-1]
+
+                added = False
+                for v_idx, alt in enumerate(vcf['ALTS']):
+                    v_idx += 1
+                    if added:
+                        #Already added so break
+                        break
+                    for i, a in enumerate(alt):
+                        if a == minor_call and idx == vcf["POS"] + i:
+                            #Match on call and position
+                            #Double check that the COV matches too
+                            if ev == cov[v_idx]:
+                                #This is the right element
+                                vcf_idx.append(v_idx)
+                                added = True
+
+                #Shouldn't be possible, but check anyway
+                assert added, f"The index of the VCF evidence could not be determined! {variant_} --> {vcf}"                        
+
+
+
+        else:
+            idx = int(variant.split("_")[0])
+            nucleotide_indices.append(idx)
+            vcf = diff.genome2.vcf_evidence.get(int(variant.split("_")[0]))
+            vcf_evidences.append(json.dumps(vcf))
+
+            #Match VCF idx on base changes + cov
+            ev = float(evidence)
+            if ev < 1:
+                #We have FRS so (due to rounding) convert the VCF's COV to FRS
+                cov = [round(x/vcf['DP'], 3) for x in vcf["COV"]]
+            else:
+                cov = vcf['COV']
+            
+            ref = vcf['REF']
+            type_ = variant.split("_")[1]
+            bases = variant.split("_")[-1]
+            added = False
+            for v_idx, alt in enumerate(vcf['ALTS']):
+                if added:
+                    break
+                v_idx += 1
+                #Use the same `simplify_call` method to decompose the ALTs into indels + snps
+                #Match on the indel + pos + cov
+                for call in diff.genome2.vcf_file._simplify_call(ref, alt):
+                    offset, t, b = call
+                    if vcf['POS'] + offset == idx and type_ == t and bases == b:
+                        #Match on pos, type and bases so check cov too
+                        if ev == cov[v_idx]:
+                            added = True
+                            vcf_idx.append(v_idx)
+            assert added, f"The index of the VCF evidence could not be determined! {variant_} --> {vcf}"                        
+            
+        if "_" in variant:
+            indel_lengths.append(len(variant.split("_")[-1]))
+            indel_nucleotides.append(variant.split("_")[-1])
+        else:
+            indel_lengths.append(0)
+            indel_nucleotides.append(None)
+
+        #Find the genes at this pos
+        genes = sorted(list(set(diff.genome1.stacked_gene_name[diff.genome1.stacked_nucleotide_index == idx])))
+        if len(genes) > 1:
+            #If we have genes, we need to duplicate some info
+            first = True
+            for gene in genes:
+                if gene == '':
+                    #If we have genes, we don't care about this one
+                    continue
+                    
+                gene_name.append(gene)
+                gene_pos.append(diff.get_gene_pos(gene, idx, variant))
+                if diff.genome1.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
+                    #Get codon idx
+                    nc_idx = diff.genome1.stacked_nucleotide_index[diff.genome1.stacked_gene_name == gene]
+                    nc_num = diff.genome1.stacked_nucleotide_number[diff.genome1.stacked_gene_name == gene]
+                    codon_idx.append(nc_num[nc_idx == idx][0] % 3)
+                else:
+                    codon_idx.append(None)
+                
+                #If this isn't the first one, we need to duplicate the row
+                if first:
+                    first = False
+                else:
+                    variants.append(variants[-1])
+                    nucleotide_indices.append(nucleotide_indices[-1])
+                    indel_lengths.append(indel_lengths[-1])
+                    indel_nucleotides.append(indel_nucleotides[-1])
+                    vcf_evidences.append(vcf_evidences[-1])
+                    vcf_idx.append(vcf_idx[-1])
+
+        else:
+            #We have 1 gene or none, so set to None if no gene is present
+            gene = genes[0] if genes[0] != '' else None
+            if gene is not None:
+                #Single gene, so pull out data
+                gene_name.append(gene)
+                gene_pos.append(diff.get_gene_pos(gene, idx, variant))
+
+                if diff.genome1.genes[gene]['codes_protein'] and gene_pos[-1] > 0:
+                    #Get codon idx
+                    nc_idx = diff.genome1.stacked_nucleotide_index[diff.genome1.stacked_gene_name == gene]
+                    nc_num = diff.genome1.stacked_nucleotide_number[diff.genome1.stacked_gene_name == gene]
+                    codon_idx.append(nc_num[nc_idx == idx][0] % 3)
+                else:
+                    codon_idx.append(None)
+            else:
+                gene_name.append(None)
+                gene_pos.append(None)
+                codon_idx.append(None)
+
 
 
-    #Split to be the same format
-    #Not exactly efficient, but this should be so infrequent that it shouldn't be impactful
     vals = {
-        'VARIANT': variants_, 
-        'NUCLEOTIDE_INDEX': [var.split(">")[0][:-1] if ">" in var else var.split("_")[0] for var in variants],
-        'IS_INDEL': ["_" in var for var in variants],
-        'IS_NULL': ["x" in var for var in variants],
-        'IS_HET': ["z" in var for var in variants],
-        'IS_SNP': [">" in var for var in variants],
-        'INDEL_LENGTH': [len(var.split("_")[-1]) if "_" in var else 0 for var in variants],
-        'INDEL_NUCLEOTIDES': [var.split("_")[-1] if "_" in var else None for var in variants]
+        'variant': variants, 
+        'nucleotide_index': nucleotide_indices,
+        'indel_length': indel_lengths,
+        'indel_nucleotides': indel_nucleotides,
+        'vcf_evidence': vcf_evidences,
+        'vcf_idx': vcf_idx,
+        'gene_name': gene_name,
+        'gene_position': gene_pos,
+        'codon_idx': codon_idx
         }
     #Convert everything to numpy arrays
     vals = {key: np.array(vals[key]) for key in vals.keys()}
-    handleIndels(vals)
     return pd.DataFrame(vals).astype({
-                                    'IS_INDEL': 'bool',
-                                    'IS_NULL': 'bool',
-                                    'IS_HET': 'bool',
-                                    'IS_SNP': 'bool'
+                                    'vcf_evidence': 'object'
                                 })
 
 
 def minority_population_mutations(diffs: [gumpy.GeneDifference], catalogue: piezo.ResistanceCatalogue) -> pd.DataFrame:
     '''Handle the logic for pulling out minority population calls for gene level variants
 
     Args:
@@ -423,43 +535,47 @@
     is_cds = []
     is_het = []
     is_null = []
     is_promoter = []
     is_snp = []
     aa_num = []
     aa_seq = []
+    variants = []
+    number_nucleotide_changes = []
 
     #Determine if FRS or COV should be used
     minor_type = get_minority_population_type(catalogue)
 
     for diff in diffs:
         #As mutations returns in GARC, split into constituents for symmetry with others
         mutations = diff.minor_populations(interpretation=minor_type)
         
         #Without gene names/evidence
-        muts = [mut.split("@")[1].split(":")[0] for mut in mutations]
+        muts = [ mut.split(":")[0]for mut in mutations]
         #Gene numbers
         numbers = [
             int(mut.split("_")[0]) if "_" in mut #Indel index: <idx>_<type>_<bases>
             else 
                 int(mut[:-1]) if "=" in mut #Synon SNP: <idx>=
                 else int(mut[1:][:-1]) #SNP: <ref><idx><alt>
             for mut in muts
             ]
 
         #Iter these to pull out all other details from the GeneDifference objects
         for mut, num, full_mut in zip(muts, numbers, mutations):
-            mutations_.append(full_mut.split("@")[1]) #Keep evidence in these
-            genes.append(full_mut.split("@")[0])
+            mutations_.append(full_mut) #Keep evidence in these
+            genes.append(diff.gene1.name)
             gene_pos.append(num)
-            codes_protein.append(diff.gene1.codes_protein)
+            codes_protein.append(diff.gene1.codes_protein and num > 0)
             is_cds.append(num > 0 and diff.gene1.codes_protein)
             is_het.append("Z" in mut.upper())
             is_null.append("X" in mut.upper())
             is_promoter.append(num < 0)
+            variants.append(None)
+            number_nucleotide_changes.append(diff.gene2.minor_nc_changes[num])
 
             if "_" in mut:
                 #Indel
                 _, t, bases = mut.split("_")
                 ref.append(None)
                 alt.append(None)
                 if t == "del":
@@ -467,241 +583,153 @@
                 else:
                     indel_length.append(len(bases))
                 indel_nucleotides.append(bases)
                 is_snp.append(False)
                 nucleotide_number.append(num)
                 nucleotide_index.append(diff.gene1.nucleotide_index[diff.gene1.nucleotide_number == num][0])
                 aa_num.append(None)
-                aa_seq.append(None)                
+                aa_seq.append(None)
                 continue
             else:
                 indel_length.append(None)
                 indel_nucleotides.append(None)
 
             if mut[0].isupper() or mut[0] == '!':
                 #Protein coding SNP
                 nucleotide_number.append(None)
                 nucleotide_index.append(None)
                 #Pull out codons for ref/alt
                 ref.append(diff.gene1.codons[diff.gene1.amino_acid_number == num][0])
-                alt.append(diff.gene2.codons[diff.gene2.amino_acid_number == num][0])
+                alt.append("zzz")
                 is_snp.append(True)
                 aa_num.append(num)
                 aa_seq.append(mut[-1])
             else:
                 #Other SNPs
                 nucleotide_number.append(num)
                 nucleotide_index.append(diff.gene1.nucleotide_index[diff.gene1.nucleotide_number == num][0])
                 aa_num.append(None)
                 aa_seq.append(None)
                 ref.append(diff.gene1.nucleotide_sequence[diff.gene1.nucleotide_number == num][0])
                 alt.append(diff.gene2.nucleotide_sequence[diff.gene2.nucleotide_number == num][0])
                 is_snp.append(True)
 
     vals = {
-        'MUTATION': mutations_,
-        'GENE': genes,
-        'NUCLEOTIDE_NUMBER': nucleotide_number,
-        'NUCLEOTIDE_INDEX': nucleotide_index,
-        'GENE_POSITION': gene_pos,
-        'ALT': alt,
-        'REF': ref,
-        'CODES_PROTEIN': codes_protein,
-        'INDEL_LENGTH': indel_length,
-        'INDEL_NUCLEOTIDES': indel_nucleotides,
-        'IS_CDS': is_cds,
-        'IS_HET': is_het,
-        'IS_NULL': is_null,
-        'IS_PROMOTER': is_promoter,
-        'IS_SNP': is_snp,
-        'AMINO_ACID_NUMBER': aa_num,
-        'AMINO_ACID_SEQUENCE': aa_seq
+        'mutation': mutations_,
+        'gene': genes,
+        'nucleotide_number': nucleotide_number,
+        'nucleotide_index': nucleotide_index,
+        'gene_position': gene_pos,
+        'alt': alt,
+        'ref': ref,
+        'codes_protein': codes_protein,
+        'indel_length': indel_length,
+        'indel_nucleotides': indel_nucleotides,
+        'amino_acid_number': aa_num,
+        'amino_acid_sequence': aa_seq,
+        'number_nucleotide_changes': number_nucleotide_changes
         }
-    #Convert everything to numpy arrays
-    vals = {key: np.array(vals[key]) for key in vals.keys()}
-
-    return pd.DataFrame(handleIndels(vals)).astype({'MUTATION': 'str',
-                                                    'GENE': 'str',
-                                                    'NUCLEOTIDE_NUMBER': 'float',
-                                                    'NUCLEOTIDE_INDEX': 'float',
-                                                    'GENE_POSITION': 'float',
-                                                    'ALT': 'str',
-                                                    'REF': 'str',
-                                                    'CODES_PROTEIN': 'bool',
-                                                    'INDEL_LENGTH': 'float',
-                                                    'INDEL_NUCLEOTIDES': 'str',
-                                                    'IS_CDS': 'bool',
-                                                    'IS_HET': 'bool',
-                                                    'IS_NULL': 'bool',
-                                                    'IS_PROMOTER': 'bool',
-                                                    'IS_SNP': 'bool',
-                                                    'AMINO_ACID_NUMBER': 'float',
-                                                    'AMINO_ACID_SEQUENCE': 'str'
-                                                })
-    
 
-
-
-def handleIndels(vals: dict) -> dict:
-    '''Due to how piezo works, we need to add alternative representations for indels
-        Gumpy returns indel mutations as <pos>_(ins|del)_<nucleotides>
-        Piezo catalogues may be that specific, or may require <pos>_indel or <pos>_(ins|del)_<n bases>
-
-    Args:
-        vals (dict): Initial mutation/variant values
-
-    Returns:
-        dict: Mutation/variant values with added indels as required
-    '''
-    #Determine if these are values from variants or mutations (as they have different struct)
-    if 'MUTATION' in vals.keys():
-        access = 'MUTATION'
-    elif 'VARIANT' in vals.keys():
-        access = 'VARIANT'
-    else:
-        raise NoVariantsException()
-
-    toAdd = {key: [] for key in vals.keys() if isinstance(vals[key], Iterable)}
-    toRemove = []
-    for (n, mutation) in enumerate(vals[access]):
-        #Check for minority populations first
-        minor = False
-        if ":" in mutation:
-            mutation, evidence = mutation.split(":")
-            minor = True
-        if 'ins' in mutation or 'del' in mutation:
-            #Is an indel so prepare extras to add and remove this
-            toRemove.append(n)
-            pos, indel, bases = mutation.split("_")
-            indels = [
-                pos + "_" + indel + "_" + bases,
-                pos + "_indel", 
-                pos + "_" + indel + "_" + str(len(bases))
-                ]
-            if minor:
-                #Add the evidence
-                indels = [i + ":" + evidence for i in indels]
-            #Add the extras to `toAdd`
-            for i in indels:
-                for key in toAdd.keys():
-                    #Add the extra to the MUTATION/VARIANT field
-                    if key == access:
-                        toAdd[key].append(i)
-                    #Leave the other fields unchanged
-                    else:
-                        toAdd[key].append(vals[key][n])
-    
-    #Concat the two dicts
-    for key in toAdd.keys():
-        vals[key] = vals[key].tolist()
-        #Delete the values, offsetting the index as required to refer to the correct item
-        for (i, n) in enumerate(toRemove):
-            del vals[key][n-i]
-        vals[key] = vals[key] + toAdd[key]
-    return vals
-    
-
-def assignMutationBools(row: pd.Series) -> pd.Series:
-    '''Create the appropriate values of 'IS_SYNONYMOUS' and ''IS_NONSYNONYMOUS' for 
-    the given row of a mutations dataframe
-
-    Args:
-        row (pd.Series): A row of the mutations dataframe
-
-    Returns:
-        pd.Series: A pandas series corresponding to [IS_SYNONYMOUS, IS_NONSYNONYMOUS]
-    '''
-    #In sp3predict this adds IS_HET and IS_NULL too, but these are added from gumpy.GeneDifference
-
-    #Synonymous mutations are within amino acids so check the mutation to see if of form X...X
-    if row['MUTATION'].isupper():
-        isSynon = row['MUTATION'][0] == row['MUTATION'][-1]
-        isNonSynon = not isSynon
-    else:
-        #Not an amino acid mutation so both False
-        isSynon = isNonSynon = False
-    
-    return pd.Series([isSynon, isNonSynon])
-
-def countNucleotideChanges(row: pd.Series) -> int:
-    '''Calculate the number of nucleotide changes required for a given row's amino acid mutation
-
-    Args:
-        row (pd.Series): A row of the mutations dataframe
-
-    Returns:
-        int: The number of mutations which occured to cause this mutation
-    '''
-    if row['REF'] is not None and len(row['REF'])==3:
-        #Numpy sum is considerably slower for this...
-        return sum(i!=j for (i,j) in zip(row['REF'],row['ALT'] ))
-    return 0
+    return pd.DataFrame(vals).astype({'mutation': 'str',
+                                        'gene': 'str',
+                                        'nucleotide_number': 'float',
+                                        'nucleotide_index': 'float',
+                                        'gene_position': 'float',
+                                        'alt': 'str',
+                                        'ref': 'str',
+                                        'codes_protein': 'bool',
+                                        'indel_length': 'float',
+                                        'indel_nucleotides': 'str',
+                                        'amino_acid_number': 'float',
+                                        'amino_acid_sequence': 'str',
+                                        'number_nucleotide_changes': 'int'
+                                    })
 
 def getMutations(mutations: pd.DataFrame, catalogue: piezo.catalogue, referenceGenes: dict) -> [[str, str]]:
     '''Get all of the mutations (including multi-mutations) from the mutations df
     Multi-mutations currently only exist within the converted WHO catalogue, and are a highly specific combination 
         of mutations which must all be present for a single resistance value.
 
     Args:
         mutations (pd.DataFrame): Mutations dataframe
         catalogue (piezo.catalogue): The resistance catalogue. Used to find which multi-mutations we care about
         referenceGenes (dict): Dictionary of geneName->gumpy.Gene
 
     Returns:
         [[str, str]]: List of [gene, mutation] or in the case of multi-mutations, [None, multi-mutation]
     '''
-    mutations = list(zip(mutations['GENE'], mutations['MUTATION']))
+    mutations = list(zip(mutations['gene'], mutations['mutation']))
     #Grab the multi-mutations from the catalogue
     #By doing this, we can check a fixed sample space rather than every permutation of the mutations
     #This makes the problem tractable, but does not address a possible issue with multi-mutations not encapsulating full codons
     multis = catalogue.catalogue.rules[catalogue.catalogue.rules['MUTATION_TYPE']=='MULTI']['MUTATION']
     if len(multis) > 0:
         #We have a catalogue including multi rules, so check if any of these are present in the mutations
         joined = [gene+'@'+mut for (gene, mut) in mutations]
         for multi in multis:
             check = True
             for mutation in multi.split("&"):
                 check = check and mutation in joined
             if check:
                 #This exact multi mutation exists, so add it to the mutations list
                 mutations.append((None, multi))
-    #Filtering out *just* nucelotide changes for cases of synon mutations
+    
+    #Check if the catalogue supports large deletions
+    if "GENE" in set(catalogue.catalogue.rules['MUTATION_AFFECTS']):
+        large_dels = True
+    else:
+        large_dels = False
+
+    #Filtering out *just* nucleotide changes for cases of synon mutations
     #The important part of these should have already been found by multi-mutations
     fixed = []
     for gene, mutation in mutations:
         if gene is not None and referenceGenes[gene].codes_protein:
             #Codes protein so check for nucleotide changes
             nucleotide = re.compile(r"""
                                 [acgtzx][0-9]+[acgtzx]
                                 """, re.VERBOSE)
             if nucleotide.fullmatch(mutation):
                 #Is a nucleotide (non-promoter) mutation in a coding gene
                 #So skip it as it may cause prediction problems
                 continue
+        #Remove large dels if not supported
+        if not large_dels:
+            #Check if this is a large del
+            large = re.compile(r"""
+                                del_(1\.0)|(0\.[0-9][0-9])
+                                """, re.VERBOSE)
+            if large.fullmatch(mutation):
+                continue
         fixed.append((gene, mutation))
     return fixed
 
 def populateEffects(
         outputDir: str, resistanceCatalogue: piezo.ResistanceCatalogue,
-        mutations: pd.DataFrame, referenceGenes: dict, vcfStem: str) -> (pd.DataFrame, dict):
+        mutations: pd.DataFrame, referenceGenes: dict, vcfStem: str, make_csv: bool, make_prediction_csv: bool) -> (pd.DataFrame, dict):
     '''Populate and save the effects DataFrame as a CSV
 
     Args:
         outputDir (str): Path to the directory to save the CSV
         resistanceCatalogue (piezo.ResistanceCatalogue): Resistance catalogue for predictions
         mutations (pd.DataFrame): Mutations dataframe
         referenceGenes (dict): Dictionary mapping gene name --> reference gumpy.Gene objects
         vcfStem (str): The basename of the given VCF - used as the sample name
+        make_csv (bool): Whether to write the CSV of the dataframe
+        make_csv (bool): Whether to write the CSV of the antibiogram
 
     Raises:
         InvalidMutationException: Raised if an invalid mutation is detected
 
     Returns:
         (pd.DataFrame, dict): (DataFrame containing the effects data, A metadata dictionary mapping drugs to their predictions)
     '''
+    if resistanceCatalogue is None:
+        logging.debug("Catalogue was None, skipping effects and predictions generation")
+        return
     #Assume wildtype behaviour unless otherwise specified
     phenotype = {drug: 'S' for drug in resistanceCatalogue.catalogue.drugs}
 
     effects = {}
     effectsCounter = 0
 
     #Default prediction values are RFUS but use piezo catalogue's values if existing
@@ -737,217 +765,199 @@
                 effects[effectsCounter] = [vcfStem, gene, mutation, resistanceCatalogue.catalogue.name, drug, prediction[drug]]
                 #Increment counter
                 effectsCounter += 1
     
     #Build the DataFrame
     effects = pd.DataFrame.from_dict(effects, 
                                         orient="index", 
-                                        columns=["UNIQUEID", "GENE", "MUTATION", 
-                                            "CATALOGUE_NAME", "DRUG", "PREDICTION"]
+                                        columns=["uniqueid", "gene", "mutation", 
+                                            "catalogue_name", "drug", "prediction"]
                                         )
-    
+    effects = effects[["uniqueid", "gene", "mutation", "drug", "prediction", "catalogue_name"]]
+    effects['catalogue_version'] = resistanceCatalogue.catalogue.version
+    effects['prediction_values'] = ''.join(resistanceCatalogue.catalogue.values)
+    effects['evidence'] = "{}"
     
     #Save as CSV
-    if len(effects) > 0:
+    if len(effects) > 0 and make_csv:
         effects.to_csv(os.path.join(outputDir, f'{vcfStem}.effects.csv'), index=False)
 
     effects.reset_index(inplace=True)
 
+    if make_prediction_csv:
+        #We need to construct a simple table here
+        predictions = [phenotype[drug] for drug in resistanceCatalogue.catalogue.drugs]
+        vals = {
+            'uniqueid': vcfStem,
+            'drug': resistanceCatalogue.catalogue.drugs,
+            'prediction': predictions,
+            'catalogue_name': resistanceCatalogue.catalogue.name,
+            'catalogue_version': resistanceCatalogue.catalogue.version,
+            'catalogue_values': ''.join(resistanceCatalogue.catalogue.values),
+            'evidence': "{}" #TODO: Add evidence
+        }
+        predictions = pd.DataFrame(vals)
+        predictions.to_csv(os.path.join(outputDir, f"{vcfStem}.predictions.csv"), index=False)
     #Return  the metadata dict to log later
     return effects, {"WGS_PREDICTION_"+drug: phenotype[drug] for drug in resistanceCatalogue.catalogue.drugs}
 
-def saveJSON(variants, mutations, effects, path: str, guid: str, values: list, gnomonicusVersion: str) -> None:
+def saveJSON(variants, mutations, effects, path: str, guid: str, catalogue: piezo.ResistanceCatalogue, gnomonicusVersion: str, time_taken: float, reference: gumpy.Genome, vcf_path: str, reference_path: str, catalogue_path: str) -> None:
     '''Create and save a single JSON output file for use within GPAS. JSON structure:
     {
         'meta': {
-            'version': gnomonicus version,
-            'guid': sample GUID,
-            'UTC-datetime-run': ISO formatted UTC datetime run,
-            'fields': Dictionary of data fields for parsing
+            'status': If this has succeeded or not (but this isn't created in cases it doesn't succeed),
+            'workflow_name': 'gnomonicus',
+            'workflow_task': 'resistance_prediction' or 'virulenece prediction',
+            'workflow_version': gnomonicus.__version__,
+            'time_taken': Time this step took,
+            'UTC_timestamp': Timestamp for the end of this run,
+            'catalogue_type': discrete_values or mic,
+            'catalogue_name': Name of catalogue,
+            'catalogue_version': Version of the catalogue,
+            'reference': Name of the reference genome used,
+            'catalogue_file': Path to the catalogue,
+            'reference_file': Path to the reference file,
+            'vcf_file': Path to the VCF file
         },
         'data': {
-            'VARIANTS': [
+            'variants': [
                 {
-                    'VARIANT': Genome level variant in GARC,
-                    'NUCLEOTIDE_INDEX': Genome index of variant
+                    'variant': Genome level variant in GARC,
+                    'nucleotide_index': Genome index of variant,
+                    'gene_name': Name of the gene this variant affects (if applicable),
+                    'gene_position': Gene position which this variant affects. Nucleotide number if non coding, codon indx if coding (if applicable),
+                    'codon_idx': Index of the base within the corresponding codon this affects (if applicable),
+                    'vcf_evidence': Parsed VCF row,
+                    'vcf_idx': Which part of the VCF row to look at for this call
                 }, ...
             ],
-            ?'MUTATIONS': [
+            ?'mutations': [
                 {
-                    'MUTATION': Gene level mutation in GARC,
-                    'GENE': Gene name,
-                    'GENE_POSITION': Position within the gene. Amino acid or nucleotide index depending on which is appropriate
+                    'mutation': Gene level mutation in GARC,
+                    'gene': Gene name,
+                    'gene_position': Position within the gene. Amino acid or nucleotide index depending on which is appropriate,
+                    'vcf_evidence': Parsed VCF row,
+                    'ref': Ref base(s),
+                    'alt': Alt base(s)
                 }
             ],
-            ?'EFFECTS': {
+            ?'effects': {
                 Drug name: [
                     {
-                        'GENE': Gene name of the mutation,
-                        'MUTATION': Gene level mutation in GARC,
-                        'PREDICTION': Prediction caused by this mutation
+                        'gene': Gene name of the mutation,
+                        'mutation': Gene level mutation in GARC,
+                        'prediction': Prediction caused by this mutation,
+                        'evidence': Evidence to support this prediction. Currently placeholder
                     }, ...,
                     {
-                        'PHENOTYPE': Resultant prediction for this drug based on prediciton heirarchy
+                        'phenotype': Resultant prediction for this drug based on prediciton heirarchy
                     }
                 ], ...
             }
+            ?'antibiogram': {
+                <drug> : <prediction> essentially json[data][effects][<drug>][phenotype]
+            }
         }
     }
     Where fields with a preceeding '?' are not always present depending on data
 
     Args:
         path (str): Path to the directory where the variant/mutation/effect CSV files are saved. Also the output dir for this.
         guid (str): Sample GUID
-        values (str): Prediction values for the resistance catalogue in priority order (values[0] is highest priority)
+        catalogue (piezo.ResistanceCatalogue): Catalogue used
         gnomonicusVersion (str): Semantic versioning string for the gnomonicus module. Can be accessed by `gnomonicus.__version__`
+        time_taken (float): Number of seconds taken to run this.
+        reference (gumpy.Genome): Reference genome object
+        vcf_path (str): Path to the VCF file used for this run
+        reference_path (str): Path to the reference genome used for this run
+        catalogue_path (str): Path to the catalogue used for this run
     '''
-
+    values = catalogue.catalogue.values if catalogue is not None else list("RFUS")
     #Define some metadata for the json
     meta = {
-        'version': gnomonicusVersion, #gnomonicus version used
+        'status': 'success',
+        'workflow_name': 'gnomonicus',
+        'workflow_version': gnomonicusVersion, #gnomonicus version used
+        'workflow_task': 'resistance_prediction', #TODO: Update this when we know how to detect a virulence catalogue
         'guid': guid, #Sample GUID
-        'UTC-datetime-run': datetime.datetime.utcnow().isoformat(), #ISO datetime run
-        'fields': dict() #Fields included. These vary according to existance of mutations/effects
+        'UTC-datetime-completed': datetime.datetime.utcnow().isoformat(), #ISO datetime run
+        'time_taken_s': time_taken,
+        'reference': reference.name,
+        'catalogue_file': catalogue_path,
+        'reference_file': reference_path,
+        'vcf_file': vcf_path
         }
+    if catalogue is not None:
+        meta['catalogue_type'] = ''.join(catalogue.catalogue.values)
+        meta['catalogue_name'] = catalogue.catalogue.name
+        meta['catalogue_version'] = catalogue.catalogue.version
+    else:
+        meta['catalogue_type'] = None
+        meta['catalogue_name'] = None
+        meta['catalogue_version'] = None
     data = {}
     #Variants field
     _variants = []
-    meta['fields']['VARIANTS'] = ['VARIANT', 'NUCLEOTIDE_INDEX']
     for _, variant in variants.iterrows():
         row = {
-            'VARIANT': variant['VARIANT'],
-            'NUCLEOTIDE_INDEX': variant['NUCLEOTIDE_INDEX'],
+            'variant': variant['variant'],
+            'nucleotide_index': variant['nucleotide_index'],
+            'gene_name': variant['gene_name'],
+            'gene_position': variant['gene_position'],
+            'codon_idx': variant['codon_idx'],
+            'vcf_evidence': json.loads(variant['vcf_evidence']),
+            'vcf_idx': variant['vcf_idx']
         }
         _variants.append(row)
-    data['VARIANTS'] = _variants
+    data['variants'] = _variants
 
     #Depending on mutations/effects, populate
     _mutations = []
     if mutations is not None:
-        meta['fields']['MUTATIONS'] = ['MUTATION', 'GENE', 'GENE_POSITION']
         for _, mutation in mutations.iterrows():
             row = {
-                'MUTATION': mutation['MUTATION'],
-                'GENE': mutation['GENE'],
-                'GENE_POSITION': mutation['GENE_POSITION']
+                'mutation': mutation['mutation'],
+                'gene': mutation['gene'],
+                'gene_position': mutation['gene_position'],
             }
+            if mutation['mutation'][0].isupper() or mutation['mutation'][0] == "!":
+                #Only add codon ref/alt for AA changes
+                row['ref'] = mutation['ref']
+                row['alt'] = mutation['alt']
             _mutations.append(row)
-        data['MUTATIONS'] = _mutations
+        data['mutations'] = _mutations
 
     _effects = defaultdict(list)
+    antibiogram = {}
+    drugs = set()
     if effects is not None and len(effects) > 0:
-        meta['fields']['EFFECTS'] = dict()
         for _, effect in effects.iterrows():
             prediction = {
-                'GENE': effect['GENE'],
-                'MUTATION': effect['MUTATION'],
-                'PREDICTION': effect['PREDICTION']
+                'gene': effect['gene'],
+                'mutation': effect['mutation'],
+                'prediction': effect['prediction'],
+                'evidence': {}
             }
-            _effects[effect['DRUG']].append(prediction)
+            _effects[effect['drug']].append(prediction)
         
         #Get the overall predictions for each drug
         for drug, predictions in _effects.items():
             phenotype = 'S'
             for prediction in predictions:
                 #Use the prediction heierarchy to use most signifiant prediction
-                if values.index(prediction['PREDICTION']) < values.index(phenotype):
+                if values.index(prediction['prediction']) < values.index(phenotype):
                     #The prediction is closer to the start of the values list, so should take priority
-                    phenotype = prediction['PREDICTION']
-            _effects[drug].append({'PHENOTYPE': phenotype})
-            meta['fields']['EFFECTS'][drug] = [['GENE', 'MUTATION', 'PREDICTION'], 'PHENOTYPE']
-        data['EFFECTS'] = _effects
+                    phenotype = prediction['prediction']
+            _effects[drug].append({'phenotype': phenotype})
+            antibiogram[drug] = phenotype
+            drugs.add(drug)
+        data['effects'] = _effects
+    if catalogue is not None:
+        for d in catalogue.catalogue.drugs:
+            if d not in drugs:
+                antibiogram[d] = "S"
+        data['antibiogram'] = antibiogram
 
     #Convert fields to a list so it can be json serialised
     with open(os.path.join(path, f'{guid}.gnomonicus-out.json'), 'w') as f:
-        f.write(json.dumps({'meta': meta, 'data': data}, indent=2, sort_keys=True))
-
-def toAltJSON(path: str, reference: gumpy.Genome, vcfStem: str, catalogue: str) -> None:
-    '''Convert the output JSON into a similar format to the COVID workflows:
-    {
-        <guid>: {
-            'WorkflowInformation': {
-                'gnomonicusVersion': Version,
-                'referenceIdentifier': ID of the reference,
-                'sampleIdentifier': ID of the sample (VCF stem),
-                'catalogueName': Name of the prediction catalogue
-            },
-            'gnomonicus': {
-                'aaDeletions': [GARC of aa deletions],
-                'aaInsertions': [GARC of aa insertions],
-                'aaSubsitutions': [GARC of aa SNPs],
-                'deletions': [GARC of deletions], #Inclusive of AA deletions
-                'insertions': [GARC of insertions], #Inclusive of AA insertions
-                'substitutions': [GARC of SNPs], #Inclusive of AA SNPs
-                'frameshifts': Number of frameshifting mutations (excluding non cds regions)
-                'effects': {
-                    <drug name>: [
-                        {
-                            'GENE': Gene name,
-                            'MUTATION': Mutation in GARC,
-                            'PREDICTION': Prediction caused by this mutation
-                        }, ...,
-                        {
-                            'PHENOTYPE': Resultant prediction following catalogue heirarchy
-                        }
-                    ], ...
-                }
-            },
-            'gnomonicusOutputJSON': Full original output JSON
-        }
-    }
-
-    Args:
-        path (str): Path to the directory containing the original JSON
-        reference (gumpy.Genome): Reference gumpy Genome object
-        vcfStem (str): Stem of the VCF file. Should be the sample GUID
-        catalogue (str): Name of the catalogue
-    '''
-    original = json.load(open(os.path.join(path, f'{vcfStem}.gnomonicus-out.json'), 'r'))
-
-    variants = [x['VARIANT'] for x in original['data']['VARIANTS']]
-    #Only insertions of form <pos>_ins_<bases>
-    insertions = [x for x in variants if "ins" in x and x[-1].isalpha()]
-    #Only deletions of form <pos>_del_<bases>
-    deletions = [x for x in variants if "del" in x and "indel" not in x and x[-1].isalpha()]
-    #Should just be SNPs left
-    snps = [x for x in variants if "ins" not in x and "del" not in x]
-
-    mutations = [x['GENE']+'@'+x['MUTATION'] for x in original['data'].get('MUTATIONS', {})]
-    #Only insertions of form <gene>@<pos>_ins_<bases>
-    aaInsertions = [x for x in mutations if "ins" in x and x[-1].isalpha()] 
-    #Only deletions of form <gene>@<pos>_del_<bases>
-    aaDeletions = [x for x in mutations if "del" in x and "indel" not in x and x[-1].isalpha()]
-    #Should just be SNPs left
-    aaSnps = [x for x in mutations if "ins" not in x and "del" not in x]
-    #Count frameshifting mutations
-    frameshifts = len([
-        x for x in mutations 
-            if ('ins' in x or 'del' in x) and 'indel' not in x 
-                and x[-1].isnumeric() and int(x.split("_")[-1]) % 3 != 0
-        ])
-
-    effects = original['data'].get('EFFECTS', {})
-
-    out = {
-        vcfStem: {
-            'WorkflowInformation': {
-                'gnomonicusVersion': original['meta']['version'],
-                'referenceIdentifier': reference.name,
-                'sampleIdentifier': vcfStem,
-                'catalogueName': catalogue.catalogue.name
-            },
-            'gnomonicus': {
-                'aaDeletions': aaDeletions,
-                'aaInsertions': aaInsertions,
-                'aaSubsitutions': aaSnps,
-                'frameshifts': frameshifts,
-                'deletions': deletions,
-                'insertions': insertions,
-                'substitutions': snps,
-                'effects': effects
-            },
-            'gnomonicusOutputJSON': original
-        }
-    }
+        f.write(json.dumps({'meta': meta, 'data': data}, indent=2))
 
-    with open(os.path.join(path, f'{vcfStem}.alt-gnomonicus-out.json'), 'w') as f:
-        f.write(json.dumps(out, indent=2))
```

### Comparing `gnomonicus-1.1.3/gnomonicus.egg-info/PKG-INFO` & `gnomonicus-2.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-Metadata-Version: 2.1
-Name: gnomonicus
-Version: 1.1.3
-Summary: Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
-Home-page: https://github.com/oxfordmmm/gnomonicus
-Author: Philip W Fowler, Jeremy Westhead
-Author-email: philip.fowler@ndm.ox.ac.uk
-License: University of Oxford License, see LICENSE
-Keywords: gnomonicus,piezo,lodestone,clockwork,TB
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Tests](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml) [![Build and release Docker](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml) [![Build and release PyPI](https://github.com/oxfordmmm/gnomonicus/actions/workflows/pypi.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/pypi.yaml) [![PyPI version](https://badge.fury.io/py/gnomonicus.svg)](https://badge.fury.io/py/gnomonicus)
+[![Tests](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/tests.yaml) 
+[![Build and release Docker](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml/badge.svg)](https://github.com/oxfordmmm/gnomonicus/actions/workflows/build.yaml) 
+[![PyPI version](https://badge.fury.io/py/gnomonicus.svg)](https://badge.fury.io/py/gnomonicus)
+[![Docs](https://github.com/oxfordmmm/gnomonicus/actions/workflows/docs.yaml/badge.svg)](https://oxfordmmm.github.io/gnomonicus/)
 
 # gnomonicus
 Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variations
 
 Provides a library of functions for use within scripts, as well as a CLI tool for linking the functions together to produce output
 
+## Documentation
+API reference for developers, and CLI instructions can be found here: https://oxfordmmm.github.io/gnomonicus/ 
 ## Usage
 ```
-usage: gnomonicus [-h] --vcf_file VCF_FILE --genome_object GENOME_OBJECT [--catalogue_file CATALOGUE_FILE] [--ignore_vcf_filter] [--progress] [--output_dir OUTPUT_DIR] [--json] [--alt_json] [--fasta FASTA]
-                  [--minor_populations MINOR_POPULATIONS]
+usage: gnomonicus [-h] --vcf_file VCF_FILE --genome_object GENOME_OBJECT [--catalogue_file CATALOGUE_FILE] [--ignore_vcf_filter] [--progress] [--output_dir OUTPUT_DIR] [--json] [--fasta FASTA] [--minor_populations MINOR_POPULATIONS]
 
 options:
   -h, --help            show this help message and exit
   --vcf_file VCF_FILE   the path to a single VCF file
   --genome_object GENOME_OBJECT
                         the path to a compressed gumpy Genome object or a genbank file
   --catalogue_file CATALOGUE_FILE
                         the path to the resistance catalogue
   --ignore_vcf_filter   whether to ignore the FILTER field in the vcf (e.g. necessary for some versions of Clockwork VCFs)
   --progress            whether to show progress using tqdm
   --output_dir OUTPUT_DIR
                         Directory to save output files to. Defaults to wherever the script is run from.
   --json                Flag to create a single JSON output as well as the CSVs
-  --alt_json            Whether to produce the alternate JSON format. Requires the --json flag too
   --fasta FASTA         Use to output a FASTA file of the resultant genome. Specify either 'fixed' or 'variable' for fixed length and variable length FASTA respectively.
   --minor_populations MINOR_POPULATIONS
                         Path to a line separated file containing genome indices of minor populations.
 ```
 
 ## Helper usage
 As the main script can utilise pickled `gumpy.Genome` objects, there is a supplied helper script. This converts a Genbank file into a pickled gumpy.Genome for significant time saving.
@@ -107,8 +96,8 @@
 
 3. In general, I would also like the option to output fixed- and variable-length FASTA files (the latter takes into account insertions and deletions described in any input VCF file).
 
 ## Unit testing
 
 For speed, rather than use NC_000962.3 (i.e. H37Rv *M. tuberculosis*), we shall use SARS-CoV-2 and have created a fictious drug resistance catalogue, along with some `vcf` files and the expected outputs in `tests/`.
 
-These can be run with `pytest -vv`
+These can be run with `pytest -vv`
```

### Comparing `gnomonicus-1.1.3/setup.cfg` & `gnomonicus-2.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gnomonicus
-version = 1.1.3
+version = 2.0.0
 author = Philip W Fowler, Jeremy Westhead
 author_email = philip.fowler@ndm.ox.ac.uk
 description = Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/oxfordmmm/gnomonicus
 keywords = gnomonicus, piezo, lodestone, clockwork, TB
@@ -12,16 +12,16 @@
 classifiers = Programming Language :: Python :: 3
 
 [options]
 package_dir = 
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	gumpy>=1.1.0
-	piezo>=0.4
+	gumpy>=1.2.1
+	piezo>=0.5
 	numpy
 	pandas
 	recursive_diff
 zip_safe = False
 include_package_data = True
 scripts = bin/gnomonicus, bin/gbkToPkl
```

