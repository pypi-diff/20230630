# Comparing `tmp/naiveautoml-0.0.8.tar.gz` & `tmp/naiveautoml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/naiveautoml-0.0.8.tar", last modified: Thu May 12 13:46:54 2022, max compression
+gzip compressed data, was "dist/naiveautoml-0.0.9.tar", last modified: Tue Oct 18 19:03:19 2022, max compression
```

## Comparing `naiveautoml-0.0.8.tar` & `naiveautoml-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-05-12 13:46:54.000000 naiveautoml-0.0.8/
--rw-r--r--   0 felix     (1000) felix     (1000)      730 2022-05-12 13:46:54.000000 naiveautoml-0.0.8/PKG-INFO
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-05-12 13:46:54.000000 naiveautoml-0.0.8/naiveautoml/
--rw-r--r--   0 felix     (1000) felix     (1000)       47 2021-10-27 14:18:32.000000 naiveautoml-0.0.8/naiveautoml/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    33459 2022-05-12 13:45:35.000000 naiveautoml-0.0.8/naiveautoml/commons.py
--rw-r--r--   0 felix     (1000) felix     (1000)    19323 2022-05-12 13:36:48.000000 naiveautoml-0.0.8/naiveautoml/naiveautoml.py
--rw-r--r--   0 felix     (1000) felix     (1000)    30332 2021-10-28 14:41:54.000000 naiveautoml-0.0.8/naiveautoml/searchspace.json
--rw-r--r--   0 felix     (1000) felix     (1000)       39 2021-10-27 14:20:17.000000 naiveautoml-0.0.8/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)     1512 2022-05-12 13:46:50.000000 naiveautoml-0.0.8/setup.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-05-12 13:46:54.000000 naiveautoml-0.0.8/test/
--rw-r--r--   0 felix     (1000) felix     (1000)     6199 2022-05-04 19:53:08.000000 naiveautoml-0.0.8/test/test_naiveautoml.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1062 2021-10-27 14:20:45.000000 naiveautoml-0.0.9/LICENSE.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      717 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/PKG-INFO
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/naiveautoml/
+-rw-r--r--   0 felix     (1000) felix     (1000)       47 2021-10-27 14:18:32.000000 naiveautoml-0.0.9/naiveautoml/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    45806 2022-10-18 17:53:44.000000 naiveautoml-0.0.9/naiveautoml/commons.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    20413 2022-10-18 18:24:51.000000 naiveautoml-0.0.9/naiveautoml/naiveautoml.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/naiveautoml.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)      717 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      303 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       62 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       12 2022-10-18 19:03:18.000000 naiveautoml-0.0.9/naiveautoml.egg-info/top_level.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       79 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)     1512 2022-10-18 19:02:33.000000 naiveautoml-0.0.9/setup.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-10-18 19:03:19.000000 naiveautoml-0.0.9/test/
+-rw-r--r--   0 felix     (1000) felix     (1000)    11260 2022-10-18 19:02:01.000000 naiveautoml-0.0.9/test/test_naiveautoml.py
```

### Comparing `naiveautoml-0.0.8/PKG-INFO` & `naiveautoml-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: naiveautoml
-Version: 0.0.8
+Version: 0.0.9
 Summary: The official package for the Naive AutoML paper
 Home-page: https://github.com/fmohr/naiveautoml
+Download-URL: https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.9.tar.gz
 Author: Felix Mohr
 Author-email: mail@felixmohr.de
 License: MIT
-Download-URL: https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.4.tar.gz
-Description: UNKNOWN
 Keywords: AutoML,sklearn,naive,simple
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE.txt
```

### Comparing `naiveautoml-0.0.8/naiveautoml/commons.py` & `naiveautoml-0.0.9/naiveautoml/commons.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 import time
 
 # sklearn
 import sklearn
 from sklearn import *
 from sklearn.pipeline import Pipeline
 from sklearn.metrics import get_scorer
+from sklearn.metrics import make_scorer
 
 
 # timeout functions
 from func_timeout import func_timeout, FunctionTimedOut
 
 # configspace
 import ConfigSpace
 from ConfigSpace.util import *
 from ConfigSpace.read_and_write import json as config_json
+import json
 
 def get_class( kls ):
     parts = kls.split('.')
     module = ".".join(parts[:-1])
     m = __import__( module )
     for comp in parts[1:]:
         m = getattr(m, comp)            
@@ -32,14 +34,18 @@
     candidates = [s[1] for s in steps if s[0] == name]
     return len(candidates) > 0
 
 def get_step_with_name(steps, name):
     candidates = [s for s in steps if s[0] == name]
     return candidates[0]
 
+def get_scoring_name(scoring):
+    return scoring if type(scoring) == str else scoring["name"]
+
+
 class EvaluationPool:
 
     def __init__(self, X, y, scoring, side_scores = None, tolerance_tuning = 0.05, tolerance_estimation_error = 0.01, logger_name = None):
         self.logger = logging.getLogger('naiveautoml.evalpool' if logger_name is None else logger_name)
         if X is None:
             raise Exception("Parameter X must not be None")
         if y is None:
@@ -64,96 +70,76 @@
     def tellEvaluation(self, pl, scores, timestamp):
         spl = str(pl)
         self.cache[spl] = (pl, scores, timestamp)
         score = np.mean(scores)
         if score > self.bestScore:
             self.bestScore = score        
             self.best_spl = spl
-            
-    def cross_validate(self, pl, X, y, scorings, errors="raise"): # just a wrapper to ease parallelism
+                        
+    def cross_validate(self, pl, X, y, scorings, errors="message"): # just a wrapper to ease parallelism
         warnings.filterwarnings('ignore', module = 'sklearn')
         try:
             if type(scorings) != list:
                 scorings = [scorings]
             skf = sklearn.model_selection.StratifiedKFold(n_splits=5, random_state=None, shuffle=True)
-            scores = {scoring: [] for scoring in scorings}
+            scores = {get_scoring_name(scoring): [] for scoring in scorings}
             for train_index, test_index in skf.split(X, y):
                 
                 X_test = X[test_index]
                 y_test = y[test_index]
                 
                 pl_copy = sklearn.base.clone(pl)
                 pl_copy.fit(X[train_index], y[train_index])
-                y_hat = pl_copy.predict(X[test_index])
-                y_prob = pl_copy.predict_proba(X[test_index])
-                labels = pl_copy.classes_
                 
                 # compute values for each metric
                 for scoring in scorings:
-                    scorer = get_scorer(scoring)
-                    is_predict_scorer = type(scorer) == sklearn.metrics._scorer._PredictScorer
-                    is_proba_scorer = type(scorer) == sklearn.metrics._scorer._ProbaScorer
-                    is_threshold_scorer = type(scorer) == sklearn.metrics._scorer._ThresholdScorer
-                    self.logger.debug(f"Now computing score for scoring function {scoring}. Predict scorer: {is_predict_scorer}, Proba sccorer: {is_proba_scorer}, Threshold scorer: {is_threshold_scorer}.")
-                    if is_predict_scorer:
-                        try:
-                            score = get_scorer(scoring)._score_func(y_test, y_hat)
-                        except:
-                            score = np.nan
-                    elif is_proba_scorer:
-                        try:
-                            score = get_scorer(scoring)._score_func(y_test, y_prob,labels=labels)
-                        except:
-                            score = np.nan
-                    elif is_threshold_scorer:
-                        try:
-                            if len(labels) == 2:
-                                score = get_scorer(scoring)._score_func(y_test, y_prob[:,1])
-                            else:
-                                score = get_scorer(scoring)._score_func(y_test, y_prob, labels=labels)
-                        except:
-                            score = np.nan
-                    else:
-                        raise Exception(f"Unsupported type {type(scorer)}")
-                    if not np.isnan(score) and scoring == "neg_log_loss":
-                        score *= -1
-                    scores[scoring].append(score)
+                    scorer = get_scorer(scoring) if type(scoring) == str else make_scorer(**{key: val for key, val in scoring.items() if key != "name"})
+                    try:
+                        score = scorer(pl_copy, X[test_index], y[test_index])
+                    except KeyboardInterrupt:
+                        raise
+                    except:
+                        score = np.nan
+                        
+                    scores[get_scoring_name(scoring)].append(score)
             return scores
+        except KeyboardInterrupt:
+            raise
         except Exception as e:
             if errors in ["message", "ignore"]:
                 if errors == "message":
                     self.logger.error(f"Observed an error: {e}")
                 return None
             else:
                 raise
 
     def evaluate(self, pl, timeout=None, deadline=None):
         if is_pipeline_forbidden(pl):
             self.logger.info(f"Preventing evaluation of forbidden pipeline {pl}")
-            return {scoring: np.nan for scoring in [self.scoring] + self.side_scores}
+            return {get_scoring_name(scoring): np.nan for scoring in [self.scoring] + self.side_scores}
         
         process = psutil.Process(os.getpid())
         self.logger.info(f"Initializing evaluation of {pl} with current memory consumption {int(process.memory_info().rss / 1024 / 1024)} MB. Now awaiting results.")
         
         start_outer = time.time()
         spl = str(pl)
         if spl in self.cache:
-            out = {scoring: np.nan for scoring in [self.scoring] + self.side_scores}
-            out[self.scoring] = np.round(np.mean(self.cache[spl][1]), 4)
+            out = {get_scoring_name(scoring): np.nan for scoring in [self.scoring] + self.side_scores}
+            out[get_scoring_name(self.scoring)] = np.round(np.mean(self.cache[spl][1]), 4)
             return out
         timestamp = time.time()
         if timeout is not None:
             scores = func_timeout(timeout, self.cross_validate, (pl, self.X, self.y, [self.scoring] + self.side_scores))
         else:
             scores = self.cross_validate(pl, self.X, self.y, [self.scoring] + self.side_scores)
         if scores is None:
-            return {scoring: np.nan for scoring in [self.scoring] + self.side_scores}
+            return {get_scoring_name(scoring): np.nan for scoring in [self.scoring] + self.side_scores}
         runtime = time.time() - start_outer
         self.logger.info(f"Completed evaluation of {spl} after {runtime}s. Scores are {scores}")
-        self.tellEvaluation(pl, scores[self.scoring], timestamp)
+        self.tellEvaluation(pl, scores[get_scoring_name(self.scoring)], timestamp)
         return {scoring: np.round(np.mean(scores[scoring]), 4) for scoring in scores}
 
     def getBestCandidate(self):
         return self.getBestCandidates(1)[0]
         
     def getBestCandidates(self, n):
         candidates = sorted([key for key in self.cache], key=lambda k: np.mean(self.cache[k][1]), reverse=True)
@@ -192,15 +178,15 @@
     else:
         raise ValueError("%s is not a bool" % str(p))
     
 def build_estimator(comp, params, X, y):
     
     if params is None:
         if get_class(comp["class"]) == sklearn.svm.SVC:
-            params = {"kernel": config_json.read(comp["params"]).get_hyperparameter("kernel").value}
+            params = {"kernel": config_json.read(json.dumps(comp["params"])).get_hyperparameter("kernel").value}
         else:
             return get_class(comp["class"])()
     
     return compile_pipeline_by_class_and_params(get_class(comp["class"]), params, X, y)
 
 
 def compile_pipeline_by_class_and_params(clazz, params, X, y):
@@ -285,14 +271,167 @@
             min_samples_split=min_samples_split,
             min_samples_leaf=min_samples_leaf,
             max_leaf_nodes=max_leaf_nodes,
             min_weight_fraction_leaf=min_weight_fraction_leaf,
             min_impurity_decrease=min_impurity_decrease,
             class_weight=None)
     
+    if clazz == sklearn.tree.DecisionTreeRegressor:
+        criterion = params["criterion"]
+        max_features = float(params["max_features"])
+        if check_none(params["max_depth_factor"]):
+            max_depth_factor = params["max_depth_factor"] = None
+        else:
+            num_features = X.shape[1]
+            max_depth_factor = int(params["max_depth_factor"])
+            max_depth_factor = max(
+                1, int(np.round(params["max_depth_factor"] * num_features, 0))
+            )
+        min_samples_split = int(params["min_samples_split"])
+        min_samples_leaf = int(params["min_samples_leaf"])
+        if check_none(params["max_leaf_nodes"]):
+            max_leaf_nodes = None
+        else:
+            max_leaf_nodes = int(params["max_leaf_nodes"])
+        min_weight_fraction_leaf = float(params["min_weight_fraction_leaf"])
+        min_impurity_decrease = float(params["min_impurity_decrease"])
+
+        return sklearn.tree.DecisionTreeRegressor(
+            criterion=criterion,
+            max_depth=max_depth_factor,
+            min_samples_split=min_samples_split,
+            min_samples_leaf=min_samples_leaf,
+            max_leaf_nodes=max_leaf_nodes,
+            min_weight_fraction_leaf=min_weight_fraction_leaf,
+            min_impurity_decrease=min_impurity_decrease
+        )
+    
+    if clazz == sklearn.ensemble.AdaBoostRegressor:
+        n_estimators = int(params["n_estimators"])
+        learning_rate = float(params["learning_rate"])
+        max_depth = int(params["max_depth"])
+        base_estimator = sklearn.tree.DecisionTreeRegressor(max_depth=max_depth)
+
+        return sklearn.ensemble.AdaBoostRegressor(
+            base_estimator=base_estimator,
+            n_estimators=n_estimators,
+            learning_rate=learning_rate,
+        )
+    
+    if clazz == sklearn.ensemble.ExtraTreesRegressor:
+        n_estimators = 10**3
+        if params["criterion"] not in ("mse", "friedman_mse", "mae"):
+            raise ValueError(
+                "'criterion' is not in ('mse', 'friedman_mse', "
+                "'mae): %s" % self.criterion
+            )
+
+        if check_none(params["max_depth"]):
+            max_depth = None
+        else:
+            max_depth = int(params["max_depth"])
+
+        if check_none(params["max_leaf_nodes"]):
+            max_leaf_nodes = None
+        else:
+            max_leaf_nodes = int(params["max_leaf_nodes"])
+
+        min_samples_leaf = int(params["min_samples_leaf"])
+        min_samples_split = int(params["min_samples_split"])
+        max_features = float(params["max_features"])
+        min_impurity_decrease = float(params["min_impurity_decrease"])
+        min_weight_fraction_leaf = float(params["min_weight_fraction_leaf"])
+        bootstrap = check_for_bool(params["bootstrap"])
+
+        return sklearn.ensemble.ExtraTreesRegressor(
+            n_estimators=n_estimators,
+            criterion=params["criterion"],
+            max_depth=max_depth,
+            min_samples_split=min_samples_split,
+            min_samples_leaf=min_samples_leaf,
+            bootstrap=bootstrap,
+            max_features=max_features,
+            max_leaf_nodes=max_leaf_nodes,
+            min_weight_fraction_leaf=min_weight_fraction_leaf,
+            min_impurity_decrease=min_impurity_decrease,
+            oob_score=False,
+            n_jobs=1
+        )
+    
+    if clazz == sklearn.gaussian_process.GaussianProcessRegressor:
+        alpha = float(params["alpha"])
+        thetaL = float(params["thetaL"])
+        thetaU = float(params["thetaU"])
+
+        #n_features = X.shape[1]
+        kernel = sklearn.gaussian_process.kernels.RBF(
+            #length_scale=[1.0] * n_features,
+            #length_scale_bounds=[(thetaL, thetaU)] * n_features,
+        )
+
+        # Instanciate a Gaussian Process model
+        return sklearn.gaussian_process.GaussianProcessRegressor(
+            kernel=kernel,
+            n_restarts_optimizer=10,
+            optimizer="fmin_l_bfgs_b",
+            alpha=alpha,
+            copy_X_train=True,
+            normalize_y=True,
+        )
+    
+    if clazz == sklearn.ensemble.HistGradientBoostingRegressor:
+        learning_rate = float(params["learning_rate"])
+        max_iter = 1000
+        min_samples_leaf = int(params["min_samples_leaf"])
+        if check_none(params["max_depth"]):
+            max_depth = None
+        else:
+            max_depth = int(params["max_depth"])
+        if check_none(params["max_leaf_nodes"]):
+            max_leaf_nodes = None
+        else:
+            max_leaf_nodes = int(params["max_leaf_nodes"])
+        max_bins = int(params["max_bins"])
+        l2_regularization = float(params["l2_regularization"])
+        tol = float(params["tol"])
+        if check_none(params["scoring"]):
+            scoring = None
+        else:
+            scoring = params["scoring"]
+            
+        if params["early_stop"] == "off":
+            n_iter_no_change = 0
+            validation_fraction_ = None
+        elif params["early_stop"] == "train":
+            n_iter_no_change = int(params["n_iter_no_change"])
+            validation_fraction_ = None
+        elif params["early_stop"] == "valid":
+            n_iter_no_change = int(params["n_iter_no_change"])
+            validation_fraction_ = float(params["validation_fraction"])
+        else:
+            raise ValueError("early_stop should be either off, train or valid")
+            
+        return sklearn.ensemble.HistGradientBoostingRegressor(
+            loss=params["loss"],
+            learning_rate=learning_rate,
+            max_iter=max_iter,
+            min_samples_leaf=min_samples_leaf,
+            max_depth=max_depth,
+            max_leaf_nodes=max_leaf_nodes,
+            max_bins=max_bins,
+            l2_regularization=l2_regularization,
+            tol=tol,
+            scoring=scoring,
+            n_iter_no_change=n_iter_no_change,
+            validation_fraction=validation_fraction_,
+            verbose=False,
+            warm_start=False,
+        )
+    
+    
     if clazz == sklearn.svm.LinearSVC:
         penalty = params["penalty"]
         loss = params["loss"]
         multi_class = params["multi_class"]
         C = float(params["C"])
         tol = float(params["tol"])
         dual = check_for_bool(params["dual"])
@@ -320,18 +459,220 @@
         else:
             coef0 = float(params["coef0"])
         tol = float(params["tol"])
         max_iter = float(params["max_iter"])
         shrinking = check_for_bool(params["shrinking"])
         
         return sklearn.svm.SVC(C=C, kernel=kernel,degree=degree,gamma=gamma,coef0=coef0,shrinking=shrinking,tol=tol, max_iter=max_iter, decision_function_shape='ovr', probability=True)
+
+    if clazz == sklearn.svm.LinearSVR:
+        C = float(params["C"])
+        tol = float(params["tol"])
+        epsilon = float(params["epsilon"])
+
+        dual = check_for_bool(params["dual"])
+        fit_intercept = check_for_bool(params["fit_intercept"])
+        intercept_scaling = float(params["intercept_scaling"])
+
+        return sklearn.svm.LinearSVR(
+            epsilon=epsilon,
+            loss=params["loss"],
+            dual=dual,
+            tol=tol,
+            C=C,
+            fit_intercept=fit_intercept,
+            intercept_scaling=intercept_scaling,
+        )
     
+    if clazz == sklearn.svm.SVR:
+        C = float(params["C"])
+        epsilon = float(params["epsilon"])
+        tol = float(params["tol"])
+        shrinking = check_for_bool(params["shrinking"])
+        degree = int(params["degree"]) if "degree" in params else 3
+        gamma = float(params["gamma"]) if "gamma" in params else 0.1
+        if not "coef0" in params or check_none(params["coef0"]):
+            coef0 = 0.0
+        else:
+            coef0 = float(params["coef0"])
+        max_iter = int(params["max_iter"])
+        
+        # Calculate the size of the kernel cache (in MB) for sklearn's LibSVM.
+        # The cache size is calculated as 2/3 of the available memory
+        # (which is calculated as the memory limit minus the used memory)
+        try:
+            # Retrieve memory limits imposed on the process
+            soft, hard = resource.getrlimit(resource.RLIMIT_AS)
+
+            if soft > 0:
+                # Convert limit to units of megabytes
+                soft /= 1024 * 1024
+
+                # Retrieve memory used by this process
+                maxrss = resource.getrusage(resource.RUSAGE_SELF)[2] / 1024
+
+                # In MacOS, the MaxRSS output of resource.getrusage in bytes;
+                # on other platforms, it's in kilobytes
+                if sys.platform == "darwin":
+                    maxrss = maxrss / 1024
+
+                cache_size = (soft - maxrss) / 1.5
+
+                if cache_size < 0:
+                    cache_size = 200
+            else:
+                cache_size = 200
+        except Exception:
+            cache_size = 200
+
+        return sklearn.svm.SVR(
+            kernel=params["kernel"],
+            C=C,
+            epsilon=epsilon,
+            tol=tol,
+            shrinking=shrinking,
+            degree=degree,
+            gamma=gamma,
+            coef0=coef0,
+            cache_size=cache_size
+        )
     
     
+    if clazz == sklearn.neural_network.MLPRegressor:
+        max_iter = 10**4
+        hidden_layer_depth = int(params["hidden_layer_depth"])
+        num_nodes_per_layer = int(params["num_nodes_per_layer"])
+        hidden_layer_sizes = tuple(
+            num_nodes_per_layer for i in range(hidden_layer_depth)
+        )
+        activation = str(params["activation"])
+        alpha = float(params["alpha"])
+        learning_rate_init = float(params["learning_rate_init"])
+        early_stopping = str(params["early_stopping"])
+        if params["early_stopping"] == "train":
+            validation_fraction = 0.0
+            tol = float(params["tol"])
+            n_iter_no_change = int(params["n_iter_no_change"])
+            early_stopping_val = False
+        elif params["early_stopping"] == "valid":
+            validation_fraction = float(params["validation_fraction"])
+            tol = float(params["tol"])
+            n_iter_no_change = int(params["n_iter_no_change"])
+            early_stopping_val = True
+        else:
+            raise ValueError(
+                "Set early stopping to unknown value %s" % self.early_stopping
+            )
+        # elif self.early_stopping == "off":
+        #     self.validation_fraction = 0
+        #     self.tol = 10000
+        #     self.n_iter_no_change = self.max_iter
+        #     self.early_stopping_val = False
+
+        solver = params["solver"]
+
+        try:
+            batch_size = int(params["batch_size"])
+        except ValueError:
+            batch_size = str(params["batch_size"])
+
+        shuffle = check_for_bool(params["shuffle"])
+        beta_1 = float(params["beta_1"])
+        beta_2 = float(params["beta_2"])
+        epsilon = float(params["epsilon"])
+        beta_1 = float(params["beta_1"])
+        
+
+        # initial fit of only increment trees
+        return sklearn.neural_network.MLPRegressor(
+            hidden_layer_sizes=hidden_layer_sizes,
+            activation=activation,
+            solver=solver,
+            alpha=alpha,
+            batch_size=batch_size,
+            learning_rate_init=learning_rate_init,
+            max_iter=max_iter,
+            shuffle=shuffle,
+            warm_start=False,
+            early_stopping=early_stopping_val,
+            validation_fraction=validation_fraction,
+            n_iter_no_change=n_iter_no_change,
+            tol=tol,
+            beta_1=beta_2,
+            beta_2=beta_1,
+            epsilon=epsilon,
+            # We do not use these, see comments below in search space
+            # momentum=self.momentum,
+            # nesterovs_momentum=self.nesterovs_momentum,
+            # power_t=self.power_t,
+            # learning_rate=self.learning_rate,
+            # max_fun=self.max_fun
+        )
     
+    if clazz == sklearn.ensemble.RandomForestRegressor:
+        n_estimators = 10**3
+        if check_none(params["max_depth"]):
+            max_depth = None
+        else:
+            max_depth = int(params["max_depth"])
+
+        min_samples_split = int(params["min_samples_split"])
+        min_samples_leaf = int(params["min_samples_leaf"])
+
+        max_features = float(params["max_features"])
+
+        bootstrap = check_for_bool(params["bootstrap"])
+
+        if check_none(params["max_leaf_nodes"]):
+            max_leaf_nodes = None
+        else:
+            max_leaf_nodes = int(params["max_leaf_nodes"])
+
+        min_impurity_decrease = float(params["min_impurity_decrease"])
+
+        return sklearn.ensemble.RandomForestRegressor(
+            n_estimators=n_estimators,
+            criterion=params["criterion"],
+            max_features=max_features,
+            max_depth=max_depth,
+            min_samples_split=min_samples_split,
+            min_samples_leaf=min_samples_leaf,
+            min_weight_fraction_leaf=params["min_weight_fraction_leaf"],
+            bootstrap=bootstrap,
+            max_leaf_nodes=max_leaf_nodes,
+            min_impurity_decrease=min_impurity_decrease,
+            warm_start=False,
+        )
+    
+    if clazz == sklearn.linear_model.SGDRegressor:
+        alpha = float(params["alpha"])
+        l1_ratio = float(params["l1_ratio"]) if "l1_ratio" in params else 0.15
+        epsilon = float(params["epsilon"]) if "epsilon" in params else 0.1
+        eta0 = float(params["eta0"]) if "eta0" in params else 0.1
+        power_t = float(params["power_t"]) if "power_t" in params else 0.25
+        average = check_for_bool(params["average"])
+        fit_intercept = check_for_bool(params["fit_intercept"])
+        tol = float(params["tol"])
+
+        return sklearn.linear_model.SGDRegressor(
+            loss=params["loss"],
+            penalty=params["penalty"],
+            alpha=alpha,
+            fit_intercept=fit_intercept,
+            tol=tol,
+            learning_rate=params["learning_rate"],
+            l1_ratio=l1_ratio,
+            epsilon=epsilon,
+            eta0=eta0,
+            power_t=power_t,
+            shuffle=True,
+            average=average,
+            warm_start=False,
+        )
+
     if clazz == sklearn.discriminant_analysis.LinearDiscriminantAnalysis:
         if params["shrinkage"] in (None, "none", "None"):
             shrinkage_ = None
             solver = 'svd'
         elif params["shrinkage"] == "auto":
             shrinkage_ = 'auto'
             solver = 'lsqr'
@@ -486,15 +827,14 @@
             min_weight_fraction_leaf=min_weight_fraction_leaf,
             bootstrap=bootstrap,
             max_leaf_nodes=max_leaf_nodes,
             min_impurity_decrease=min_impurity_decrease,
             warm_start=True)
     
     if clazz == sklearn.ensemble.GradientBoostingClassifier:
-        from sklearn.experimental import enable_hist_gradient_boosting  # noqa
         learning_rate = float(params["learning_rate"])
         max_iter = int(params["max_iter"]) if "max_iter" in params else 512
         min_samples_leaf = int(params["min_samples_leaf"])
         loss = params["loss"]
         scoring = params["scoring"]
         if check_none(params["max_depth"]):
             max_depth = None
@@ -667,15 +1007,15 @@
         self.index_in_steps = index_in_steps
         self.comp = comp
         self.X = X
         self.y = y
         self.mandatory_pre_processing = mandatory_pre_processing
         self.other_step_component_instances = other_step_component_instances
         self.execution_timeout = execution_timeout
-        config_space_as_string = comp["params"]
+        config_space_as_string = json.dumps(comp["params"])
         self.config_space = config_json.read(config_space_as_string)
         self.space_size = get_hyperparameter_space_size(self.config_space)
         self.eval_runtimes = []
         self.configs_since_last_imp = 0
         self.time_since_last_imp = 0
         self.evaled_configs = set([])
         self.active = self.space_size >= 1
@@ -728,15 +1068,15 @@
                 params[hp.name] = sampled_config[hp.name]
 
         # evaluate configured pipeline
         time_start_eval = time.time()
         scores = self.evalComp(params)
         if type(scores) != dict:
             raise ValueError(f"The scores must be a dictionary as a function of the scoring functions. Observed type is {type(scores)}: {scores}")
-        score = scores[self.scoring]
+        score = scores[get_scoring_name(self.scoring)]
         runtime = time.time() - time_start_eval
         self.eval_runtimes.append(runtime)
         self.logger.info(f"Observed score of {score} for {self.comp['class']} with params {params}")
         if score > self.best_score:
             self.logger.info("This is a NEW BEST SCORE!")
             self.best_score = score
             self.time_since_last_imp = 0
```

### Comparing `naiveautoml-0.0.8/naiveautoml/naiveautoml.py` & `naiveautoml-0.0.9/naiveautoml/naiveautoml.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,37 +22,21 @@
 from ConfigSpace.read_and_write import json as config_json
 
 # naiveautoml commons
 from naiveautoml.commons import *
 
 class NaiveAutoML:
 
-    def __init__(self, search_space = None, scoring = None, side_scores = None , num_cpus = 8, execution_timeout = 10, max_hpo_iterations = 100, timeout = None, standard_classifier=sklearn.neighbors.KNeighborsClassifier, logger_name = None, show_progress = False, opt_ordering = None, strictly_naive=False, sparse = False):
-        
-        ''' search_space is a string or a list of dictionaries
-            - if it is a dict, the last one for the learner and all the others for pre-processing. Each dictionary has an entry "name" and an entry "components", which is a list of components with their parameters.
-            - if it is a string, a json file with the name of search_space is read in with the same semantics
-         '''
-        if search_space is None or type(search_space) == str:
-            if search_space is None:
-                json_str = pkg_resources.read_text('naiveautoml', 'searchspace.json')
-                search_space = json.loads(json_str)
-            elif type(search_space) == str:
-                f = open(search_space)
-                search_space = json.load(f)
-            
-            # randomly shuffle elements in the search space
-            self.search_space = []
-            for step in search_space:
-                comps = step["components"]
-                random.shuffle(comps)
-                self.search_space.append(step)
-            
+    def __init__(self, search_space = None, scoring = None, side_scores = None , num_cpus = 8, execution_timeout = 10, max_hpo_iterations = 100, timeout = None, standard_classifier=sklearn.neighbors.KNeighborsClassifier, standard_regressor = sklearn.linear_model.LinearRegression(), logger_name = None, show_progress = False, opt_ordering = None, strictly_naive=False, sparse = False, task_type = "auto"):
+        if type(search_space) == str:
+            f = open(search_space)
+            self.search_space = json.load(f)
         else:
             self.search_space = search_space
+            
         self.scoring = scoring
         self.side_scores = side_scores
         self.num_cpus = num_cpus
         self.execution_timeout = execution_timeout
         self.max_hpo_iterations = max_hpo_iterations
         self.strictly_naive = strictly_naive
         self.timeout = timeout
@@ -63,35 +47,60 @@
         self.stage_entrypoints = {}
         self.standard_classifier = standard_classifier
         
         # mandatory pre-processing steps
         self.sparse = sparse # do one-hot encoding via sparse representations (default is False since this is not supported by all algorithms)
         self.mandatory_pre_processing = None
         
-        # define ordering of slots for optimization
-        if opt_ordering is None:
-            opt_ordering = ["classifier"]
-            for step in self.search_space:
-                if step["name"] != "classifier":
-                    opt_ordering.append(step["name"])
+        self.task_type = task_type
         self.opt_ordering = opt_ordering
-        
+
+                
         ## init logger
         self.logger_name = logger_name
         self.logger = logging.getLogger('naiveautoml' if logger_name is None else logger_name)
         
+
+    def get_task_type(self, X, y):
+        # infer task type
+        if self.task_type == "auto":
+            return "regression" if len(np.unique(y)) > 100 else "classification"
+        else:
+            return self.task_type
+        
+    def register_search_space(self, X, y):
+        
+
+        task_type = self.get_task_type(X, y)
+        self.logger.info(f"Automatically inferred task type: {task_type}")
+        
+        ''' search_space is a string or a list of dictionaries
+            - if it is a dict, the last one for the learner and all the others for pre-processing. Each dictionary has an entry "name" and an entry "components", which is a list of components with their parameters.
+            - if it is a string, a json file with the name of search_space is read in with the same semantics
+         '''
+        json_str = pkg_resources.read_text('naiveautoml', 'searchspace-' + task_type + '.json')
+        self.search_space = json.loads(json_str)
+        
+    def get_shuffled_version_of_search_space(self):
+        search_space = []
+        for step in self.search_space:
+            comps = step["components"].copy()
+            random.shuffle(comps)
+            search_space.append(step)
+        return search_space
+        
     def check_combinations(self, X, y):
         
         pool = EvaluationPool(X, y, self.scoring, self.side_scores)
         algorithms_per_stage = []
         names = []
         for step in self.search_space:
             names.append(step["name"])
             cands = []
-            if step["name"] != "classifier":
+            if step["name"] != "learner":
                 cands.append(None)
             cands.extend([get_class(comp["class"]) for comp in step["components"]])
             algorithms_per_stage.append(cands)
             
         for combo in it.product(*algorithms_per_stage):
             pl = sklearn.pipeline.Pipeline(steps=[(names[i], clazz()) for i, clazz in enumerate(combo) if clazz is not None])
             if is_pipeline_forbidden(pl):
@@ -111,20 +120,20 @@
         return steps
     
     def get_pipeline_for_decision_in_step(self, step_name, comp, X, y, decisions):
         
         if self.strictly_naive: ## strictly naive case
             
             # build pipeline to be evaluated here
-            if step_name == "classifier":
-                steps = [("classifier", build_estimator(comp, None, X, y))]
+            if step_name == "learner":
+                steps = [("learner", build_estimator(comp, None, X, y))]
             elif comp is None:
-                steps = [("classifier", self.standard_classifier())]
+                steps = [("learner", self.standard_classifier())]
             else:
-                steps = [(step_name, build_estimator(comp, None, X, y)), ("classifier", self.standard_classifier())]
+                steps = [(step_name, build_estimator(comp, None, X, y)), ("learner", self.standard_classifier())]
             return Pipeline(steps = self.mandatory_pre_processing + steps)
         
         else: ## semi-naive case (consider previous decisions)
             steps_tmp = [(s[0], build_estimator(s[1], None, X, y)) for s in decisions]
             if comp is not None:
                 steps_tmp.append((step_name, build_estimator(comp, None, X, y)))
             steps_ordered = []
@@ -154,23 +163,34 @@
         decisions = []
         components_with_score = {}
         
                 
         if self.show_progress:
             print("Progress for algorithm selection:")
             pbar = tqdm(total=sum([len(step["components"]) for step in self.search_space]))
+            
+        
+        # retrieve ordering of slots for optimization
+        if self.opt_ordering is None:
+            opt_ordering = ["learner"]
+            for step in self.search_space:
+                if step["name"] != "learner":
+                    opt_ordering.append(step["name"])
+        else:
+            opt_ordering = self.opt_ordering
+            
                 
-        for step_index, step_name in enumerate(self.opt_ordering):
+        for step_index, step_name in enumerate(opt_ordering):
             
             # create list of components to try for this slot
             step = [step for step in self.search_space if step["name"] == step_name][0]
             self.logger.info("--------------------------------------------------")
             self.logger.info(f"Selecting component for step with name: {step_name}")
             self.logger.info("--------------------------------------------------")
-            if not step_name in ["classifier"]:
+            if not step_name in ["learner"]:
                 components = [None] + step["components"]
             else:
                 components = step["components"]
             
             # find best default parametrization for this slot (depending on choice of previously configured slots)
             pool = EvaluationPool(X, y, self.scoring, self.side_scores, logger_name = None if self.logger_name is None else self.logger_name + ".pool")
             best_score = -np.inf
@@ -189,15 +209,15 @@
                 # get and evaluate pipeline for this step
                 pl = self.get_pipeline_for_decision_in_step(step_name, comp, X, y, decisions)
                 try:
                     scores = pool.evaluate(pl, min(self.execution_timeout, remaining_time if self.deadline is not None else 10**10))
                 except FunctionTimedOut:
                     self.logger.debug("TIMEOUT!")
                     scores = {scoring: np.nan for scoring in [self.scoring] + (self.side_scores if self.side_scores is not None else [])}
-                score = scores[self.scoring]
+                score = scores[get_scoring_name(self.scoring)]
                 self.logger.debug(f"Observed score of {score} for default configuration of {None if comp is None else comp['class']}")
                 
                 # update history
                 self.history.append({"time": time.time() - self.start_time, "pl": str(pl), "score_internal": score, "scores": scores, "new_best": score > self.best_score_overall})
                 
                 # update best score
                 if not np.isnan(score) and score > best_score:
@@ -211,14 +231,16 @@
                         self.pl = pl    
                     
                 # update progress bar
                 if self.show_progress:
                     pbar.update(1)
                     
             if decision is None:
+                if step_name == "learner":
+                    raise Exception("No learner was chosen in the initial phase. This is typically caused by too low timeouts or bugs in a custom scoring function (if applicable).")
                 self.logger.debug("No component chosen for this slot. Leaving it blank")
             else:
                 self.logger.debug(f"Added {decision['class']} as the decision for step {step_name}")
                 decisions.append((step_name, decision))
         
         # ordering decisions by their order in the pipeline
         decisions_tmp = [d for d in decisions]
@@ -246,18 +268,18 @@
         decisions = self.decisions
         components_with_score = self.components_with_score
         
         # create HPO processes for each slot, taking into account the default parametrized component of each other slot
         self.hpo_processes = hpo_processes = {}
         step_names = [d[0] for d in decisions]
         for step_name, comp in decisions:
-            if step_name == "classifier":
+            if step_name == "learner":
                 other_instances = [(step_name, None)]
             else:
-                other_instances = [(step_name, None), ("classifier", self.standard_classifier())]
+                other_instances = [(step_name, None), ("learner", self.standard_classifier())]
             index = 0 # it is (rather by coincidence) the first step we want to optimize
             hpo = HPOProcess(step_name, comp, X, y, self.scoring, self.side_scores, self.execution_timeout, self.mandatory_pre_processing, other_instances, index, 1800, 1000, allow_exhaustive_search = (self.max_hpo_iterations is None), logger_name =  None if self.logger_name is None else self.logger_name + ".hpo")
             hpo.best_score = components_with_score[step_name] # performance of default config
             hpo_processes[step_name] = hpo
         
         # starting HPO process
         opt_round = 1
@@ -284,25 +306,26 @@
             for name in active_for_optimization:
                 hpo = hpo_processes[name]
                 self.logger.debug(f"Stepping HPO for {name}")
                 try:
                     res = hpo.step(remaining_time)
                     if res is not None:
                         pl, scores, runtime = res
-                        score = scores[self.scoring]
+                        score = scores[get_scoring_name(self.scoring)]
                         if score > self.best_score_overall:
                             self.best_score_overall = score
                         self.history.append({"time": time.time() - self.start_time, "pl": str(pl), "score_internal": score, "scores": scores, "new_best": score > self.best_score_overall})
                         if not hpo.active:
                             self.logger.info(f"Deactivating {name}")
                             inactive.append(name)
                 except KeyboardInterrupt:
                     raise
                 except Exception as e:
                     self.logger.error(f"An error occurred in the HPO step: {e}")
+                    raise
                     
             round_runtimes.append(time.time() - round_start)
             for name in inactive:
                 active_for_optimization.remove(name)
             opt_round += 1
             newPl = self.build_pipeline(hpo_processes, X, y)
             if str(newPl) != str(self.pl):
@@ -316,24 +339,32 @@
         # close progress bar for HPO
         if self.show_progress:
             pbar.close()
         
 
     def fit(self, X, y):
         
+        # register search space
+        self.register_search_space(X, y)
+
         # initialize
         self.pl = None
         self.best_score_overall = -np.inf
         self.history = []
         self.start_time = time.time()
         self.deadline = self.start_time + self.timeout if self.timeout is not None else None
         self.sparse_training_data = type(X) == scipy.sparse.csr.csr_matrix or type(X) == scipy.sparse.lil.lil_matrix
         if self.scoring is None:
-            self.scoring = "roc_auc" if len(np.unique(y)) == 2 else "neg_log_loss"
-            
+            task_type = self.get_task_type(X, y)
+            print(task_type)
+            if task_type == "classification":
+                self.scoring = "roc_auc" if len(np.unique(y)) == 2 else "neg_log_loss"
+            else:
+                self.scoring = "neg_mean_squared_error"
+        
         # determine fixed pre-processing steps for imputation and binarization
         types = [set([type(v) for v in r]) for r in X.T]
         numeric_features = [c for c, t in enumerate(types) if len(t) == 1 and list(t)[0] != str]
         numeric_transformer = Pipeline([("imputer", sklearn.impute.SimpleImputer(strategy="median"))])
         categorical_features = [i for i in range(X.shape[1]) if i not in numeric_features]
         missing_values_per_feature = np.sum(pd.isnull(X), axis=0)
         self.logger.info(f"There are {len(categorical_features)} categorical features, which will be binarized.")
@@ -391,11 +422,12 @@
         pool = EvaluationPool(X, y, self.scoring, self.side_scores)
         scores = []
         for entry in self.history:
             scores.append(pool.evaluate(entry["pl"]))
         return scores
 
     def predict(self, X):
+        print(self.pl)
         return self.pl.predict(X)
     
     def predict_proba(self, X):
         return self.pl.predict_proba(X)
```

### Comparing `naiveautoml-0.0.8/setup.py` & `naiveautoml-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'naiveautoml',         # How you named your package folder (MyLib)
   packages = ['naiveautoml'],   # Chose the same as "name"
-  version = '0.0.8',      # Start with a small number and increase it with every change you make
+  version = '0.0.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'The official package for the Naive AutoML paper',   # Give a short description about your library
   author = 'Felix Mohr',                   # Type in your name
   author_email = 'mail@felixmohr.de',      # Type in your E-Mail
   url = 'https://github.com/fmohr/naiveautoml',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.4.tar.gz',
+  download_url = 'https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.9.tar.gz',
   keywords = ['AutoML', 'sklearn', 'naive', 'simple'],
   install_requires=[
           'numpy',
           'scikit-learn',
           'configspace',
           'scipy',
           'func_timeout',
```

