# Comparing `tmp/pySpade-0.0.1.tar.gz` & `tmp/pySpade-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pySpade-0.0.1.tar", last modified: Fri Dec  9 16:49:40 2022, max compression
+gzip compressed data, was "dist/pySpade-0.0.2.tar", last modified: Fri Jun 30 19:44:05 2023, max compression
```

## Comparing `pySpade-0.0.1.tar` & `pySpade-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2022-12-09 16:49:40.000000 pySpade-0.0.1/
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     1066 2022-09-29 20:16:43.000000 pySpade-0.0.1/LICENSE
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       36 2022-12-09 16:49:13.000000 pySpade-0.0.1/MANIFEST.in
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     4575 2022-12-09 16:49:40.000000 pySpade-0.0.1/PKG-INFO
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     4074 2022-12-09 16:16:44.000000 pySpade-0.0.1/README.md
-drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2022-12-09 16:49:40.000000 pySpade-0.0.1/pySpade/
--rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     3794 2022-12-09 16:20:08.000000 pySpade-0.0.1/pySpade/DEobs.py
--rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     7196 2022-12-09 16:20:31.000000 pySpade-0.0.1/pySpade/DErand.py
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       36 2022-12-09 16:23:38.000000 pySpade-0.0.1/pySpade/__init__.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     3586 2022-12-09 16:13:44.000000 pySpade-0.0.1/pySpade/__main__.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     1863 2022-12-09 16:20:46.000000 pySpade-0.0.1/pySpade/explevel.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     4353 2022-12-09 16:20:59.000000 pySpade-0.0.1/pySpade/fc.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     6074 2022-12-09 16:21:08.000000 pySpade-0.0.1/pySpade/global.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     4878 2022-12-09 16:21:20.000000 pySpade-0.0.1/pySpade/local.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    14732 2022-12-09 16:21:49.000000 pySpade-0.0.1/pySpade/parsers.py
--rwxr-----   0 s426305  (426305) Hon_lab   (7001)  2220577 2022-09-29 20:13:53.000000 pySpade-0.0.1/pySpade/plot_annotation.txt
--rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     6200 2022-12-09 16:22:04.000000 pySpade-0.0.1/pySpade/process.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    10866 2022-12-09 16:22:35.000000 pySpade-0.0.1/pySpade/utils.py
-drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2022-12-09 16:49:40.000000 pySpade-0.0.1/pySpade.egg-info/
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     4575 2022-12-09 16:49:40.000000 pySpade-0.0.1/pySpade.egg-info/PKG-INFO
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)      423 2022-12-09 16:49:40.000000 pySpade-0.0.1/pySpade.egg-info/SOURCES.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        1 2022-12-09 16:49:40.000000 pySpade-0.0.1/pySpade.egg-info/dependency_links.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       51 2022-12-09 16:49:40.000000 pySpade-0.0.1/pySpade.egg-info/entry_points.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        8 2022-12-09 16:49:40.000000 pySpade-0.0.1/pySpade.egg-info/top_level.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       38 2022-12-09 16:49:40.000000 pySpade-0.0.1/setup.cfg
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)      981 2022-12-09 16:44:09.000000 pySpade-0.0.1/setup.py
+drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2023-06-30 19:44:05.000000 pySpade-0.0.2/
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     1066 2022-09-29 20:16:43.000000 pySpade-0.0.2/LICENSE
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       36 2022-12-09 16:49:13.000000 pySpade-0.0.2/MANIFEST.in
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     4617 2023-06-30 19:44:05.000000 pySpade-0.0.2/PKG-INFO
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     4110 2022-12-09 21:55:57.000000 pySpade-0.0.2/README.md
+drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2023-06-30 19:44:05.000000 pySpade-0.0.2/pySpade/
+-rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     4212 2023-05-26 20:39:47.000000 pySpade-0.0.2/pySpade/DEobs.py
+-rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     6971 2023-05-26 20:43:30.000000 pySpade-0.0.2/pySpade/DErand.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)       36 2022-12-15 21:19:05.000000 pySpade-0.0.2/pySpade/__init__.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     3672 2023-06-16 18:27:48.000000 pySpade-0.0.2/pySpade/__main__.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     2835 2022-12-15 21:18:46.000000 pySpade-0.0.2/pySpade/explevel.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     7047 2023-05-26 20:40:17.000000 pySpade-0.0.2/pySpade/fc.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     7945 2023-06-16 19:48:17.000000 pySpade-0.0.2/pySpade/global.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     6138 2023-06-30 19:27:45.000000 pySpade-0.0.2/pySpade/local.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    15491 2023-06-16 18:28:07.000000 pySpade-0.0.2/pySpade/parsers.py
+-rwxr-----   0 s426305  (426305) Hon_lab   (7001)  2220577 2022-09-29 20:13:53.000000 pySpade-0.0.2/pySpade/plot_annotation.txt
+-rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     6259 2023-05-25 15:07:24.000000 pySpade-0.0.2/pySpade/process.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    11729 2023-06-30 19:17:20.000000 pySpade-0.0.2/pySpade/utils.py
+drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2023-06-30 19:44:05.000000 pySpade-0.0.2/pySpade.egg-info/
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     4617 2023-06-30 19:44:04.000000 pySpade-0.0.2/pySpade.egg-info/PKG-INFO
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)      423 2023-06-30 19:44:04.000000 pySpade-0.0.2/pySpade.egg-info/SOURCES.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        1 2023-06-30 19:44:04.000000 pySpade-0.0.2/pySpade.egg-info/dependency_links.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       51 2023-06-30 19:44:04.000000 pySpade-0.0.2/pySpade.egg-info/entry_points.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        8 2023-06-30 19:44:04.000000 pySpade-0.0.2/pySpade.egg-info/top_level.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       38 2023-06-30 19:44:05.000000 pySpade-0.0.2/setup.cfg
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)      987 2023-06-30 19:38:59.000000 pySpade-0.0.2/setup.py
```

### Comparing `pySpade-0.0.1/LICENSE` & `pySpade-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pySpade-0.0.1/PKG-INFO` & `pySpade-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pySpade
-Version: 0.0.1
-Summary: Single cell Perturbation Analysis of Differential Expression
-Home-page: https://github.com/yihan1119/pySpade
+Version: 0.0.2
+Summary: Single cell Perturbations - Analysis of Differential gene Expression
+Home-page: https://github.com/Hon-lab/pySpade
 Author: Yihan Wang
 Author-email: Yihan.Wang@UTSouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pySpade: Single cell Perturbation Analysis of Differential Expression
+# pySpade: Single cell Perturbations - Analysis of Differential gene Expression
 
 ## Overview
 _________
 `pySpade` is a user friendly tool to perform the whole transcriptome analysis of single cell perturbation dataset. With the direct output of Cellranger, `pySpade` utilizes hypergeomtric test to analyze the whole transcriptome differential expression and generates hits table csv file. User can use the table to do downstream processing like generating Manhattan plots (tutorial includes). Currently we support human genome.     
 
 ## Requirement
 _________
@@ -45,21 +45,21 @@
 Version: 0.0.1
 
 optional arguments:
   -h, --help  show this help message and exit
 
 functions:
   
-    process   process mapping output and reformat to downstream analysis.
+    process   process mapping output and reformat for downstream analysis.
     explevel  check the average expression level of query genes in single cell matrix
     fc        check the fold change of sgrna
-    DEobs     perform differential expression analysis of observe cells
+    DEobs     perform differential expression analysis of observed cells
     DErand    perform differential expression analysis of random selection background
-    local     perform local hit analysis with obs and random background
-    global    perform global hit analysis with obs and random background
+    local     perform local hit analysis with observation data and random background
+    global    perform global hit analysis with observation data and random background
     
 ```
 
 * `process` : Process transcriptome output and sgrna output to remove experimental doublets sgrna outlier cells. Transcriptome matrix is from Cellranger output (outs folder). sgrna matrix column: cell barcodes consistent with transcriptome matrix, rows: sgrna sequence. The final output format is h5 file. The final output can be compressed to save disk space, but it may take more time to write the final output file.
 
 * `explevel` : Check the average expression level of query genes in single cell matrix. Input: processed transcriptome matrix from the `process` output, query genes list has to be txt file, genes are seperated with new line.
```

### Comparing `pySpade-0.0.1/README.md` & `pySpade-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pySpade: Single cell Perturbation Analysis of Differential Expression
+# pySpade: Single cell Perturbations - Analysis of Differential gene Expression
 
 ## Overview
 _________
 `pySpade` is a user friendly tool to perform the whole transcriptome analysis of single cell perturbation dataset. With the direct output of Cellranger, `pySpade` utilizes hypergeomtric test to analyze the whole transcriptome differential expression and generates hits table csv file. User can use the table to do downstream processing like generating Manhattan plots (tutorial includes). Currently we support human genome.     
 
 ## Requirement
 _________
@@ -29,21 +29,21 @@
 Version: 0.0.1
 
 optional arguments:
   -h, --help  show this help message and exit
 
 functions:
   
-    process   process mapping output and reformat to downstream analysis.
+    process   process mapping output and reformat for downstream analysis.
     explevel  check the average expression level of query genes in single cell matrix
     fc        check the fold change of sgrna
-    DEobs     perform differential expression analysis of observe cells
+    DEobs     perform differential expression analysis of observed cells
     DErand    perform differential expression analysis of random selection background
-    local     perform local hit analysis with obs and random background
-    global    perform global hit analysis with obs and random background
+    local     perform local hit analysis with observation data and random background
+    global    perform global hit analysis with observation data and random background
     
 ```
 
 * `process` : Process transcriptome output and sgrna output to remove experimental doublets sgrna outlier cells. Transcriptome matrix is from Cellranger output (outs folder). sgrna matrix column: cell barcodes consistent with transcriptome matrix, rows: sgrna sequence. The final output format is h5 file. The final output can be compressed to save disk space, but it may take more time to write the final output file.
 
 * `explevel` : Check the average expression level of query genes in single cell matrix. Input: processed transcriptome matrix from the `process` output, query genes list has to be txt file, genes are seperated with new line.
```

### Comparing `pySpade-0.0.1/pySpade/DErand.py` & `pySpade-0.0.2/pySpade/DErand.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,33 +49,25 @@
     if (sub_df_file.endswith('pkl')):
         sub_df = pd.read_pickle(sub_df_file)
     elif (sub_df_file.endswith('h5')):
         sub_df = pd.read_hdf(sub_df_file, 'df')
     
     #read the plotting annotation
     annot_df = read_annot_df()
-    
-    #filter the genes
-    nonzero_idx = np.where(np.sum(sub_df > 0, axis = 1) > 1)[0]
-    idx = list(set(nonzero_idx) & set(annot_df.idx))
-    del nonzero_idx
-    del annot_df
-        
+    idx = np.arange(0, len(sub_df.index))
+  
     #normalize the matrix.
     if (norm == 'cpm'):
         cpm_matrix = cpm_normalization(sub_df)
         
     elif (norm == 'metacell'):
         cpm_matrix = metacelll_normalization(sub_df)
      
     logger.info('Finished transcriptome normalization.')
     
-    #create input ndarray
-    input_array = cpm_matrix[idx]
-    del cpm_matrix
 
     if (sgrna_df.endswith('pkl')):
         sgrna_df_adj_bool = pd.read_pickle(sgrna_df) > 0 
     elif (sgrna_df.endswith('h5')):
         sgrna_df_adj_bool = pd.read_hdf(sgrna_df, 'df') > 0
 
     [g,c] = sgrna_df_adj_bool.shape
@@ -111,15 +103,15 @@
         pval_list_up = np.zeros(len(sub_df.index))
         fc_list = np.ones(len(sub_df.index))
         cpm_list = np.zeros(len(sub_df.index))
             
         #perform the differential gene analysis by using Virtual FACS
         num_sgrna_cell, pval_list_up, pval_list_down, fc_list, cpm_list = perform_DE(
                                                                             sgrna_idx,
-                                                                            input_array,
+                                                                            cpm_matrix,
                                                                             idx,
                                                                             num_processing,
                                                                             pval_list_down,
                                                                             pval_list_up,
                                                                             fc_list,
                                                                             cpm_list
                                                                         )
```

### Comparing `pySpade-0.0.1/pySpade/__main__.py` & `pySpade-0.0.2/pySpade/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,31 +33,30 @@
 
 
     elif (args.command == 'explevel'):
         logger.info('Running explevel command ...')
         m = importlib.import_module(name=f'pySpade.{args.command}')
 
         _ = m.Calculate_gene_expression(
-            TRANSCRIPTOME_DF=args.transcriptome_df,
+            TRANSCRIPTOME_DIR=args.transcriptome_dir,
             GENE_FILE=args.gene,
             OUTPUT_FILE=args.output_file
         )
         logger.info('Done.')
 
 
     elif (args.command == 'fc'):
         logger.info('Running fc command ...')
         m = importlib.import_module(name=f'pySpade.{args.command}')
 
         _ = m.Calculate_fc(
-            TRANSCRIPTOME_DF=args.transcriptome_df,
-            SGRNA = args.input_sgrna,
+            TRANSCRIPTOME_DIR=args.transcriptome_dir,
             SGRNA_DICT = args.dict,
             TARGET_FILE = args.region,
-            OUTPUT_FILE = args.output_file
+            OUTPUT_FOLDER = args.output_folder
         )        
         logger.info('Done.')
 
 
     elif (args.command == 'DEobs'):
         logger.info('Running DEobs command ...')
         m = importlib.import_module(name=f'pySpade.{args.command}')
@@ -89,26 +88,29 @@
         logger.info('Done.')
 
     elif (args.command == 'local'):
         logger.info('Running local command ...')
         m = importlib.import_module(name=f'pySpade.{args.command}')
 
         _ = m.local_analysis(
-            data_dir = args.data_dir,
+            FILE_DIR = args.file_dir,
+            OBS_DIR = args.data_dir,
             DISTRI_DIR = args.distr,
+            SGRNA_DICT = args.sgrna_dict,
             OUTPUT_DF = args.output_file
             )        
         logger.info('Done.')
 
     elif (args.command == 'global'):
         logger.info('Running global command ...')
         m = importlib.import_module(name=f'pySpade.{args.command}')
 
         _ = m.global_analysis(
-            data_dir = args.data_dir,
+            FILE_DIR = args.file_dir,
+            OBS_DIR = args.data_dir,
             SGRNA_DICT = args.sgrna_dict,
             DISTRI_DIR = args.distr,
             OUTPUT_DF = args.output_file
             )        
         logger.info('Done.')
 
 if __name__ == "__main__":
```

### Comparing `pySpade-0.0.1/pySpade/explevel.py` & `pySpade-0.0.2/pySpade/explevel.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,62 +5,78 @@
 import sys
 import collections
 import argparse
 import tables
 import itertools
 import matplotlib
 import numba
-
+import glob
 import numpy as np
 import pandas as pd
 import scipy.stats as stats
 import scipy.sparse as sp_sparse
 
 from collections import defaultdict
 from scipy import sparse, io
 from scipy.sparse import csr_matrix
 
 from importlib import resources
 from pySpade.utils import get_logger
 
 logger = get_logger(logger_name=__name__)
 
-def Calculate_gene_expression(TRANSCRIPTOME_DF, 
+def Calculate_gene_expression(TRANSCRIPTOME_DIR, 
                               GENE_FILE, 
                               OUTPUT_FILE):
 
-    if (TRANSCRIPTOME_DF.endswith('pkl')):
-        sub_df = pd.read_pickle(TRANSCRIPTOME_DF)
-    elif (TRANSCRIPTOME_DF.endswith('h5')):
-        sub_df = pd.read_hdf(TRANSCRIPTOME_DF, 'df')
+    TRANSCRIPTOME_FILE = glob.glob(TRANSCRIPTOME_DIR + 'Singlet_sub_df.*')
+    if TRANSCRIPTOME_FILE[0].endswith('h5') == True:
+        sub_df = pd.read_hdf(TRANSCRIPTOME_FILE[0], 'df')
+    if TRANSCRIPTOME_FILE[0].endswith('pkl') == True:
+        sub_df = pd.read_pickle(TRANSCRIPTOME_FILE[0])
 
     #load quired genes
     GENE_LIST = []
-    with open(GENE_FILE) as ft:
-        for line in ft:
-            gene = line.strip()
-            GENE_LIST.append(gene)
-    
+    if GENE_FILE.endswith('.txt'):
+        with open(GENE_FILE) as ft:
+            for line in ft:
+                gene = line.strip()
+                GENE_LIST.append(gene)
+    else:
+        for i in GENE_FILE.split(','):
+            GENE_LIST.append(i)
 
     total_seq_reads = sub_df.sum(axis=0)
     logger.info('Finished loading data.')
 
     #calculate average cpm and write to output file
-    output_file=open(OUTPUT_FILE, 'w')
-    output_file.write('Gene' + '\t' + 'Average expression (cpm)' + '\t' + 'Median cpm' + '\t' + 'Portion of cell express' + '\n')
-    for gene in GENE_LIST:
-        if (gene in sub_df.index) == False:
-            logger.critical(str(gene) + ' is missing from the transcriptome dataframe.')
-            continue
-        dist = sub_df.loc[gene ,:] / total_seq_reads * 1000000
-        ave_cpm = np.mean(dist)
-        median_cpm = np.median(dist)
-        perc_cell = np.sum(dist > 0) /len(dist)
-        output_file.write(str(gene) + '\t' + str(ave_cpm) + '\t' + str(median_cpm) + '\t' + str(perc_cell) + '\n')
-
-        logger.info('Finish processing ' + str(gene))
-
-    output_file.close()
+    if OUTPUT_FILE != None:
+        output_file=open(OUTPUT_FILE, 'w')
+        output_file.write('Gene' + '\t' + 'Average expression (cpm)' + '\t' + 'Median cpm' + '\t' + 'Portion of cell express' + '\n')
+        for gene in GENE_LIST:
+            if (gene in sub_df.index) == False:
+                logger.critical(str(gene) + ' is missing from the transcriptome dataframe.')
+                continue
+            dist = sub_df.loc[gene ,:] / total_seq_reads * 1000000
+            ave_cpm = np.mean(dist)
+            median_cpm = np.median(dist)
+            perc_cell = np.sum(dist > 0) /len(dist)
+            output_file.write(str(gene) + '\t' + str(ave_cpm) + '\t' + str(median_cpm) + '\t' + str(perc_cell) + '\n')
+            logger.info('Finish processing ' + str(gene))
+        output_file.close()
+
+    else:
+        logger.info('Gene' + '\t' + 'Average expression (cpm)' + '\t' + 'Median cpm' + '\t' + 'Portion of cell express' + '\n')
+        for gene in GENE_LIST:
+            if (gene in sub_df.index) == False:
+                logger.critical(str(gene) + ' is missing from the transcriptome dataframe.')
+                continue
+            dist = sub_df.loc[gene ,:] / total_seq_reads * 1000000
+            ave_cpm = np.mean(dist)
+            median_cpm = np.median(dist)
+            perc_cell = np.sum(dist > 0) /len(dist)
+            logger.info(str(gene) + '\t' + str(ave_cpm) + '\t' + str(median_cpm) + '\t' + str(perc_cell) + '\n')
 
+    
 
 if __name__ == '__main__':
     pass
```

### Comparing `pySpade-0.0.1/pySpade/global.py` & `pySpade-0.0.2/pySpade/local.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,144 @@
-#global.py
+#local.py
+
 import os
 import re
 import sys
 import collections
 import argparse
+from threading import local
 import tables
 import itertools 
 import scipy
-import matplotlib
 import csv
 import glob
 
 import numpy as np
 import pandas as pd
 import scipy.stats as stats
 import scipy.sparse as sp_sparse
 import scipy.io as sio
 
-from sklearn.cluster import KMeans
-from sklearn.decomposition import PCA
-from multiprocessing import Pool
 from collections import defaultdict
 from scipy import sparse
 from scipy.sparse import csr_matrix
-from scipy.cluster.hierarchy import dendrogram, linkage
-import scipy.io as io
 
-from pySpade.utils import get_logger, read_annot_df, read_sgrna_dict, load_data
+from pySpade.utils import get_logger, read_annot_df, get_neighbor_genes, get_distance, read_sgrna_dict
 
 logger = get_logger(logger_name=__name__)
 
-def global_analysis(data_dir,
-                    SGRNA_DICT,
+def local_analysis(FILE_DIR,
+                    OBS_DIR,
                     DISTRI_DIR,
+                    SGRNA_DICT,
                     OUTPUT_DF):
     
     logger.info('Loading files.')
 
+    #read the gene sequence file 
+    gene_seq = np.load(FILE_DIR + 'Trans_genome_seq.npy', allow_pickle=True)
+    if len(gene_seq) != len(set(gene_seq)):
+        logger.critical('Duplication of mapping genes.')
     #read the plotting annotation
-    annot_df = read_annot_df()
-
-    ##Load sgRNA dict: All regions 
+    annot_df_dup = read_annot_df()
+    #There are many non-coding genes duplication in the annot_df, only keep one.
+    annot_df = annot_df_dup.drop_duplicates(subset='gene_names', keep='first')
+    
+    #Load sgRNA dict: All regions 
     sgrna_dict  = read_sgrna_dict(SGRNA_DICT)
 
-    #Save the randomized bin with list 
-    
+    #read all the perturbation files
+    pval_files = glob.glob(OBS_DIR + '*-down_log-pval')
+
+    df_column_list = [
+        'gene_names', 'chromosome', 'pos', 'strand', 
+        'color_idx', 'chr_idx', 'region', 'distance', 'num_cell', 'bin', 
+        'pval', 'fc', 'padj-Gaussian', 'fc_by_rand_dist_cpm', 'cpm_perturb', 'cpm_bg']
+    local_gene_df = pd.DataFrame(columns=df_column_list)
+
+    #Read the background distribution file
     Num = [int(i.split('/')[-1].split('.')[0].split('-')[-1]) for i in glob.glob(DISTRI_DIR+ '/Down_dist_mean-*')]
     if len([int(i.split('/')[-1].split('.')[0].split('-')[-1]) for i in glob.glob(DISTRI_DIR+ '/Down_dist_mean-*')]) != \
         len([int(i.split('/')[-1].split('.')[0].split('-')[-1]) for i in glob.glob(DISTRI_DIR+ '/Up_dist_mean-*')]):
         logger.critical('Background distribution files error!')
         sys.exit(0)
 
-    logger.info(f'{len(Num)} sets of background distribution for global analysis.')
-
-    #Calcualte pval
-    df_column_list = [
-        'idx', 'gene_names', 'chromosome', 'pos', 'strand', 
-        'color_idx', 'chr_idx', 
-        'region', 'num_cell', 'bin',
-        'pval', 'fc', 'padj-Gaussian', 'fc_by_rand_dist_cpm']
-    global_hits_df = pd.DataFrame(columns=df_column_list)
-
-    #Generate bin-region dictionary 
-    bin_dict = defaultdict(list)
+    #start calculating local hits for each perturbation region
+    logger.info('Start analysis of ' + str(len(pval_files)) + ' regions.')
     for region in list(sgrna_dict.keys()):
-        fc_files = glob.glob(data_dir + region + '*-foldchange')
-        fc_file = fc_files[0]
-        cell_num = int(fc_file.split('/')[-1].split('-')[2])
-        chosen_bin = Num[np.argmin([np.absolute(n-cell_num) for n in Num])]
-        bin_dict[chosen_bin].append(region)
-    logger.info('Finish generating bin-region dictionary')
-    
-    pval_cutoff = -1
-    fc_cutoff = 0.1
-
-    for b in Num:
-        logger.info(f'Processing bin: {b}')
-        logger.info(f'Num of regions in this bin: {len(bin_dict[b])}')
-
-        #Load the background files
-        down_mean = np.load(DISTRI_DIR + 'Down_dist_mean-%s.npy'%(str(b)))
-        down_std = np.load(DISTRI_DIR + 'Down_dist_std-%s.npy'%(str(b))) 
-        up_mean = np.load(DISTRI_DIR + 'Up_dist_mean-%s.npy'%(str(b)))
-        up_std = np.load(DISTRI_DIR + 'Up_dist_std-%s.npy'%(str(b)))
-        cpm_mean = np.load(DISTRI_DIR + 'Cpm_mean-%s.npy'%(str(b)))
-
-        for region in bin_dict[b]:
-            pval_list_up, pval_list_down, cpm, fc, cell_num = load_data(data_dir, region)
-            fc_cpm = (cpm + 0.01)/(cpm_mean + 0.01)
-
-            #preprocess pval list 
-            pval_list_up[np.argwhere(pval_list_up == 0)] = 1
-            pval_list_up[np.isinf(pval_list_up)] = 0
-            pval_list_up[np.isnan(pval_list_up)] = 0
-            pval_list_down[np.argwhere(pval_list_down == 0)] = 1
-            pval_list_down[np.isinf(pval_list_down)] = 0
-            pval_list_down[np.isnan(pval_list_down)] = 0
-
-            #split up-regulation and down-regulation
-            up_i = np.where(np.array(fc_cpm) > (1 + fc_cutoff))[0]
-            up_idx = np.array(list(set(up_i).intersection(set(np.where(pval_list_up < pval_cutoff)[0]))))
-
-            down_i = np.where(np.array(fc_cpm) < (1 - fc_cutoff))[0]
-            down_idx = np.array(list(set(down_i).intersection(set(np.where(pval_list_down < pval_cutoff)[0]))))
-
-            #Calculate p-value adj for Gaussian method 
-            down_zscore_list = (pval_list_down[down_idx] - down_mean[down_idx]) / down_std[down_idx]
-            down_padj_list = scipy.stats.norm.logsf(abs(down_zscore_list))
-            down_hit_fc_list = fc_cpm[down_idx]
-
-            up_zscore_list = (pval_list_up[up_idx] - up_mean[up_idx]) / up_std[up_idx]
-            up_padj_list = scipy.stats.norm.logsf(abs(up_zscore_list))
-            up_hit_fc_list = fc_cpm[up_idx]
-
-            #save to csv file: down-regulation gene 
-            global_gene_series = annot_df.set_index('idx').loc[down_idx, :]
-            global_gene_series['region'] = region
-            global_gene_series['num_cell'] = cell_num
-            global_gene_series['bin'] = b
-            global_gene_series['pval'] = pval_list_down[down_idx]
-            global_gene_series['fc'] = fc[down_idx]
-            global_gene_series['padj-Gaussian'] = down_padj_list
-            global_gene_series['fc_by_rand_dist_cpm'] = down_hit_fc_list
-            global_gene_series['idx'] = global_gene_series.index
-            global_hits_df = global_hits_df.append(global_gene_series)
-
-            #save to csv file: up-regulation gene 
-            global_gene_series = annot_df.set_index('idx').loc[up_idx, :]
-            global_gene_series['region'] = region
-            global_gene_series['num_cell'] = cell_num
-            global_gene_series['bin'] = b
-            global_gene_series['pval'] = pval_list_up[up_idx]
-            global_gene_series['fc'] = fc[up_idx]
-            global_gene_series['padj-Gaussian'] = up_padj_list
-            global_gene_series['fc_by_rand_dist_cpm'] = up_hit_fc_list
-            global_gene_series['idx'] = global_gene_series.index
-            global_hits_df = global_hits_df.append(global_gene_series)
+        logger.info(f'  Processing region: {region}')
+        if region.startswith('chr') == False:   
+            logger.info('No chromosome coordination in this region, cannot compute local analysis.')
+            continue
+
+        cpm_file = OBS_DIR + region + '-cpm'
+        cpm = sio.loadmat(cpm_file)['matrix'][0]        
+        fc_files = glob.glob(OBS_DIR + region + '*-foldchange')
+        if len(fc_files) == 1:
+            fc_file = fc_files[0]
+            cell_num = int(fc_file.split('/')[-1].split('-')[-2])
+        else:    
+            numbers = np.array([int(float(i.split('/')[-1].split('-')[2])) for i in fc_files])
+            chosen_num = np.max(numbers)
+            cell_num = int(chosen_num)
+            fc_file = OBS_DIR + region + '-' + str(chosen_num) + '-foldchange'
+        
+        fc = sio.loadmat(fc_file)['matrix'][0]  #compare to all the other cells as background
+
+        #get the gene idx within local analysis window and filter with fold change 
+        local_gene = get_neighbor_genes(region, 2e6, annot_df)
+        fc_cutoff = 0.01
+        #Calculate the overlap genes with annot_df, and only save the information on those genes.
+        down_idx = np.where(np.array(fc) < (1 - fc_cutoff))[0]
+        unique_elements, unique_indices = np.unique(gene_seq, return_index=True)
+        down_keep_genes = list((set(annot_df['gene_names']).intersection(set(gene_seq[down_idx]))).intersection(set(local_gene)))
+        down_keep_genes_idx = sorted(list(unique_indices[np.where(np.isin(unique_elements, down_keep_genes))[0]]))
+
+        if len(down_keep_genes_idx) ==0:
+            logger.info(f'  No down-regulation genes within local analysis windown. ')
+            continue
             
-            logger.info(f'Finish region: {region}')
-    
-    global_hits_df = global_hits_df.reindex(columns=df_column_list)
+        #read the pval matrix
+        pval = sio.loadmat(OBS_DIR + region + '-down_log-pval')['matrix'][0] #raw hypergeom p value
+        
+        #Calculate the adjusted pval with closet cell number distribution
+        chosen_dist = Num[np.argmin([np.absolute(n - cell_num) for n in Num])]
+        
+        #Load the file
+        down_mean = np.load(DISTRI_DIR + 'Down_dist_mean-%s.npy'%(str(chosen_dist)))
+        down_std = np.load(DISTRI_DIR + 'Down_dist_std-%s.npy'%(str(chosen_dist)))
+        cpm_mean = np.load(DISTRI_DIR + 'Cpm_mean-%s.npy'%(str(chosen_dist)))
+        
+        fc_rand = cpm/cpm_mean
+        
+        #Calculate adjusted p value of Gaussian padj
+        down_zscore_list = (pval[down_keep_genes_idx] - down_mean[down_keep_genes_idx]) / down_std[down_keep_genes_idx]
+        down_padj_list = scipy.stats.norm.logsf(abs(down_zscore_list))
+        hits_fc = fc[down_keep_genes_idx]
+        hits_fc_rand = fc_rand[down_keep_genes_idx]
+
+        #save to csv file 
+        local_gene_series = annot_df[annot_df['gene_names'].isin(down_keep_genes)].set_index('idx')
+        local_gene_series['region'] = region
+        dist_list = []
+        for i in local_gene_series['pos']:
+            dist = get_distance(region, i)
+            dist_list.append(dist)
+        local_gene_series['distance'] = dist_list
+        local_gene_series['num_cell'] = cell_num
+        local_gene_series['bin'] = chosen_dist
+        local_gene_series['pval'] = pval[down_keep_genes_idx] 
+        local_gene_series['fc'] = hits_fc
+        local_gene_series['padj-Gaussian'] = down_padj_list
+        local_gene_series['fc_by_rand_dist_cpm'] = hits_fc_rand
+        local_gene_series['cpm_perturb'] = cpm[down_keep_genes_idx]
+        local_gene_series['cpm_bg'] = cpm_mean[down_keep_genes_idx]
+        local_gene_df = local_gene_df.append(local_gene_series)        
+        local_gene_df = local_gene_df.reindex(columns=df_column_list)
 
     if OUTPUT_DF.endswith('.csv'):
-        global_hits_df[global_hits_df['padj-Gaussian'] < pval_cutoff].to_csv(OUTPUT_DF)
+        local_gene_df.to_csv(OUTPUT_DF)
     else:
-        global_hits_df[global_hits_df['padj-Gaussian'] < pval_cutoff].to_csv(OUTPUT_DF + '.csv')
+        local_gene_df.to_csv(OUTPUT_DF + '.csv')
 
 if __name__ == '__main__':
-    pass
+    pass
```

### Comparing `pySpade-0.0.1/pySpade/parsers.py` & `pySpade-0.0.2/pySpade/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     return parser.parse_args(args)
 
 # process
 def add_process_subparser(subparsers):
     parser = subparsers.add_parser(
         'process',
-        help='process mapping output and reformat to downstream analysis.',
+        help='process mapping output and reformat for downstream analysis.',
         description=(
             'Process transcriptome output and sgrna output to remove experimental doublets. '
             'Transcriptome matrix is from Cellranger output (outs folder),'
             'sgrna matrix is from fba output, other accepted format include pkl and csv file.'
             'sgrna matrix column: cell barcodes consistent with transcriptome matrix, rows: sgrna sequence.'
             'The final output format is h5 file.'))
 
@@ -89,58 +89,51 @@
         help='check the average expression level of query genes in single cell matrix',
         description=(
             'Check the average expression level of query genes in single cell matrix'
             'Input: processed transcriptome matrix from the process output,'
             'query genes list has to be txt file, genes are seperated with new line.'))
 
     parser.add_argument('-t', 
-                        '--transcriptome_df', 
-                        dest='transcriptome_df', 
+                        '--transcriptome_dir', 
+                        dest='transcriptome_dir', 
                         required=True,
                         type=str,
-                        help='specify the processed transcriptome file')
+                        help='specify the directory from process function.')
 
     parser.add_argument('-g', 
                         '--gene',
                         dest='gene', 
                         required=True,
                         type=str,
                         help='specify the query genes.')
 
     parser.add_argument('-o', 
                         '--output_file', 
                         dest='output_file', 
-                        required=True,
+                        required=False,
                         help='specify output file.')
 
 #fc
 def add_fc_subparser(subparsers):
     parser = subparsers.add_parser(
         'fc',
         help='check the fold change of genes in given perturbation',
         description=(
             'Check the fold change of perturbed region and individual sgRNA for query region and gene.'
             'Input: processed transcriptome matrix and sgrna matrix from the process output,'
             'sgrna dict file: perturbation region hg38 coordinates and the sgrna sequence targeting that region.'
             'Region and sgrnas separated by tab, and sgrnas separated by comma'))
 
     parser.add_argument('-t', 
-                        '--transcriptome_df', 
-                        dest='transcriptome_df', 
+                        '--transcriptome_dir', 
+                        dest='transcriptome_dir', 
                         required=True,
                         type=str,
                         help='specify the processed transcriptome matrix file')
 
-    parser.add_argument('-s', 
-                        '--sgrna', 
-                        dest='input_sgrna', 
-                        required=True,
-                        type=str,
-                        help='specify the processed sgrna matrix file.')
-    
     parser.add_argument('-d', 
                         '-dict', 
                         dest='dict', 
                         required=True,
                         type=str, 
                         help='specify the perturbation coordinates (hg38) and the sgRNA txt file.')
 
@@ -148,18 +141,18 @@
                         '--region', 
                         dest='region', 
                         required=True,
                         type=str,
                         help='specify the query regions and their target genes to calculate repression efficiency.')
 
     parser.add_argument('-o', 
-                        '--output_file', 
-                        dest='output_file', 
+                        '--output_folder', 
+                        dest='output_folder', 
                         required=True,
-                        help='specify output file.')
+                        help='specify output folder directory.')
 
 #DEobs
 def add_DEobs_subparser(subparsers):
     parser = subparsers.add_parser(
         'DEobs',
         help='perform differential expression analysis of observe cells',
         description=(
@@ -282,51 +275,72 @@
                         required=True,
                         help='specify an output directory.')
 
 #local
 def add_local_subparser(subparsers):
     parser = subparsers.add_parser(
         'local',
-        help='perform local hit analysis (+-2Mb) with obs and random background',
+        help='perform local hit analysis (+-2Mb) with observation data and random background',
         description=('Using the observation p value and randomization bavckground p value'
                      'to calculate the adjusted p value based on Gaussian distribution approximation'
                      'Local hits calculation includes the genes within plus and minus 2 Mb of the perturbation region.'
                      'The output is a csv file with all hits information.'))
-
+   
+    parser.add_argument('-f', 
+                        '--file_dir', 
+                        dest='file_dir', 
+                        required=True,
+                        type=str,
+                        help='specify the file directory of "process" function output, the Trans_genome_seq.npy file is required at this step.')
+   
     parser.add_argument('-d', 
                         '--data_dir', 
                         dest='data_dir', 
                         required=True,
                         type=str,
                         help='specify the p-value matrix directory of observation test.')
 
     parser.add_argument('-t', 
                         '--distr', 
                         dest='distr', 
                         required=True,
                         type=str,
                         help='specify the random cell mean/std/10_perc file directory.')
+    
+    parser.add_argument('-s', 
+                        '-sgrna_dict', 
+                        dest='sgrna_dict', 
+                        required=True,
+                        type=str, 
+                        help='specify the perturbation coordinates (hg38) and the sgRNA txt file.')
 
     parser.add_argument('-o', 
                         '--output_file', 
                         dest='output_file', 
                         required=True,
                         type=str,
                         help='specify an output file name incluseing the directory, it has to be in csv format.')
 
 #global
 def add_global_subparser(subparsers):
     parser = subparsers.add_parser(
         'global',
-        help='perform global hit analysis with obs and random background',
+        help='perform global hit analysis with observation data and random background',
         description=('Using the observation p value and randomization bavckground p value'
                      'to calculate the adjusted p value based on Gaussian distribution approximation'
                      'The output is a csv file with all hits information.'
                      'cutoff for p value is -1 (ln), fold change is 10%'))
-
+    
+    parser.add_argument('-f', 
+                        '--file_dir', 
+                        dest='file_dir', 
+                        required=True,
+                        type=str,
+                        help='specify the file directory of "process" function output, the Trans_genome_seq.npy file is required at this step.')
+    
     parser.add_argument('-d', 
                         '--data_dir', 
                         dest='data_dir', 
                         required=True,
                         type=str,
                         help='specify the p-value matrix directory of observation test.')
```

### Comparing `pySpade-0.0.1/pySpade/plot_annotation.txt` & `pySpade-0.0.2/pySpade/plot_annotation.txt`

 * *Files identical despite different names*

### Comparing `pySpade-0.0.1/pySpade/process.py` & `pySpade-0.0.2/pySpade/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,15 @@
     stats_output.write('sgRNA mean after filter sgRNA outlier: ' + str(sgrna_mean_out) + '\n')
     stats_output.write('sgRNA median after filter sgRNA outlier: ' + str(sgrna_median_out) + '\n')
     stats_output.write('Cells after filter experimental doublets and sgRNA outliers: ' + str(len(no_outlier_sgrna_df.columns)) + '\n')
     stats_output.close()
 
     #write output matrix
     sub_df = pd.DataFrame(data=filtered_feature_bc_matrix.matrix.todense(), columns=filtered_feature_bc_matrix.barcodes.astype(str), index=filtered_feature_bc_matrix.feature_ref['name'].astype(str))
+    np.save(OUTPUT_DIR + 'Trans_genome_seq', sub_df.index)
     if (COMP=='True'):
         no_outlier_sgrna_df.to_hdf(OUTPUT_DIR + '/Singlet_sgRNA_df.h5', key='df', mode='w', complevel=9, complib='zlib')    
         sub_df[no_outlier_sgrna_df.columns].to_hdf(OUTPUT_DIR + '/Singlet_sub_df.h5', key='df', mode='w', complevel=9, complib='zlib')
     elif (COMP=='False'):
         no_outlier_sgrna_df.to_hdf(OUTPUT_DIR + '/Singlet_sgRNA_df.h5', key='df', mode='w')    
         sub_df[no_outlier_sgrna_df.columns].to_hdf(OUTPUT_DIR + '/Singlet_sub_df.h5', key='df', mode='w')
```

### Comparing `pySpade-0.0.1/pySpade/utils.py` & `pySpade-0.0.2/pySpade/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import itertools 
 from importlib import resources
 from scipy import sparse, io
 from scipy.sparse import csr_matrix
 import glob
 import re
 import tables
+import matplotlib.pyplot as plt
 
 def get_logger(logger_name, log_file=False):
     """Creates a custom logger."""
 
     FORMATTER = '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 
     logger = logging.getLogger(logger_name)
@@ -159,14 +160,32 @@
         index = [i for i,e in enumerate(trans_df.columns) if e.split('-')[1] == lib]
         one_cell_cpm = np.array((trans_df.iloc[:,index].sum(axis = 1) + 1)\
                         / np.sum(trans_df.iloc[:,index].values) * 1e6).flatten()
         for i in index:
             cell_cpm = trans_df.iloc[:,i] / np.sum(trans_df.iloc[:,i].values) * 1e6
             cpm_matrix[:,i] = cell_cpm / one_cell_cpm  
 
+def set_axis_style(ax, labels):
+    ax.xaxis.set_tick_params(direction='out')
+    ax.xaxis.set_ticks_position('bottom')
+    ax.set_xticks(np.arange(1, len(labels) + 1))
+    ax.set_xticklabels(labels, fontsize=14, color='#000000')
+    ax.set_xlim(0.25, len(labels) + 0.75)
+
+def sc_exp_box_plot(sgrna_cells_expression, other_cells_expression, target_gene, region, output_file):
+    fig, ax = plt.subplots(figsize= (8,6))
+    ax.set_title(target_gene + ' expression in ' + region, fontsize=20)
+    flierprops = dict(marker='o', markerfacecolor='#000000', markersize=6, alpha=0.5,
+                    linestyle='none')
+    ax.boxplot([sgrna_cells_expression, other_cells_expression], whis=[10, 90],
+            showfliers=True, flierprops=flierprops)
+    labels = ['sgRNA cells', 'other cells']
+    set_axis_style(ax, labels)
+    plt.savefig(output_file)
+
 def hypergeo_test(non_zero_array, sgrna_idx, i):
     #find indecies of cells in which expression of given gene is
     #equal or less than the median of this gene in the whole population
     median_cell_idx  = np.argwhere(non_zero_array <= np.median(non_zero_array))
 
     #find the same cells subset in the cells with a given sgRNA
     overlap_cell_idx = np.intersect1d(median_cell_idx, sgrna_idx)
@@ -221,25 +240,24 @@
     up_pval_file   = data_dir + region + '-up_log-pval'
     down_pval_file = data_dir + region + '-down_log-pval'
     cpm_file = data_dir + region + '-cpm'
     fc_files = glob.glob(data_dir + region + '*-foldchange')
     if len(fc_files) == 1:
         fc_file = fc_files[0]
     else:
-        
-        numbers = np.array([int(float(i.split('/')[-1].split('-')[2])) for i in fc_files])
+        numbers = np.array([int(float(i.split('/')[-1].split('-')[-2])) for i in fc_files])
         chosen_num = np.max(numbers)
-        fc_file = data_dir + region + '-' + str(chosen_num) + '*-foldchange'
+        fc_file = data_dir + region + '-' + str(chosen_num) + '-foldchange'
     
     pval_list_up = io.loadmat(up_pval_file)['matrix'][0]
     pval_list_down = io.loadmat(down_pval_file)['matrix'][0]
     cpm = io.loadmat(cpm_file)['matrix'][0]
     fc = io.loadmat(fc_file)['matrix'][0]
     
-    num_sgrna_cell = int(fc_file.split('/')[-1].split('-')[2])
+    num_sgrna_cell = int(fc_file.split('/')[-1].split('-')[-2])
     return pval_list_up, pval_list_down, cpm, fc, num_sgrna_cell
 
 def get_neighbor_genes(region, query_range, annot_df):
     
     length_list = [
         0, 248956422,491149951,689445510,879660065,1061198324,
         1232004303,1391350276,1536488912,1674883629,1808681051,
@@ -252,20 +270,20 @@
         'chr1', 'chr2', 'chr3', 'chr4', 'chr5', 'chr6', 'chr7', 'chr8',
         'chr9', 'chr10', 'chr11', 'chr12', 'chr13', 'chr14', 'chr15',
         'chr16', 'chr17', 'chr18', 'chr19', 'chr20', 'chr21', 'chr22', 'chrX'
     ]
 
     enh_chrom, left, right = re.split('[:|-]', region)
     position = int(left) + length_list[chr_order.index(enh_chrom)]
-    gene_idx = annot_df.loc[(annot_df.pos < position + query_range) \
+    gene = annot_df.loc[(annot_df.pos < position + query_range) \
                             & (annot_df.pos > position - query_range)\
-                            & (annot_df.chromosome == enh_chrom)].index.values
-    return(gene_idx)
+                            & (annot_df.chromosome == enh_chrom)].gene_names.values
+    return(gene)
 
-def get_distance(region, gene_pos, annot_df):
+def get_distance(region, gene_pos):
     length_list = [
         0, 248956422,491149951,689445510,879660065,1061198324,               
         1232004303,1391350276,1536488912,1674883629,1808681051,
         1943767673,2077042982,2191407310,2298451028,2400442217,
         2490780562,2574038003,2654411288,2713028904,2777473071,
         2824183054,2875001522,3031029399
     ]
```

### Comparing `pySpade-0.0.1/pySpade.egg-info/PKG-INFO` & `pySpade-0.0.2/pySpade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pySpade
-Version: 0.0.1
-Summary: Single cell Perturbation Analysis of Differential Expression
-Home-page: https://github.com/yihan1119/pySpade
+Version: 0.0.2
+Summary: Single cell Perturbations - Analysis of Differential gene Expression
+Home-page: https://github.com/Hon-lab/pySpade
 Author: Yihan Wang
 Author-email: Yihan.Wang@UTSouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pySpade: Single cell Perturbation Analysis of Differential Expression
+# pySpade: Single cell Perturbations - Analysis of Differential gene Expression
 
 ## Overview
 _________
 `pySpade` is a user friendly tool to perform the whole transcriptome analysis of single cell perturbation dataset. With the direct output of Cellranger, `pySpade` utilizes hypergeomtric test to analyze the whole transcriptome differential expression and generates hits table csv file. User can use the table to do downstream processing like generating Manhattan plots (tutorial includes). Currently we support human genome.     
 
 ## Requirement
 _________
@@ -45,21 +45,21 @@
 Version: 0.0.1
 
 optional arguments:
   -h, --help  show this help message and exit
 
 functions:
   
-    process   process mapping output and reformat to downstream analysis.
+    process   process mapping output and reformat for downstream analysis.
     explevel  check the average expression level of query genes in single cell matrix
     fc        check the fold change of sgrna
-    DEobs     perform differential expression analysis of observe cells
+    DEobs     perform differential expression analysis of observed cells
     DErand    perform differential expression analysis of random selection background
-    local     perform local hit analysis with obs and random background
-    global    perform global hit analysis with obs and random background
+    local     perform local hit analysis with observation data and random background
+    global    perform global hit analysis with observation data and random background
     
 ```
 
 * `process` : Process transcriptome output and sgrna output to remove experimental doublets sgrna outlier cells. Transcriptome matrix is from Cellranger output (outs folder). sgrna matrix column: cell barcodes consistent with transcriptome matrix, rows: sgrna sequence. The final output format is h5 file. The final output can be compressed to save disk space, but it may take more time to write the final output file.
 
 * `explevel` : Check the average expression level of query genes in single cell matrix. Input: processed transcriptome matrix from the `process` output, query genes list has to be txt file, genes are seperated with new line.
```

### Comparing `pySpade-0.0.1/setup.py` & `pySpade-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,18 +5,18 @@
     long_description = fh.read()
 
     setup(
     name='pySpade',
     version=__version__,
     author='Yihan Wang',
     author_email='Yihan.Wang@UTSouthwestern.edu',
-    description='Single cell Perturbation Analysis of Differential Expression',
+    description='Single cell Perturbations - Analysis of Differential gene Expression',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/yihan1119/pySpade',
+    url='https://github.com/Hon-lab/pySpade',
     packages=find_packages(exclude=('docs', 'tests')),
     package_dir={'pySpade': 'pySpade'},
     package_data={'pySpade': ['*.txt']},
     include_package_data=True,
     classifiers=[
                 'Programming Language :: Python :: 3',
                 'License :: OSI Approved :: MIT License',
```

