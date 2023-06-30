# Comparing `tmp/degex-0.0.23.tar.gz` & `tmp/degex-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degex-0.0.23.tar", last modified: Sun Jun 25 21:26:38 2023, max compression
+gzip compressed data, was "degex-0.0.24.tar", last modified: Fri Jun 30 16:31:39 2023, max compression
```

## Comparing `degex-0.0.23.tar` & `degex-0.0.24.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:26:38.680722 degex-0.0.23/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-03-21 13:23:11.000000 degex-0.0.23/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-03-21 13:23:11.000000 degex-0.0.23/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:26:38.680577 degex-0.0.23/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      291 2023-05-26 15:02:30.000000 degex-0.0.23/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:26:38.679552 degex-0.0.23/degex/
--rw-r--r--   0 solst      (501) staff       (20)       23 2023-06-25 21:26:28.000000 degex-0.0.23/degex/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    18909 2023-06-25 21:26:28.000000 degex-0.0.23/degex/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)    21038 2023-06-25 21:26:28.000000 degex-0.0.23/degex/adata.py
--rw-r--r--   0 solst      (501) staff       (20)    21299 2023-05-26 15:02:24.000000 degex-0.0.23/degex/branches.py
--rw-r--r--   0 solst      (501) staff       (20)      531 2023-06-25 21:26:28.000000 degex-0.0.23/degex/core.py
--rw-r--r--   0 solst      (501) staff       (20)    21040 2023-05-26 15:02:24.000000 degex-0.0.23/degex/granger.py
--rw-r--r--   0 solst      (501) staff       (20)     2850 2023-06-25 21:26:28.000000 degex-0.0.23/degex/plots.py
--rw-r--r--   0 solst      (501) staff       (20)     4892 2023-06-25 21:26:28.000000 degex-0.0.23/degex/preprocessing.py
--rw-r--r--   0 solst      (501) staff       (20)     2601 2023-06-25 21:26:28.000000 degex-0.0.23/degex/static.py
--rw-r--r--   0 solst      (501) staff       (20)     2564 2023-06-25 21:26:28.000000 degex-0.0.23/degex/types.py
--rw-r--r--   0 solst      (501) staff       (20)     2109 2023-06-25 21:26:28.000000 degex-0.0.23/degex/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-25 21:26:38.680400 degex-0.0.23/degex.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)      968 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      438 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       32 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-05-26 15:02:38.000000 degex-0.0.23/degex.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      165 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        6 2023-06-25 21:26:38.000000 degex-0.0.23/degex.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)     1095 2023-06-25 21:26:26.000000 degex-0.0.23/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-25 21:26:38.680760 degex-0.0.23/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2541 2023-03-21 13:23:12.000000 degex-0.0.23/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-30 16:31:39.809887 degex-0.0.24/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-03-21 13:23:11.000000 degex-0.0.24/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-03-21 13:23:11.000000 degex-0.0.24/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)      953 2023-06-30 16:31:39.809734 degex-0.0.24/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      276 2023-06-30 16:30:49.000000 degex-0.0.24/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-30 16:31:39.808234 degex-0.0.24/degex/
+-rw-r--r--   0 solst      (501) staff       (20)       23 2023-06-30 16:30:38.000000 degex-0.0.24/degex/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     6220 2023-06-30 16:30:38.000000 degex-0.0.24/degex/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)    21213 2023-06-30 16:30:38.000000 degex-0.0.24/degex/adata.py
+-rw-r--r--   0 solst      (501) staff       (20)     2757 2023-06-30 16:30:38.000000 degex-0.0.24/degex/plots.py
+-rw-r--r--   0 solst      (501) staff       (20)     5098 2023-06-30 16:30:38.000000 degex-0.0.24/degex/preprocessing.py
+-rw-r--r--   0 solst      (501) staff       (20)     2601 2023-06-30 16:30:38.000000 degex-0.0.24/degex/static.py
+-rw-r--r--   0 solst      (501) staff       (20)     2564 2023-06-30 16:30:38.000000 degex-0.0.24/degex/types.py
+-rw-r--r--   0 solst      (501) staff       (20)     2118 2023-06-30 16:30:38.000000 degex-0.0.24/degex/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-30 16:31:39.809512 degex-0.0.24/degex.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)      953 2023-06-30 16:31:39.000000 degex-0.0.24/degex.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      389 2023-06-30 16:31:39.000000 degex-0.0.24/degex.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-30 16:31:39.000000 degex-0.0.24/degex.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       32 2023-06-30 16:31:39.000000 degex-0.0.24/degex.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-05-26 15:02:38.000000 degex-0.0.24/degex.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      129 2023-06-30 16:31:39.000000 degex-0.0.24/degex.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        6 2023-06-30 16:31:39.000000 degex-0.0.24/degex.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)     1043 2023-06-30 16:31:29.000000 degex-0.0.24/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-30 16:31:39.809929 degex-0.0.24/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2541 2023-03-21 13:23:12.000000 degex-0.0.24/setup.py
```

### Comparing `degex-0.0.23/LICENSE` & `degex-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `degex-0.0.23/PKG-INFO` & `degex-0.0.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.23
+Version: 0.0.24
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
@@ -13,16 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-DEtect Gene EXpression (degex)
-================
+# DEtect Gene EXpression (degex)
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
 ``` sh
 # create conda environment
```

### Comparing `degex-0.0.23/degex/adata.py` & `degex-0.0.24/degex/adata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_adata.ipynb.
 
 # %% auto 0
-__all__ = ['QC_VARS', 'PCA_KWARGS', 'PHATE_KWARGS', 'G_KWARGS', 'set_gene_symbol_as_var_names', 'set_var_names_as_gene_ids',
-           'remove_mitochondrial_genes', 'score_doublets', 'add_gene_annotations', 'stack', 'stack_batchs',
-           'var_starts_with_pattern', 'make_var_starts_with', 'calc_qc_stats', 'filter_by_cutoffs',
+__all__ = ['QC_VARS', 'PCA_KWARGS', 'PHATE_KWARGS', 'G_KWARGS', 'MAGIC_KWARGS', 'set_gene_symbol_as_var_names',
+           'set_var_names_as_gene_ids', 'remove_mitochondrial_genes', 'score_doublets', 'add_gene_annotations', 'stack',
+           'stack_batchs', 'var_starts_with_pattern', 'make_var_starts_with', 'calc_qc_stats', 'filter_by_cutoffs',
            'apply_filter_by_cutoffs', 'add_prenormalization_layer', 'add_gene_detection_layer',
            'sqrt_library_size_normalize', 'add_batch_mean_center_layer',
            'score_genes_cell_cycle_with_batch_mean_center_data', 'load_human_genes', 'select_hvg_per_batch',
            'add_tf_annotations_from_csv', 'add_human_tfs_from_csv', 'add_mouse_tfs_from_csv', 'zscore_markers_in_layer',
            'subset_markers', 'run_pca', 'run_pca_on_hvg', 'run_phate_using_g', 'run_phate_on_hvg', 'run_magic']
 
 # %% ../nbs/03_adata.ipynb 3
@@ -17,15 +17,15 @@
 #hyper needs the four following aliases to be done manually.
 collections.Iterable = collections.abc.Iterable
 collections.Mapping = collections.abc.Mapping
 collections.MutableSet = collections.abc.MutableSet
 collections.MutableMapping = collections.abc.MutableMapping
 
 # %% ../nbs/03_adata.ipynb 4
-import os, copy
+import copy
 
 import numpy as np, pandas as pd, scipy
 import phate, magic, graphtools as gt
 import scprep, anndata as ad, scanpy as sc, scrublet as scr
 from scipy.stats import zscore
 
 from typing import TypeAlias, List, Sequence, Tuple, Optional, Dict
@@ -684,16 +684,17 @@
 
     adata.obs[obs_key] = (found).replace({True: marker_name, False: other_name})
     return adata
 
 
 # %% ../nbs/03_adata.ipynb 27
 PCA_KWARGS: dict = dict(n_components=100)
-PHATE_KWARGS: dict = dict(t=70)
+PHATE_KWARGS: dict = dict(n_components=3, t=70)
 G_KWARGS: dict = dict(knn=10)
+MAGIC_KWARGS: dict = dict(solver='approximate', n_jobs=-1, knn_max=60)
 
 # %% ../nbs/03_adata.ipynb 29
 def run_pca(
     adata: AnnData,
     pca_kwargs: dict = PCA_KWARGS,
     plot_scree: bool = False,
     emb_key: str = X_PCA,
@@ -762,17 +763,18 @@
     return run_phate_using_g(
         adata, g, phate_kwargs, g_kwargs, emb_key
     )
 
 
 # %% ../nbs/03_adata.ipynb 33
 def run_magic(
-    adata: AnnData, g: Graph, knn_max: int = 60
+    adata: AnnData, g: Graph, magic_kwargs: dict = MAGIC_KWARGS
 ) -> AnnData:
     G = copy.deepcopy(g)
+    knn_max = MAGIC_KWARGS.get('knn_max', 60)
     G.knn_max = knn_max
     G.data = adata.to_df()
     G.data_nu = adata.to_df()
-    magic_op = magic.MAGIC().fit(adata.to_df(), graph=G)
+    magic_op = magic.MAGIC(**magic_kwargs).fit(adata.to_df(), graph=G)
     data_magic = magic_op.transform(genes='all_genes')
     adata.layers[X_MAGIC] = scipy.sparse.csr_matrix(data_magic)
     return adata
```

### Comparing `degex-0.0.23/degex/plots.py` & `degex-0.0.24/degex/plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,21 +10,17 @@
 #hyper needs the four following aliases to be done manually.
 collections.Iterable = collections.abc.Iterable
 collections.Mapping = collections.abc.Mapping
 collections.MutableSet = collections.abc.MutableSet
 collections.MutableMapping = collections.abc.MutableMapping
 
 # %% ../nbs/04_plots.ipynb 4
-import os, copy
-
-import numpy as np, pandas as pd
+import os
 import scanpy as sc
 
-from typing import TypeAlias, List, Sequence, Tuple
-
 # %% ../nbs/04_plots.ipynb 5
 from degex.static import (
     TOTAL_COUNTS, PCT_COUNTS_MITO, PCT_COUNTS_RIBO,
 )
 from .types import (AnnData, )
 from .utils import (make_qc_fig_filename)
```

### Comparing `degex-0.0.23/degex/preprocessing.py` & `degex-0.0.24/degex/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,17 @@
 #hyper needs the four following aliases to be done manually.
 collections.Iterable = collections.abc.Iterable
 collections.Mapping = collections.abc.Mapping
 collections.MutableSet = collections.abc.MutableSet
 collections.MutableMapping = collections.abc.MutableMapping
 
 # %% ../nbs/05_preprocessing.ipynb 4
-import os, copy, warnings
-
-import numpy as np, pandas as pd, scipy
-import phate, magic, graphtools as gt
-import scprep, anndata as ad, scanpy as sc, scrublet as scr
-
-from typing import TypeAlias, List, Sequence, Tuple
+import copy, warnings
+from typing import Sequence, Tuple
+import scanpy as sc
 
 # %% ../nbs/05_preprocessing.ipynb 5
 from degex.static import (
     GENE_IDS, TOTAL_COUNTS, 
     PCT_COUNTS_MITO, PCT_COUNTS_RIBO, DOUBLET_SCORES,
 )
 from degex.types import (
@@ -42,86 +38,99 @@
     add_batch_mean_center_layer,
     score_genes_cell_cycle_with_batch_mean_center_data,
     select_hvg_per_batch,
     run_pca, run_pca_on_hvg,
     run_phate_on_hvg, run_phate_using_g, run_magic,
 )
 
+from degex.adata import (
+    PCA_KWARGS, PHATE_KWARGS, G_KWARGS, MAGIC_KWARGS
+)
+
 # %% ../nbs/05_preprocessing.ipynb 6
-def prepare_h5ad_file(filename:str, plot:bool=False) -> AnnData:
+def prepare_h5ad_file(filename: str, plot: bool = False) -> AnnData:
     try:
         adata = sc.read_10x_h5(filename, gex_only = True)
     except ValueError:
         warnings.warn('Failed to use sc.read_10x_h5 to load file. Using read_h5ad as fallback. Is your data from 10x?')
         adata = sc.read_h5ad(filename)
     adata = set_gene_symbol_as_var_names(adata)
     try:
         adata = set_var_names_as_gene_ids(adata)
     except KeyError:
         warnings.warn(f'Failed to find a feature named {GENE_IDS} in adata.var. Not setting adata.names to `{GENE_IDS}`.')
     adata = score_doublets(adata, plot)
     return adata
 
 def filter_pipeline(
-    adata:AnnData,
-    cutoff_specs:CutoffSpecs = [
+    adata: AnnData,
+    cutoff_specs: CutoffSpecs = [
         CutoffSpec(TOTAL_COUNTS,     500,  10000),
         CutoffSpec(PCT_COUNTS_MITO, None, 15),
         CutoffSpec(PCT_COUNTS_RIBO, None, 15),
         CutoffSpec(DOUBLET_SCORES,  None, 0.4),
     ],
-    min_cells:int=5,
-    remove_mt_genes:bool=False,
+    min_cells: int = 5,
+    min_genes: int = 200,
+    remove_mt_genes: bool = False,
 ) -> AnnData:    
-    adata = apply_filter_by_cutoffs(adata, cutoff_specs)
-    sc.pp.filter_genes(adata, min_cells=min_cells)
+    if cutoff_specs is not None:
+        adata = apply_filter_by_cutoffs(adata, cutoff_specs)
+    
+    if min_genes:
+        sc.pp.filter_cells(adata, min_genes=min_genes)
+    
+    if min_cells:
+        sc.pp.filter_genes(adata, min_cells=min_cells)
+    
     if remove_mt_genes:
         adata = remove_mitochondrial_genes(adata)    
     return adata
 
 def normalization_pipeline(
     adata:AnnData,
-    s_genes:Sequence[str]=None,
-    g2m_genes:Sequence[str]=None
+    s_genes: Sequence[str] = None,
+    g2m_genes: Sequence[str] = None
 ) -> AnnData:
     adata = add_prenormalization_layer(adata)
     adata = add_gene_detection_layer(adata)
     adata = sqrt_library_size_normalize(adata)
     adata = add_batch_mean_center_layer(adata)
     if s_genes is not None and g2m_genes is not None:
         adata = score_genes_cell_cycle_with_batch_mean_center_data(
             adata, s_genes, g2m_genes
         )
     return adata
 
 def embedding_pipeline(
-    adata:AnnData,
+    adata: AnnData,
 
     # PCA on adata.X
-    pca_kwargs:dict=dict(n_components=100),
-    plot_scree:bool=False,
+    pca_kwargs: dict = PCA_KWARGS,
+    plot_scree: bool = False,
     
     # PHATE on pca
-    phate_kwargs=dict(t=70),
-    g_kwargs=dict(knn=10),
+    phate_kwargs = PHATE_KWARGS,
+    g_kwargs = G_KWARGS,
     
-    do_hvg:bool=True,
+    do_hvg: bool = True,
 
     # How to calc hvg
-    hvg_kwargs:dict=dict(cutoff=None, percentile=90),
+    hvg_kwargs: dict = dict(cutoff=None, percentile=90),
 
     # PCA on hvg
-    hvg_pca_kwargs:dict=None,
+    hvg_pca_kwargs: dict=None,
     
     # PHATE on hvg
-    hvg_phate_kwargs:dict=None,
-    hvg_g_kwargs:dict=None,
+    hvg_phate_kwargs: dict = None,
+    hvg_g_kwargs: dict = None,
     
     # MAGIC on g_hvg
-    magic_knn_max:int=60
+    do_magic: bool = True,
+    magic_kwargs: dict = MAGIC_KWARGS
 ) -> Tuple[AnnData, Graph, Graph]:
     g, g_hvg = None, None
 
     # STEP 1: PCA on adata.X --> X_pca
     adata = run_pca(adata, pca_kwargs=pca_kwargs, plot_scree=plot_scree)
     
     # STEP 2: PHATE on X_pca --> X_phate
@@ -144,10 +153,11 @@
         # STEP 5: PCA on adata.X[:, HVGs] --> X_pca_hvg
         adata = run_pca_on_hvg(adata, hvg_pca_kwargs, plot_scree)
 
         # STEP 6: PHATE on X_pca_hvg --> X_phate_hvg
         adata, g_hvg = run_phate_on_hvg(adata, g_hvg, hvg_phate_kwargs, hvg_g_kwargs)
 
         # STEP 7: MAGIC on g_hvg --> X_magic
-        adata = run_magic(adata, g_hvg, magic_knn_max)
+        if do_magic:
+            adata = run_magic(adata, g_hvg, magic_kwargs)
 
     return adata, g, g_hvg
```

### Comparing `degex-0.0.23/degex/static.py` & `degex-0.0.24/degex/static.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.23/degex/types.py` & `degex-0.0.24/degex/types.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.23/degex/utils.py` & `degex-0.0.24/degex/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 # %% ../nbs/02_utils.ipynb 4
 import os
 
 # %% ../nbs/02_utils.ipynb 5
 from .types import AnnData, AnnDatas, ndarray
 
 # %% ../nbs/02_utils.ipynb 6
-def remove_non_numeric_from_str(s:str) -> str:
+def remove_non_numeric_from_str(s: str) -> str:
     '''
     Removes non-numbers from string.
     Utility function used in `time_to_num_from_idx_to_time`.
     '''
     s = ''.join(filter(str.isdigit, s))
     return s
 
-def time_to_num_from_idx_to_time(idx_to_time:dict) -> dict:
+def time_to_num_from_idx_to_time(idx_to_time: dict) -> dict:
     '''
     Examples:
         idx_to_time = {
             '0': '12hr', 
             '1': '18hr', 
             '2': '24hr'
         }
@@ -49,16 +49,16 @@
     time_to_num = {
         v: remove_non_numeric_from_str(v)
         for v in idx_to_time.values()
     }
     return time_to_num
 
 def make_qc_fig_filename(
-    save_dir:str,  study_name:str,
-    x:str, y:str, postfix:str=''
+    save_dir: str,  study_name: str,
+    x: str, y: str, postfix: str = ''
 ) -> str:     
     '''
     Utility function used in make_qc_figs to name files.
     Output files are in the form of:
     `{save_dir}/.QC_{study_name}_{x}_{y}_{postfix}.png`
     '''
     if postfix:
```

### Comparing `degex-0.0.23/degex.egg-info/PKG-INFO` & `degex-0.0.24/degex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.23
+Version: 0.0.24
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
@@ -13,16 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-DEtect Gene EXpression (degex)
-================
+# DEtect Gene EXpression (degex)
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
 ``` sh
 # create conda environment
```

### Comparing `degex-0.0.23/settings.ini` & `degex-0.0.24/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = degex
 lib_name = degex
-version = 0.0.23
+version = 0.0.24
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = degex
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -23,17 +23,17 @@
 description = Detect Gene Expression in Single-CEll data
 keywords = nbdev jupyter notebook python single cell detect gene expression spot marker genes
 language = English
 status = 3
 user = dsm-72
 conda_user = dsm-72
 host = github
-requirements = pandas scipy seaborn scikit-learn numpy graphtools matplotlib==3.7.0 scanpy==1.9.2 anndata==0.8.0
-pip_requirements = phate scprep magic-impute meld scrublet gseapy DiffusionEMD
-conda_requirements = bioconda::gseapy
+requirements = pandas scipy seaborn scikit-learn numpy>=1.22 graphtools matplotlib scanpy anndata
+pip_requirements = iza phate scprep magic-impute scrublet
+conda_requirements = 
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `degex-0.0.23/setup.py` & `degex-0.0.24/setup.py`

 * *Files identical despite different names*

