# Comparing `tmp/NeuroGraph-1.0.2.tar.gz` & `tmp/NeuroGraph-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NeuroGraph-1.0.2.tar", last modified: Sun Jun 25 20:17:26 2023, max compression
+gzip compressed data, was "dist/NeuroGraph-1.1.2.tar", last modified: Fri Jun 30 16:51:57 2023, max compression
```

## Comparing `NeuroGraph-1.0.2.tar` & `NeuroGraph-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     1067 2023-06-24 14:47:00.000000 NeuroGraph-1.0.2/LICENSE.txt
-drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/NeuroGraph/
--rw-rw-r--   0 anwar     (1000) anwar     (1000)        0 2023-06-25 15:58:57.000000 NeuroGraph-1.0.2/NeuroGraph/__init__.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     7067 2023-06-25 18:10:54.000000 NeuroGraph-1.0.2/NeuroGraph/datasets.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)    51030 2023-06-25 15:59:31.000000 NeuroGraph-1.0.2/NeuroGraph/preprocess.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      151 2023-06-25 20:10:33.000000 NeuroGraph-1.0.2/NeuroGraph/test.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     3284 2023-06-25 20:10:42.000000 NeuroGraph-1.0.2/NeuroGraph/utils.py
-drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-06-25 20:17:25.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/PKG-INFO
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      309 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/SOURCES.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)        1 2023-06-25 20:17:25.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/dependency_links.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)       53 2023-06-25 20:17:25.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/requires.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)       11 2023-06-25 20:17:25.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/top_level.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/PKG-INFO
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      169 2023-06-25 16:17:37.000000 NeuroGraph-1.0.2/README.md
--rw-rw-r--   0 anwar     (1000) anwar     (1000)       38 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/setup.cfg
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      797 2023-06-25 18:33:47.000000 NeuroGraph-1.0.2/setup.py
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     1067 2023-06-24 14:47:00.000000 NeuroGraph-1.1.2/LICENSE.txt
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)        0 2023-06-25 15:58:57.000000 NeuroGraph-1.1.2/NeuroGraph/__init__.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     6848 2023-06-29 15:03:47.000000 NeuroGraph-1.1.2/NeuroGraph/datasets.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)    39747 2023-06-29 15:03:47.000000 NeuroGraph-1.1.2/NeuroGraph/preprocess.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      345 2023-06-30 16:44:30.000000 NeuroGraph-1.1.2/NeuroGraph/test.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     5663 2023-06-30 16:43:00.000000 NeuroGraph-1.1.2/NeuroGraph/utils.py
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/PKG-INFO
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      309 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)        1 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       53 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/requires.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       11 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/NeuroGraph.egg-info/top_level.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/PKG-INFO
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      522 2023-06-27 17:54:10.000000 NeuroGraph-1.1.2/README.md
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       38 2023-06-30 16:51:57.000000 NeuroGraph-1.1.2/setup.cfg
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      797 2023-06-30 16:51:00.000000 NeuroGraph-1.1.2/setup.py
```

### Comparing `NeuroGraph-1.0.2/LICENSE.txt` & `NeuroGraph-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuroGraph-1.0.2/NeuroGraph/datasets.py` & `NeuroGraph-1.1.2/NeuroGraph/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,32 @@
+import torch
 from torch_geometric.data import Data, InMemoryDataset
 from torch_geometric.data import InMemoryDataset, download_url
-import os,glob
-import torch
+import os
+
 import zipfile
 
 class NeuroGraphStatic(InMemoryDataset):
-
-    r"""
+    """
     Graph-based neuroimaging benchmark datasets, e.g.,
     :obj:`"HCPGender"`, :obj:`"HCPAge"`, :obj:`"HCPActivity"`,
     :obj:`"HCP-WM"`, or :obj:`"HCP-FI"`
 
     Args:
         root (str): Root directory where the dataset should be saved.
-        name (str): The `name
-            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-            dataset.
-        transform (callable, optional): A function/transform that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a transformed
-            version. The data object will be transformed before every access.
-            (default: :obj:`None`)
-        pre_transform (callable, optional): A function/transform that takes in
-            an :obj:`torch_geometric.data.Data` object and returns a
-            transformed version. The data object will be transformed before
-            being saved to disk. (default: :obj:`None`)
-        pre_filter (callable, optional): A function that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a boolean
-            value, indicating whether the data object should be included in the
-            final dataset. (default: :obj:`None`)
-        return: Pytorch geometric dataset
+        name (str): The name of the dataset.
+        transform (callable, optional): A function/transform that takes in an :obj:`torch_geometric.data.Data` object and returns a transformed version. The data object will be transformed before every access. (default: :obj:`None`)
+        pre_transform (callable, optional): A function/transform that takes in an :obj:`torch_geometric.data.Data` object and returns a transformed version. The data object will be transformed before being saved to disk. (default: :obj:`None`)
+        pre_filter (callable, optional): A function that takes in an :obj:`torch_geometric.data.Data` object and returns a boolean value, indicating whether the data object should be included in the final dataset. (default: :obj:`None`)
+        
+    Returns:
+        PyTorch Geometric dataset
     """
 
+
     def __init__(self, root, dataset_name,transform=None, pre_transform=None, pre_filter=None):
         self.root, self.name = root, dataset_name
         self.root = root
         self.urls = {"HCPGender":'https://vanderbilt.box.com/shared/static/r6hlz2arm7yiy6v6981cv2nzq3b0meax.zip',
                     "HCPActivity":'https://vanderbilt.box.com/shared/static/b4g59ibn8itegr0rpcd16m9ajb2qyddf.zip',
                     "HCPAge":'https://vanderbilt.box.com/shared/static/lzzks4472czy9f9vc8aikp7pdbknmtfe.zip',
                     "HCPWM":'https://vanderbilt.box.com/shared/static/xtmpa6712fidi94x6kevpsddf9skuoxy.zip',
@@ -94,30 +86,28 @@
         if self.pre_transform is not None:
             data_list = [self.pre_transform(data) for data in data_list]
 
         data, slices = self.collate(data_list)
         torch.save((data, slices), self.processed_paths[0])
        
 class NeuroGraphDynamic():
+    """
+        Graph-based neuroimaging benchmark datasets, e.g.,
+        :obj:`"DynHCPGender"`, :obj:`"DynHCPAge"`, :obj:`"DynHCPActivity"`,
+        :obj:`"DynHCP-WM"`, or :obj:`"DynHCP-FI"`
+
+        Args:
+            root (str): Root directory where the dataset should be saved.
+            name (str): The name of the dataset.
 
-    r"""
-    Graph-based neuroimaging benchmark datasets, *.e.g.*,
-    :obj:`"DynHCPGender"`, :obj:`"DynHCPAge"`, :obj:`"DynHCPActivity"`,
-    :obj:`"DynHCP-WM"`, or :obj:`"DynHCP-FI"`
-
-
-    Args:
-        root (str): Root directory where the dataset should be saved.
-        name (str): The `name
-            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-            dataset.
-        
-        return: a list of graphs in pyg format. Each graph has dynamic graphs batched in pyg batch 
+        Returns:
+            list: A list of graphs in PyTorch Geometric (pyg) format. Each graph has dynamic graphs batched in pyg batch.
     """
 
+
     def __init__(self,root, name):
         self.root = root
         self.name = name
         self.urls = {"DynHCPGender":'https://vanderbilt.box.com/shared/static/mj0z6unea34lfz1hkdwsinj7g22yohxn.zip',
                     "DynHCPActivity":'https://vanderbilt.box.com/shared/static/2so3fnfqakeu6hktz322o3nm2c8ocus7.zip',
                     "DynHCPAge":'https://vanderbilt.box.com/shared/static/195f9teg4t4apn6kl6hbc4ib4g9addtq.zip',
                     "DynHCPWM":'https://vanderbilt.box.com/shared/static/mxy8fq3ghm60q6h7uhnu80pgvfxs6xo2.zip',
```

### Comparing `NeuroGraph-1.0.2/NeuroGraph/preprocess.py` & `NeuroGraph-1.1.2/NeuroGraph/preprocess.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,29 +4,18 @@
 import pickle
 import numpy as np
 from nilearn.datasets import fetch_atlas_schaefer_2018
 from nilearn.image import load_img
 from nilearn.connectome import ConnectivityMeasure
 from scipy.stats import zscore
 import torch
-from torch_geometric.data import Data
+from torch_geometric.data import Data,InMemoryDataset
 from random import randrange
-
-from torch_geometric.data import Data, InMemoryDataset
-from torch_geometric.data import InMemoryDataset
-import os,glob
 import math
-# from nilearn.input_data import NiftiLabelsMasker
-from nilearn.image import load_img
-import pandas as pd
 import zipfile
-from torch_geometric.data import Data
-import os
-import pickle
-from scipy.stats import zscore
 from joblib import Parallel, delayed
 from tqdm import tqdm
 import itertools
 import random
 
 
 
@@ -263,47 +252,14 @@
         dynamic_fc_list.append(corr)
     return dynamic_fc_list
 
 
 
 
 class Brain_connectome_Rest(InMemoryDataset):
-    r"""
-    Graph-based neuroimaging benchmark datasets,
-
-
-    Args:
-        root (str): Root directory where the dataset should be saved.
-
-        name (str): The `name
-            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-            dataset.
-
-        rois (int): the number of ROIs to be used for parcellation. 
-        Options are: {100, 200, 300, 400, 500, 600, 700, 800, 900, 1000}
-
-        path_to_data: Path to the fMRI data.
-
-        n_jobs: the number of jobs to process the data in parallel.
-
-        transform (callable, optional): A function/transform that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a transformed
-            version. The data object will be transformed before every access.
-            (default: :obj:`None`)
-        pre_transform (callable, optional): A function/transform that takes in
-            an :obj:`torch_geometric.data.Data` object and returns a
-            transformed version. The data object will be transformed before
-            being saved to disk. (default: :obj:`None`)
-        pre_filter (callable, optional): A function that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a boolean
-            value, indicating whether the data object should be included in the
-            final dataset. (default: :obj:`None`)
-        
-        return: Pytroch geometric dataset with four classes: [0] - gender, [1]-age, [2]- working memory and [3] -fluid intelligence 
-    """
     def __init__(self, root,name,n_rois, threshold,path_to_data,n_jobs, transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name,self.n_rois,self.threshold,self.path_to_data,self.n_jobs = root, name,n_rois,threshold,path_to_data,n_jobs
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
 
 
@@ -419,44 +375,15 @@
             dataset = [self.pre_transform(data) for data in dataset]
 
         data, slices = self.collate(dataset)
         print("saving path:",self.processed_paths[0])
         torch.save((data, slices), self.processed_paths[0])
 
 class Gender_Dataset(InMemoryDataset):
-    r"""
-    Graph-based neuroimaging dataset,
-
-
-    Args:
-        root (str): Root directory where the dataset should be saved.
-
-        name (str): The `name
-            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-            dataset.
-
-        
-
-        dataset: Pyg dataset obtained from Brain_connectome_Rest class 
-
-        transform (callable, optional): A function/transform that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a transformed
-            version. The data object will be transformed before every access.
-            (default: :obj:`None`)
-        pre_transform (callable, optional): A function/transform that takes in
-            an :obj:`torch_geometric.data.Data` object and returns a
-            transformed version. The data object will be transformed before
-            being saved to disk. (default: :obj:`None`)
-        pre_filter (callable, optional): A function that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a boolean
-            value, indicating whether the data object should be included in the
-            final dataset. (default: :obj:`None`)
-        
-        return: Pytroch geometric dataset
-    """
+   
     def __init__(self, root,dataset_name, dataset,transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name, self.dataset = root, dataset_name,dataset
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
         
     @property
@@ -478,44 +405,15 @@
 
         data, slices = self.collate(gender_dataset)
         print("saving path:",self.processed_paths[0])
         torch.save((data, slices), self.processed_paths[0])
 
 
 class Age_Dataset(InMemoryDataset):
-    r"""
-    Graph-based neuroimaging dataset,
-
-
-    Args:
-        root (str): Root directory where the dataset should be saved.
-
-        name (str): The `name
-            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-            dataset.
-
-        
-
-        dataset: Pyg dataset obtained from Brain_connectome_Rest class 
-
-        transform (callable, optional): A function/transform that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a transformed
-            version. The data object will be transformed before every access.
-            (default: :obj:`None`)
-        pre_transform (callable, optional): A function/transform that takes in
-            an :obj:`torch_geometric.data.Data` object and returns a
-            transformed version. The data object will be transformed before
-            being saved to disk. (default: :obj:`None`)
-        pre_filter (callable, optional): A function that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a boolean
-            value, indicating whether the data object should be included in the
-            final dataset. (default: :obj:`None`)
-        
-        return: Pytroch geometric dataset
-    """
+    
     def __init__(self, root,dataset_name, dataset,transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name, self.dataset = root, dataset_name,dataset
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
         
     @property
@@ -537,44 +435,15 @@
             age_dataset = [self.pre_transform(data) for data in age_dataset]
 
         data, slices = self.collate(age_dataset)
         print("saving path:",self.processed_paths[0])
         torch.save((data, slices), self.processed_paths[0])
 
 class WM_Dataset(InMemoryDataset):
-    r"""
-    Graph-based neuroimaging dataset,
-
-
-    Args:
-        root (str): Root directory where the dataset should be saved.
-
-        name (str): The `name
-            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-            dataset.
-
-        
-
-        dataset: Pyg dataset obtained from Brain_connectome_Rest class 
-
-        transform (callable, optional): A function/transform that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a transformed
-            version. The data object will be transformed before every access.
-            (default: :obj:`None`)
-        pre_transform (callable, optional): A function/transform that takes in
-            an :obj:`torch_geometric.data.Data` object and returns a
-            transformed version. The data object will be transformed before
-            being saved to disk. (default: :obj:`None`)
-        pre_filter (callable, optional): A function that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a boolean
-            value, indicating whether the data object should be included in the
-            final dataset. (default: :obj:`None`)
-        
-        return: Pytroch geometric dataset with working memory values  as labels
-        """
+    
     def __init__(self, root,dataset_name, dataset,transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name, self.dataset = root, dataset_name,dataset
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
         
 
@@ -600,44 +469,15 @@
             wm_dataset = [self.pre_transform(data) for data in wm_dataset]
 
         data, slices = self.collate(wm_dataset)
         print("saving path:",self.processed_paths[0])
         torch.save((data, slices), self.processed_paths[0])
 
 class FI_Dataset(InMemoryDataset):
-    r"""
-    Graph-based neuroimaging dataset,
-
-
-    Args:
-        root (str): Root directory where the dataset should be saved.
-
-        name (str): The `name
-            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-            dataset.
-
-        
-
-        dataset: Pyg dataset obtained from Brain_connectome_Rest class 
-
-        transform (callable, optional): A function/transform that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a transformed
-            version. The data object will be transformed before every access.
-            (default: :obj:`None`)
-        pre_transform (callable, optional): A function/transform that takes in
-            an :obj:`torch_geometric.data.Data` object and returns a
-            transformed version. The data object will be transformed before
-            being saved to disk. (default: :obj:`None`)
-        pre_filter (callable, optional): A function that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a boolean
-            value, indicating whether the data object should be included in the
-            final dataset. (default: :obj:`None`)
-        
-        return: Pytroch geometric dataset with Fluid Intelligence values as labels
-        """
+    
     def __init__(self, root,dataset_name, dataset,transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name, self.dataset = root, dataset_name,dataset
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
         
 
@@ -665,48 +505,15 @@
             fl_dataset = [self.pre_transform(data) for data in fl_dataset]
 
         data, slices = self.collate(fl_dataset)
         print("saving path:",self.processed_paths[0])
         torch.save((data, slices), self.processed_paths[0])
 
 class Brain_connectome_Activity(InMemoryDataset):
-    r"""
-    Graph-based neuroimaging benchmark datasets,
-
-
-    Args:
-        root (str): Root directory where the dataset should be saved.
-
-        name (str): The `name
-            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-            dataset.
-
-        rois (int): the number of ROIs to be used for parcellation. 
-        Options are: {100, 200, 300, 400, 500, 600, 700, 800, 900, 1000}
-
-        path_to_data: Path to the fMRI data.
-
-        n_jobs: the number of jobs to process the data in parallel.
-
-        transform (callable, optional): A function/transform that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a transformed
-            version. The data object will be transformed before every access.
-            (default: :obj:`None`)
-        pre_transform (callable, optional): A function/transform that takes in
-            an :obj:`torch_geometric.data.Data` object and returns a
-            transformed version. The data object will be transformed before
-            being saved to disk. (default: :obj:`None`)
-        pre_filter (callable, optional): A function that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a boolean
-            value, indicating whether the data object should be included in the
-            final dataset. (default: :obj:`None`)
-        
-        return: Pytroch geometric dataset with activity as class
-    """
-
+    
     def __init__(self, root, dataset_name,n_rois, threshold,path_to_data,n_jobs,transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name,self.n_rois,self.threshold,self.path_to_data,self.n_jobs = root, dataset_name,n_rois,threshold,path_to_data,n_jobs
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
 
     @property
@@ -834,47 +641,15 @@
 
         data, slices = self.collate(dataset)
         print("saving path:",self.processed_paths[0])
         torch.save((data, slices), self.processed_paths[0])
 
 
 class Brain_connectome_Rest_Download(InMemoryDataset):
-    r"""
-        Graph-based neuroimaging benchmark datasets crawling from HCP S3 bucket,
-
-
-        Args:
-            root (str): Root directory where the dataset should be saved.
-
-            name (str): The `name
-                <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-                dataset.
-
-            rois (int): the number of ROIs to be used for parcellation. 
-            Options are: {100, 200, 300, 400, 500, 600, 700, 800, 900, 1000}
-
-            path_to_data: Path where the data to be stored and processed.
-
-            n_jobs: the number of jobs to process the data in parallel.
-
-            transform (callable, optional): A function/transform that takes in an
-                :obj:`torch_geometric.data.Data` object and returns a transformed
-                version. The data object will be transformed before every access.
-                (default: :obj:`None`)
-            pre_transform (callable, optional): A function/transform that takes in
-                an :obj:`torch_geometric.data.Data` object and returns a
-                transformed version. The data object will be transformed before
-                being saved to disk. (default: :obj:`None`)
-            pre_filter (callable, optional): A function that takes in an
-                :obj:`torch_geometric.data.Data` object and returns a boolean
-                value, indicating whether the data object should be included in the
-                final dataset. (default: :obj:`None`)
-            
-            return: Pytroch geometric dataset with four classes: [0] - gender, [1]-age, [2]- working memory and [3] -fluid intelligence 
-        """
+    
     def __init__(self, root,name,n_rois, threshold,path_to_data,n_jobs,s3, transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name,self.n_rois,self.threshold,self.target_path,self.n_jobs,self.s3 = root, name,n_rois,threshold,path_to_data,n_jobs,s3
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
 
 
@@ -997,48 +772,15 @@
 
         data, slices = self.collate(dataset)
         print("saving path:",self.processed_paths[0])
         torch.save((data, slices), self.processed_paths[0])
 
 
 class Brain_connectome_Activity_Download(InMemoryDataset):
-    r"""
-    Graph-based neuroimaging benchmark datasets,
-
-
-    Args:
-        root (str): Root directory where the dataset should be saved.
-
-        name (str): The `name
-            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
-            dataset.
-
-        rois (int): the number of ROIs to be used for parcellation. 
-        Options are: {100, 200, 300, 400, 500, 600, 700, 800, 900, 1000}
-
-        path_to_data: Path to the fMRI data.
-
-        n_jobs: the number of jobs to process the data in parallel.
-
-        transform (callable, optional): A function/transform that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a transformed
-            version. The data object will be transformed before every access.
-            (default: :obj:`None`)
-        pre_transform (callable, optional): A function/transform that takes in
-            an :obj:`torch_geometric.data.Data` object and returns a
-            transformed version. The data object will be transformed before
-            being saved to disk. (default: :obj:`None`)
-        pre_filter (callable, optional): A function that takes in an
-            :obj:`torch_geometric.data.Data` object and returns a boolean
-            value, indicating whether the data object should be included in the
-            final dataset. (default: :obj:`None`)
-        
-        return: Pytroch geometric dataset with activity as class
-    """
-
+    
     def __init__(self, root, dataset_name,n_rois, threshold,path_to_data,n_jobs,s3,transform=None, pre_transform=None, pre_filter=None):
         self.root, self.dataset_name,self.n_rois,self.threshold,self.target_path,self.n_jobs,self.s3 = root, dataset_name,n_rois,threshold,path_to_data,n_jobs,s3
         super().__init__(root, transform, pre_transform, pre_filter)
         
         self.data, self.slices = torch.load(self.processed_paths[0])
 
     @property
```

### Comparing `NeuroGraph-1.0.2/NeuroGraph.egg-info/PKG-INFO` & `NeuroGraph-1.1.2/NeuroGraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroGraph
-Version: 1.0.2
+Version: 1.1.2
 Summary: A Python package for graph-based Neuroimaging benchmarks and tools
 Author: Anwar Said
 Author-email: <anwar.said@vanderbilt.edu>
 Keywords: python,neuroimaging,graph machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuroGraph-1.0.2/PKG-INFO` & `NeuroGraph-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroGraph
-Version: 1.0.2
+Version: 1.1.2
 Summary: A Python package for graph-based Neuroimaging benchmarks and tools
 Author: Anwar Said
 Author-email: <anwar.said@vanderbilt.edu>
 Keywords: python,neuroimaging,graph machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NeuroGraph-1.0.2/setup.py` & `NeuroGraph-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='NeuroGraph',
-    version='1.0.2',
+    version='1.1.2',
     description='A Python package for graph-based Neuroimaging benchmarks and tools',
     author='Anwar Said',
     author_email='<anwar.said@vanderbilt.edu>',
     packages=['NeuroGraph'],
     install_requires=[
         # List any dependencies your package requires
         'boto3==1.26.158',
```

