# Comparing `tmp/hdlib-0.1.7.tar.gz` & `tmp/hdlib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdlib-0.1.7.tar", last modified: Thu Jun 15 20:19:48 2023, max compression
+gzip compressed data, was "dist/hdlib-0.1.8.tar", last modified: Fri Jun 30 17:05:33 2023, max compression
```

## Comparing `hdlib-0.1.7.tar` & `hdlib-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 20:19:48.446390 hdlib-0.1.7/
--rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.7/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)     3028 2023-06-15 20:19:48.444930 hdlib-0.1.7/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     2225 2023-06-13 01:38:11.000000 hdlib-0.1.7/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 20:19:48.298274 hdlib-0.1.7/hdlib/
--rw-r--r--   0 fabio      (501) staff       (20)      102 2023-06-15 20:14:44.000000 hdlib-0.1.7/hdlib/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     2480 2023-06-01 14:38:17.000000 hdlib-0.1.7/hdlib/arithmetic.py
--rw-r--r--   0 fabio      (501) staff       (20)    29987 2023-06-15 20:14:36.000000 hdlib-0.1.7/hdlib/model.py
--rw-r--r--   0 fabio      (501) staff       (20)     2534 2023-06-08 21:27:39.000000 hdlib-0.1.7/hdlib/parser.py
--rw-r--r--   0 fabio      (501) staff       (20)    21854 2023-06-08 20:17:24.000000 hdlib-0.1.7/hdlib/space.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 20:19:48.398650 hdlib-0.1.7/hdlib.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     3028 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      295 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)       50 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-15 20:19:48.000000 hdlib-0.1.7/hdlib.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-15 20:19:48.446735 hdlib-0.1.7/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)     1462 2023-06-15 14:40:58.000000 hdlib-0.1.7/setup.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-15 20:19:48.423976 hdlib-0.1.7/test/
--rw-r--r--   0 fabio      (501) staff       (20)     8033 2023-06-13 01:24:19.000000 hdlib-0.1.7/test/test.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-30 17:05:33.000000 hdlib-0.1.8/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.8/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     3317 2023-06-30 17:05:33.000000 hdlib-0.1.8/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     2225 2023-06-13 01:38:11.000000 hdlib-0.1.8/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-30 17:05:33.000000 hdlib-0.1.8/hdlib/
+-rw-r--r--   0 fabio      (501) staff       (20)      102 2023-06-30 15:21:23.000000 hdlib-0.1.8/hdlib/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     5724 2023-06-30 15:21:08.000000 hdlib-0.1.8/hdlib/arithmetic.py
+-rw-r--r--   0 fabio      (501) staff       (20)    33770 2023-06-30 16:36:29.000000 hdlib-0.1.8/hdlib/model.py
+-rw-r--r--   0 fabio      (501) staff       (20)     3862 2023-06-30 14:42:35.000000 hdlib-0.1.8/hdlib/parser.py
+-rw-r--r--   0 fabio      (501) staff       (20)    41140 2023-06-30 15:26:03.000000 hdlib-0.1.8/hdlib/space.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-30 17:05:33.000000 hdlib-0.1.8/hdlib.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     3317 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      295 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       50 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-30 17:05:33.000000 hdlib-0.1.8/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1462 2023-06-15 14:40:58.000000 hdlib-0.1.8/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-30 17:05:33.000000 hdlib-0.1.8/test/
+-rw-r--r--   0 fabio      (501) staff       (20)     8036 2023-06-30 16:29:04.000000 hdlib-0.1.8/test/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `hdlib-0.1.7/LICENSE` & `hdlib-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.7/PKG-INFO` & `hdlib-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: hdlib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python
 Home-page: http://github.com/cumbof/hdlib
 Author: Fabio Cumbo
 Author-email: fabio.cumbo@gmail.com
 License: MIT
 Project-URL: Issues, https://github.com/cumbof/hdlib/issues
 Project-URL: Source, https://github.com/cumbof/hdlib
 Project-URL: Wiki, https://github.com/cumbof/hdlib/wiki
+Description: # hdlib
+        
+        Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python 3.
+        
+        ![Conda](https://img.shields.io/conda/dn/conda-forge/hdlib?label=hdlib%20on%20Conda)
+        
+        Please refer to the official [Wiki](https://github.com/cumbof/hdlib/wiki) for any information about the implemented modules and how to use the library.
+        
+        Here is the table of content:
+        
+        - [Getting started](https://github.com/cumbof/hdlib/wiki/Getting-started)
+          - [Installing `hdlib`](https://github.com/cumbof/hdlib/wiki/Getting-started#installing-hdlib)
+          - [Dependencies](https://github.com/cumbof/hdlib/wiki/Getting-started#dependencies)
+        - [Vector-Symbolic Architectures](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures)
+          - [Hyperdimensional Vectors and Space](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures#hyperdimensional-vectors-and-space)
+          - [Arithmetic operations](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures#arithmetic-operations)
+        - [Examples](https://github.com/cumbof/hdlib/wiki/Examples)
+          - [What is the Dollar of Mexico?](https://github.com/cumbof/hdlib/wiki/Examples#what-is-the-dollar-of-mexico)
+          - [Supervised Machine Learning Model](https://github.com/cumbof/hdlib/wiki/Examples#supervised-machine-learning-model)
+          - [Stepwise Feature Selection](https://github.com/cumbof/hdlib/wiki/Examples#stepwise-feature-selection)
+        - [Support and contributions](https://github.com/cumbof/hdlib/wiki/Support-and-contributions)
+        
+        ## Credits
+        
+        Please credit our work in your manuscript by citing:
+        
+        > _Manuscript in preparation_
+        
+        ## Support and contributions
+        
+        Long-term discussion and bug reports are maintained via GitHub Issues, while code review is managed via GitHub Pull Requests.
+        
+        Please, (i) be sure that there are no existing issues/PR concerning the same bug or improvement before opening a new issue/PR; (ii) write a clear and concise description of what the bug/PR is about; (iii) specifying the list of steps to reproduce the behavior in addition to versions and other technical details is highly recommended.
+        
+        Copyright © 2022 [Fabio Cumbo](https://github.com/cumbof). See [LICENSE](https://github.com/cumbof/hdlib/blob/main/LICENSE) for additional details.
+        
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# hdlib
-
-Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python 3.
-
-![Conda](https://img.shields.io/conda/dn/conda-forge/hdlib?label=hdlib%20on%20Conda)
-
-Please refer to the official [Wiki](https://github.com/cumbof/hdlib/wiki) for any information about the implemented modules and how to use the library.
-
-Here is the table of content:
-
-- [Getting started](https://github.com/cumbof/hdlib/wiki/Getting-started)
-  - [Installing `hdlib`](https://github.com/cumbof/hdlib/wiki/Getting-started#installing-hdlib)
-  - [Dependencies](https://github.com/cumbof/hdlib/wiki/Getting-started#dependencies)
-- [Vector-Symbolic Architectures](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures)
-  - [Hyperdimensional Vectors and Space](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures#hyperdimensional-vectors-and-space)
-  - [Arithmetic operations](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures#arithmetic-operations)
-- [Examples](https://github.com/cumbof/hdlib/wiki/Examples)
-  - [What is the Dollar of Mexico?](https://github.com/cumbof/hdlib/wiki/Examples#what-is-the-dollar-of-mexico)
-  - [Supervised Machine Learning Model](https://github.com/cumbof/hdlib/wiki/Examples#supervised-machine-learning-model)
-  - [Stepwise Feature Selection](https://github.com/cumbof/hdlib/wiki/Examples#stepwise-feature-selection)
-- [Support and contributions](https://github.com/cumbof/hdlib/wiki/Support-and-contributions)
-
-## Credits
-
-Please credit our work in your manuscript by citing:
-
-> _Manuscript in preparation_
-
-## Support and contributions
-
-Long-term discussion and bug reports are maintained via GitHub Issues, while code review is managed via GitHub Pull Requests.
-
-Please, (i) be sure that there are no existing issues/PR concerning the same bug or improvement before opening a new issue/PR; (ii) write a clear and concise description of what the bug/PR is about; (iii) specifying the list of steps to reproduce the behavior in addition to versions and other technical details is highly recommended.
-
-Copyright © 2022 [Fabio Cumbo](https://github.com/cumbof). See [LICENSE](https://github.com/cumbof/hdlib/blob/main/LICENSE) for additional details.
```

### Comparing `hdlib-0.1.7/README.md` & `hdlib-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.7/hdlib/model.py` & `hdlib-0.1.8/hdlib/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Classification Model with Hyperdimensional Computing
-"""
+"""Classification Model with Hyperdimensional Computing."""
 
 import copy
 import itertools
 import multiprocessing as mp
 import statistics
 from functools import partial
 from typing import Dict, List, Optional, Set, Tuple
@@ -15,31 +13,56 @@
 from hdlib import __version__
 from hdlib.space import Space, Vector
 from hdlib.arithmetic import bundle, permute
 from hdlib.parser import kfolds_split
 
 
 class Model(object):
-    """
-    Classification Model
-    """
+    """Classification Model."""
 
     def __init__(
         self,
         size: int=10000,
         levels: int=2,
         vtype: str="bipolar",
     ) -> "Model":
-        """
-        Initialize a Model object
+        """Initialize a Model object.
+
+        Parameters
+        ----------
+        size : int, default 10000
+            The size of vectors used to create a Space and define Vector objects.
+        levels : int, default 2
+            The number of level vectors used to represent numerical data. It is 2 by default.
+        vtype : {'binary', 'bipolar'}, default 'bipolar'
+            The vector type in space, which is bipolar by default.
+
+        Raises
+        ------
+        TypeError
+            If the vector size or the number of levels are not integer numbers.
+        ValueError
+            If the vector size is lower than 10,000 or the number of level vectors is lower than 2.
+
+        Examples
+        --------
+        >>> from hdlib.model import Model
+        >>> model = Model(size=10000, levels=100, vtype='bipolar')
+        >>> type(model)
+        <class 'hdlib.model.Model'>
+
+        This creates a new Model object around a Space that can host random bipolar Vector objects with size 10,000.
+        It also defines the number of level vectors to 100.
+
+        Notes
+        -----
+        The classification model based on the hyperdimensional computing paradigm has been originally described in [1]_.
 
-        :param size:        Vector size or dimensionality
-        :param levels:      Number of levels
-        :param vtype:       Vector type: bipolar or binary
-        :return:            A Model object
+        .. [1] Cumbo, Fabio, Eleonora Cappelli, and Emanuel Weitschek. "A brain-inspired hyperdimensional computing approach 
+        for classifying massive dna methylation data of cancer." Algorithms 13.9 (2020): 233.
         """
 
         if not isinstance(size, int):
             raise TypeError("Vectors size must be an integer number")
 
         if size < 10000:
             raise ValueError("Vectors size must be greater than or equal to 10000")
@@ -68,16 +91,40 @@
         # Class labels
         self.classes = set()
 
         # Keep track of hdlib version
         self.version = __version__
 
     def __str__(self) -> None:
-        """
-        Print the Model object properties
+        """Print the Model object properties.
+
+        Returns
+        -------
+        str
+            A description of the Model object. It reports the vectors size, the vector type,
+            the number of level vectors, the number of data points, and the number of class labels.
+
+        Examples
+        --------
+        >>> from hdlib.model import Model
+        >>> model = Model()
+        >>> print(model)
+
+                Class:   hdlib.model.Model
+                Size:    10000
+                Type:    bipolar
+                Levels:  2
+                Points:  0
+                Classes:
+
+                []
+
+        Print the Model object properties. By default, the size of vectors in space is 10,000,
+        their types is bipolar, and the number of level vectors is 2. The number of data points 
+        and the number of class labels are empty here since no dataset has been processed yet.
         """
 
         return """
             Class:   hdlib.model.Model
             Version: {}
             Size:    {}
             Type:    {}
@@ -91,43 +138,62 @@
             self.size,
             self.vtype,
             self.levels,
             len(self.space.memory()) - self.levels if self.space is not None else 0,
             np.array(list(self.classes))
         )
 
-    def init_fit_predict(
+    def _init_fit_predict(
         self,
         size: int=10000,
         levels: int=2,
         vtype: str="bipolar",
         points: Optional[List[List[float]]]=None,
         labels: Optional[List[str]]=None,
         cv: int=5,
         distance_method: str="cosine",
         retrain: int=0,
         n_jobs: int=1,
         metric: str="accuracy"
     ) -> Tuple[int, int, float]:
-        """
-        Initialize a new Model, then fit and cross-validate it.
-        Used for size and levels hyperparameters tuning
+        """Initialize a new Model, then fit and cross-validate it. Used for size and levels hyperparameters tuning.
 
-        :param size:            Vector size or dimensionality
-        :param levels:          Number of levels
-        :param vtype:           Vector type: bipolar or binary
-        :param points:          List of data points
-        :param labels:          Class labels
-        :param cv:              Number of folds for the cross validation
-        :param distance_method: Method used to compute the distance between vectors in the space
-                                Look at the dist() method of htlib.space.Vector class for a list of supported distance methods
-        :param retrain:         Maximum number of retraining iterations
-        :param n_jobs:          Number of jobs for processing folds in parallel
-        :param metric:          Model score: accuracy, f1, precision, and recall
-        :return:                The dimensionality, the number of levels, and the model score
+        Parameters
+        ----------
+        size : int, default 10000
+            The size of vectors used to create a Space and define Vector objects.
+        levels : int, default 2
+            The number of level vectors used to represent numerical data. It is 2 by default.
+        vtype : {'binary', 'bipolar'}, default 'bipolar'
+            The vector type in space, which is bipolar by default.
+        points : list
+            List of lists with numerical data (floats).
+        labels : list
+            List with class labels. It has the same size of `points`.
+        cv : int, default 5
+            Number of folds for cross-validating the model.
+        distance_method : {'cosine', 'euclidean', 'hamming'}, default 'cosine'
+            Method used to compute the distance/similarity between vectors in space.
+        retrain : int, default 0
+            Number of retraining iterations.
+        n_jobs : int, default 1,
+            Number of jobs for processing folds in parallel.
+        metric: {'accuracy', 'f1', 'precision', 'recall'}, default 'accuracy'
+            Metric used to evaluate the model.
+
+        Returns
+        -------
+        tuple
+            A tuple with the input size, the number of level vectors, and the model score
+            according to the input metric.
+
+        Raises
+        ------
+        ValueError
+            If the provided metric is not supported.
         """
 
         # Available score metrics
         score_metrics = {
             "accuracy": accuracy_score,
             "f1": f1_score,
             "precision": precision_score,
@@ -172,20 +238,29 @@
         return size, levels, statistics.mean(scores)
 
     def fit(
         self,
         points: List[List[float]],
         labels: List[str],
     ) -> None:
-        """
-        Build a vector-symbolic architecture.
-        Define level vectors and encode samples
+        """Build a vector-symbolic architecture. Define level vectors and encode samples.
 
-        :param points:  List of data points
-        :param labels:  Class labels
+        Parameters
+        ----------
+        points : list
+            List of lists with numerical data (floats).
+        labels : list
+            List with class labels. It has the same size of `points`.
+
+        Raises
+        ------
+        Exception
+            - if there are not enough data points (the length of `points` is < 3);
+            - if the length of `points` does not match the length of `labels`;
+            - if there is only one class label.
         """
 
         if len(points) < 3:
             # This is based on the assumption that the minimum number of data points for training
             # the classification model is 2, while 1 data point is enough for the test set
             raise Exception("Not enough data points")
 
@@ -296,25 +371,36 @@
 
     def predict(
         self,
         test_indices: List[int],
         distance_method: str="cosine",
         retrain: int=0
     ) -> Tuple[List[int], List[str], int]:
-        """
-        Supervised Learning.
-        Predict the class labels of the data points in the test set
+        """Supervised Learning. Predict the class labels of the data points in the test set.
 
-        :param test_indices:    Indices of data points in the list of points used with fit() to be used for testing the classification model.
-                                Note that all the other points will be used for training the model
-        :param distance_method: Method used to compute the distance between vectors in the space
-                                Look at the dist() method of htlib.space.Vector class for a list of supported distance methods
-        :param retrain:         Maximum number of retraining iterations
-        :return:                The list test_indices in addition to a list with the predicted class labels with the same size of test_indices and
-                                the total number of retraining iterations used to retrain the classification model
+        Parameters
+        ----------
+        test_indices : list
+            Indices of data points in the list of points used with fit() to be used for testing the classification model.
+            Note that all the other points will be used for training the model.
+        distance_method : {'cosine', 'euclidean', 'hamming'}, default 'cosine'
+            Method used to compute the distance between vectors in the space.
+        retrain : int, default 0
+            Maximum number of retraining iterations.
+
+        Returns
+        -------
+        tuple
+            A tuple with the input list `test_indices` in addition to a list with the predicted class labels with the 
+            same size of `test_indices` and the total number of retraining iterations used to retrain the classification model.
+
+        Raises
+        ------
+        Exception
+            If the number of test indices does not match the number of points retrieved from the space.
         """
 
         # List with test vector names
         test_points = list()
 
         # List with training vector names
         training_points = list()
@@ -442,25 +528,44 @@
         points: List[List[float]],
         labels: List[str],
         cv: int=5,
         distance_method: str="cosine",
         retrain: int=0,
         n_jobs: int=1
     ) -> List[Tuple[List[int], List[str], int]]:
-        """
-        Run predict() in cross validation
+        """Run `predict()` in cross validation.
 
-        :param points:          List with data points. Same used for fit()
-        :param labels:          Class labels. Same used for fit()
-        :param cv:              Number of folds for the cross validation
-        :param distance_method: Method used to compute the distance between vectors in the space
-                                Look at the dist() method of htlib.space.Vector class for a list of supported distance methods
-        :param retrain:         Maximum number of retraining iterations
-        :param n_jobs:          Number of jobs for processing folds in parallel
-        :return:                A list with the result of predict() for each fold
+        Parameters
+        ----------
+        points : list
+            List of lists with numerical data (floats).
+        labels : list
+            List with class labels. It has the same size of `points`.
+        cv : int, default 5
+            Number of folds for cross-validating the model.
+        distance_method : {'cosine', 'euclidean', 'hamming'}, default 'cosine'
+            Method used to compute the distance/similarity between vectors in space.
+        retrain : int, default 0
+            Number of retraining iterations.
+        n_jobs : int, default 1,
+            Number of jobs for processing folds in parallel.
+
+        Returns
+        -------
+        list
+            A list with the results of `predict()` for each fold.
+
+        Raises
+        ------
+        Exception
+            - if the number of data points does not match with the number of class labels;
+            - if there is only one class label.
+        ValueError
+            - if the number of folds is a number < 1;
+            - if the number of folds exceeds the number of data points.
         """
 
         if len(points) != len(labels):
             raise Exception("The number of data points does not match with the number of class labels")
 
         if len(set(labels)) < 2:
             raise Exception("The number of unique class labels must be > 1")
@@ -519,34 +624,45 @@
         levels_range: range,
         cv: int=5,
         distance_method: str="cosine",
         retrain: int=0,
         n_jobs: int=1,
         metric: str="accuracy"
     ) -> Tuple[int, int, float]:
-        """
-        Automated hyperparameters tuning.
-        Performe a Parameter Sweep Analysis (PSA) on space dimensionality and number of levels.
-        It returns the best size and levels according to the accuracies of the cross-validated models
-
-        :param points:          List of data points
-        :param labels:          Class labels
-        :param size_range:      Range of dimensionalities for performing PSA
-        :param levels_range:    Range of number of levels for performing PSA
-        :param cv:              Number of folds for the cross validation
-        :param distance_method: Method used to compute the distance between vectors in the space
-                                Look at the dist() method of htlib.space.Vector class for a list of supported distance methods
-        :param retrain:         Maximum number of retraining iterations
-        :param n_jobs:          Number of jobs for processing models in parallel
-        :param metric:          Model score: accuracy, f1, precision, and recall
-        :return:                Best size, number of levels, and metric
+        """Automated hyperparameters tuning. Perform a Parameter Sweep Analysis (PSA) on space dimensionality and number of levels.
+
+        Parameters
+        ----------
+        points : list
+            List of lists with numerical data (floats).
+        labels : list
+            List with class labels. It has the same size of `points`.
+        size_range : range
+            Range of dimensionalities for performing PSA.
+        levels_range : range
+            Range of number of levels for performing PSA.
+        cv : int, default 5
+            Number of folds for cross-validating the model.
+        distance_method : {'cosine', 'euclidean', 'hamming'}, default 'cosine'
+            Method used to compute the distance/similarity between vectors in space.
+        retrain : int, default 0
+            Number of retraining iterations.
+        n_jobs : int, default 1,
+            Number of jobs for processing folds in parallel.
+        metric: {'accuracy', 'f1', 'precision', 'recall'}, default 'accuracy'
+            Metric used to evaluate the model.
+
+        Returns
+        -------
+        tuple
+            A tuple with the best size and levels according to the accuracies of the cross-validated models.
         """
 
         partial_init_fit_predict = partial(
-            self.init_fit_predict,
+            self._init_fit_predict,
             vtype=self.vtype,
             points=points,
             labels=labels,
             cv=cv,
             distance_method=distance_method,
             retrain=retrain,
             n_jobs=1,
@@ -571,62 +687,73 @@
             for job in jobs:
                 job_size, job_levels, job_metric = job.get()
 
                 if best_metric is None:
                     best_metric = job_metric
                     best_size = job_size
                     best_levels = job_levels
-                
+
                 else:
                     if job_metric > best_metric:
                         # Get the size and levels of the classification model with the best score metric
                         best_metric = job_metric
                         best_size = job_size
                         best_levels = job_levels
-                    
+
                     elif job_metric == best_metric:
                         # Minimize the number of levels in this case
                         if job_levels < best_levels:
                             best_size = job_size
                             best_levels = job_levels
-                        
+
                         elif job_levels == best_levels:
                             # Minimize the size in this case
                             if job_size < best_size:
                                 best_size = job_size
 
         return best_size, best_levels, best_metric
 
-    def stepwise_regression_iter(
+    def _stepwise_regression_iter(
         self,
         features_indices: Set[int],
         points: List[List[float]],
         labels: List[str],
         cv: int=5,
         distance_method: str="cosine",
         retrain: int=0,
         metric: str="accuracy"
-    ) -> Tuple[List[List[float]], float]:
-        """
-        Just a single iteration of the feature selection method.
+    ) -> Tuple[Set[float], float]:
+        """Just a single iteration of the feature selection method.
 
-        :param features_indices:    Indices of features for shaping points
-        :param points:              List of data points
-        :param labels:              Class labels
-        :param cv:                  Number of folds for the cross validation
-        :param distance_method:     Method used to compute the distance between vectors in the space
-                                    Look at the dist() method of htlib.space.Vector class for a list of supported distance methods
-        :param retrain:             Maximum number of retraining iterations
-        :param metric:              Model score: accuracy, f1, precision, and recall
-        :return:                    The considered features and the score of the classification model based on metric
+        Parameters
+        ----------
+        features_indices : set
+            Indices of features for shaping points.
+        points : list
+            List of lists with numerical data (floats).
+        labels : list
+            List with class labels. It has the same size of `points`.
+        cv : int, default 5
+            Number of folds for cross-validating the model.
+        distance_method : {'cosine', 'euclidean', 'hamming'}, default 'cosine'
+            Method used to compute the distance/similarity between vectors in space.
+        retrain : int, default 0
+            Number of retraining iterations.
+        metric: {'accuracy', 'f1', 'precision', 'recall'}, default 'accuracy'
+            Metric used to evaluate the model.
+
+        Returns
+        -------
+        tuple
+            A tuple with the considered features and the score of the classification model based on the provided metric.
         """
 
         data_points = [[point[i] for i in range(len(point)) if i in features_indices] for point in points]
 
-        _, _, score = self.init_fit_predict(
+        _, _, score = self._init_fit_predict(
             size=self.size,
             levels=self.levels,
             vtype=self.vtype,
             points=data_points,
             labels=labels,
             cv=cv,
             distance_method=distance_method,
@@ -648,33 +775,49 @@
         retrain: int=0,
         n_jobs: int=1,
         metric: str="accuracy",
         threshold: float=0.6,
         uncertainty: float=5.0,
         stop_if_worse: bool=False
     ) -> Tuple[Dict[str, int], Dict[int, float], int]:
-        """
-        Stepwise feature selection as backward variable elimination or forward variable selection
+        """Stepwise regression as backward variable elimination or forward variable selection.
 
-        :param points:              List of data points
-        :param features:            List of features
-        :param labels:              Class labels
-        :param method:              Type of stepwise regression: backward or forward
-        :param cv:                  Number of folds for the cross validation
-        :param distance_method:     Method used to compute the distance between vectors in the space
-                                    Look at the dist() method of htlib.space.Vector class for a list of supported distance methods
-        :param retrain:             Maximum number of retraining iterations
-        :param n_jobs:              Number of jobs for processing models in parallel
-        :param metric:              Model score: accuracy, f1, precision, and recall
-        :param threshold:           Threshold on the model score metric
-                                    Stop running the feature selection if the best reached score is lower than this threshold
-        :param uncertainty:         Uncertainty threshold for comparing models accuracies
-        :param stop_if_worse:       Stop running the feature selection if the accuracy reached at the iteration i is lower than the accuracy reached at i-1
-        :return:                    A dictionary with features and their importance in addition to the best score for each importance rank and the top importance
-                                    In case of backward, the lower the better. In case of forward, the higher the better
+        Parameters
+        ----------
+        points : list
+            List of lists with numerical data (floats).
+        features : list
+            List of features
+        labels : list
+            List with class labels. It has the same size of `points`.
+        method : {'backward', 'forward'}, default 'backward'
+            Feature selection method.
+        cv : int, default 5
+            Number of folds for cross-validating the model.
+        distance_method : {'cosine', 'euclidean', 'hamming'}, default 'cosine'
+            Method used to compute the distance/similarity between vectors in space.
+        retrain : int, default 0
+            Number of retraining iterations.
+        n_jobs : int, default 1,
+            Number of jobs for processing models in parallel.
+        metric: {'accuracy', 'f1', 'precision', 'recall'}, default 'accuracy'
+            Metric used to evaluate the model.
+        threshold : float, default 0.6
+            Threshold on the model score metric. Stop running the feature selection if the best 
+            reached score is lower than this threshold.
+        uncertainty : float, default 5.0
+            Uncertainty percentage threshold for comparing models metrics.
+        stop_if_worse : bool, default False
+            Stop running the feature selection if the accuracy reached at the iteration i is lower than the accuracy reached at i-1.
+
+        Returns
+        -------
+        tuple
+            A tuple with a dictionary with features and their importance in addition to the best score for each importance rank 
+            and the top importance. In case of backward, the lower the better. In case of forward, the higher the better.
         """
 
         method = method.lower()
 
         if method not in ("backward", "forward"):
             raise ValueError("Stepwise method {} is not supported".format(method))
 
@@ -705,15 +848,15 @@
                     break
 
             if features_set_size > 0:
                 best_score = 0.0
                 classification_results = list()
 
                 partial_stepwise_regression_iter = partial(
-                    self.stepwise_regression_iter,
+                    self._stepwise_regression_iter,
                     points=points,
                     labels=labels,
                     cv=cv,
                     distance_method=distance_method,
                     retrain=retrain,
                     metric=metric
                 )
```

### Comparing `hdlib-0.1.7/hdlib/parser.py` & `hdlib-0.1.8/hdlib/parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-"""
-Utility to parse input files
-"""
+"""Utility to parse input files."""
 
 import errno
 import os
 import random
 from typing import List, Tuple
 
 import numpy as np
 
 
 def load_dataset(
     filepath: os.path.abspath,
     sep: str="\t"
 ) -> Tuple[List[str], List[List[float]], List[str]]:
-    """
-    Load the input dataset
+    """Load the input dataset.
 
-    :param filepath:    Path to the input dataset
-    :param sep:         Field separator
-    :return:            The list of sample IDs, the list of features, the content as list of lists, and the list of classes
+    Parameters
+    ----------
+    filepath : str
+        Path to the input dataset.
+    sep : str
+        Filed separator for the input dataset.
+
+    Returns
+    -------
+    tuple
+        A tuple with a list of sample IDs, a list of features, a list of lists with the
+        actual numerical data (floats), and a list with class labels.
     """
 
     if not os.path.isfile(filepath):
         raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), filepath)
 
     samples = list()
     content = list()
@@ -50,41 +56,87 @@
                 # Take track of the class
                 classes.append(line_split[-1])
 
     return samples, features, content, classes
 
 
 def kfolds_split(points: int, folds: int) -> List[List[int]]:
-    """
-    Given a number of data points and the number of folds, split a dataset into different folds
+    """Given a number of data points and the number of folds, split a dataset into different folds.
+
+    Parameters
+    ----------
+    points : int
+        Number of data points in the input dataset.
+    folds : int
+        Number of folds.
+
+    Returns
+    -------
+    list
+        A list of lists. Every list is a fold with the indices of data points in the original dataset.
+
+    Raises
+    ------
+    ValueError
+        If the number of folds is greater than the number of data points.
+
+    Examples
+    --------
+    >>> from hdlib.parser import kfolds_split
+    >>> kfolds_split(10, 3)
+    [[0, 3, 6, 9], [1, 4, 7], [2, 5, 8]]
 
-    :param points:  Number of data points
-    :param folds:   Number of folds
-    :return:        List of lists with the indices of data points
+    Considering a dataset with 10 data points, split them into 3 folds.
     """
 
     if folds > points:
         raise ValueError("The number of folds cannot exceed the number of data points")
 
     data_points = list(range(points))
 
     return [data_points[i::folds] for i in range(folds)]
 
 
-def percentage_split(points: int, percentage: float) -> List[int]:
-    """
-    Given a number of data points and a percentage number, split a dataset in two and report
-    the indices of the smallest set
+def percentage_split(points: int, percentage: float, seed: int=0) -> List[int]:
+    """Given a number of data points and a percentage number, split a dataset and report the indices of the of data points.
+
+    Parameters
+    ----------
+    points : int
+        Number of data points in the input dataset.
+    percentage : float
+        Percentage of points to split out of the original dataset.
+    seed : int
+        Random seed for reproducing the same results.
+
+    Returns
+    -------
+    list
+        A list with the indices of selected points.
+
+    Raises
+    ------
+    ValueError
+        - if the input `percentage` is lower than or equal to 0.0 or greater than 100.0;
+        - if the input `seed` is not an integer number.
+
+    Examples
+    --------
+    >>> from hdlib.parser import percentage_split
+    >>> percentage_split(10, 20.0, seed=0)
+    [6, 9]
 
-    :param points:      Number of data points
-    :param percentage:  Percentage split
-    :return:            List with indices of the smallest set after split
+    Consider a dataset with 10 data points, select 20% of the points (2 points in this case),
+    and report their indices in the original dataset.
     """
 
     if percentage <= 0.0 or percentage > 100.0:
         raise ValueError("Percentage must be greater than 0 and lower than or equal to 100")
 
+    if not isinstance(seed, int):
+        raise ValueError("The input seed must be an integer number")
+
     select_points = percentage * points / 100.0
 
-    random.seed(0)
+    random.seed(seed)
 
     return random.sample(list(range(points)), int(select_points))
```

### Comparing `hdlib-0.1.7/hdlib.egg-info/PKG-INFO` & `hdlib-0.1.8/hdlib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: hdlib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python
 Home-page: http://github.com/cumbof/hdlib
 Author: Fabio Cumbo
 Author-email: fabio.cumbo@gmail.com
 License: MIT
 Project-URL: Issues, https://github.com/cumbof/hdlib/issues
 Project-URL: Source, https://github.com/cumbof/hdlib
 Project-URL: Wiki, https://github.com/cumbof/hdlib/wiki
+Description: # hdlib
+        
+        Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python 3.
+        
+        ![Conda](https://img.shields.io/conda/dn/conda-forge/hdlib?label=hdlib%20on%20Conda)
+        
+        Please refer to the official [Wiki](https://github.com/cumbof/hdlib/wiki) for any information about the implemented modules and how to use the library.
+        
+        Here is the table of content:
+        
+        - [Getting started](https://github.com/cumbof/hdlib/wiki/Getting-started)
+          - [Installing `hdlib`](https://github.com/cumbof/hdlib/wiki/Getting-started#installing-hdlib)
+          - [Dependencies](https://github.com/cumbof/hdlib/wiki/Getting-started#dependencies)
+        - [Vector-Symbolic Architectures](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures)
+          - [Hyperdimensional Vectors and Space](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures#hyperdimensional-vectors-and-space)
+          - [Arithmetic operations](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures#arithmetic-operations)
+        - [Examples](https://github.com/cumbof/hdlib/wiki/Examples)
+          - [What is the Dollar of Mexico?](https://github.com/cumbof/hdlib/wiki/Examples#what-is-the-dollar-of-mexico)
+          - [Supervised Machine Learning Model](https://github.com/cumbof/hdlib/wiki/Examples#supervised-machine-learning-model)
+          - [Stepwise Feature Selection](https://github.com/cumbof/hdlib/wiki/Examples#stepwise-feature-selection)
+        - [Support and contributions](https://github.com/cumbof/hdlib/wiki/Support-and-contributions)
+        
+        ## Credits
+        
+        Please credit our work in your manuscript by citing:
+        
+        > _Manuscript in preparation_
+        
+        ## Support and contributions
+        
+        Long-term discussion and bug reports are maintained via GitHub Issues, while code review is managed via GitHub Pull Requests.
+        
+        Please, (i) be sure that there are no existing issues/PR concerning the same bug or improvement before opening a new issue/PR; (ii) write a clear and concise description of what the bug/PR is about; (iii) specifying the list of steps to reproduce the behavior in addition to versions and other technical details is highly recommended.
+        
+        Copyright © 2022 [Fabio Cumbo](https://github.com/cumbof). See [LICENSE](https://github.com/cumbof/hdlib/blob/main/LICENSE) for additional details.
+        
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# hdlib
-
-Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python 3.
-
-![Conda](https://img.shields.io/conda/dn/conda-forge/hdlib?label=hdlib%20on%20Conda)
-
-Please refer to the official [Wiki](https://github.com/cumbof/hdlib/wiki) for any information about the implemented modules and how to use the library.
-
-Here is the table of content:
-
-- [Getting started](https://github.com/cumbof/hdlib/wiki/Getting-started)
-  - [Installing `hdlib`](https://github.com/cumbof/hdlib/wiki/Getting-started#installing-hdlib)
-  - [Dependencies](https://github.com/cumbof/hdlib/wiki/Getting-started#dependencies)
-- [Vector-Symbolic Architectures](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures)
-  - [Hyperdimensional Vectors and Space](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures#hyperdimensional-vectors-and-space)
-  - [Arithmetic operations](https://github.com/cumbof/hdlib/wiki/Vector-Symbolic-Architectures#arithmetic-operations)
-- [Examples](https://github.com/cumbof/hdlib/wiki/Examples)
-  - [What is the Dollar of Mexico?](https://github.com/cumbof/hdlib/wiki/Examples#what-is-the-dollar-of-mexico)
-  - [Supervised Machine Learning Model](https://github.com/cumbof/hdlib/wiki/Examples#supervised-machine-learning-model)
-  - [Stepwise Feature Selection](https://github.com/cumbof/hdlib/wiki/Examples#stepwise-feature-selection)
-- [Support and contributions](https://github.com/cumbof/hdlib/wiki/Support-and-contributions)
-
-## Credits
-
-Please credit our work in your manuscript by citing:
-
-> _Manuscript in preparation_
-
-## Support and contributions
-
-Long-term discussion and bug reports are maintained via GitHub Issues, while code review is managed via GitHub Pull Requests.
-
-Please, (i) be sure that there are no existing issues/PR concerning the same bug or improvement before opening a new issue/PR; (ii) write a clear and concise description of what the bug/PR is about; (iii) specifying the list of steps to reproduce the behavior in addition to versions and other technical details is highly recommended.
-
-Copyright © 2022 [Fabio Cumbo](https://github.com/cumbof). See [LICENSE](https://github.com/cumbof/hdlib/blob/main/LICENSE) for additional details.
```

### Comparing `hdlib-0.1.7/setup.py` & `hdlib-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.7/test/test.py` & `hdlib-0.1.8/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         with self.subTest():
             # There should be a prediction for each fold
             self.assertEqual(len(predictions), 5)
 
         # Collect the accuracy scores computed on each fold
         scores = list()
 
-        for y_indices, y_pred in predictions:
+        for y_indices, y_pred, _ in predictions:
             y_true = [label for position, label in enumerate(classes) if position in y_indices]
             accuracy = accuracy_score(y_true, y_pred)
         
             with self.subTest():
                 self.assertTrue(accuracy > 0.0)
 
     def test_dollar_of_mexico(self):
```

