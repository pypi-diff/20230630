# Comparing `tmp/aisquared-0.3.6.dev0.tar.gz` & `tmp/aisquared-0.3.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisquared-0.3.6.dev0.tar", last modified: Wed Apr 19 16:49:30 2023, max compression
+gzip compressed data, was "aisquared-0.3.7.dev0.tar", last modified: Fri Jun 30 12:14:20 2023, max compression
```

## Comparing `aisquared-0.3.6.dev0.tar` & `aisquared-0.3.7.dev0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.488554 aisquared-0.3.6.dev0/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    19223 2023-04-19 16:49:30.488266 aisquared-0.3.6.dev0/PKG-INFO
--rw-r--r--   0 jwrenn4    (501) staff       (20)    18899 2023-04-19 16:47:20.000000 aisquared-0.3.6.dev0/README.md
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.456450 aisquared-0.3.6.dev0/aisquared/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      483 2023-04-19 16:46:40.000000 aisquared-0.3.6.dev0/aisquared/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.461121 aisquared-0.3.6.dev0/aisquared/base/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/base/BaseObject.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      756 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/base/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4473 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/base/css.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      581 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/base/endpoints.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      220 2023-02-24 19:53:35.000000 aisquared-0.3.6.dev0/aisquared/base/harvesting.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      119 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/base/platform.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      136 2023-02-24 19:53:35.000000 aisquared-0.3.6.dev0/aisquared/base/preprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      683 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/base/rendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      169 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/base/stages.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.462615 aisquared-0.3.6.dev0/aisquared/config/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1406 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/CustomObject.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8935 2023-04-19 16:44:10.000000 aisquared-0.3.6.dev0/aisquared/config/GraphConfiguration.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    21226 2023-04-19 16:46:21.000000 aisquared-0.3.6.dev0/aisquared/config/ModelConfiguration.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      451 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.464625 aisquared-0.3.6.dev0/aisquared/config/analytic/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2189 2023-02-20 17:59:37.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/DeployedAnalytic.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2226 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/DeployedModel.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1911 2023-02-20 18:21:49.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/LocalAnalytic.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1446 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/LocalModel.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3519 2023-03-24 17:10:38.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/ReverseMLWorkflow.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      316 2023-02-20 18:02:37.000000 aisquared-0.3.6.dev0/aisquared/config/analytic/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.466691 aisquared-0.3.6.dev0/aisquared/config/feedback/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1138 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/BinaryFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2771 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/ModelFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1131 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/MulticlassFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1921 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/QualitativeFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/RegressionFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      578 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/SimpleFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      395 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/feedback/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.468124 aisquared-0.3.6.dev0/aisquared/config/harvesting/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1100 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/ImageHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3285 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/InputHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2620 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/QueryParameterHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3510 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/TextHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      293 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/harvesting/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.469628 aisquared-0.3.6.dev0/aisquared/config/postprocessing/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1995 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/BinaryClassification.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1499 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/MulticlassClassification.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1816 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/ObjectDetection.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2094 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/Regression.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      322 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/postprocessing/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.469923 aisquared-0.3.6.dev0/aisquared/config/preprocessing/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      357 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.470930 aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1701 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/ImagePreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8268 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      186 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.471869 aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8761 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1563 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/TabularPreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      187 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.472916 aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    11803 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1740 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/TextPreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      175 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.478709 aisquared-0.3.6.dev0/aisquared/config/rendering/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4554 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/BarChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     6083 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/ContainerRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     9187 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/DashboardRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1889 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/DashboardReplacementRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4829 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/DocumentRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4524 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/DoughnutChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2666 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/FilterRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3683 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/HTMLTagRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4940 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/ImageRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4506 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/LineChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3884 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/ObjectRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4539 2023-02-10 15:11:26.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/PieChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1547 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/SOSRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2841 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/TableRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4377 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/WordRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      901 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      562 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/config/rendering/utils.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.479072 aisquared-0.3.6.dev0/aisquared/logging/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      271 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/logging/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.482609 aisquared-0.3.6.dev0/aisquared/platform/
--rw-r--r--   0 jwrenn4    (501) staff       (20)       49 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/AISquaredAPIException.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    46109 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/AISquaredPlatformClient.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)       47 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/NoResultsFoundError.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      375 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/platform/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      666 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/additional_utils.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3539 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/crudl.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3335 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/feedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2287 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/metrics.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3224 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/sharing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    13405 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/platform/user_group.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.483668 aisquared-0.3.6.dev0/aisquared/serving/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1323 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/serving/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4929 2023-03-31 18:41:55.000000 aisquared-0.3.6.dev0/aisquared/serving/deploy_model.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1587 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/serving/get_remote_prediction.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.484337 aisquared-0.3.6.dev0/aisquared/utils/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      459 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/aisquared/utils/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    10636 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/aisquared/utils/utils.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.457567 aisquared-0.3.6.dev0/aisquared.egg-info/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    19223 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/PKG-INFO
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3731 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/SOURCES.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)        1 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/dependency_links.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)      109 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/requires.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)       10 2023-04-19 16:49:30.000000 aisquared-0.3.6.dev0/aisquared.egg-info/top_level.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)       38 2023-04-19 16:49:30.488643 aisquared-0.3.6.dev0/setup.cfg
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1422 2023-02-24 19:53:35.000000 aisquared-0.3.6.dev0/setup.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-04-19 16:49:30.487880 aisquared-0.3.6.dev0/tests/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4320 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_air.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      853 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_analytics.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      958 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_base.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      341 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/tests/test_custom.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3578 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_feedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3490 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_harvesters.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1345 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_postprocessors.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1980 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_preprocessors.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    21527 2023-03-09 19:06:33.000000 aisquared-0.3.6.dev0/tests/test_renderers.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      107 2023-01-11 13:58:17.000000 aisquared-0.3.6.dev0/tests/test_simple.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.952237 aisquared-0.3.7.dev0/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19558 2023-06-30 12:14:20.951951 aisquared-0.3.7.dev0/PKG-INFO
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19234 2023-06-30 12:11:56.000000 aisquared-0.3.7.dev0/README.md
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.929644 aisquared-0.3.7.dev0/aisquared/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      483 2023-05-31 16:52:11.000000 aisquared-0.3.7.dev0/aisquared/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.933395 aisquared-0.3.7.dev0/aisquared/base/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/base/BaseObject.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      811 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/base/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3474 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/base/css.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      581 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/base/endpoints.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      220 2023-02-24 19:53:35.000000 aisquared-0.3.7.dev0/aisquared/base/harvesting.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      119 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/base/platform.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      136 2023-02-24 19:53:35.000000 aisquared-0.3.7.dev0/aisquared/base/preprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      683 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/base/rendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      169 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/base/stages.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.934408 aisquared-0.3.7.dev0/aisquared/config/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1406 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/CustomObject.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8935 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/GraphConfiguration.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    21366 2023-05-31 16:41:03.000000 aisquared-0.3.7.dev0/aisquared/config/ModelConfiguration.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      451 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.935751 aisquared-0.3.7.dev0/aisquared/config/analytic/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3293 2023-06-30 12:12:29.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/DeployedAnalytic.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2226 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/DeployedModel.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1911 2023-02-20 18:21:49.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/LocalAnalytic.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1446 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/LocalModel.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5569 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/ReverseMLWorkflow.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      316 2023-02-20 18:02:37.000000 aisquared-0.3.7.dev0/aisquared/config/analytic/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.937279 aisquared-0.3.7.dev0/aisquared/config/feedback/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1138 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/BinaryFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2771 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/ModelFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1131 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/MulticlassFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1921 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/QualitativeFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/RegressionFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      578 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/SimpleFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      395 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/feedback/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.938549 aisquared-0.3.7.dev0/aisquared/config/harvesting/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1100 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/ImageHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3285 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/InputHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2620 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/QueryParameterHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3510 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/TextHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      293 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/harvesting/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.939660 aisquared-0.3.7.dev0/aisquared/config/postprocessing/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1995 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/BinaryClassification.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1499 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/MulticlassClassification.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1816 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/ObjectDetection.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2094 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/Regression.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      322 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/postprocessing/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.939885 aisquared-0.3.7.dev0/aisquared/config/preprocessing/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      357 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.940657 aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1701 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/ImagePreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8268 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      186 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.941461 aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8761 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1563 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/TabularPreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      187 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.942128 aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    11803 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1740 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/TextPreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      175 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.945790 aisquared-0.3.7.dev0/aisquared/config/rendering/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5083 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/BarChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     6083 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/ContainerRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     9187 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/DashboardRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1889 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/DashboardReplacementRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4829 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/DocumentRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5053 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/DoughnutChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2666 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/FilterRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3683 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/HTMLTagRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4940 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/ImageRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5036 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/LineChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3884 2023-02-10 15:11:26.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/ObjectRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5068 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/PieChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1547 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/SOSRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2841 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/TableRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5031 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/WordRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      901 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      754 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/aisquared/config/rendering/utils.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.946023 aisquared-0.3.7.dev0/aisquared/logging/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      271 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/logging/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.948222 aisquared-0.3.7.dev0/aisquared/platform/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       49 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/AISquaredAPIException.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    46109 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/AISquaredPlatformClient.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       47 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/NoResultsFoundError.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      375 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/platform/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      666 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/additional_utils.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3539 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/crudl.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3335 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/feedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2287 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/metrics.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3224 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/sharing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    13405 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/platform/user_group.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.948843 aisquared-0.3.7.dev0/aisquared/serving/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1323 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/serving/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4929 2023-03-31 18:41:55.000000 aisquared-0.3.7.dev0/aisquared/serving/deploy_model.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1587 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/serving/get_remote_prediction.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.949368 aisquared-0.3.7.dev0/aisquared/utils/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      459 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/aisquared/utils/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    10636 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/aisquared/utils/utils.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.930961 aisquared-0.3.7.dev0/aisquared.egg-info/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19558 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/PKG-INFO
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3731 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/SOURCES.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)        1 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/dependency_links.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      108 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/requires.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       10 2023-06-30 12:14:20.000000 aisquared-0.3.7.dev0/aisquared.egg-info/top_level.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       38 2023-06-30 12:14:20.952297 aisquared-0.3.7.dev0/setup.cfg
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1422 2023-02-24 19:53:35.000000 aisquared-0.3.7.dev0/setup.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-06-30 12:14:20.951637 aisquared-0.3.7.dev0/tests/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4320 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_air.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1070 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_analytics.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      958 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/tests/test_base.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      341 2023-03-09 19:06:33.000000 aisquared-0.3.7.dev0/tests/test_custom.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3578 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/tests/test_feedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3490 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/tests/test_harvesters.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1345 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_postprocessors.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1980 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_preprocessors.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    22069 2023-05-30 14:21:20.000000 aisquared-0.3.7.dev0/tests/test_renderers.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      107 2023-01-11 13:58:17.000000 aisquared-0.3.7.dev0/tests/test_simple.py
```

### Comparing `aisquared-0.3.6.dev0/PKG-INFO` & `aisquared-0.3.7.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisquared
-Version: 0.3.6.dev0
+Version: 0.3.7.dev0
 Summary: Utilities for interacting with the AI Squared Technology Stack
 Home-page: https://github.com/AISquaredInc/aisquared
 Author: The AI Squared Team
 Author-email: staff@squared.ai
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: full
@@ -327,7 +327,14 @@
 
 ## Version 0.3.5
 - Changed `file_name` parameter in `ReverseMLWorkflow` to `file_names`
 - Added `documentation_link` parameter to `ModelConfiguration` class
 
 ## Version 0.3.6
 - Fixed issue with type checking for `ModelConfiguration` Rendering classes
+- Restricted TensorFlow version to below `2.12.0` to prevent import issues
+- Added `position` parameter to `WordRendering` class
+- Changed default CSS styling for rendering classes
+- Changed name of all `processor` classes to `processer`
+
+## Version 0.3.7
+- Changed schema of the `DeployedAnalytic` class to include API key management
```

### Comparing `aisquared-0.3.6.dev0/README.md` & `aisquared-0.3.7.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -316,7 +316,14 @@
 
 ## Version 0.3.5
 - Changed `file_name` parameter in `ReverseMLWorkflow` to `file_names`
 - Added `documentation_link` parameter to `ModelConfiguration` class
 
 ## Version 0.3.6
 - Fixed issue with type checking for `ModelConfiguration` Rendering classes
+- Restricted TensorFlow version to below `2.12.0` to prevent import issues
+- Added `position` parameter to `WordRendering` class
+- Changed default CSS styling for rendering classes
+- Changed name of all `processor` classes to `processer`
+
+## Version 0.3.7
+- Changed schema of the `DeployedAnalytic` class to include API key management
```

### Comparing `aisquared-0.3.6.dev0/aisquared/base/BaseObject.py` & `aisquared-0.3.7.dev0/aisquared/base/BaseObject.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/base/__init__.py` & `aisquared-0.3.7.dev0/aisquared/base/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 """
 
 from .BaseObject import BaseObject
 from .rendering import LOCATIONS, COLORS, BADGES, WORD_LISTS, QUALIFIERS, POSITIONS, STATIC_POSITIONS
 from .stages import ALLOWED_STAGES
 from .harvesting import ALLOWED_INPUT_TYPES, ALLOWED_HOWS
 from .preprocessing import ALLOWED_PADS
-from .css import DEFAULT_CONTAINER_RENDERING_CSS, DEFAULT_HTML_TAG_RENDERING_CSS, DEFAULT_TABLE_RENDERING_CSS, TABLE_RENDERING_CSS_FILE, HTML_TAG_RENDERING_CSS_FILE, CONTAINER_RENDERING_CSS_FILE, DIRECTORY
+from .css import DEFAULT_CONTAINER_RENDERING_CSS, DEFAULT_HTML_TAG_RENDERING_CSS, DEFAULT_TABLE_RENDERING_CSS, TABLE_RENDERING_CSS_FILE, HTML_TAG_RENDERING_CSS_FILE, CONTAINER_RENDERING_CSS_FILE, DEFAULT_CHART_RENDERING_CSS, CHART_RENDERING_CSS_FILE, DIRECTORY
 from .platform import CLIENT_CONFIG_FILE
 from .endpoints import ENDPOINTS
```

### Comparing `aisquared-0.3.6.dev0/aisquared/base/endpoints.py` & `aisquared-0.3.7.dev0/aisquared/base/endpoints.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/base/rendering.py` & `aisquared-0.3.7.dev0/aisquared/base/rendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/CustomObject.py` & `aisquared-0.3.7.dev0/aisquared/config/CustomObject.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/GraphConfiguration.py` & `aisquared-0.3.7.dev0/aisquared/config/GraphConfiguration.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/ModelConfiguration.py` & `aisquared-0.3.7.dev0/aisquared/config/ModelConfiguration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 from aisquared.base import BaseObject, ALLOWED_STAGES
 from .CustomObject import CustomObject
 from aisquared.config.harvesting import ImageHarvester, TextHarvester, InputHarvester, QueryParameterHarvester
-from aisquared.config.preprocessing.tabular import TabularPreprocessor
-from aisquared.config.preprocessing.image import ImagePreprocessor
-from aisquared.config.preprocessing.text import TextPreprocessor
+from aisquared.config.preprocessing.tabular import TabularPreprocesser
+from aisquared.config.preprocessing.image import ImagePreprocesser
+from aisquared.config.preprocessing.text import TextPreprocesser
 from aisquared.config.analytic import DeployedAnalytic, DeployedModel, LocalModel, LocalAnalytic, ReverseMLWorkflow
 from aisquared.config.postprocessing import BinaryClassification, MulticlassClassification, ObjectDetection, Regression
 from aisquared.config.rendering import ImageRendering, ObjectRendering, DocumentRendering, WordRendering, FilterRendering, ContainerRendering, HTMLTagRendering, DoughnutChartRendering, TableRendering, BarChartRendering, LineChartRendering, DashboardReplacementRendering, PieChartRendering, SOSRendering  # , DashboardRendering
 from aisquared.config.feedback import SimpleFeedback, BinaryFeedback, MulticlassFeedback, RegressionFeedback, ModelFeedback, QualitativeFeedback
 
 import tensorflowjs as tfjs
 import tensorflow as tf
@@ -21,17 +21,17 @@
     TextHarvester,
     InputHarvester,
     QueryParameterHarvester,
     CustomObject
 )
 
 PREPROCESSING_CLASSES = (
-    TabularPreprocessor,
-    ImagePreprocessor,
-    TextPreprocessor,
+    TabularPreprocesser,
+    ImagePreprocesser,
+    TextPreprocesser,
     CustomObject
 )
 
 ANALYTIC_CLASSES = (
     DeployedAnalytic,
     DeployedModel,
     LocalModel,
@@ -209,15 +209,15 @@
             self._preprocessing_steps = value
         elif isinstance(value, list) and all([isinstance(val, list) for val in value]) and all([isinstance(v, PREPROCESSING_CLASSES) for val in value for v in val]):
             self._preprocessing_steps = value
         elif value is None:
             self._preprocessing_steps = value
         else:
             raise ValueError(
-                'preprocessing_steps must a single Preprocessor object, a list of Preprocessor objects, or a list of list of preprocessor objects')
+                'preprocessing_steps must a single Preprocesser object, a list of Preprocesser objects, or a list of list of preprocesser objects')
 
     # analytic
     @property
     def analytic(self):
         return self._analytic
 
     @analytic.setter
@@ -565,15 +565,18 @@
             for f in filenames:
                 if os.path.splitext(f)[-1] == '.h5':
                     model = tf.keras.models.load_model(f)
                     model_dir = os.path.join(dirname, os.path.split(f)[-1])
                     tfjs.converters.save_keras_model(
                         model, model_dir, quantization_dtype_map=dtype_map)
                 else:
-                    shutil.copy(f, dirname)
+                    if os.path.isdir(f):
+                        shutil.copytree(f, os.path.join(dirname, f))
+                    else:
+                        shutil.copy(f, dirname)
 
         # go through the entire directory of dirname, grab all files, and make
         # the archive file
         shutil.make_archive(filename, 'zip', dirname)
 
         # Move the archive file to just have .air
         shutil.move(filename + '.zip', filename)
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/analytic/DeployedAnalytic.py` & `aisquared-0.3.7.dev0/aisquared/config/analytic/DeployedModel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from aisquared.base import BaseObject
 
 
-class DeployedAnalytic(BaseObject):
+class DeployedModel(BaseObject):
     """
-    Interaction with a remote analytic
+    Interaction with a remote model
 
     Example usage:
 
     >>> import aisquared
-    >>> analytic = aisquared.config.analytic.DeployedAnalytic(
-        'analytic_url',
+    >>> analytic = aisquared.config.analytic.DeployedModel(
+        'model_url',
         'text'
     )
     >>> analytic.to_dict()
-    {'className': 'DeployedAnalytic',
-    'params': {'url': 'analytic_url',
+    {'className': 'DeployedModel',
+    'params': {'url': 'model_url',
     'inputType': 'text',
     'secret': 'request',
     'header': None}}
+
     """
 
     def __init__(
         self,
         url: str,
         input_type: str,
         secret: str = 'request',
         header: dict = None
     ):
         """
         Parameters
         ----------
         url : str
-            The base URL for the remote analytic
+            The base URL for the remote endpoint
         input_type : str
-            The input types supplied to the analytic. Either one of 'cv', 'text', or 'tabular'
+            The input type to the model. Either one of 'cv', 'text', or 'tabular'
         secret : str (default 'request')
             The secret key used to interact with the service. Default value of 'request'
             indicates that the user inputs the key whenever the analytic is started again
         header : dict or None (default None)
             Header to use when calling the endpoint
         """
         super().__init__()
@@ -75,16 +76,19 @@
         return self._header
 
     @header.setter
     def header(self, value):
         self._header = value
 
     def to_dict(self) -> dict:
+        """
+        Get the config object as a dictionary
+        """
         return {
-            'className': 'DeployedAnalytic',
+            'className': 'DeployedModel',
             'params': {
                 'url': self.url,
                 'inputType': self.input_type,
                 'secret': self.secret,
                 'header': self.header
             }
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/analytic/DeployedModel.py` & `aisquared-0.3.7.dev0/aisquared/config/analytic/LocalModel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,66 @@
 from aisquared.base import BaseObject
 
 
-class DeployedModel(BaseObject):
+class LocalModel(BaseObject):
     """
-    Interaction with a remote model
+    Interaction with a model currently saved to the local
+    file system
 
     Example usage:
 
     >>> import aisquared
-    >>> analytic = aisquared.config.analytic.DeployedModel(
-        'model_url',
+    >>> analytic = aisquared.config.analytic.LocalModel(
+        'model_path',
         'text'
     )
     >>> analytic.to_dict()
-    {'className': 'DeployedModel',
-    'params': {'url': 'model_url',
-    'inputType': 'text',
-    'secret': 'request',
-    'header': None}}
+    {'className': 'LocalModel',
+    'params': {'path': 'model_path',
+    'inputType': 'text'}}
 
     """
 
     def __init__(
         self,
-        url: str,
-        input_type: str,
-        secret: str = 'request',
-        header: dict = None
+        path: str,
+        input_type: str
     ):
         """
         Parameters
         ----------
-        url : str
-            The base URL for the remote endpoint
+        path : str or path-like or file-like
+            The file path of the saved model
         input_type : str
-            The input type to the model. Either one of 'cv', 'text', or 'tabular'
-        secret : str (default 'request')
-            The secret key used to interact with the service. Default value of 'request'
-            indicates that the user inputs the key whenever the analytic is started again
-        header : dict or None (default None)
-            Header to use when calling the endpoint
+            Input type to the model. Must be one of 'cv', 'text', or 'tabular'
         """
         super().__init__()
-        self.url = url
+        self.path = path
         self.input_type = input_type
-        self.secret = secret
-        self.header = header
 
     @property
-    def url(self):
-        return self._url
+    def path(self):
+        return self._path
 
-    @url.setter
-    def url(self, value):
-        self._url = value
+    @path.setter
+    def path(self, value):
+        self._path = value
 
     @property
     def input_type(self):
         return self._input_type
 
     @input_type.setter
     def input_type(self, value):
         self._input_type = value
 
-    @property
-    def secret(self):
-        return self._secret
-
-    @secret.setter
-    def secret(self, value):
-        self._secret = value
-
-    @property
-    def header(self):
-        return self._header
-
-    @header.setter
-    def header(self, value):
-        self._header = value
-
     def to_dict(self) -> dict:
         """
-        Get the config object as a dictionary
+        Get the configuration object as a dictionary
         """
         return {
-            'className': 'DeployedModel',
+            'className': 'LocalModel',
             'params': {
-                'url': self.url,
-                'inputType': self.input_type,
-                'secret': self.secret,
-                'header': self.header
+                'path': self.path,
+                'inputType': self.input_type
             }
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/analytic/LocalAnalytic.py` & `aisquared-0.3.7.dev0/aisquared/config/analytic/LocalAnalytic.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/analytic/ReverseMLWorkflow.py` & `aisquared-0.3.7.dev0/aisquared/config/analytic/ReverseMLWorkflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,38 +27,46 @@
 
     def __init__(
         self,
         bucket: str,
         filenames: list,
         column: str,
         input_type: str,
+        filter_type: str,
+        filter_by_columns: list = None,
         period: int = None,
         secret: str = ''
     ):
         """
         Parameters
         ----------
         bucket : str
             The bucket the file lives in
         filenames : list of str
             The names for any specific files
         column : str
             The column name in the CSV file
         input_type : str
             Either one of 'text' or 'cv'
+        filter_type : str
+            The filter type
+        filter_by_columns : str
+            How to filter the columns of the ReverseMLWorkflow
         period : None or int (default None)
             The period for this to run
         secret : str (default '')
             A secret, if needed
         """
         super().__init__()
         self.bucket = bucket
         self.filenames = filenames
         self.column = column
         self.input_type = input_type
+        self.filter_type = filter_type
+        self.filter_by_columns = filter_by_columns
         self.period = period
         self.secret = secret
 
     @property
     def bucket(self):
         return self._bucket
 
@@ -97,14 +105,60 @@
         return self._input_type
 
     @input_type.setter
     def input_type(self, value):
         self._input_type = value
 
     @property
+    def filter_type(self):
+        return self._filter_type
+
+    @filter_type.setter
+    def filter_type(self, value):
+        if not isinstance(value, str):
+            raise TypeError('filter_type must be str')
+        self._filter_type = value
+
+    @property
+    def filter_by_columns(self):
+        return self._filter_by_columns
+
+    @filter_by_columns.setter
+    def filter_by_columns(self, value):
+        if not isinstance(value, list):
+            raise TypeError('filter_by_columns must be list')
+        if not all([isinstance(v, dict) for v in value]):
+            raise TypeError('All items in filter_by_columns must be dict')
+
+        def _check_item(v):
+            if 'inputType' not in v.keys():
+                raise ValueError(
+                    'All items in filter_by_columns must have "inputType" key')
+
+            if v['inputType'] not in v.keys():
+                if 'columnValue' not in v.keys():
+                    raise ValueError(
+                        'All items in filter_by_columns must have "columnValue" key if "inputType" is "static"')
+
+            if 'columnName' not in v.keys():
+                raise ValueError(
+                    'All items in filter_by_columns must have "columnName" ke')
+
+            if v['inputType'] not in ['group', 'input', 'static']:
+                raise ValueError(
+                    f'"inputType" must be one of "group", "input", or "static", got {v["inputType"]}')
+
+            return True
+
+        if not all([_check_item(v) for v in value]):
+            raise ValueError('Not all items pass validation')
+
+        self._filter_by_columns = value
+
+    @property
     def period(self):
         return self._period
 
     @period.setter
     def period(self, value):
         if value is not None:
             if not isinstance(value, int):
@@ -127,12 +181,14 @@
         """
         return {
             'className': 'ReverseMLWorkflow',
             'params': {
                 'bucket': self.bucket,
                 'fileNames': self.filenames,
                 'inputType': self.input_type,
+                'filterType': self.filter_type,
                 'column': self.column,
                 'period': self.period,
-                'secret': self.secret
+                'secret': self.secret,
+                'filterByColumns': self.filter_by_columns
             }
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/feedback/BinaryFeedback.py` & `aisquared-0.3.7.dev0/aisquared/config/feedback/BinaryFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/feedback/ModelFeedback.py` & `aisquared-0.3.7.dev0/aisquared/config/feedback/ModelFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/feedback/MulticlassFeedback.py` & `aisquared-0.3.7.dev0/aisquared/config/feedback/MulticlassFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/feedback/QualitativeFeedback.py` & `aisquared-0.3.7.dev0/aisquared/config/feedback/QualitativeFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/feedback/RegressionFeedback.py` & `aisquared-0.3.7.dev0/aisquared/config/feedback/RegressionFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/feedback/SimpleFeedback.py` & `aisquared-0.3.7.dev0/aisquared/config/feedback/SimpleFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/harvesting/ImageHarvester.py` & `aisquared-0.3.7.dev0/aisquared/config/harvesting/ImageHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/harvesting/InputHarvester.py` & `aisquared-0.3.7.dev0/aisquared/config/harvesting/InputHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/harvesting/QueryParameterHarvester.py` & `aisquared-0.3.7.dev0/aisquared/config/harvesting/QueryParameterHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/harvesting/TextHarvester.py` & `aisquared-0.3.7.dev0/aisquared/config/harvesting/TextHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/postprocessing/BinaryClassification.py` & `aisquared-0.3.7.dev0/aisquared/config/postprocessing/BinaryClassification.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/postprocessing/MulticlassClassification.py` & `aisquared-0.3.7.dev0/aisquared/config/postprocessing/MulticlassClassification.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/postprocessing/ObjectDetection.py` & `aisquared-0.3.7.dev0/aisquared/config/postprocessing/ObjectDetection.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/postprocessing/Regression.py` & `aisquared-0.3.7.dev0/aisquared/config/postprocessing/Regression.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/ImagePreprocessing.py` & `aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/ImagePreprocessing.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     MultiplyValue,
     DivideValue,
     ConvertToColor,
     Resize
 )
 
 
-class ImagePreprocessor(BaseObject):
+class ImagePreprocesser(BaseObject):
     """
-    Preprocessor object for image data
+    Preprocesser object for image data
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.image.AddValue(255.0)
     )
     """
 
     def __init__(
             self,
@@ -47,24 +47,24 @@
         else:
             return [
                 step.to_dict() for step in self.steps
             ]
 
     def add_step(self, step):
         """
-        Add a step to the preprocessor object
+        Add a step to the preprocesser object
         """
         if not isinstance(step, ALLOWED_STEPS):
             raise TypeError(f'Each step must be one of {ALLOWED_STEPS}')
         if self.steps is None:
             self.steps = [step]
         else:
             self.steps = self.steps + [step]
 
     def to_dict(self) -> dict:
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'ImagePreprocessor',
+            'className': 'ImagePreprocesser',
             'steps': self.step_dict
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/preprocessing/image/Steps.py` & `aisquared-0.3.7.dev0/aisquared/config/preprocessing/image/Steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class AddValue(BaseObject):
     """
     Preprocessing step to add a value to all pixels in an image
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.image.AddValue(255.0)
     )
     """
 
     def __init__(
             self,
@@ -53,15 +53,15 @@
 class SubtractValue(BaseObject):
     """
     Preprocessing step to subtract a value from all pixels in an image
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.image.SubtractValue(255.0)
     )
     """
 
     def __init__(
             self,
@@ -101,15 +101,15 @@
 class MultiplyValue(BaseObject):
     """
     Preprocessing step to multiply all pixels in an image by a value
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.image.MultiplyValue(2.0)
     )
     """
 
     def __init__(
             self,
@@ -149,15 +149,15 @@
 class DivideValue(BaseObject):
     """
     Preprocessing step to divide all pixels in an image by a value
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.image.DivideValue(255.0)
     )
     """
 
     def __init__(
             self,
@@ -197,15 +197,15 @@
 class ConvertToColor(BaseObject):
     """
     Preprocessing step to convert images to a color scheme
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.image.ConvertToColor('RGB')
     )
     """
 
     def __init__(self, color: str):
         """
@@ -242,15 +242,15 @@
 
 
 class Resize(BaseObject):
     """
     Preprocessing step to resize an image
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.image.ImagePreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.image.Resize([100, 100])
     )
     """
 
     def __init__(
             self,
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/Steps.py` & `aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/Steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     Z-Score normalization takes each supplied column value, subtracts that column's provided mean, and divides
     by the provided standard deviation.
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.tabular.ZScore(
             [0, 1, 2],
             [0.2, 0.4, 0.6]
         )
     )
     """
@@ -103,15 +103,15 @@
 
     Min-Max Scaling takes all associated columns and maps values relative to the minimum and maximum values
     of the training data.
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.tabular.MinMax(
             [0, 1.1, 2],
             [0.2, 14, 18.3]
         )
     )
     """
@@ -198,15 +198,15 @@
 class OneHot(BaseObject):
     """
     One Hot encoding preprocessing step
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.tabular.OneHot(
             6,
             ['one', 'two', 'three']
         )
     )
     """
@@ -265,15 +265,15 @@
 class DropColumn(BaseObject):
     """
     Drop a column from tabular data
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.tabular.DropColumn(
             3
         )
     )
     """
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/preprocessing/tabular/TabularPreprocessing.py` & `aisquared-0.3.7.dev0/aisquared/config/preprocessing/tabular/TabularPreprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,24 @@
     ZScore,
     MinMax,
     OneHot,
     DropColumn
 )
 
 
-class TabularPreprocessor(BaseObject):
+class TabularPreprocesser(BaseObject):
     """
-    Preprocessor object for tabular data
+    Preprocesser object for tabular data
 
     Example usage:
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.tabular.TabularPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.tabular.ZScore(
             [0, 1, 2],
             [0.2, 0.4, 0.6]
         )
     )
     """
@@ -31,36 +31,36 @@
             self,
             steps: list = None
     ):
         """
         Parameters
         ----------
         steps : list or None (default None)
-            List of preprocessor steps for tabular data
+            List of preprocesser steps for tabular data
         """
         super().__init__()
         self.steps = None
         if steps is not None:
             for step in steps:
                 self.add_step(step)
 
     def add_step(self, step):
         """
-        Add a step to the preprocessor object
+        Add a step to the preprocesser object
         """
         if not isinstance(step, ALLOWED_STEPS):
             raise TypeError(f'Each step must be one of {ALLOWED_STEPS}')
         if self.steps is None:
             self.steps = [step]
         else:
             self.steps = self.steps + [step]
 
     def to_dict(self):
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'TabularPreprocessor',
+            'className': 'TabularPreprocesser',
             'steps': [
                 step.to_dict() for step in self.steps
             ]
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/Steps.py` & `aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/Steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class Tokenize(BaseObject):
     """Preprocessing Step to tokenize text
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.text.Tokenize()
     )
 
     """
 
     def __init__(
@@ -82,15 +82,15 @@
 
 class RemoveCharacters(BaseObject):
     """Preprocessing step to remove characters from text
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.text.RemoveCharacters()
     )
     """
 
     def __init__(
         self,
@@ -144,15 +144,15 @@
 
 class ConvertToCase(BaseObject):
     """Text preprocessing object to convert inputs to all lowercase or all uppercase
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.text.ConvertToCase()
     )
     """
 
     def __init__(
         self,
@@ -191,15 +191,15 @@
 
 class ConvertToVocabulary(BaseObject):
     """Text preprocessing object to convert tokens to integer vocabularies
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.text.ConvertToVocabulary(
             {
                 'test' : 3,
                 'vocabulary' : 4
             }
         )
@@ -293,15 +293,15 @@
 
 class PadSequences(BaseObject):
     """Text preprocessing object to pad sequences
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.text.PadSequences()
     )
     """
 
     def __init__(
         self,
@@ -394,15 +394,15 @@
 
 class Trim(BaseObject):
     """Text preprocessing class to trim whitespace from text
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.text.Trim()
     )
     """
 
     def __init__(self):
         super().__init__()
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/preprocessing/text/TextPreprocessing.py` & `aisquared-0.3.7.dev0/aisquared/config/preprocessing/text/TextPreprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     ConvertToCase,
     ConvertToVocabulary,
     PadSequences,
     Trim
 )
 
 
-class TextPreprocessor(BaseObject):
+class TextPreprocesser(BaseObject):
     """
-    Preprocessor object for natural language
+    Preprocesser object for natural language
 
     Example usage:
 
     >>> import aisquared
-    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocessor()
+    >>> preprocesser = aisquared.config.preprocessing.text.TextPreprocesser()
     >>> preprocesser.add_step(
         aisquared.config.preprocessing.text.Tokenize()
     )
     """
 
     def __init__(
             self,
@@ -47,24 +47,24 @@
         else:
             return [
                 step.to_dict() for step in self.steps
             ]
 
     def add_step(self, step):
         """
-        Add a step to the preprocessor object
+        Add a step to the preprocesser object
         """
         if not isinstance(step, ALLOWED_STEPS):
             raise TypeError(f'Each step must be one of {ALLOWED_STEPS}')
         if self.steps is None:
             self.steps = [step]
         else:
             self.steps = self.steps + [step]
 
     def to_dict(self) -> dict:
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'TextPreprocessor',
+            'className': 'TextPreprocesser',
             'steps': self.step_dict
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/BarChartRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/PieChartRendering.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-from aisquared.base import BaseObject
+from aisquared.base import BaseObject, DEFAULT_CHART_RENDERING_CSS, CHART_RENDERING_CSS_FILE
+import json
+import os
 
 
-class BarChartRendering(BaseObject):
-
+class PieChartRendering(BaseObject):
     """
-    Rendering class for rendering a Bar Chart
+    Rendering class for rendering a Pie Chart
 
     Example usage:
 
     >>> import aisquared
-    >>> my_obj = aisquared.config.rendering.BarChartRendering(
-        'my_label',
-        'my_id',
-        'my_bar_chart',
-        'my_container_id',
-        'name',
-        'value',
-        'name_value',
-        True,
-        'circle'
-    )
+    >>> my_obj = aisquared.config.rendering.PieChartRendering(
+            'my_label',
+            'my_id',
+            'my_doughnut_chart',
+            'my_container_id',
+            'name',
+            'value',
+            'name_value',
+            True,
+            'circle'
+        )
     >>> my_obj.to_dict()
-    {'className': 'BarChartRendering',
-        'label': 'my_label',
-        'params': {'id': 'my_id',
-        'chartName': 'my_bar_chart',
-        'containerId': 'my_container_id',
-        'displayLegend': True,
-        'legendIcon': 'circle',
-        'width': 'auto',
-        'height': 'auto',
-        'xOffset': '0',
-        'yOffset': '0',
-        'datasource': [{'labels': None,
-            'labelsKey': None,
-            'consolidateRows': True,
-            'predictionNameKey': 'name',
-            'predictionValueKey': 'value',
-            'predictionNameValue': 'name_value'}]}}
+    {'className': 'PieChartRendering',
+    'label': 'my_label',
+    'params': {'id': 'my_id',
+    'chartName': 'my_doughnut_chart',
+    'containerId': 'my_container_id',
+    'displayLegend': True,
+    'legendIcon': 'circle',
+    'width': 'auto',
+    'height': 'auto',
+    'xOffset': '0',
+    'yOffset': '0',
+    'datasource': [{'labels': None,
+        'labelsKey': None,
+        'consolidateRows': True,
+        'predictionNameKey': 'name',
+        'predictionValueKey': 'value',
+        'predictionNameValue': 'name_value'}]}}
+
     """
 
     def __init__(
         self,
         label: str,
         id: str,
         chart_name: str,
@@ -53,16 +55,16 @@
         legend_icon: str,
         labels_key: str = None,
         width: str = 'auto',
         height: str = 'auto',
         xOffset: str = '0',
         yOffset: str = '0',
         labels: list = None,
-        consolidate_rows: bool = True
-
+        consolidate_rows: bool = True,
+        css_params: dict = None
     ):
         """
         Parameters
         ----------
         label : str
             The label for the chart
         id : str
@@ -91,15 +93,16 @@
             The offset on the x axis
         yOffset : str (default '0')
             The offset on the y axis
         labels : list of str or None (default None)
             Labels, if hard-coded
         consolidate_rows : bool (default True)
             Whether to consolidate rows in the data
-
+        css_params : dict or None (default None)
+            Additional CSS parameters
         """
         super().__init__()
         self.label = label
         self.id = id
         self.chart_name = chart_name
         self.labels = labels
         self.container_id = container_id
@@ -111,20 +114,27 @@
         self.width = width
         self.height = height
         self.xOffset = xOffset
         self.yOffset = yOffset
         self.consolidate_rows = consolidate_rows
         self.labels_key = labels_key
 
+        if css_params is None:
+            if os.path.exists(CHART_RENDERING_CSS_FILE):
+                with open(CHART_RENDERING_CSS_FILE, 'r') as f:
+                    self.css_params = json.load(f)
+            else:
+                self.css_params = DEFAULT_CHART_RENDERING_CSS
+
     def to_dict(self) -> dict:
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'BarChartRendering',
+            'className': 'PieChartRendering',
             'label': self.label,
             'params': {
                 'id': self.id,
                 'chartName': self.chart_name,
                 'containerId': self.container_id,
                 'displayLegend': self.display_legend,
                 'legendIcon': self.legend_icon,
@@ -135,12 +145,13 @@
                 'datasource': [
                     {
                         'labels': self.labels,
                         'labelsKey': self.labels_key,
                         'consolidateRows': self.consolidate_rows,
                         'predictionNameKey': self.prediction_name_key,
                         'predictionValueKey': self.prediction_value_key,
-                        'predictionNameValue': self.prediction_name_value,
+                        'predictionNameValue': self.prediction_name_value
                     }
-                ]
+                ],
+                'style': self.css_params['style']
             }
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/ContainerRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/ContainerRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/DashboardRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/DashboardRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/DashboardReplacementRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/DashboardReplacementRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/DocumentRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/DocumentRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/DoughnutChartRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/LineChartRendering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-from aisquared.base import BaseObject
+from aisquared.base import BaseObject, DEFAULT_CHART_RENDERING_CSS, CHART_RENDERING_CSS_FILE
+import json
+import os
 
 
-class DoughnutChartRendering(BaseObject):
+class LineChartRendering(BaseObject):
+
     """
-    Rendering class for rendering a Doughnut Chart
+    Rendering class for rendering a Line Chart
 
     Example usage:
 
     >>> import aisquared
-    >>> my_obj = aisquared.config.rendering.DoughnutChartRendering(
+    >>> my_obj = aisquared.config.rendering.LineChartRendering(
         'my_label',
         'my_id',
-        'my_doughnut_chart',
+        'my_line_chart',
         'my_container_id',
         'name',
         'value',
         'name_value',
         True,
-        'circle'
+        'circle',
+        'labels'
     )
     >>> my_obj.to_dict()
-    {'className': 'DoughnutChartRendering',
+    {'className': 'LineChartRendering',
     'label': 'my_label',
     'params': {'id': 'my_id',
-    'chartName': 'my_doughnut_chart',
+    'chartName': 'my_line_chart',
     'containerId': 'my_container_id',
     'displayLegend': True,
     'legendIcon': 'circle',
     'width': 'auto',
     'height': 'auto',
     'xOffset': '0',
     'yOffset': '0',
     'datasource': [{'labels': None,
-        'labelsKey': None,
+        'labelsKey': 'labels',
         'consolidateRows': True,
         'predictionNameKey': 'name',
         'predictionValueKey': 'value',
         'predictionNameValue': 'name_value'}]}}
 
     """
 
@@ -47,22 +51,22 @@
         chart_name: str,
         container_id: str,
         prediction_name_key: str,
         prediction_value_key: str,
         prediction_name_value: str,
         display_legend: bool,
         legend_icon: str,
-        labels_key: str = None,
+        labels_key: str,
         width: str = 'auto',
         height: str = 'auto',
         xOffset: str = '0',
         yOffset: str = '0',
         labels: list = None,
-        consolidate_rows: bool = True
-
+        consolidate_rows: bool = True,
+        css_params: dict = None
     ):
         """
         Parameters
         ----------
         label : str
             The label for the chart
         id : str
@@ -74,15 +78,15 @@
         prediction_name_key : str
             The key to use for the prediction name
         prediction_value_key : str
             The key to use for the prediction value
         prediction_name_value : str
             The value to use for the prediction name
         display_legend : bool
-            Whether to display the chart legend
+            Whether to display the legend
         legend_icon : str
             The legend icon to display
         labels_key : str
             The key to use for the labels
         width : str (default 'auto')
             The width of the chart
         height : str (default 'auto')
@@ -91,40 +95,48 @@
             The offset on the x axis
         yOffset : str (default '0')
             The offset on the y axis
         labels : list of str or None (default None)
             Labels, if hard-coded
         consolidate_rows : bool (default True)
             Whether to consolidate rows in the data
-
+        css_params : dict or None (default None)
+            Additional CSS parameters
         """
         super().__init__()
         self.label = label
         self.id = id
         self.chart_name = chart_name
-        self.labels = labels
         self.container_id = container_id
         self.prediction_name_key = prediction_name_key
         self.prediction_value_key = prediction_value_key
         self.prediction_name_value = prediction_name_value
         self.display_legend = display_legend
         self.legend_icon = legend_icon
         self.width = width
         self.height = height
         self.xOffset = xOffset
         self.yOffset = yOffset
         self.consolidate_rows = consolidate_rows
         self.labels_key = labels_key
+        self.labels = labels
+
+        if css_params is None:
+            if os.path.exists(CHART_RENDERING_CSS_FILE):
+                with open(CHART_RENDERING_CSS_FILE, 'r') as f:
+                    self.css_params = json.load(f)
+            else:
+                self.css_params = DEFAULT_CHART_RENDERING_CSS
 
     def to_dict(self) -> dict:
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'DoughnutChartRendering',
+            'className': 'LineChartRendering',
             'label': self.label,
             'params': {
                 'id': self.id,
                 'chartName': self.chart_name,
                 'containerId': self.container_id,
                 'displayLegend': self.display_legend,
                 'legendIcon': self.legend_icon,
@@ -135,12 +147,13 @@
                 'datasource': [
                     {
                         'labels': self.labels,
                         'labelsKey': self.labels_key,
                         'consolidateRows': self.consolidate_rows,
                         'predictionNameKey': self.prediction_name_key,
                         'predictionValueKey': self.prediction_value_key,
-                        'predictionNameValue': self.prediction_name_value
+                        'predictionNameValue': self.prediction_name_value,
                     }
-                ]
+                ],
+                'style': self.css_params['style']
             }
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/FilterRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/FilterRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/HTMLTagRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/HTMLTagRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/ImageRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/ImageRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/LineChartRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/BarChartRendering.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from aisquared.base import BaseObject
+from aisquared.base import BaseObject, DEFAULT_CHART_RENDERING_CSS, CHART_RENDERING_CSS_FILE
+import json
+import os
 
 
-class LineChartRendering(BaseObject):
+class BarChartRendering(BaseObject):
 
     """
-    Rendering class for rendering a Line Chart
+    Rendering class for rendering a Bar Chart
 
     Example usage:
 
     >>> import aisquared
-    >>> my_obj = aisquared.config.rendering.LineChartRendering(
+    >>> my_obj = aisquared.config.rendering.BarChartRendering(
         'my_label',
         'my_id',
-        'my_line_chart',
+        'my_bar_chart',
         'my_container_id',
         'name',
         'value',
         'name_value',
         True,
-        'circle',
-        'labels'
+        'circle'
     )
     >>> my_obj.to_dict()
-    {'className': 'LineChartRendering',
-    'label': 'my_label',
-    'params': {'id': 'my_id',
-    'chartName': 'my_line_chart',
-    'containerId': 'my_container_id',
-    'displayLegend': True,
-    'legendIcon': 'circle',
-    'width': 'auto',
-    'height': 'auto',
-    'xOffset': '0',
-    'yOffset': '0',
-    'datasource': [{'labels': None,
-        'labelsKey': 'labels',
-        'consolidateRows': True,
-        'predictionNameKey': 'name',
-        'predictionValueKey': 'value',
-        'predictionNameValue': 'name_value'}]}}
-
+    {'className': 'BarChartRendering',
+        'label': 'my_label',
+        'params': {'id': 'my_id',
+        'chartName': 'my_bar_chart',
+        'containerId': 'my_container_id',
+        'displayLegend': True,
+        'legendIcon': 'circle',
+        'width': 'auto',
+        'height': 'auto',
+        'xOffset': '0',
+        'yOffset': '0',
+        'datasource': [{'labels': None,
+            'labelsKey': None,
+            'consolidateRows': True,
+            'predictionNameKey': 'name',
+            'predictionValueKey': 'value',
+            'predictionNameValue': 'name_value'}]}}
     """
 
     def __init__(
         self,
         label: str,
         id: str,
         chart_name: str,
         container_id: str,
         prediction_name_key: str,
         prediction_value_key: str,
         prediction_name_value: str,
         display_legend: bool,
         legend_icon: str,
-        labels_key: str,
+        labels_key: str = None,
         width: str = 'auto',
         height: str = 'auto',
         xOffset: str = '0',
         yOffset: str = '0',
         labels: list = None,
-        consolidate_rows: bool = True
-
+        consolidate_rows: bool = True,
+        css_params: dict = None
     ):
         """
         Parameters
         ----------
         label : str
             The label for the chart
         id : str
@@ -76,15 +76,15 @@
         prediction_name_key : str
             The key to use for the prediction name
         prediction_value_key : str
             The key to use for the prediction value
         prediction_name_value : str
             The value to use for the prediction name
         display_legend : bool
-            Whether to display the legend
+            Whether to display the chart legend
         legend_icon : str
             The legend icon to display
         labels_key : str
             The key to use for the labels
         width : str (default 'auto')
             The width of the chart
         height : str (default 'auto')
@@ -93,39 +93,49 @@
             The offset on the x axis
         yOffset : str (default '0')
             The offset on the y axis
         labels : list of str or None (default None)
             Labels, if hard-coded
         consolidate_rows : bool (default True)
             Whether to consolidate rows in the data
+        css_params: dict or None (default None)
+            Additional CSS parameters
+
         """
         super().__init__()
         self.label = label
         self.id = id
         self.chart_name = chart_name
+        self.labels = labels
         self.container_id = container_id
         self.prediction_name_key = prediction_name_key
         self.prediction_value_key = prediction_value_key
         self.prediction_name_value = prediction_name_value
         self.display_legend = display_legend
         self.legend_icon = legend_icon
         self.width = width
         self.height = height
         self.xOffset = xOffset
         self.yOffset = yOffset
         self.consolidate_rows = consolidate_rows
         self.labels_key = labels_key
-        self.labels = labels
+
+        if css_params is None:
+            if os.path.exists(CHART_RENDERING_CSS_FILE):
+                with open(CHART_RENDERING_CSS_FILE, 'r') as f:
+                    self.css_params = json.load(f)
+            else:
+                self.css_params = DEFAULT_CHART_RENDERING_CSS
 
     def to_dict(self) -> dict:
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'LineChartRendering',
+            'className': 'BarChartRendering',
             'label': self.label,
             'params': {
                 'id': self.id,
                 'chartName': self.chart_name,
                 'containerId': self.container_id,
                 'displayLegend': self.display_legend,
                 'legendIcon': self.legend_icon,
@@ -138,10 +148,11 @@
                         'labels': self.labels,
                         'labelsKey': self.labels_key,
                         'consolidateRows': self.consolidate_rows,
                         'predictionNameKey': self.prediction_name_key,
                         'predictionValueKey': self.prediction_value_key,
                         'predictionNameValue': self.prediction_name_value,
                     }
-                ]
+                ],
+                'style': self.css_params['style']
             }
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/ObjectRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/ObjectRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/PieChartRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/DoughnutChartRendering.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from aisquared.base import BaseObject
+from aisquared.base import BaseObject, DEFAULT_CHART_RENDERING_CSS, CHART_RENDERING_CSS_FILE
+import json
+import os
 
 
-class PieChartRendering(BaseObject):
+class DoughnutChartRendering(BaseObject):
     """
-    Rendering class for rendering a Pie Chart
+    Rendering class for rendering a Doughnut Chart
 
     Example usage:
 
     >>> import aisquared
-    >>> my_obj = aisquared.config.rendering.PieChartRendering(
-            'my_label',
-            'my_id',
-            'my_doughnut_chart',
-            'my_container_id',
-            'name',
-            'value',
-            'name_value',
-            True,
-            'circle'
-        )
+    >>> my_obj = aisquared.config.rendering.DoughnutChartRendering(
+        'my_label',
+        'my_id',
+        'my_doughnut_chart',
+        'my_container_id',
+        'name',
+        'value',
+        'name_value',
+        True,
+        'circle'
+    )
     >>> my_obj.to_dict()
-    {'className': 'PieChartRendering',
+    {'className': 'DoughnutChartRendering',
     'label': 'my_label',
     'params': {'id': 'my_id',
     'chartName': 'my_doughnut_chart',
     'containerId': 'my_container_id',
     'displayLegend': True,
     'legendIcon': 'circle',
     'width': 'auto',
@@ -53,16 +55,16 @@
         legend_icon: str,
         labels_key: str = None,
         width: str = 'auto',
         height: str = 'auto',
         xOffset: str = '0',
         yOffset: str = '0',
         labels: list = None,
-        consolidate_rows: bool = True
-
+        consolidate_rows: bool = True,
+        css_params: dict = None
     ):
         """
         Parameters
         ----------
         label : str
             The label for the chart
         id : str
@@ -91,14 +93,16 @@
             The offset on the x axis
         yOffset : str (default '0')
             The offset on the y axis
         labels : list of str or None (default None)
             Labels, if hard-coded
         consolidate_rows : bool (default True)
             Whether to consolidate rows in the data
+        css_params: dict or None (default None)
+            Additional CSS parameters
 
         """
         super().__init__()
         self.label = label
         self.id = id
         self.chart_name = chart_name
         self.labels = labels
@@ -111,20 +115,27 @@
         self.width = width
         self.height = height
         self.xOffset = xOffset
         self.yOffset = yOffset
         self.consolidate_rows = consolidate_rows
         self.labels_key = labels_key
 
+        if css_params is None:
+            if os.path.exists(CHART_RENDERING_CSS_FILE):
+                with open(CHART_RENDERING_CSS_FILE, 'r') as f:
+                    self.css_params = json.load(f)
+            else:
+                self.css_params = DEFAULT_CHART_RENDERING_CSS
+
     def to_dict(self) -> dict:
         """
         Get the configuration object as a dictionary
         """
         return {
-            'className': 'PieChartRendering',
+            'className': 'DoughnutChartRendering',
             'label': self.label,
             'params': {
                 'id': self.id,
                 'chartName': self.chart_name,
                 'containerId': self.container_id,
                 'displayLegend': self.display_legend,
                 'legendIcon': self.legend_icon,
@@ -137,10 +148,11 @@
                         'labels': self.labels,
                         'labelsKey': self.labels_key,
                         'consolidateRows': self.consolidate_rows,
                         'predictionNameKey': self.prediction_name_key,
                         'predictionValueKey': self.prediction_value_key,
                         'predictionNameValue': self.prediction_name_value
                     }
-                ]
+                ],
+                'style': self.css_params['style']
             }
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/SOSRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/SOSRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/TableRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/TableRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/WordRendering.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/WordRendering.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,30 @@
     'params': {'wordList': 'input',
     'resultKey': None,
     'contentKey': None,
     'badgeShape': 'star',
     'badgeColor': 'blue',
     'classes': None,
     'thresholdKey': None,
-    'thresholdValue': None}}
+    'thresholdValue': None
+    'position': 'after'}}
 
     """
 
     def __init__(
             self,
             word_list: str = WORD_LISTS[0],
             result_key: str = None,
             content_key: str = None,
             badge_shape: str = BADGES[-2],
             badge_color: str = 'blue',
             classes: list = None,
             threshold_key: str = None,
-            threshold_value: Union[int, float] = None
+            threshold_value: Union[int, float] = None,
+            position: str = 'after'
     ):
         """
         Parameters
         ----------
         word_list : str (default 'input')
             How to identify words to render, must be one of 'input', 'result'
         results_key : str or None (default None)
@@ -49,24 +51,27 @@
             The badge color to use
         classes : None or list (default None)
             If provided, list of classes that will be rendered
         threshold_key : None or string (default None)
             If provided, the key to look for to threshold
         theshold_value : None or numeric (default None)
             If provided with threshold_key, the minimum value required to render
+        position : str (default 'after')
+            The position of the rendering widget, either 'before' or 'after'
         """
         super().__init__()
         self.word_list = word_list
         self.result_key = result_key
         self.content_key = content_key
         self.badge_shape = badge_shape
         self.badge_color = badge_color
         self.classes = classes
         self.threshold_key = threshold_key
         self.threshold_value = threshold_value
+        self.position = position
 
     @property
     def word_list(self):
         return self._word_list
 
     @word_list.setter
     def word_list(self, value):
@@ -129,24 +134,38 @@
     def threshold_value(self):
         return self._threshold_value
 
     @threshold_value.setter
     def threshold_value(self, value):
         self._threshold_value = value
 
+    @property
+    def position(self):
+        return self._position
+
+    @position.setter
+    def position(self, value):
+        if not isinstance(value, str):
+            raise TypeError('position must be string')
+        if value not in ['before', 'after']:
+            raise ValueError(
+                f'position must be either "before" or "after", got {value}')
+        self._position = value
+
     def to_dict(self) -> dict:
         """
         Get the configuration object as a dictionary
         """
         return {
             'className': 'WordRendering',
             'params': {
                 'wordList': self.word_list,
                 'resultKey': self.result_key,
                 'contentKey': self.content_key,
                 'badgeShape': self.badge_shape,
                 'badgeColor': self.badge_color,
                 'classes': self.classes,
                 'thresholdKey': self.threshold_key,
-                'thresholdValue': self.threshold_value
+                'thresholdValue': self.threshold_value,
+                'position': self.position
             }
         }
```

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/__init__.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/config/rendering/utils.py` & `aisquared-0.3.7.dev0/aisquared/config/rendering/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 from aisquared.base import DEFAULT_CONTAINER_RENDERING_CSS, DEFAULT_HTML_TAG_RENDERING_CSS, DEFAULT_TABLE_RENDERING_CSS, CONTAINER_RENDERING_CSS_FILE, HTML_TAG_RENDERING_CSS_FILE, TABLE_RENDERING_CSS_FILE
 import json
 
 
 def save_default_css():
+    """
+    Save default CSS so that default CSS can be edited and automatically utilized with changes
+
+    Notes
+    -----
+    - Saves all CSS files to the `~/.aisquared/` directory
+    """
+
     with open(CONTAINER_RENDERING_CSS_FILE, 'w') as f:
         json.dump(DEFAULT_CONTAINER_RENDERING_CSS, f)
 
     with open(HTML_TAG_RENDERING_CSS_FILE, 'w') as f:
         json.dump(DEFAULT_HTML_TAG_RENDERING_CSS, f)
 
     with open(TABLE_RENDERING_CSS_FILE, 'w') as f:
```

### Comparing `aisquared-0.3.6.dev0/aisquared/platform/AISquaredPlatformClient.py` & `aisquared-0.3.7.dev0/aisquared/platform/AISquaredPlatformClient.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/platform/additional_utils.py` & `aisquared-0.3.7.dev0/aisquared/platform/additional_utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/platform/crudl.py` & `aisquared-0.3.7.dev0/aisquared/platform/crudl.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/platform/feedback.py` & `aisquared-0.3.7.dev0/aisquared/platform/feedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/platform/metrics.py` & `aisquared-0.3.7.dev0/aisquared/platform/metrics.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/platform/sharing.py` & `aisquared-0.3.7.dev0/aisquared/platform/sharing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/platform/user_group.py` & `aisquared-0.3.7.dev0/aisquared/platform/user_group.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/serving/__init__.py` & `aisquared-0.3.7.dev0/aisquared/serving/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/serving/deploy_model.py` & `aisquared-0.3.7.dev0/aisquared/serving/deploy_model.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/serving/get_remote_prediction.py` & `aisquared-0.3.7.dev0/aisquared/serving/get_remote_prediction.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared/utils/utils.py` & `aisquared-0.3.7.dev0/aisquared/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/aisquared.egg-info/PKG-INFO` & `aisquared-0.3.7.dev0/aisquared.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisquared
-Version: 0.3.6.dev0
+Version: 0.3.7.dev0
 Summary: Utilities for interacting with the AI Squared Technology Stack
 Home-page: https://github.com/AISquaredInc/aisquared
 Author: The AI Squared Team
 Author-email: staff@squared.ai
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: full
@@ -327,7 +327,14 @@
 
 ## Version 0.3.5
 - Changed `file_name` parameter in `ReverseMLWorkflow` to `file_names`
 - Added `documentation_link` parameter to `ModelConfiguration` class
 
 ## Version 0.3.6
 - Fixed issue with type checking for `ModelConfiguration` Rendering classes
+- Restricted TensorFlow version to below `2.12.0` to prevent import issues
+- Added `position` parameter to `WordRendering` class
+- Changed default CSS styling for rendering classes
+- Changed name of all `processor` classes to `processer`
+
+## Version 0.3.7
+- Changed schema of the `DeployedAnalytic` class to include API key management
```

### Comparing `aisquared-0.3.6.dev0/aisquared.egg-info/SOURCES.txt` & `aisquared-0.3.7.dev0/aisquared.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/setup.py` & `aisquared-0.3.7.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/tests/test_air.py` & `aisquared-0.3.7.dev0/tests/test_air.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     x = tf.keras.layers.Dense(100, activation='relu')(x)
     output_layer = tf.keras.layers.Dense(1, activation='relu')(x)
 
     model = tf.keras.models.Model(input_layer, output_layer)
     model.save(os.path.join(tmp_path, 'model.h5'))
 
     harvester = aisquared.config.harvesting.TextHarvester()
-    preproc = aisquared.config.preprocessing.text.TextPreprocessor(
+    preproc = aisquared.config.preprocessing.text.TextPreprocesser(
         [
             aisquared.config.preprocessing.text.Tokenize(),
             aisquared.config.preprocessing.text.ConvertToVocabulary(
                 {
                     'this': 3,
                     'is': 4,
                     'a': 5,
@@ -100,15 +100,15 @@
     input_layer = tf.keras.layers.Input((30, 30, 3))
     x = tf.keras.layers.Flatten()(input_layer)
     x = tf.keras.layers.Dense(1, activation='sigmoid')(x)
     model = tf.keras.models.Model(input_layer, x)
     model.save(os.path.join(tmp_path, 'test_model.h5'))
 
     harvester = aisquared.config.harvesting.InputHarvester('image')
-    preprocesser = aisquared.config.preprocessing.image.ImagePreprocessor(
+    preprocesser = aisquared.config.preprocessing.image.ImagePreprocesser(
         [
             aisquared.config.preprocessing.image.Resize([30, 30]),
             aisquared.config.preprocessing.image.DivideValue(255)
         ]
     )
     analytic = aisquared.config.analytic.LocalModel(
         os.path.join(tmp_path, 'test_model.h5'), 'cv')
```

### Comparing `aisquared-0.3.6.dev0/tests/test_analytics.py` & `aisquared-0.3.7.dev0/tests/test_analytics.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,11 +26,18 @@
     )
     aisquared.config.analytic.DeployedModel(
         'test',
         'cv'
     )
     aisquared.config.analytic.ReverseMLWorkflow(
         'bucket',
-        'filename',
-        'column',
-        10
+        ['filename1.csv'],
+        'name',
+        input_type='text',
+        filter_type='static',
+        filter_by_columns=[{
+            'inputType': 'static',
+            'columnName': 'status',
+            'columnValue': 'pending'
+        }],
+        period=1
     )
```

### Comparing `aisquared-0.3.6.dev0/tests/test_base.py` & `aisquared-0.3.7.dev0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/tests/test_feedback.py` & `aisquared-0.3.7.dev0/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/tests/test_harvesters.py` & `aisquared-0.3.7.dev0/tests/test_harvesters.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.6.dev0/tests/test_postprocessors.py` & `aisquared-0.3.7.dev0/tests/test_postprocessors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type
 import pytest
 import aisquared
 
 
-def test_postprocessor_init():
+def test_postprocesser_init():
     with pytest.raises(TypeError):
         aisquared.config.postprocessing.BinaryClassification(
             ['zero', 'one'],
             0
         )
         aisquared.config.postprocessing.ObjectDetection(
             ['zero', 'one'],
```

### Comparing `aisquared-0.3.6.dev0/tests/test_preprocessors.py` & `aisquared-0.3.7.dev0/tests/test_preprocessors.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     aisquared.config.preprocessing.tabular.ZScore([0, 0, 0], [1, 1, 1])
     aisquared.config.preprocessing.tabular.MinMax([0, 0, 0], [1, 1, 1])
     aisquared.config.preprocessing.tabular.OneHot(2, ['cat', 'dog', 'lizard'])
     aisquared.config.preprocessing.tabular.DropColumn(4)
 
 
 def test_processers_init():
-    tabular = aisquared.config.preprocessing.tabular.TabularPreprocessor()
-    image = aisquared.config.preprocessing.image.ImagePreprocessor()
-    text = aisquared.config.preprocessing.text.TextPreprocessor()
+    tabular = aisquared.config.preprocessing.tabular.TabularPreprocesser()
+    image = aisquared.config.preprocessing.image.ImagePreprocesser()
+    text = aisquared.config.preprocessing.text.TextPreprocesser()
 
     tabular.add_step(
         aisquared.config.preprocessing.tabular.ZScore([0], [0])
     )
     image.add_step(
         aisquared.config.preprocessing.image.SubtractValue(10)
     )
```

### Comparing `aisquared-0.3.6.dev0/tests/test_renderers.py` & `aisquared-0.3.7.dev0/tests/test_renderers.py`

 * *Files 14% similar despite different names*

```diff
@@ -109,29 +109,31 @@
             'wordList': 'input',
             'resultKey': None,
             'contentKey': None,
             'badgeShape': 'star',
             'badgeColor': 'blue',
             'classes': None,
             'thresholdKey': None,
-            'thresholdValue': None
+            'thresholdValue': None,
+            'position': 'after'
         }
     }
     word = aisquared.config.rendering.WordRendering(badge_shape='underline')
     assert word.to_dict() == {
         'className': 'WordRendering',
         'params': {
             'wordList': 'input',
             'resultKey': None,
             'contentKey': None,
             'badgeShape': 'underline',
             'badgeColor': 'blue',
             'classes': None,
             'thresholdKey': None,
-            'thresholdValue': None
+            'thresholdValue': None,
+            'position': 'after'
         }
     }
 
 
 def test_document_rendering():
     document = aisquared.config.rendering.DocumentRendering()
     assert document.to_dict() == {
@@ -159,39 +161,38 @@
         prediction_name_key='',
         prediction_value_key='',
         prediction_name_value='',
         display_legend=True,
         legend_icon='circle',
         labels_key='labels'
     )
-    assert renderer.to_dict() == {
-        'className': 'BarChartRendering',
-        'label': 'test',
-        'params': {
-            'id': 'test',
-            'chartName': 'test',
-            'containerId': 'test',
-            'displayLegend': True,
-            'legendIcon': 'circle',
-            'width': 'auto',
-            'height': 'auto',
-            'xOffset': '0',
-            'yOffset': '0',
-            'datasource': [
-                {
-                    'labels': None,
-                    'labelsKey': 'labels',
-                    'consolidateRows': True,
-                    'predictionNameKey': '',
-                    'predictionValueKey': '',
-                    'predictionNameValue': ''
-                }
-            ]
-        }
-    }
+    assert renderer.to_dict() == {'className': 'BarChartRendering',
+                                  'label': 'test',
+                                  'params': {'id': 'test',
+                                             'chartName': 'test',
+                                             'containerId': 'test',
+                                             'displayLegend': True,
+                                             'legendIcon': 'circle',
+                                             'width': 'auto',
+                                             'height': 'auto',
+                                             'xOffset': '0',
+                                             'yOffset': '0',
+                                             'datasource': [{'labels': None,
+                                                             'labelsKey': 'labels',
+                                                             'consolidateRows': True,
+                                                             'predictionNameKey': '',
+                                                             'predictionValueKey': '',
+                                                             'predictionNameValue': ''}],
+                                             'style': {'container': {'color': 'black',
+                                                                     'border': '1px solid lightgray',
+                                                                     'margin': '0',
+                                                                     'padding': '24px',
+                                                                     'fontSize': '16px',
+                                                                     'background': 'white',
+                                                                     'borderRadius': '10px'}}}}
 
 
 def test_line_chart_rendering():
     renderer = aisquared.config.rendering.LineChartRendering(
         label='test',
         id='test',
         chart_name='test',
@@ -199,39 +200,38 @@
         prediction_name_key='',
         prediction_value_key='',
         prediction_name_value='',
         display_legend=True,
         legend_icon='circle',
         labels_key='labels'
     )
-    assert renderer.to_dict() == {
-        'className': 'LineChartRendering',
-        'label': 'test',
-        'params': {
-            'id': 'test',
-            'chartName': 'test',
-            'containerId': 'test',
-            'displayLegend': True,
-            'legendIcon': 'circle',
-            'width': 'auto',
-            'height': 'auto',
-            'xOffset': '0',
-            'yOffset': '0',
-            'datasource': [
-                {
-                    'labels': None,
-                    'labelsKey': 'labels',
-                    'consolidateRows': True,
-                    'predictionNameKey': '',
-                    'predictionValueKey': '',
-                    'predictionNameValue': '',
-                }
-            ]
-        }
-    }
+    assert renderer.to_dict() == {'className': 'LineChartRendering',
+                                  'label': 'test',
+                                  'params': {'id': 'test',
+                                             'chartName': 'test',
+                                             'containerId': 'test',
+                                             'displayLegend': True,
+                                             'legendIcon': 'circle',
+                                             'width': 'auto',
+                                             'height': 'auto',
+                                             'xOffset': '0',
+                                             'yOffset': '0',
+                                             'datasource': [{'labels': None,
+                                                             'labelsKey': 'labels',
+                                                             'consolidateRows': True,
+                                                             'predictionNameKey': '',
+                                                             'predictionValueKey': '',
+                                                             'predictionNameValue': ''}],
+                                             'style': {'container': {'color': 'black',
+                                                                     'border': '1px solid lightgray',
+                                                                     'margin': '0',
+                                                                     'padding': '24px',
+                                                                     'fontSize': '16px',
+                                                                     'background': 'white',
+                                                                     'borderRadius': '10px'}}}}
 
 
 def test_doughnut_chart_rendering():
     renderer = aisquared.config.rendering.DoughnutChartRendering(
         label='test',
         id='test',
         chart_name='test',
@@ -239,39 +239,38 @@
         prediction_name_key='',
         prediction_value_key='',
         prediction_name_value='',
         display_legend=True,
         legend_icon='circle',
         labels_key='labels'
     )
-    assert renderer.to_dict() == {
-        'className': 'DoughnutChartRendering',
-        'label': 'test',
-        'params': {
-            'id': 'test',
-            'chartName': 'test',
-            'containerId': 'test',
-            'displayLegend': True,
-            'legendIcon': 'circle',
-            'width': 'auto',
-            'height': 'auto',
-            'xOffset': '0',
-            'yOffset': '0',
-            'datasource': [
-                {
-                    'labels': None,
-                    'labelsKey': 'labels',
-                    'consolidateRows': True,
-                    'predictionNameKey': '',
-                    'predictionValueKey': '',
-                    'predictionNameValue': '',
-                }
-            ]
-        }
-    }
+    assert renderer.to_dict() == {'className': 'DoughnutChartRendering',
+                                  'label': 'test',
+                                  'params': {'id': 'test',
+                                             'chartName': 'test',
+                                             'containerId': 'test',
+                                             'displayLegend': True,
+                                             'legendIcon': 'circle',
+                                             'width': 'auto',
+                                             'height': 'auto',
+                                             'xOffset': '0',
+                                             'yOffset': '0',
+                                             'datasource': [{'labels': None,
+                                                             'labelsKey': 'labels',
+                                                             'consolidateRows': True,
+                                                             'predictionNameKey': '',
+                                                             'predictionValueKey': '',
+                                                             'predictionNameValue': ''}],
+                                             'style': {'container': {'color': 'black',
+                                                                     'border': '1px solid lightgray',
+                                                                     'margin': '0',
+                                                                     'padding': '24px',
+                                                                     'fontSize': '16px',
+                                                                     'background': 'white',
+                                                                     'borderRadius': '10px'}}}}
 
 
 def test_pie_chart_rendering():
     renderer = aisquared.config.rendering.PieChartRendering(
         label='test',
         id='test',
         chart_name='test',
@@ -279,39 +278,38 @@
         prediction_name_key='',
         prediction_value_key='',
         prediction_name_value='',
         display_legend=True,
         legend_icon='circle',
         labels_key='labels'
     )
-    assert renderer.to_dict() == {
-        'className': 'PieChartRendering',
-        'label': 'test',
-        'params': {
-            'id': 'test',
-            'chartName': 'test',
-            'containerId': 'test',
-            'displayLegend': True,
-            'legendIcon': 'circle',
-            'width': 'auto',
-            'height': 'auto',
-            'xOffset': '0',
-            'yOffset': '0',
-            'datasource': [
-                {
-                    'labels': None,
-                    'labelsKey': 'labels',
-                    'consolidateRows': True,
-                    'predictionNameKey': '',
-                    'predictionValueKey': '',
-                    'predictionNameValue': '',
-                }
-            ]
-        }
-    }
+    assert renderer.to_dict() == {'className': 'PieChartRendering',
+                                  'label': 'test',
+                                  'params': {'id': 'test',
+                                             'chartName': 'test',
+                                             'containerId': 'test',
+                                             'displayLegend': True,
+                                             'legendIcon': 'circle',
+                                             'width': 'auto',
+                                             'height': 'auto',
+                                             'xOffset': '0',
+                                             'yOffset': '0',
+                                             'datasource': [{'labels': None,
+                                                             'labelsKey': 'labels',
+                                                             'consolidateRows': True,
+                                                             'predictionNameKey': '',
+                                                             'predictionValueKey': '',
+                                                             'predictionNameValue': ''}],
+                                             'style': {'container': {'color': 'black',
+                                                                     'border': '1px solid lightgray',
+                                                                     'margin': '0',
+                                                                     'padding': '24px',
+                                                                     'fontSize': '16px',
+                                                                     'background': 'white',
+                                                                     'borderRadius': '10px'}}}}
 
 
 def test_container_rendering():
     renderer = aisquared.config.rendering.ContainerRendering(
         label='test',
         id='test',
         query_selector='test'
@@ -324,24 +322,20 @@
                                              'display': 'flex',
                                              'xOffset': '0',
                                              'yOffset': '0',
                                              'position': 'absolute',
                                              'orientation': 'column',
                                              'querySelector': 'test',
                                              'staticPosition': None,
-                                             'style': {'container': {'border': 'none',
+                                             'style': {'container': {'color': 'black',
                                                                      'margin': '0',
-                                                                     'padding': '8px',
-                                                                     'background': '#ffffff',
-                                                                     'borderRadius': '0',
-                                                                     'color': '#000000',
+                                                                     'padding': '24px',
                                                                      'fontSize': '16px',
-                                                                     'textAlign': 'left',
-                                                                     'textDecoration': 'none',
-                                                                     'textTransform': 'none'}}}}
+                                                                     'background': 'white',
+                                                                     'borderRadius': '10px'}}}}
 
 
 def test_dashboard_replacement_rendering():
     renderer = aisquared.config.rendering.DashboardReplacementRendering(
         'test'
     )
     assert renderer.to_dict() == {
@@ -380,32 +374,32 @@
                                              'content': '',
                                              'style': {'content': {'border': 'none',
                                                                    'margin': '0',
                                                                    'padding': '8px',
                                                                    'background': 'transparent',
                                                                    'borderRadius': '0',
                                                                    'color': '#000000',
-                                                                   'fontSize': '16px',
+                                                                   'fontSize': '14px',
                                                                    'textAlign': 'left',
                                                                    'textDecoration': 'none',
                                                                    'textTransform': 'none',
-                                                                   'fontWeight': '',
+                                                                   'fontWeight': 'bold',
                                                                    'width': 'auto',
                                                                    'height': 'auto'},
                                                        'extraContent': {'border': 'none',
                                                                         'margin': '0',
                                                                         'padding': '8px',
                                                                         'background': 'transparent',
                                                                         'borderRadius': '0',
                                                                         'color': '#000000',
-                                                                        'fontSize': '16px',
+                                                                        'fontSize': '14px',
                                                                         'textAlign': 'left',
                                                                         'textDecoration': 'none',
                                                                         'textTransform': 'none',
-                                                                        'fontWeight': '',
+                                                                        'fontWeight': 'bold',
                                                                         'width': 'auto',
                                                                         'height': 'auto'}}}}
 
 
 def test_sos_rendering():
     renderer = aisquared.config.rendering.SOSRendering(True)
     assert renderer.to_dict() == {
@@ -430,75 +424,35 @@
                                   'label': 'test',
                                   'params': {'id': 'test',
                                              'containerId': 'test',
                                              'predictionNameKey': 'test',
                                              'predictionValueKey': 'test',
                                              'predictionNameValues': ['name1', 'name2'],
                                              'tableName': '',
-                                             'style': {'container': {'border': 'none',
-                                                                     'margin': '0',
-                                                                     'padding': '8px',
-                                                                     'background': '#ffffff',
-                                                                     'borderRadius': '0',
+                                             'style': {'container': {'border': '1px solid lightgray',
+                                                                     'margin': '8px 0',
+                                                                     'padding': '10px',
+                                                                     'background': '#f3f3f3',
+                                                                     'borderRadius': '10px',
                                                                      'color': '#000000',
-                                                                     'fontSize': '16px',
+                                                                     'fontSize': '14px',
                                                                      'textAlign': 'left',
-                                                                     'textDecoration': 'none',
-                                                                     'textTransform': 'none'},
-                                                       'title': {'color': 'inherit',
-                                                                 'fontSize': '16px',
-                                                                 'textAlign': 'left',
-                                                                 'textDecoration': 'none',
-                                                                 'textTransform': 'capitalize',
-                                                                 'textShadow': 'none',
-                                                                 'textIndent': '',
-                                                                 'letterSpacing': '',
-                                                                 'lineHeight': '',
-                                                                 'wordSpacing': '',
-                                                                 'whiteSpace': ''},
+                                                                     'fontFamily': 'Raleway, sans-serif'},
+                                                       'title': {'fontWeight': 'bold', 'marginBottom': '4px'},
                                                        'table': {'border': '1px solid lightgray',
-                                                                 'margin': '8px',
-                                                                 'padding': '8px',
-                                                                 'background': 'transparent',
-                                                                 'color': '#000000',
-                                                                 'fontSize': '16px',
-                                                                 'textAlign': 'left',
-                                                                 'textDecoration': 'none',
+                                                                 'textAlign': 'center',
                                                                  'textTransform': 'capitalize',
-                                                                 'width': 'auto',
-                                                                 'height': 'auto'},
+                                                                 'width': '100%',
+                                                                 'fontFamily': 'Raleway, sans-serif'},
                                                        'tableHeader': {'border': '1px solid lightgray',
-                                                                       'background': 'transparent',
-                                                                       'color': '#000000',
-                                                                       'margin': '0',
-                                                                       'padding': '0',
-                                                                       'fontSize': '16px',
-                                                                       'textAlign': 'left',
-                                                                       'textDecoration': 'none',
+                                                                       'padding': '4px',
+                                                                       'fontWeight': 'bold',
                                                                        'textTransform': 'capitalize'},
-                                                       'tableBody': {'border': '1px solid lightgray',
-                                                                     'background': 'transparent',
-                                                                     'color': '#000000',
-                                                                     'margin': '8px',
-                                                                     'padding': '8px',
-                                                                     'fontSize': '16px',
-                                                                     'textAlign': 'left',
-                                                                     'textDecoration': 'none',
-                                                                     'textTransform': 'capitalize'},
-                                                       'tableRows': {'border': '1px solid lightgray',
-                                                                     'background': 'transparent',
-                                                                     'color': '#000000',
-                                                                     'margin': '0',
-                                                                     'padding': '0',
-                                                                     'fontSize': '16px',
-                                                                     'textAlign': 'left',
-                                                                     'textDecoration': 'none',
-                                                                     'textTransform': 'capitalize'},
+                                                       'tableBody': {},
+                                                       'tableRows': {'border': '1px solid lightgray'},
                                                        'rowCells': {'border': '1px solid lightgray',
-                                                                    'background': 'transparent',
-                                                                    'color': '#000000',
-                                                                    'margin': '0',
-                                                                    'padding': '0',
-                                                                    'fontSize': '16px',
-                                                                    'textAlign': 'left',
-                                                                    'textDecoration': 'none',
-                                                                    'textTransform': 'capitalize'}}}}
+                                                                    'fontWeight': 'normal',
+                                                                    'padding': '8px'},
+                                                       'headerCells': {'border': '1px solid lightgray',
+                                                                       'padding': '8px',
+                                                                       'fontWeight': 'bolder',
+                                                                       'backgroundColor': 'white'}}}}
```

