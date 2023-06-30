# Comparing `tmp/tune_sklearn-0.4.5-py3-none-any.whl.zip` & `tmp/tune_sklearn-0.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 41077 bytes, number of entries: 14
+Zip file size: 41916 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx      217 b- defN 21-Jul-05 20:33 tune_sklearn/__init__.py
 -rw-rw-r--  2.0 unx     1409 b- defN 21-Jul-05 20:33 tune_sklearn/_detect_booster.py
--rw-rw-r--  2.0 unx    18273 b- defN 22-Nov-14 19:22 tune_sklearn/_trainable.py
--rw-rw-r--  2.0 unx       23 b- defN 22-Nov-14 19:22 tune_sklearn/_version.py
+-rw-rw-r--  2.0 unx    21983 b- defN 23-Jun-30 21:27 tune_sklearn/_trainable.py
+-rw-rw-r--  2.0 unx       23 b- defN 23-Jun-30 21:34 tune_sklearn/_version.py
 -rw-rw-r--  2.0 unx     1543 b- defN 22-Oct-05 16:55 tune_sklearn/list_searcher.py
--rw-rw-r--  2.0 unx    35652 b- defN 22-Nov-14 19:22 tune_sklearn/tune_basesearch.py
+-rw-rw-r--  2.0 unx    36019 b- defN 23-Jun-30 21:27 tune_sklearn/tune_basesearch.py
 -rw-rw-r--  2.0 unx    14606 b- defN 22-Nov-14 19:22 tune_sklearn/tune_gridsearch.py
 -rw-rw-r--  2.0 unx    38240 b- defN 22-Nov-14 19:22 tune_sklearn/tune_search.py
--rw-rw-r--  2.0 unx    12616 b- defN 22-Oct-04 21:02 tune_sklearn/utils.py
--rw-rw-r--  2.0 unx    13079 b- defN 22-Nov-14 19:23 tune_sklearn-0.4.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx    11261 b- defN 22-Nov-14 19:23 tune_sklearn-0.4.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Nov-14 19:23 tune_sklearn-0.4.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 22-Nov-14 19:23 tune_sklearn-0.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1172 b- defN 22-Nov-14 19:23 tune_sklearn-0.4.5.dist-info/RECORD
-14 files, 148196 bytes uncompressed, 39135 bytes compressed:  73.6%
+-rw-rw-r--  2.0 unx    12616 b- defN 23-Jun-30 21:27 tune_sklearn/utils.py
+-rw-rw-r--  2.0 unx    13079 b- defN 23-Jun-30 21:35 tune_sklearn-0.4.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    11239 b- defN 23-Jun-30 21:35 tune_sklearn-0.4.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-30 21:35 tune_sklearn-0.4.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jun-30 21:35 tune_sklearn-0.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1172 b- defN 23-Jun-30 21:35 tune_sklearn-0.4.6.dist-info/RECORD
+14 files, 152251 bytes uncompressed, 39974 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: tune_sklearn/tune_search.py
 Comment: 
 
 Filename: tune_sklearn/utils.py
 Comment: 
 
-Filename: tune_sklearn-0.4.5.dist-info/LICENSE
+Filename: tune_sklearn-0.4.6.dist-info/LICENSE
 Comment: 
 
-Filename: tune_sklearn-0.4.5.dist-info/METADATA
+Filename: tune_sklearn-0.4.6.dist-info/METADATA
 Comment: 
 
-Filename: tune_sklearn-0.4.5.dist-info/WHEEL
+Filename: tune_sklearn-0.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: tune_sklearn-0.4.5.dist-info/top_level.txt
+Filename: tune_sklearn-0.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: tune_sklearn-0.4.5.dist-info/RECORD
+Filename: tune_sklearn-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tune_sklearn/_trainable.py

```diff
@@ -1,23 +1,33 @@
 """ Helper class to train models using Ray backend
 """
 from sklearn.model_selection import cross_validate
 from sklearn.utils.metaestimators import _safe_split
+from sklearn.model_selection._validation import _score, check_cv, is_classifier
 from sklearn.base import clone
 import numpy as np
 import os
 from pickle import PicklingError
 import warnings
+import traceback
 import inspect
 
 from ray.tune import Trainable
 import ray.cloudpickle as cpickle
 from tune_sklearn.utils import (EarlyStopping, _aggregate_score_dicts)
 
 
+def _replace_score_warning_details(warning: warnings.WarningMessage,
+                                   new_traceback: str):
+    idx = warning.message.args[0].find("Traceback")
+    if idx > -1:
+        message = warning.message.args[0][:idx] + new_traceback
+        warning.message.args = (message, ) + warning.message.args[1:]
+
+
 class _Trainable(Trainable):
     """Class to be passed in as the first argument of tune.run to train models.
 
     Overrides Ray Tune's Trainable class to specify the setup, train, save,
     and restore routines.
 
     """
@@ -52,27 +62,32 @@
 
         """
         self.early_stopping = config.pop("early_stopping")
         self.early_stop_type = config.pop("early_stop_type")
         self.groups = config.pop("groups")
         self.scoring = config.pop("scoring")
         self.max_iters = config.pop("max_iters")
-        self.cv = config.pop("cv")
         self.return_train_score = config.pop("return_train_score")
         self.n_jobs = config.pop("n_jobs")
         self.metric_name = config.pop("metric_name", "average_test_score")
+        self.error_score = config.pop("error_score", "raise")
         self.estimator_config = config
         self.train_accuracy = None
         self.test_accuracy = None
         self.saved_models = []  # XGBoost specific
 
         self.estimator_list = [
             clone(est) for est in self.original_estimator_list
         ]
 
+        self.cv = check_cv(
+            config.pop("cv"),
+            self.y,
+            classifier=is_classifier(self.main_estimator))
+
         if self.early_stopping:
             n_splits = self._setup_early_stopping()
 
             for i in range(n_splits):
                 self.estimator_list[i].set_params(**self.estimator_config)
 
             if self.early_stop_type in (EarlyStopping.XGB, EarlyStopping.LGBM,
@@ -173,51 +188,88 @@
         as well as the individual folds' accuracies as a dictionary.
 
         Returns:
             ret (:obj:`dict): Dictionary of results as a basis for
                 ``cv_results_`` for one of the cross-validation interfaces.
 
         """
+        fit_failed = False
         if self.early_stopping:
             for i, (train, test) in enumerate(
                     self.cv.split(self.X, self.y, groups=self.groups)):
                 estimator = self.estimator_list[i]
                 X_train, y_train = _safe_split(estimator, self.X, self.y,
                                                train)
                 X_test, y_test = _safe_split(
                     estimator, self.X, self.y, test, train_indices=train)
-                if self.early_stop_type == EarlyStopping.PARTIAL_FIT:
-                    self._early_stopping_partial_fit(i, estimator, X_train,
-                                                     y_train)
-                elif self.early_stop_type == EarlyStopping.XGB:
-                    self._early_stopping_xgb(i, estimator, X_train, y_train)
-                elif self.early_stop_type == EarlyStopping.LGBM:
-                    self._early_stopping_lgbm(i, estimator, X_train, y_train)
-                elif self.early_stop_type == EarlyStopping.CATBOOST:
-                    self._early_stopping_catboost(i, estimator, X_train,
+                bad_early_stop_type = False
+                fit_exception_traceback_str = None
+                try:
+                    if self.early_stop_type == EarlyStopping.PARTIAL_FIT:
+                        self._early_stopping_partial_fit(
+                            i, estimator, X_train, y_train)
+                    elif self.early_stop_type == EarlyStopping.XGB:
+                        self._early_stopping_xgb(i, estimator, X_train,
+                                                 y_train)
+                    elif self.early_stop_type == EarlyStopping.LGBM:
+                        self._early_stopping_lgbm(i, estimator, X_train,
                                                   y_train)
-                elif self.early_stop_type == EarlyStopping.WARM_START_ITER:
-                    self._early_stopping_iter(i, estimator, X_train, y_train)
-                elif self.early_stop_type == EarlyStopping.WARM_START_ENSEMBLE:
-                    self._early_stopping_ensemble(i, estimator, X_train,
+                    elif self.early_stop_type == EarlyStopping.CATBOOST:
+                        self._early_stopping_catboost(i, estimator, X_train,
+                                                      y_train)
+                    elif self.early_stop_type == EarlyStopping.WARM_START_ITER:
+                        self._early_stopping_iter(i, estimator, X_train,
                                                   y_train)
-                else:
+                    elif (self.early_stop_type ==
+                          EarlyStopping.WARM_START_ENSEMBLE):
+                        self._early_stopping_ensemble(i, estimator, X_train,
+                                                      y_train)
+                    else:
+                        bad_early_stop_type = True
+                except Exception as e:
+                    if self.error_score == "raise":
+                        raise e
+                    fit_failed = True
+                    fit_exception_traceback_str = traceback.format_exc()
+
+                if bad_early_stop_type:
                     raise RuntimeError(
                         "Early stopping set but model is not: "
                         "xgb model, supports partial fit, or warm-startable.")
 
-                if self.return_train_score:
-                    self.fold_train_scores[i] = {
-                        name: score(estimator, X_train, y_train)
-                        for name, score in self.scoring.items()
-                    }
-                self.fold_scores[i] = {
-                    name: score(estimator, X_test, y_test)
-                    for name, score in self.scoring.items()
-                }
+                # If fit_exception_traceback_str is set, the warnings raised
+                # by _score will have a NotFittedError, because
+                # the model couldn't have been fitted due to a fit error.
+                # We want to show the actual cause to the user, so we replace
+                # the traceback with the one stored in
+                # fit_exception_traceback_str.
+                with warnings.catch_warnings(record=True) as caught_warnings:
+                    if self.return_train_score:
+                        self.fold_train_scores[i] = _score(
+                            estimator,
+                            X_train,
+                            y_train,
+                            self.scoring,
+                            error_score=self.error_score)
+                        if fit_exception_traceback_str:
+                            _replace_score_warning_details(
+                                caught_warnings[-1],
+                                fit_exception_traceback_str)
+                    self.fold_scores[i] = _score(
+                        estimator,
+                        X_test,
+                        y_test,
+                        self.scoring,
+                        error_score=self.error_score)
+                    if fit_exception_traceback_str:
+                        _replace_score_warning_details(
+                            caught_warnings[-1], fit_exception_traceback_str)
+
+                for warning in caught_warnings:
+                    warnings.warn(warning.message)
 
             ret = {}
             agg_fold_scores = _aggregate_score_dicts(self.fold_scores)
             for name, scores in agg_fold_scores.items():
                 total = 0
                 for i, score in enumerate(scores):
                     total += score
@@ -235,39 +287,67 @@
                         total += score
                         key_str = f"split{i}_train_%s" % name
                         ret[key_str] = score
                     self.mean_train_score = total / len(scores)
                     ret["average_train_%s" % name] = self.mean_train_score
         else:
             try:
-                scores = cross_validate(
-                    self.main_estimator,
-                    self.X,
-                    self.y,
-                    cv=self.cv,
-                    n_jobs=self.n_jobs,
-                    fit_params=self.fit_params,
-                    groups=self.groups,
-                    scoring=self.scoring,
-                    return_train_score=self.return_train_score,
-                    error_score="raise")
-            except PicklingError:
-                warnings.warn("An error occurred in parallelizing the cross "
-                              "validation. Proceeding to cross validate with "
-                              "one core.")
-                scores = cross_validate(
-                    self.main_estimator,
-                    self.X,
-                    self.y,
-                    cv=self.cv,
-                    fit_params=self.fit_params,
-                    groups=self.groups,
-                    scoring=self.scoring,
-                    return_train_score=self.return_train_score,
-                    error_score="raise")
+                try:
+                    scores = cross_validate(
+                        self.main_estimator,
+                        self.X,
+                        self.y,
+                        cv=self.cv,
+                        n_jobs=self.n_jobs,
+                        fit_params=self.fit_params,
+                        groups=self.groups,
+                        scoring=self.scoring,
+                        return_train_score=self.return_train_score,
+                        error_score=self.error_score)
+                except PicklingError:
+                    warnings.warn(
+                        "An error occurred in parallelizing the cross "
+                        "validation. Proceeding to cross validate with "
+                        "one core.")
+                    scores = cross_validate(
+                        self.main_estimator,
+                        self.X,
+                        self.y,
+                        cv=self.cv,
+                        fit_params=self.fit_params,
+                        groups=self.groups,
+                        scoring=self.scoring,
+                        return_train_score=self.return_train_score,
+                        error_score=self.error_score)
+            except ValueError as e:
+                if ("It is very likely that your"
+                        "model is misconfigured") not in str(e):
+                    raise e
+                fit_failed = True
+
+            if fit_failed:
+                # If all folds fail, sklearn will raise an error, even
+                # if error_score is not set to "raise".
+                # We want to fail gracefully instead by setting
+                # everything to error score.
+                fake_test_scores = {
+                    f"test_{name}": [self.error_score] * self.cv.get_n_splits(
+                        self.X, self.y, self.groups)
+                    for name in self.scoring
+                }
+                if self.return_train_score:
+                    fake_train_scores = {
+                        f"train_{name}":
+                        [self.error_score] * self.cv.get_n_splits(
+                            self.X, self.y, self.groups)
+                        for name in self.scoring
+                    }
+                else:
+                    fake_train_scores = {}
+                scores = {**fake_test_scores, **fake_train_scores}
 
             ret = {}
             for name in self.scoring:
                 for i, score in enumerate(scores["test_%s" % name]):
                     key_str = f"split{i}_test_%s" % name
                     ret[key_str] = score
                 self.test_accuracy = sum(scores["test_%s" % name]) / len(
```

## tune_sklearn/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.4.5"
+__version__ = "0.4.6"
```

## tune_sklearn/tune_basesearch.py

```diff
@@ -523,14 +523,15 @@
         config["groups"] = groups
         config["cv"] = cv
         config["scoring"] = self.scoring_
         config["max_iters"] = self.max_iters
         config["return_train_score"] = self.return_train_score
         config["n_jobs"] = self.sk_n_jobs
         config["metric_name"] = self._metric_name
+        config["error_score"] = self.error_score
 
         self._fill_config_hyperparam(config)
         self.analysis_ = self._tune_run(X, y, config, resources_per_trial,
                                         tune_params, fit_params)
 
         self.cv_results_ = self._format_results(self.n_splits, self.analysis_)
 
@@ -541,15 +542,15 @@
             warnings.warn(
                 "Cannot refit estimator due to required data being missing "
                 "(probably due to trials not completing). `best_estimator` "
                 "will not be set.", UserWarning)
             return self
 
         # For multi-metric evaluation, store the best_index, best_params and
-        # best_score iff refit is one of the scorer names
+        # best_score if refit is one of the scorer names
         # In single metric evaluation, refit_metric is "score"
         if self.refit or not self._is_multi:
             # If callable, refit is expected to return the index of the best
             # parameter set.
             if callable(self.refit):
                 self.best_index = self.refit(self.cv_results_)
                 if not isinstance(self.best_index, numbers.Integral):
@@ -560,14 +561,19 @@
             else:
                 self.best_index = self.cv_results_[
                     f"rank_test_{base_metric}"].argmin()
                 self.best_score = self.cv_results_[f"mean_test_{base_metric}"][
                     self.best_index]
             best_config = self.analysis_.get_best_config(
                 metric=metric, mode="max", scope="last")
+            if best_config is None:
+                raise ValueError("Couldn't obtain best config. "
+                                 "This usually means that all trials "
+                                 "have failed. Set `error_score=\"raise\" "
+                                 "to debug the issue.")
             self.best_params = self._clean_config_dict(best_config)
 
         if self.refit:
             base_estimator = clone(self.estimator)
             if self.early_stop_type == EarlyStopping.WARM_START_ENSEMBLE:
                 logger.info("tune-sklearn uses `n_estimators` to warm "
                             "start, so this parameter can't be "
@@ -742,15 +748,15 @@
                 configurations without the output from ``tune.run``., Keys for
                 hyperparameters are the hyperparameter variable names
                 and the values are the numeric values set to those variables.
         """
         for key in [
                 "early_stopping", "groups", "cv", "scoring", "max_iters",
                 "return_train_score", "n_jobs", "metric_name",
-                "early_stop_type"
+                "early_stop_type", "error_score"
         ]:
             config.pop(key, None)
         return config
 
     def _format_results(self, n_splits, out):
         """Helper to generate the ``cv_results_`` dictionary.
```

## tune_sklearn/utils.py

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 from enum import Enum, auto
 from collections.abc import Sequence
 import inspect
 from ray.tune.logger import (Logger, JsonLoggerCallback, CSVLoggerCallback,
                              TBXLoggerCallback, LegacyLoggerCallback,
                              LoggerCallback)
-from ray.tune.integration.mlflow import MLflowLoggerCallback
+from ray.air.integrations.mlflow import MLflowLoggerCallback
 
 try:
     from ray.tune.stopper import MaximumIterationStopper
 except ImportError:
     from ray.tune.stopper import Stopper
 
     class MaximumIterationStopper(Stopper):
```

## Comparing `tune_sklearn-0.4.5.dist-info/LICENSE` & `tune_sklearn-0.4.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tune_sklearn-0.4.5.dist-info/METADATA` & `tune_sklearn-0.4.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: tune-sklearn
-Version: 0.4.5
+Version: 0.4.6
 Summary: A drop-in replacement for Scikit-Learn's GridSearchCV / RandomizedSearchCV with cutting edge hyperparameter tuning techniques.
 Home-page: https://github.com/ray-project/tune-sklearn
 Author: Michael Chau, Anthony Yu, and Ray Team
 Author-email: ray-dev@googlegroups.com
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: numpy (>=1.16)
+Requires-Dist: ray[tune] (>=2.0.0)
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
-Requires-Dist: ray[tune] (>=2.0.0)
-Requires-Dist: numpy (>=1.16)
 
 # tune-sklearn
 [![pytest](https://github.com/ray-project/tune-sklearn/workflows/Development/badge.svg)](https://github.com/ray-project/tune-sklearn/actions?query=workflow%3A%22Development%22)
 
 Tune-sklearn is a drop-in replacement for Scikit-Learn’s model selection module (GridSearchCV, RandomizedSearchCV) with cutting edge hyperparameter tuning techniques.
 
 ## Features
```

## Comparing `tune_sklearn-0.4.5.dist-info/RECORD` & `tune_sklearn-0.4.6.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 tune_sklearn/__init__.py,sha256=a2hHwQGdYpAo54HqAPVWiQ5jSIV4wIznzcV282PcYSA,217
 tune_sklearn/_detect_booster.py,sha256=ZkDua7Sn-oIpbArHJfiYGiO2TRkxSaP6dIpBBjfbsDc,1409
-tune_sklearn/_trainable.py,sha256=UQl9ACEsTE4v_eWTmC92KZ1a-v-j460hD46hrdn8fSk,18273
-tune_sklearn/_version.py,sha256=5sY1DeKiZH6JvK162uYsRRKgG3xiZNWUmMiarFZ4clI,23
+tune_sklearn/_trainable.py,sha256=0PJzCcmosAV5XpGM6pxL1akkkxXapIir2tdqGPSQVPs,21983
+tune_sklearn/_version.py,sha256=QlYINYptvwKWC16uojxmWEY3Q-AWi0Lc26uPWkTxKyk,23
 tune_sklearn/list_searcher.py,sha256=JLRREp-2iSTJlYA0BrUL-w8vFqhHNhgw8TMqueu7OHc,1543
-tune_sklearn/tune_basesearch.py,sha256=m3qrEghgQm84ryGK4s5izWdUsdpH7uZQdOh6HvZBxeI,35652
+tune_sklearn/tune_basesearch.py,sha256=Jfy8fnpNuugUxfwcyNXNGpYboFQ0PmyRcjesdPjYm2Q,36019
 tune_sklearn/tune_gridsearch.py,sha256=Z2h7ct_X6gZTM0qf_40-OcQSPa7fOgcHm5_w5Ds7ooE,14606
 tune_sklearn/tune_search.py,sha256=tovHbizKMUy4Yq85ZNT6GkHSUXBc3IdRlPoVNEOrKwM,38240
-tune_sklearn/utils.py,sha256=Z8mj71CsWCfAg8fTWoOyHT2UtnOWKWI9itejfGP_RK8,12616
-tune_sklearn-0.4.5.dist-info/LICENSE,sha256=uNZTUNFjvx1Tg5YPSH8-nQjJDCO-ZXdQFp_HjEkC-E8,13079
-tune_sklearn-0.4.5.dist-info/METADATA,sha256=GiqbOTVpFzNeGx4EvOQHA6ePJAoVSy1EWOqnQBaiwhQ,11261
-tune_sklearn-0.4.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-tune_sklearn-0.4.5.dist-info/top_level.txt,sha256=4q9SrVu-JeJwmz4JoRR4eGJmzSBsvHTqh60OXXSsVIw,13
-tune_sklearn-0.4.5.dist-info/RECORD,,
+tune_sklearn/utils.py,sha256=H_dSqWpUgnInFKZpdK0zUdgaSlBkVXHnGkv6H-Wa2Qc,12616
+tune_sklearn-0.4.6.dist-info/LICENSE,sha256=uNZTUNFjvx1Tg5YPSH8-nQjJDCO-ZXdQFp_HjEkC-E8,13079
+tune_sklearn-0.4.6.dist-info/METADATA,sha256=I7gzIq7GyZ6JslyyNFLm5Mq4ezba9MdcRHAWuui0m-o,11239
+tune_sklearn-0.4.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+tune_sklearn-0.4.6.dist-info/top_level.txt,sha256=4q9SrVu-JeJwmz4JoRR4eGJmzSBsvHTqh60OXXSsVIw,13
+tune_sklearn-0.4.6.dist-info/RECORD,,
```

