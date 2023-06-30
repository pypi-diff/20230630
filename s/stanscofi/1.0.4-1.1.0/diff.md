# Comparing `tmp/stanscofi-1.0.4.tar.gz` & `tmp/stanscofi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stanscofi-1.0.4.tar", last modified: Wed Jun 21 16:53:37 2023, max compression
+gzip compressed data, was "stanscofi-1.1.0.tar", last modified: Fri Jun 30 16:51:54 2023, max compression
```

## Comparing `stanscofi-1.0.4.tar` & `stanscofi-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:37.316577 stanscofi-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-21 16:53:37.316577 stanscofi-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-21 16:53:27.000000 stanscofi-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 16:53:27.000000 stanscofi-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:53:37.316577 stanscofi-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-21 16:53:27.000000 stanscofi-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:37.316577 stanscofi-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:37.316577 stanscofi-1.0.4/src/stanscofi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/training_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-21 16:53:27.000000 stanscofi-1.0.4/src/stanscofi/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:53:37.316577 stanscofi-1.0.4/src/stanscofi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 16:53:37.000000 stanscofi-1.0.4/src/stanscofi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:54.115854 stanscofi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-30 16:51:54.115854 stanscofi-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-30 16:51:43.000000 stanscofi-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 16:51:43.000000 stanscofi-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:51:54.115854 stanscofi-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 16:51:44.000000 stanscofi-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:54.111854 stanscofi-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:54.115854 stanscofi-1.1.0/src/stanscofi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27734 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19202 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19399 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/training_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-06-30 16:51:43.000000 stanscofi-1.1.0/src/stanscofi/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:51:54.115854 stanscofi-1.1.0/src/stanscofi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 16:51:54.000000 stanscofi-1.1.0/src/stanscofi.egg-info/top_level.txt
```

### Comparing `stanscofi-1.0.4/PKG-INFO` & `stanscofi-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanscofi
-Version: 1.0.4
+Version: 1.1.0
 Summary: Package for STANdard drug Screening by COllaborative FIltering. Performs benchmarks against datasets and SotA algorithms, and implements training, validation and testing procedures.
 Home-page: https://github.com/RECeSS-EU-Project/stanscofi
 Author: Clémence Réda
 Author-email: recess-project@proton.me
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -14,15 +14,15 @@
 
 ![funding logo](https://raw.githubusercontent.com/RECeSS-EU-Project/RECeSS-EU-Project.github.io/main/assets/images/header%2BEU_rescale.jpg)
 
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
-[![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![PyPI version](https://badge.fury.io/py/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847)
+[![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10-pink)](https://badge.fury.io/py/stanscofi) [![PyPI version](https://img.shields.io/pypi/v/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847) ![GitHub](https://img.shields.io/github/license/recess-eu-project/stanscofi.svg) [![Build Status](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml/badge.svg)](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml) [![Codecov](https://codecov.io/github/recess-eu-project/stanscofi/coverage.svg?branch=master)](https://codecov.io/github/recess-eu-project/stanscofi?branch=master) [![Codefactor](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi/badge?style=plastic)](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi)
 
 ## Statement of need 
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
```

### Comparing `stanscofi-1.0.4/README.md` & `stanscofi-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![funding logo](https://raw.githubusercontent.com/RECeSS-EU-Project/RECeSS-EU-Project.github.io/main/assets/images/header%2BEU_rescale.jpg)
 
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
-[![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![PyPI version](https://badge.fury.io/py/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847)
+[![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10-pink)](https://badge.fury.io/py/stanscofi) [![PyPI version](https://img.shields.io/pypi/v/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847) ![GitHub](https://img.shields.io/github/license/recess-eu-project/stanscofi.svg) [![Build Status](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml/badge.svg)](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml) [![Codecov](https://codecov.io/github/recess-eu-project/stanscofi/coverage.svg?branch=master)](https://codecov.io/github/recess-eu-project/stanscofi?branch=master) [![Codefactor](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi/badge?style=plastic)](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi)
 
 ## Statement of need 
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
```

### Comparing `stanscofi-1.0.4/setup.py` & `stanscofi-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "stanscofi"
-VERSION = "1.0.4"
+VERSION = "1.1.0"
 
 setup(name=NAME,
     version=VERSION,
     author="Clémence Réda",
     author_email="recess-project@proton.me",
     url="https://github.com/RECeSS-EU-Project/stanscofi",
     license_files = ('LICENSE'),
@@ -29,10 +29,11 @@
         "scipy>=1.5.4",
         "matplotlib>=3.3.2",
         "threadpoolctl>=3.1.0",
         "joblib>=1.0.1",
         "tqdm>=4.58.0",
         "codecarbon>=2.2.2",
         "seaborn>=0.11.0",
+        "umap-learn>=0.5.3",
     ],
     entry_points={},
 )
```

### Comparing `stanscofi-1.0.4/src/stanscofi/datasets.py` & `stanscofi-1.1.0/src/stanscofi/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import numpy as np
 import seaborn as sns
 
 import matplotlib.pyplot as plt
 import matplotlib.lines as mlines
 
 from sklearn.decomposition import PCA
-from sklearn.manifold import TSNE
-from sklearn.preprocessing import StandardScaler
+import warnings
+with warnings.catch_warnings():
+    warnings.filterwarnings("ignore", message=".*he 'nopython' keyword argument was not supplied to the 'numba.jit' decorator.*")
+    import umap
 
 import stanscofi.utils
 import stanscofi.preprocessing
 
 def generate_dummy_dataset(npositive, nnegative, nfeatures, mean, std, random_state=12454):
     '''
     Creates a dummy dataset where the positive and negative (item, user) pairs are arbitrarily similar. 
@@ -83,14 +85,16 @@
         a list of the item feature names in the order of column indices in ratings_mat
     items : array-like of shape (n_user_features, n_users)
         a list of the item feature names in the order of column indices in ratings_mat
     same_item_user_features : bool
         a list of the item feature names in the order of column indices in ratings_mat
     name : str
         the name of the dataset (if it exists)
+    folds : array-like of shape (n_ratings, 3)
+        a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3) (if the dataset is masked, see below)
 
     Attributes
     ----------
     name : str
         the name of the dataset (if it exists)
     ratings_mat : array-like of shape (n_items, n_users)
         a matrix which contains values in {-1, 0, 1} describing the known and unknown user-item matchings
@@ -117,16 +121,18 @@
         Initialize the Dataset object and creates all attributes
     summary(sep="-"*70)
         Prints out the characteristics of the drug repurposing dataset
     visualize(withzeros=False, X=None, y=None, figsize=(5,5), fontsize=20, dimred_args={}, predictions=None, use_ratings=False, random_state=1234, show_errors=False, verbose=False)
         Plots datapoints in the dataset annotated by the ground truth or predicted ratings
     get_folds(folds, subset_name="subset")
         Creates a subset of the dataset based on the folds given as input
+    mask_dataset(folds, subset_name="dataset")
+        Creates a masked dataset where only some of the ratings are known
     '''
-    def __init__(self, ratings_mat=None, users=None, items=None, same_item_user_features=False, name="dataset"):
+    def __init__(self, ratings_mat=None, users=None, items=None, same_item_user_features=False, name="dataset", folds=None):
         '''
         Creates an instance of stanscofi.Dataset
 
         ...
 
         Parameters
         ----------
@@ -164,14 +170,15 @@
         assert all([a in items.columns for a in self.ratings[:,1]])
         self.ratings[:,0] = [self.user_list.index(x) for x in self.ratings[:,0]] 
         self.ratings[:,1] = [self.item_list.index(x) for x in self.ratings[:,1]] 
         self.users = users.values
         self.items = items.values
         self.name = name
         self.same_item_user_features = same_item_user_features
+        self.folds = folds
 
     def summary(self, sep="-"*70):
         '''
         Prints out a summary of the contents of a stanscofi.Dataset: the number of items, users, the number of positive, negative, unknown matchings, the sparsity number, and the shape and percentage of missing values in the item and user feature matrices
 
         ...
 
@@ -199,15 +206,15 @@
             print("Total #Diseases: %d\t#Disease features: %d\tPerc. Missing features: %d" % (self.users.shape[1], self.users.shape[0], np.sum(np.isnan(self.users))*100/(self.users.shape[0]*self.users.shape[1])))
         if (self.users.shape[0]+self.items.shape[0]==0):
             print("No feature matrices.")
         print(sep+"\n")
 
     def visualize(self, withzeros=False, X=None, y=None, metric="euclidean", figsize=(5,5), fontsize=20, dimred_args={}, predictions=None, use_ratings=False, random_state=1234, show_errors=False, verbose=False):
         '''
-        Plots a representation of the datapoints in a stanscofi.Dataset which is annotated either by the ground truth labels or the predicted labels. The representation is the plot of the datapoints according to the first two Principal Components, or the first two dimensions in tSNE, if the feature matrices can be converted into a (n_ratings, n_features) shaped matrix where n_features>1, else it plots a heatmap with the values in the matrix for each rating pair. 
+        Plots a representation of the datapoints in a stanscofi.Dataset which is annotated either by the ground truth labels or the predicted labels. The representation is the plot of the datapoints according to the first two Principal Components, or the first two dimensions in UMAP, if the feature matrices can be converted into a (n_ratings, n_features) shaped matrix where n_features>1, else it plots a heatmap with the values in the matrix for each rating pair. 
 
         In the legend, ground truth labels are denoted with brackets: e.g., [0] (unknown), [1] (positive) and [-1] (negative); predicted ratings are denoted by "pos" (positive) and "neg" (negative); correct (resp., incorrect) predictions are denoted by "correct", resp. "error"
 
         ...
 
         Parameters
         ----------
@@ -220,15 +227,15 @@
         metric : str
             metric to consider to perform hierarchical clustering on the dataset. Should belong to [‘cityblock’, ‘cosine’, ‘euclidean’, ‘l1’, ‘l2’, ‘manhattan’, ‘braycurtis’, ‘canberra’, ‘chebyshev’, ‘correlation’, ‘dice’, ‘hamming’, ‘jaccard’, ‘kulsinski’, ‘mahalanobis’, ‘minkowski’, ‘rogerstanimoto’, ‘russellrao’, ‘seuclidean’, ‘sokalmichener’, ‘sokalsneath’, ‘sqeuclidean’, ‘yule’]
         figsize : tuple of size 2
             width and height of the figure
         fontsize : int
             size of the legend, title and labels of the figure
         dimred_args : dict
-            dictionary which lists the parameters to the dimensionality reduction method (either PCA, by default, or tSNE, if parameter "perplexity" is provided)
+            dictionary which lists the parameters to the dimensionality reduction method (either PCA, by default, or UMAP, if parameter "n_neighbors" is provided)
         predictions : array-like of shape (n_ratings, 3) or None
             a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3); if predictions=None, then the ground truth ratings will be used to color datapoints, otherwise, the predicted ratings will be used
         use_ratings : bool
             if set to True, use the ratings in the dataset as predictions (for debugging purposes)
         random_state : int
             random seed
         show_errors : bool
@@ -295,35 +302,37 @@
                 ## item i, user u, rating r, scatter style (color + marker shape)
                 all_pairs = np.concatenate((all_pairs[:,[0,1,3]],values), axis=1, dtype=object)
                 assert all_pairs.shape[1]==4 and all_pairs.shape[0]==X.shape[0]
         all_pairs[:,:-1] = all_pairs[:,:-1].astype(int)
         if (verbose):
             print("<datasets.visualize> Reducing dimension and plotting matrix X of size %d x %d" % X.shape)
         dimred_args.update({"n_components":min(2,X.shape[1]), "random_state":random_state})
-        use_pca = ("perplexity" not in dimred_args)
+        use_pca = ("n_neighbors" not in dimred_args)
         if (use_pca):
             with np.errstate(invalid="ignore"): # for NaN or 0 variance matrices
                 pca = PCA(**dimred_args)
                 dimred_X = pca.fit_transform(X)
                 var12 = pca.explained_variance_ratio_[:2]*100
         else:
-            dimred_args.update({"perplexity":max(5,min(dimred_args["perplexity"],min(30,all_pairs.shape[0])))})
+            dimred_args.update({"n_neighbors":max(5,min(dimred_args["n_neighbors"],min(50,all_pairs.shape[0])))})
+            dimred_args.update({"min_dist":max(0.5,min(dimred_args.get("min_dist", 0.1), 0.001))})
+            dimred_args.update({"metric":dimred_args.get("metric", 'correlation')})
             if (verbose):
-                print("<datasets.visualize> Perplexity = %d" % dimred_args["perplexity"])
+                print("<datasets.visualize> n_neighbors = %d\tmin_dist = %.2f\tmetric = %s" % (dimred_args["n_neighbors"], dimred_args["min_dist"], dimred_args["metric"]))
             with np.errstate(invalid="ignore"): # for NaN or 0 variance matrices
-                tsne = TSNE(**dimred_args)
-                dimred_X = tsne.fit_transform(X-np.min(X)+1)
-                var12 = tsne.kl_divergence_
+                umap_model = umap.UMAP(**dimred_args)
+                dimred_X = umap_model.fit_transform(X, y)
+                var12 = [np.nan]*2
         ## Put points in the front layer
         layer = {"g.": 1, "r.": 1, "y.": 0} if (predictions is None) else ({"g.": 0, "r.": 0, "y.": 0, "g+": 0, "r+": 1, "y+": 0, "gv": 0, "rv": 0, "yv": 0} if (not show_errors) else {"g.": 0, "r.": 0, "y.": 0, "g+": 0, "r+": 1, "y+": 0, "gv": 1, "rv": 0, "yv": 0})
         ## More visible points
         alpha = {"g.": 0.75, "r.": 1, "y.": 0.1}
         plt.figure(figsize=figsize)
         if (X.shape[1]>1):
-            ## Prints a PCA
+            ## Prints a PCA / UMAP
             for mkr in np.unique(np.ravel(all_pairs[:,3])).tolist():
                 all_pairs_k = np.argwhere(all_pairs[:,3]==mkr)[:,0].tolist()
                 if ((not withzeros) and (((predictions is None) and (mkr=="y.")) or ((predictions is not None) and (mkr[-1]==".")))):
                     plt.scatter(dimred_X[all_pairs_k,0], dimred_X[all_pairs_k,1], c="w", marker=".", zorder=0, alpha=0)
                 else:
                     plt.scatter(dimred_X[all_pairs_k,0], dimred_X[all_pairs_k,1], c=mkr[0], marker=mkr[1], zorder=layer[mkr], alpha=alpha[mkr] if (predictions is None) else (0.8 if (not show_errors) else 1))
             if (show_errors):
@@ -341,15 +350,15 @@
                     handles = [mlines.Line2D([], [], color={'r':'red','g':'green','y':'yellow'}[k[0]], 
                         label={'r':'neg','g':"pos", 'y':'unl'}[k[0]]+" "+{".": "[ 0]", "+": "[ 1]", "v": "[-1]"}[k[1]],
 		        marker=k[1] if (predictions is not None) else '.', markersize=fontsize,
 		        ) for k in np.unique(np.asarray(all_pairs[:,-1], dtype=str)).tolist() if (withzeros or k[0]!="y")]
             plt.xticks(fontsize=fontsize, rotation=90)
             plt.yticks(fontsize=fontsize)
             plt.ylabel(("PC2 ("+str(int(var12[1]))+"%)" if (use_pca) else "Dim2") if (not np.isnan(var12[1])) else "C2", fontsize=fontsize)
-            plt.xlabel((("PC1 ("+str(int(var12[0]))+"%)" if (use_pca) else "Dim1 (KL div=%.2f)" % var12)) if (not np.isnan(var12[0] if (use_pca) else var12)) else "C1", fontsize=fontsize)
+            plt.xlabel((("PC1 ("+str(int(var12[0]))+"%)" if (use_pca) else "Dim1")) if (not np.isnan(var12[0])) else "C1", fontsize=fontsize)
             plt.title("on %d features" % X.shape[1], fontsize=fontsize//2)
             plt.legend(handles=handles, fontsize=fontsize, loc='upper right', bbox_to_anchor=(1.6,0.9))
             plt.show()
         elif ((dimred_X!=0).any()):
             ## Prints a heatmap according to values in X
             X_heatmap = X.reshape(self.ratings_mat.shape)
             annot = self.ratings_mat.copy().astype(str)
@@ -374,15 +383,15 @@
         Obtains a subset of a stanscofi.Dataset based on a set of user and item indices
 
         ...
 
         Parameters
         ----------
         folds : array-like of shape (n_ratings, 3)
-            a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3)
+            a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3). /!\ the ratings in the last column overrides values in dataset.ratings_mat
         subset_name : str
             name of the newly created stanscofi.Dataset
 
         Returns
         subset : stanscofi.Dataset
             dataset corresponding to the folds in input
         ----------
@@ -399,8 +408,40 @@
         user_lst = np.unique(folds[:,0]).tolist() ## order of unique
         item_lst = np.unique(folds[:,1]).tolist() ## order of unique
         A = stanscofi.utils.ratings2matrix(ratings, user_col="user", item_col="item", rating_col="rating")
         P = pd.DataFrame(self.users[:,user_lst], index=self.user_features, 
                 columns=[self.user_list[i] for i in user_lst])
         S = pd.DataFrame(self.items[:,item_lst], index=self.item_features, 
                 columns=[self.item_list[i] for i in item_lst])
-        return Dataset(A, P, S, name=subset_name, same_item_user_features=self.same_item_user_features)
+        return Dataset(A, P, S, name=subset_name, same_item_user_features=self.same_item_user_features)
+
+    def mask_dataset(self, folds, subset_name="dataset"):
+        '''
+        Obtains a copy of a stanscofi.Dataset based on a set of user and item indices where some values in the initial ratings matrix are masked with 0's. Contrary to get_folds, the shapes of the user and item feature matrices are preserved, as well as ratings_mat. Some values (not in folds) are masked with 0's in the ratings_mat matrix.
+
+        ...
+
+        Parameters
+        ----------
+        folds : array-like of shape (n_ratings, 3)
+            a matrix which contains the user indices (column 1), the item indices (column 2) and the class for the corresponding (user, item) pair (value in {-1, 0, 1} in column 3). /!\ the ratings in the last column DO NOT override values in dataset.ratings_mat
+        subset_name : str
+            name of the newly created stanscofi.Dataset
+
+        Returns
+        subset : stanscofi.Dataset
+            dataset where ratings values outside of the folds in input are masked
+        ----------
+        '''
+        if (len(folds)==0):
+            raise ValueError("Fold is empty!")
+        assert folds.shape[1]==3
+        assert np.max(folds[:,0])<=self.ratings_mat.shape[1]
+        assert np.max(folds[:,1])<=self.ratings_mat.shape[0]
+        assert ((folds[:,-1]==1)|(folds[:,-1]==-1)|(folds[:,-1]==0)).all()
+        P = pd.DataFrame(self.users, index=self.user_features, columns=self.user_list)
+        S = pd.DataFrame(self.items, index=self.item_features, columns=self.item_list)
+        A = pd.DataFrame(self.ratings_mat, index=self.item_list, columns=self.user_list)
+        y = np.zeros(self.ratings_mat.shape)
+        y[folds[:,1],folds[:,0]] = folds[:,2]
+        y = pd.DataFrame(y, index=A.index, columns=A.columns)
+        return Dataset(ratings_mat=y, users=P, items=S, name=subset_name, same_item_user_features=self.same_item_user_features, folds=folds)
```

### Comparing `stanscofi-1.0.4/src/stanscofi/models.py` & `stanscofi-1.1.0/src/stanscofi/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,71 @@
     grid = np.argwhere(np.ones(df.shape))
     res_df = pd.DataFrame([], index=range(grid.shape[0]))
     res_df[user_col] = [df.columns[x] for x in list(grid[:, 1].flatten())]
     res_df[item_col] = [df.index[x] for x in list(grid[:, 0].flatten())]
     res_df[rating_col] = [df.values[i,j] for i,j in grid.tolist()]
     return res_df[[user_col, item_col, rating_col]]
 
+def create_scores(preds, dataset):
+    '''
+    Converts a score vector or a score value into a list of scores
+
+    ...
+
+    Parameters
+    ----------
+    preds : int or float or array-like of shape (n_ratings, )
+        the matrix of scores
+    dataset : stanscofi.datasets.Dataset
+        dataset to apply the scores to
+
+    Returns
+    ----------
+    scores : array-like of shape (n_ratings, 3)
+        the list of scores where the first column correspond to users, second to items, third to scores
+    '''
+    assert str(type(preds)) in ["<class 'float'>", "<class 'int'>"] or len(preds.shape)==1 or preds.shape[1]==1
+    ids = np.argwhere(np.ones(dataset.ratings_mat.shape))
+    assert str(type(preds)) in ["<class 'float'>", "<class 'int'>"] or preds.shape[0]==ids.shape[0]
+    scores = np.zeros((ids.shape[0], 3))
+    scores[:,0] = ids[:,1] 
+    scores[:,1] = ids[:,0] 
+    scores[:,2] = np.ravel(preds)
+    return scores
+
+def create_overscores(preds, dataset):
+    '''
+    Converts a sublist of scores into a list of scores on the full dataset
+
+    ...
+
+    Parameters
+    ----------
+    preds : array-like of shape (n_ratings, 3)
+        the list of scores where the first column correspond to users, second to items, third to scores, where ratings are a subset of all possible ratings in the input dataset
+    dataset : stanscofi.datasets.Dataset
+        over-dataset which was used
+
+    Returns
+    ----------
+    scores : array-like of shape (n_ratings, 3)
+        the list of scores where the first column correspond to users, second to items, third to scores on all possible pairs in the dataset
+    '''
+    assert preds.shape[1]==3
+    assert np.max(preds[:,0])<=np.max(dataset.ratings_mat.shape[1])
+    assert np.max(preds[:,1])<=np.max(dataset.ratings_mat.shape[0])
+    ids = np.argwhere(np.ones(dataset.ratings_mat.shape))
+    scores = np.zeros((ids.shape[0], 3))
+    scores[:,0] = ids[:,1]
+    scores[:,1] = ids[:,0]
+    in_preds = [((preds[:,0]==i)&(preds[:,1]==j)).any() for i,j in ids[:,:2].tolist()]
+    assert sum(in_preds)==preds.shape[0]
+    scores[in_preds,2] = preds[:,2]
+    return scores
+
 ###############################################################################################################
 ###################
 # Basic model     #
 ###################
 
 class BasicModel(object):
     '''
@@ -431,32 +488,16 @@
         Returns
         ----------
         X : array-like of shape (n_ratings, n_pair_features)
             (user, item) feature matrix (the actual contents of the matrix depends on parameters "preprocessing" and "subset" given as input
         y : array-like of shape (n_ratings, )
             response vector for each (user, item) pair
         '''
-        if (self.preprocessing_str == "Perlman_procedure"):
-            X, y = eval("stanscofi.preprocessing."+self.preprocessing_str)(dataset, njobs=1, sep_feature="-", missing=-666, verbose=False)
-            scalerS, scalerP = None, None
-        if (self.preprocessing_str == "meanimputation_standardize"):
-            X, y, scalerS, scalerP = eval("stanscofi.preprocessing."+self.preprocessing_str)(dataset, subset=self.subset, scalerS=self.scalerS, scalerP=self.scalerP, inf=2, verbose=False)
-        if (self.preprocessing_str == "same_feature_preprocessing"):
-            X, y = eval("stanscofi.preprocessing."+self.preprocessing_str)(dataset)
-            scalerS, scalerP = None, None
-        if (self.preprocessing_str != "meanimputation_standardize"):
-            if ((self.subset is not None) or (self.filter is not None)):
-                if ((self.subset is not None) and (self.filter is None)):
-                    with np.errstate(over="ignore"):
-                        x_vars = [np.nanvar(X[:,i]) if (np.sum(~np.isnan(X[:,i]))>0) else 0 for i in range(X.shape[1])]
-                        x_vars = [x if (not np.isnan(x) and not np.isinf(x)) else 0 for x in x_vars]
-                        x_ids_vars = np.argsort(x_vars).tolist()
-                        features = x_ids_vars[-self.subset:]
-                        self.filter = features
-                X = X[:,self.filter]
+        X, y, scalerS, scalerP, filter_ = stanscofi.preprocessing.preprocessing_routine(dataset, self.preprocessing_str, subset_=self.subset, filter_=self.filter, scalerS=self.scalerS, scalerP=self.scalerP, inf=2, njobs=1)
+        self.filter = filter_
         self.scalerS = scalerS
         self.scalerP = scalerP
         return X, y
     
     def fit(self, train_dataset):
         '''
         Fitting the Logistic Regression model on the training dataset.
@@ -479,14 +520,10 @@
 
         Parameters
         ----------
         test_dataset : stanscofi.Dataset
             testing dataset on which the model should be validated
         '''
         X, _ = self.preprocessing(test_dataset)
-        preds = self.model.predict_proba(X)
-        ids = np.argwhere(np.ones(test_dataset.ratings_mat.shape))
-        predicted_ratings = np.zeros((X.shape[0], 3))
-        predicted_ratings[:,0] = ids[:X.shape[0],1] 
-        predicted_ratings[:,1] = ids[:X.shape[0],0] 
-        predicted_ratings[:,2] = preds.max(axis=1)
-        return predicted_ratings
+        preds = self.model.predict_proba(X).max(axis=1)
+        scores = create_scores(preds, test_dataset)
+        return scores
```

### Comparing `stanscofi-1.0.4/src/stanscofi/preprocessing.py` & `stanscofi-1.1.0/src/stanscofi/preprocessing.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,74 @@
 
 from joblib import Parallel, delayed
 from tqdm import tqdm
 
 from sklearn.preprocessing import StandardScaler
 from sklearn.impute import SimpleImputer
 
+def preprocessing_routine(dataset, preprocessing_str, subset_=None, filter_=None, scalerS=None, scalerP=None, inf=2, njobs=1):
+    '''
+    Converts a score vector or a score value into a list of scores
+
+    ...
+
+    Parameters
+    ----------
+    dataset : stanscofi.datasets.Dataset
+        dataset to preprocess
+    preprocessing_str : str
+        type of preprocessing: in ["Perlman_procedure","meanimputation_standardize","same_feature_preprocessing"]. see notebook for further details
+    subset_ : None or int
+        Number of features to restrict the dataset to (Top-subset_ features in terms of cross-sample variance) /!\ across user and item features if preprocessing_str!="meanimputation_standardize" otherwise 2*subset_ features are preserved (subset_ for item features, subset_ for user features)
+    filter_ : None or list
+        list of feature indices to keep (of length subset_) (overrides the subset_ parameter if both are fed)
+    scalerS : None or stanscofi.models.CustomScaler instance
+        scaler for items; the scaler fitted on item feature vectors
+    scalerP : None or stanscofi.models.CustomScaler instance
+        scaler for users; the scaler fitted on user feature vectors
+    inf : float or int
+        placeholder value for infinity values (positive : +inf, negative : -inf)
+    njobs : int
+        number of jobs to run in parallel (njobs > 0) for the Perlman procedure
+
+    Returns
+    ----------
+    X : array-like of shape (n_items x n_users, n_item_features+n_user_features)
+        the feature matrix
+    y : array-like of shape (n_items x n_users, )
+        the response/outcome vector
+    scalerS : None or stanscofi.models.CustomScaler instance
+        scaler for items; if the input value was None, returns the scaler fitted on item feature vectors
+    scalerP : None or stanscofi.models.CustomScaler instance
+        scaler for users; if the input value was None, returns the scaler fitted on user feature vectors
+    filter_ : None or list
+        list of feature indices to keep (of length subset_)
+    '''
+    assert njobs>0
+    assert preprocessing_str in ["Perlman_procedure","meanimputation_standardize","same_feature_preprocessing"]
+    if (preprocessing_str == "Perlman_procedure"):
+        X, y = eval(preprocessing_str)(dataset, njobs=njobs, sep_feature="-", missing=-666, verbose=False)
+        scalerS, scalerP = None, None
+    if (preprocessing_str == "meanimputation_standardize"):
+        X, y, scalerS, scalerP = eval(preprocessing_str)(dataset, subset=subset_, scalerS=scalerS, scalerP=scalerP, inf=inf, verbose=False)
+    if (preprocessing_str == "same_feature_preprocessing"):
+        X, y = eval(preprocessing_str)(dataset)
+        scalerS, scalerP = None, None
+    if (preprocessing_str != "meanimputation_standardize"):
+        if ((subset_ is not None) or (filter_ is not None)):
+            if ((subset_ is not None) and (filter_ is None)):
+                with np.errstate(over="ignore"):
+                    x_vars = [np.nanvar(X[:,i]) if (np.sum(~np.isnan(X[:,i]))>0) else 0 for i in range(X.shape[1])]
+                    x_vars = [x if (not np.isnan(x) and not np.isinf(x)) else 0 for x in x_vars]
+                    x_ids_vars = np.argsort(x_vars).tolist()
+                    features = x_ids_vars[-subset_:]
+                    filter_ = features
+            X = X[:,filter_]
+    return X, y, scalerS, scalerP, filter_
+
 class CustomScaler(object):
     '''
     A class used to encode a simple preprocessing pipeline for feature matrices. Does mean imputation for features, feature filtering, correction of infinity errors and standardization
 
     ...
 
     Parameters
```

### Comparing `stanscofi-1.0.4/src/stanscofi/training_testing.py` & `stanscofi-1.1.0/src/stanscofi/training_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
     return train_set.astype(int), test_set.astype(int), val1_set.astype(int), val2_set.astype(int)
 
 ##############################
 # Common training procedure  #
 ##############################
 
-def cv_training(template, params, train_dataset, metric="AUC", beta=1, njobs=1, nsplits=5, random_state=1234, show_plots=True, verbose=False):
+def cv_training(template, params, train_dataset, is_masked=False, metric="AUC", beta=1, njobs=1, nsplits=5, random_state=1234, show_plots=True, verbose=False):
     '''
     Trains a model on a dataset using cross-validation using sklearn.model_selection.StratifiedKFold
 
     ...
 
     Parameters
     ----------
@@ -257,16 +257,20 @@
     full_list = full_list.astype(int)
     cv_folds = cv_generator.split(full_list[:,:2], np.ravel(full_list[:,2]))
     best_estimator, best_metric = {}, -float("inf")
     def single_run(ncv, tfolds, sfolds, full_list):
         if (verbose):
             print("Crossvalidation step #%d/%d" % (ncv+1,nsplits))
         model = template(params)
-        tdataset = train_dataset.get_folds(full_list[tfolds,:])
-        sdataset = train_dataset.get_folds(full_list[sfolds,:])
+        if (is_masked):
+            tdataset = train_dataset.mask_dataset(full_list[tfolds,:])
+            sdataset = train_dataset.mask_dataset(full_list[sfolds,:])            
+        else:
+            tdataset = train_dataset.get_folds(full_list[tfolds,:])
+            sdataset = train_dataset.get_folds(full_list[sfolds,:])
         model.fit(tdataset)
         scores_train = model.predict(tdataset)
         predictions_train = model.classify(scores_train)
         metrics_train, _ = stanscofi.validation.compute_metrics(scores_train, predictions_train, tdataset, beta=beta, verbose=verbose)
         scores_test = model.predict(sdataset)
         predictions_test = model.classify(scores_test)
         metrics_test, plot_args = stanscofi.validation.compute_metrics(scores_test, predictions_test, sdataset, beta=beta, verbose=verbose)
@@ -282,15 +286,15 @@
     best_metric = metric_test[best_id]
     best_train_metric = metrics_list[best_id][0]
     best_model = metrics_list[best_id][3]
     best_folds = [full_list[ids,:] for ids in metrics_list[best_id][2]]
     best_estimator = {"test_"+metric: best_metric, "train_"+metric: best_train_metric, "model_params": best_model, "cv_folds": best_folds}
     return best_estimator
 
-def grid_search(search_params, template, params, train_dataset, metric="AUC", njobs=1, nsplits=5, random_state=1234, show_plots=True, verbose=False):
+def grid_search(search_params, template, params, train_dataset, is_masked=False, metric="AUC", njobs=1, nsplits=5, random_state=1234, show_plots=True, verbose=False):
     '''
     Grid-search over hyperparameters, iteratively optimizing over one parameter at a time, and internally calling cv_training.
 
     ...
 
     Parameters
     ----------
@@ -334,15 +338,15 @@
     '''
     best_params, best_model, best_metric = {}, None, -float("inf")
     for param in search_params:
         for param_val in search_params[param]:
             params_ = params.copy()
             params_.update(best_params)
             params_.update({param: param_val})
-            best_estimator = cv_training(template, params_, train_dataset, metric=metric, njobs=njobs, nsplits=nsplits, random_state=random_state, show_plots=show_plots, verbose=verbose)
+            best_estimator = cv_training(template, params_, train_dataset, is_masked=is_masked, metric=metric, njobs=njobs, nsplits=nsplits, random_state=random_state, show_plots=show_plots, verbose=verbose)
             if (verbose):
                 print("<training_testing.grid_search> [%s=%s] %s on Test %f (Train %f)" % (param, str(param_val), metric, best_estimator["test_"+metric], best_estimator["train_"+metric]))
             if (best_estimator["test_"+metric]>best_metric):
                 best_params.update(params_)
                 best_model = deepcopy(best_estimator)
                 best_metric = best_estimator["test_"+metric]
     return best_params, best_model
```

### Comparing `stanscofi-1.0.4/src/stanscofi/utils.py` & `stanscofi-1.1.0/src/stanscofi/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         the path to the folder where dataset-related files are or will be stored
 
     Returns
     -------
     dataset_di : dictionary
         a dictionary where key "ratings_mat" contains the drug-disease matching pandas.DataFrame of shape (n_drugs, n_diseases) (where missing values are denoted by 0), key "users" correspond to the disease pandas.DataFrame of shape (n_disease_features, n_diseases), and "items" correspond to the drug feature pandas.DataFrame of shape (n_drug_features, n_drugs)
     '''
-    assert model_name in ["Gottlieb", "Cdataset_Aonly", "indep", "Fdataset", "DNdataset", "Cdataset", "TRANSCRIPT", "PREDICT", "LRSSL", "LRSSL2", "PREDICT_Gottlieb"]
+    assert model_name in ["Gottlieb", "Cdataset_Aonly", "indep", "Fdataset", "DNdataset", "Cdataset", "TRANSCRIPT", "PREDICT", "LRSSL", "LRSSL2", "PREDICT_Gottlieb", "TRANSCRIPT_v1", "PREDICT_v1"]
     if (model_name == "LRSSL"):
         url_lrssl = "https://raw.githubusercontent.com/LiangXujun/LRSSL/master/"
         lrssl_dataset_path = save_folder+"LRSSL/"
         fnames = {
             "A": "drug_dis_mat.txt", "P": "disease_similarity.txt", "S1": "drug_from_drugbank_without_ind_dommat.txt",
             "S2": "drug_pubchem_mat.txt", "S3": "drug_target_domain_mat.txt", "N4": "drug_target_go_mat.txt", 
             "N5": "drug_without_ind_dommat_new.txt", "S6": "drug_without_ind_gomat_new.txt", 
@@ -202,45 +202,52 @@
             S = pd.DataFrame(np.concatenate((S_chemical,S_domain,S_GO), axis=0), index=range(S_chemical.shape[0]+S_domain.shape[0]+S_GO.shape[0]), columns=["drug%d" % (i+1) for i in range(S_chemical.shape[1])])
             S.index = [("chemical" if (iss < S_chemical.shape[0]) else ("domain" if (iss < S_chemical.shape[0]+S_domain.shape[0]) else "go"))+sep_feature+("drug%d" % (s+1)) for iss, s in enumerate(list(S.index))]
             P = ddt['predictSimMatdg']
             P = pd.DataFrame(P, index=["disease%d" % (i+1) for i in range(P.shape[0])], columns=["disease%d" % (i+1) for i in range(P.shape[1])])
         else:
             raise ValueError("Undefined dataset '%s'" % mmodel_name)
         A = pd.DataFrame(A, index=S.columns, columns=P.columns)
-    if (model_name in ["TRANSCRIPT", "PREDICT"]):
+    if (model_name in ["TRANSCRIPT", "TRANSCRIPT_v1", "PREDICT", "PREDICT_v1"]):
         path=save_folder+model_name+"/" 
         fnames = {"A": "ratings_mat.csv", "P": "users.csv", "S": "items.csv"} 
         if (not os.path.exists(path+fnames["A"])):
-            if (model_name == "TRANSCRIPT"):
-                url_dataset = "https://zenodo.org/record/7982976/files/TRANSCRIPT_dataset_v2.0.0.zip"
+            if ("TRANSCRIPT" in model_name):
+                url_dataset = "https://zenodo.org/record/7982976/files/TRANSCRIPT_dataset_v2.0.0.zip" if (model_name=="TRANSCRIPT") else "https://zenodo.org/record/7982970/files/TRANSCRIPT_dataset_v1.0.0.zip"
             else:
                 print("Run the notebook or use the publicly available data (by default, download the latest public dataset)")
-                url_dataset = "https://zenodo.org/record/7983090/files/PREDICT_dataset_v2.0.0.zip"
-            subprocess.call(" ".join(["wget", "-qO", save_folder+model_name+".zip", "\""+url_dataset+"\""]), shell=True)  
-            subprocess.call(" ".join(["unzip", save_folder+model_name+".zip", "&&", "mv", model_name+"_dataset_v2.0.0", save_folder+model_name, "&&", "rm", "-f", save_folder+model_name+".zip"]), shell=True)   
-        if (model_name == "TRANSCRIPT"):
+                url_dataset = "https://zenodo.org/record/7983090/files/PREDICT_dataset_v2.0.0.zip" if (model_name=="PREDICT") else "https://zenodo.org/record/8087306/files/PREDICT_dataset_v1.0.0.zip"
+            subprocess.call(" ".join(["wget", "-qO", save_folder+model_name+".zip", "\""+url_dataset+"\""]), shell=True)
+            subprocess.call(" ".join(["unzip", "-qq", save_folder+model_name+".zip"]), shell=True)   
+            subprocess.call(" ".join(["mv", model_name.split("_")[0]+"_dataset_v"+("2" if ("v1" not in model_name) else "1")+".0.0", save_folder+model_name, "&&", "rm", "-f", save_folder+model_name+".zip"]), shell=True) 
+        if ("TRANSCRIPT" in model_name):
             assert os.path.exists(path+fnames["A"])
             assert os.path.exists(path+fnames["P"])
             assert os.path.exists(path+fnames["S"])
-            A, P, S = [pd.read_csv(path+fnames[k], engine="python", index_col=0) for k in ["A", "P", "S"]]
+            A, P, S = [pd.read_csv(path+fnames[k], engine="python", index_col=0) for k in ["A", "P", "S"]]  
         else:
             assert os.path.exists(path+fnames["A"])
             if (os.path.exists(path+fnames["P"]) and os.path.exists(path+fnames["S"])):
-                A, P, S = [pd.read_csv(path+fnames[k], engine="python", index_col=0) for k in ["A", "P", "S"]]
+                A, P, S = [pd.read_csv(path+fnames[k], engine="python", index_col=0) for k in ["A", "P", "S"]] 
             else: ## use publicly available data 
                 A = pd.read_csv(path+fnames["A"], engine="python", index_col=0)
+                A = A[[a for a in A.columns if (".1"!=a[-len(".1"):])]]
+                A.index = A.index.astype(str)
                 P_phenotype = pd.read_csv(path+"disease_phenotype_PREDICT_matrix.csv", engine="python", index_col=0)
                 P_semantic = pd.read_csv(path+"disease_semantic_PREDICT_matrix.csv", engine="python", index_col=0)
                 S_se = pd.read_csv(path+"se_PREDICT_matrix.csv", engine="python", index_col=0)
                 S_signature = pd.read_csv(path+"signature_PREDICT_matrix.csv", engine="python", index_col=0)
                 P = P_phenotype.T.join(P_semantic.T, how="outer").T
                 P.index = [("phenotype" if (iss < P_phenotype.shape[0]) else "semantic")+sep_feature+str(s) for iss, s in enumerate(list(P.index))]
                 S = S_se.T.join(S_signature.T, how="outer").T
-                S.index = [("se" if (iss < S_se.shape[0]) else "signature")+sep_feature+str(s) for iss, s in enumerate(list(S.index))]
+                if ("v1" not in model_name):
+                    S.index = [("se" if (iss < S_se.shape[0]) else "signature")+sep_feature+str(s) for iss, s in enumerate(list(S.index))]
+                else:
+                    S = S[[s for s in S.columns if (s in A.index)]]
                 A = A.loc[S.columns][P.columns]
+        A.index = A.index.astype(str) 
     if (model_name == "Gottlieb"):
         url_mbirw = "https://raw.githubusercontent.com/bioinfomaticsCSU/MBiRW/master/Datasets/"
         gottlieb_dataset_path = save_folder+"Gottlieb_dataset/MBiRW_files/"
         if (not os.path.exists(gottlieb_dataset_path+"DiDrAMat")):
             subprocess.call(" ".join(['mkdir', '-p', gottlieb_dataset_path]), shell=True)
             for fname in ["DiDrAMat","DiseaseSimMat","DiseasesName","DrugSimMat","DrugsName"]:
                 subprocess.call(" ".join(["wget", "-qO", gottlieb_dataset_path+fname, url_mbirw+fname]), shell=True)
```

### Comparing `stanscofi-1.0.4/src/stanscofi/validation.py` & `stanscofi-1.1.0/src/stanscofi/validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,35 +40,47 @@
     '''
     assert scores.shape[1]==3
     assert predictions.shape[1]==3
     assert predictions.shape[0]==scores.shape[0]
     assert beta>0
     y_true_all = np.array([test_dataset.ratings_mat[j,i] for i,j in scores[:,:2].astype(int).tolist()])
     y_pred_all = predictions[:,2].flatten()
-    if (not ignore_zeroes):
+    if (test_dataset.folds is not None):
+        ids = np.argwhere(np.ones(test_dataset.ratings_mat.shape))
+        folds_ids = [((test_dataset.folds[:,0]==i)&(test_dataset.folds[:,1]==j)).any() for i,j in ids[:,:2].tolist()]
+        y_true_all = y_true_all[folds_ids]
+        y_pred_all = y_pred_all[folds_ids]
+        scores_ = scores[folds_ids,:]
+        assert y_true_all.shape[0] == test_dataset.folds.shape[0]
+        assert y_pred_all.shape[0] == test_dataset.folds.shape[0]
+    else:
         scores_ = deepcopy(scores)
+    if (not ignore_zeroes):
         predictions_ = deepcopy(predictions)
         y_true = (y_true_all>0).astype(int) 
         y_pred = (y_pred_all>0).astype(int)
     else:
-        ids = np.argwhere(y_true!=0)
+        ids = np.argwhere(y_true_all!=0)
         scores_ = scores[ids.flatten().tolist(),:]
         predictions_ = predictions[ids,:]
         y_true = (y_true_all[ids]>0).astype(int)
         y_pred = (y_pred_all[ids]>0).astype(int)
-    assert y_true.shape[0]==y_pred.shape[0]
+    assert y_true.shape[0]==y_pred.shape[0]==scores_.shape[0]
     assert all([x in [-1,0,1] for x in np.unique(y_true).flatten()])
     ## Compute average metric per user
     user_ids = np.unique(scores_[:,0].flatten()).astype(int).tolist()
     n_ignored = 0
     aucs, tprs, recs, fscores = [], [], [], []
     base_fpr = np.linspace(0, 1, 101)
     base_pres = np.linspace(0, 1, 101)
     for user_id in user_ids:
         user_ids_i = np.argwhere(scores_[:,0].flatten()==user_id)
+        if (len(user_ids_i)==0):
+            n_ignored += 1
+            continue
         user_truth = y_true[user_ids_i].reshape(1, -1)
         user_pred = y_pred[user_ids_i].reshape(1, -1)
         if (len(np.unique(user_truth))==2):
             fpr, tpr, _ = ROC(user_truth.flatten(), user_pred.flatten())
             pres, rec, _ = PRC(user_truth.flatten(), user_pred.flatten())
             aucs.append(AUC(user_truth.flatten(), user_pred.flatten()))
             fscores.append(fbeta_score(user_truth.flatten(), user_pred.flatten(), beta=beta))
@@ -77,14 +89,18 @@
             tprs.append(tpr)
             rec = np.interp(base_pres, pres, rec)
             recs.append(rec)
         else:
             n_ignored += 1
     if (verbose and n_ignored>0):
         print("<validation.compute_metrics> Computed on #users=%d, %d ignored (%2.f perc)" % (len(user_ids), n_ignored, 100*n_ignored/len(user_ids)))
+    if (len(aucs)==0 or len(fscores)==0):
+        metrics = pd.DataFrame([], index=["AUC", "F_%.1f" % beta], 
+		columns=["Avg. across users", "Std"])
+        return metrics, {}
     metrics = pd.DataFrame([[f(x) for f in [np.mean, np.std]] for x in [aucs, fscores]], index=["AUC", "F_%.1f" % beta], 
 		columns=["Avg. across users", "Std"])
     return metrics, {"y_true": y_true, "y_pred": y_pred, "scores": scores_[:,2].flatten(), "predictions": y_pred_all, "ground_truth": y_true_all, "aucs": aucs, "fscores": fscores, "tprs": np.array(tprs), "recs": np.array(recs)}
 
 def plot_metrics(y_true=None, y_pred=None, scores=None, ground_truth=None, predictions=None, aucs=None, fscores=None, tprs=None, recs=None, figsize=(16,5), model_name="Model"):
     '''
     Plots the ROC curve, the Precision-Recall curve, the boxplot of predicted scores and the piechart of classes associated to the predictions y_pred in input w.r.t. ground truth y_true
@@ -128,16 +144,16 @@
     assert ((y_pred==1)|(y_pred==0)).all()
     assert ground_truth.shape[0]==predictions.shape[0]==scores.shape[0]
     assert ((ground_truth==1)|(ground_truth==0)|(ground_truth==-1)).all()
     assert ((predictions==1)|(predictions==0)|(predictions==-1)).all()
     assert len(aucs)==len(fscores)
     assert tprs.shape[0]==recs.shape[0]
     assert len(figsize)==2
-    base_fpr = np.linspace(0, 1, 101)
-    base_pres = np.linspace(0, 1, 101)
+    base_fpr = np.linspace(0, 1, tprs.shape[1])
+    base_pres = np.linspace(0, 1, np.array(recs).shape[1])
     ## Compute average values across users
     if (len(aucs) > 0):
         mean_tprs = tprs.mean(axis=0)
         std_tprs = tprs.std(axis=0)
         recs = np.array(recs)
         mean_recs = recs.mean(axis=0)
         std_recs = recs.std(axis=0)
@@ -151,23 +167,23 @@
         return None
     tprs_upper = np.minimum(mean_tprs + std_tprs, 1)
     tprs_lower = mean_tprs - std_tprs
     recs_upper = np.minimum(mean_recs + std_recs, 1)
     recs_lower = mean_recs - std_recs
     fig, axes = plt.subplots(nrows=2, ncols=2, figsize=figsize)
     ## ROC curve
-    axes[0,0].plot(base_fpr, mean_tprs, 'b', alpha = 0.8, label=model_name+' (AUC = %0.2f $\pm$ %0.2f)' % (auc, std_auc))
+    axes[0,0].plot(base_fpr, mean_tprs, 'b', alpha = 0.8, label=model_name+' (AUC = %0.2f %s %0.2f)' % (auc, "$\\pm$", std_auc))
     axes[0,0].fill_between(base_fpr, tprs_lower, tprs_upper, color = 'blue', alpha = 0.2)
     axes[0,0].plot([0, 1], [0, 1], linestyle = '--', lw = 2, color = 'r', alpha= 0.8, label="Constant")
     axes[0,0].set_ylabel('True Positive Rate')
     axes[0,0].set_xlabel('False Positive Rate')
     axes[0,0].legend(loc="lower right")
     axes[0,0].set_title('Avg. user ROC curve')
     ## Precision-recall curve
-    axes[0,1].plot(base_pres, mean_recs, 'b', alpha=0.8, label=model_name+' (F = %0.2f $\pm$ %0.2f)' % (fs, std_fs))
+    axes[0,1].plot(base_pres, mean_recs, 'b', alpha=0.8, label=model_name+' (F = %0.2f %s %0.2f)' % (fs, "$\\pm$", std_fs))
     axes[0,1].fill_between(base_pres, recs_lower, recs_upper, color="blue", alpha=0.2)
     axes[0,1].plot([0,1], [1,0], linestyle="--", lw=2, color="r", alpha=0.8, label="Constant")
     axes[0,1].set_xlabel('Precision')
     axes[0,1].set_ylabel('Recall')
     axes[0,1].set_title('Avg. user precision-recall curve')
     axes[0,1].legend(loc='lower left')
     ## Boxplot of predicted values
```

### Comparing `stanscofi-1.0.4/src/stanscofi.egg-info/PKG-INFO` & `stanscofi-1.1.0/src/stanscofi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanscofi
-Version: 1.0.4
+Version: 1.1.0
 Summary: Package for STANdard drug Screening by COllaborative FIltering. Performs benchmarks against datasets and SotA algorithms, and implements training, validation and testing procedures.
 Home-page: https://github.com/RECeSS-EU-Project/stanscofi
 Author: Clémence Réda
 Author-email: recess-project@proton.me
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -14,15 +14,15 @@
 
 ![funding logo](https://raw.githubusercontent.com/RECeSS-EU-Project/RECeSS-EU-Project.github.io/main/assets/images/header%2BEU_rescale.jpg)
 
 # STANdard for drug Screening by COllaborative FIltering (stanscofi) Python Package
 
 This repository is a part of the EU-funded [RECeSS project](https://recess-eu-project.github.io) (#101102016), and hosts the code for the open-source Python package *stanscofi* for the development of collaborative filtering-based drug repurposing algorithms.
 
-[![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![PyPI version](https://badge.fury.io/py/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847)
+[![Python Version](https://img.shields.io/badge/python-3.8%7C3.9%7C3.10-pink)](https://badge.fury.io/py/stanscofi) [![PyPI version](https://img.shields.io/pypi/v/stanscofi.svg)](https://badge.fury.io/py/stanscofi) [![Anaconda version](https://anaconda.org/recess/stanscofi/badges/version.svg)](https://anaconda.org/recess/stanscofi) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.8038847.svg)](https://doi.org/10.5281/zenodo.8038847) ![GitHub](https://img.shields.io/github/license/recess-eu-project/stanscofi.svg) [![Build Status](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml/badge.svg)](https://github.com/recess-eu-project/stanscofi/actions/workflows/post-push-test.yml) [![Codecov](https://codecov.io/github/recess-eu-project/stanscofi/coverage.svg?branch=master)](https://codecov.io/github/recess-eu-project/stanscofi?branch=master) [![Codefactor](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi/badge?style=plastic)](https://www.codefactor.io/repository/github/recess-eu-project/stanscofi)
 
 ## Statement of need 
 
 As of 2022, current drug development pipelines last around 10 years, costing $2billion in average, while drug commercialization failure rates go up to 90%. These issues can be mitigated by drug repurposing, where chemical compounds are screened for new therapeutic indications in a systematic fashion. In prior works, this approach has been implemented through collaborative filtering. This semi-supervised learning framework leverages known drug-disease matchings in order to recommend new ones.
 
 The **stanscofi** package comprises method-agnostic training, validation, preprocessing and visualization procedures on several published drug repurposing datasets. The proper implementation of these steps is crucial in order to avoid data leakage, *i*.*e*., the model is learnt over information that should be unavailable at prediction time. Indeed, data leakage is the source of a major reproducibility crisis in machine learning. This will be avoided by building training and validation sets which are weakly correlated with respect to the drug and disease feature vectors. The main performance metric will be the area under the curve (AUC), which estimates the diagnostic ability of a recommender system better than accuracy in imbalanced datasets.
```

