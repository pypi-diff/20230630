# Comparing `tmp/tfads_o_builder-0.0.157.tar.gz` & `tmp/tfads_o_builder-0.0.158.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfads_o_builder-0.0.157.tar", max compression
+gzip compressed data, was "tfads_o_builder-0.0.158.tar", max compression
```

## Comparing `tfads_o_builder-0.0.157.tar` & `tfads_o_builder-0.0.158.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1076 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/LICENSE
--rw-r--r--   0        0        0      104 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/README.md
--rw-r--r--   0        0        0      916 2023-06-30 01:17:12.045464 tfads_o_builder-0.0.157/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/Line.py
--rw-r--r--   0        0        0     6541 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/Point.py
--rw-r--r--   0        0        0      187 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/ActiveDeletedCode.py
--rw-r--r--   0        0        0      783 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/CompilationDate.py
--rw-r--r--   0        0        0      201 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/ControlReleasabilityCode.py
--rw-r--r--   0        0        0      199 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/CoordinatePrecisionFlag.py
--rw-r--r--   0        0        0     4505 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/CountryCode.py
--rw-r--r--   0        0        0      180 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/DeficiencyCode.py
--rw-r--r--   0        0        0      192 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/DeletingOrganization.py
--rw-r--r--   0        0        0      192 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/DerivingOrganization.py
--rw-r--r--   0        0        0     1503 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/FACCCode.py
--rw-r--r--   0        0        0     1208 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/FACCName.py
--rw-r--r--   0        0        0     3318 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/FeatureTypeCode.py
--rw-r--r--   0        0        0     1241 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/FeatureTypeName.py
--rw-r--r--   0        0        0      217 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/HeightAGLAccuracy.py
--rw-r--r--   0        0        0      219 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/HeightAMSLAccuracy.py
--rw-r--r--   0        0        0      218 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/HorizontalAccuracy.py
--rw-r--r--   0        0        0      182 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/HorizontalDatum.py
--rw-r--r--   0        0        0      476 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/Latitude.py
--rw-r--r--   0        0        0      163 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/Lights.py
--rw-r--r--   0        0        0      216 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/LocationElevation.py
--rw-r--r--   0        0        0      233 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/LocationElevationAccuracy.py
--rw-r--r--   0        0        0      483 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/Longitude.py
--rw-r--r--   0        0        0      180 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/MultipleNumber.py
--rw-r--r--   0        0        0      223 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/ObstructionHeightAGL.py
--rw-r--r--   0        0        0      225 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/ObstructionHeightAMSL.py
--rw-r--r--   0        0        0      172 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/OriginalID.py
--rw-r--r--   0        0        0      178 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/OutputRemarks.py
--rw-r--r--   0        0        0      202 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/PreviousVOIdentifierCode.py
--rw-r--r--   0        0        0      174 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/ProcessCode.py
--rw-r--r--   0        0        0     1105 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/ProvinceCode.py
--rw-r--r--   0        0        0      755 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/RevisionDate.py
--rw-r--r--   0        0        0      392 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/SecurityClassification.py
--rw-r--r--   0        0        0      418 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/SingleMultipleFlag.py
--rw-r--r--   0        0        0      751 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/SourceDate.py
--rw-r--r--   0        0        0      191 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/SurfaceMaterialCode.py
--rw-r--r--   0        0        0      546 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/TransactionType.py
--rw-r--r--   0        0        0      919 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/UUID.py
--rw-r--r--   0        0        0      184 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/VOIdentification.py
--rw-r--r--   0        0        0      185 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/VOSequenceNumber.py
--rw-r--r--   0        0        0      180 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/ValidationCode.py
--rw-r--r--   0        0        0      165 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/WACINNR.py
--rw-r--r--   0        0        0      176 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/WACNumber.py
--rw-r--r--   0        0        0     1850 2023-06-30 01:17:11.357430 tfads_o_builder-0.0.157/tfads_o_builder/feature_types/_Base.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 tfads_o_builder-0.0.157/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/LICENSE
+-rw-r--r--   0        0        0      104 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/README.md
+-rw-r--r--   0        0        0      916 2023-06-30 01:22:07.056101 tfads_o_builder-0.0.158/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/Line.py
+-rw-r--r--   0        0        0     6541 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/Point.py
+-rw-r--r--   0        0        0      187 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/ActiveDeletedCode.py
+-rw-r--r--   0        0        0      783 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/CompilationDate.py
+-rw-r--r--   0        0        0      201 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/ControlReleasabilityCode.py
+-rw-r--r--   0        0        0      199 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/CoordinatePrecisionFlag.py
+-rw-r--r--   0        0        0     4505 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/CountryCode.py
+-rw-r--r--   0        0        0      180 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/DeficiencyCode.py
+-rw-r--r--   0        0        0      192 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/DeletingOrganization.py
+-rw-r--r--   0        0        0      192 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/DerivingOrganization.py
+-rw-r--r--   0        0        0     1503 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/FACCCode.py
+-rw-r--r--   0        0        0     1208 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/FACCName.py
+-rw-r--r--   0        0        0     3318 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/FeatureTypeCode.py
+-rw-r--r--   0        0        0     1241 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/FeatureTypeName.py
+-rw-r--r--   0        0        0      217 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/HeightAGLAccuracy.py
+-rw-r--r--   0        0        0      219 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/HeightAMSLAccuracy.py
+-rw-r--r--   0        0        0      218 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/HorizontalAccuracy.py
+-rw-r--r--   0        0        0      182 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/HorizontalDatum.py
+-rw-r--r--   0        0        0      476 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/Latitude.py
+-rw-r--r--   0        0        0      163 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/Lights.py
+-rw-r--r--   0        0        0      216 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/LocationElevation.py
+-rw-r--r--   0        0        0      233 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/LocationElevationAccuracy.py
+-rw-r--r--   0        0        0      483 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/Longitude.py
+-rw-r--r--   0        0        0      180 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/MultipleNumber.py
+-rw-r--r--   0        0        0      223 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/ObstructionHeightAGL.py
+-rw-r--r--   0        0        0      225 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/ObstructionHeightAMSL.py
+-rw-r--r--   0        0        0      172 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/OriginalID.py
+-rw-r--r--   0        0        0      178 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/OutputRemarks.py
+-rw-r--r--   0        0        0      202 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/PreviousVOIdentifierCode.py
+-rw-r--r--   0        0        0      174 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/ProcessCode.py
+-rw-r--r--   0        0        0     1105 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/ProvinceCode.py
+-rw-r--r--   0        0        0      755 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/RevisionDate.py
+-rw-r--r--   0        0        0      392 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/SecurityClassification.py
+-rw-r--r--   0        0        0      418 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/SingleMultipleFlag.py
+-rw-r--r--   0        0        0      751 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/SourceDate.py
+-rw-r--r--   0        0        0      191 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/SurfaceMaterialCode.py
+-rw-r--r--   0        0        0      546 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/TransactionType.py
+-rw-r--r--   0        0        0      919 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/UUID.py
+-rw-r--r--   0        0        0      184 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/VOIdentification.py
+-rw-r--r--   0        0        0      185 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/VOSequenceNumber.py
+-rw-r--r--   0        0        0      180 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/ValidationCode.py
+-rw-r--r--   0        0        0      165 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/WACINNR.py
+-rw-r--r--   0        0        0      176 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/WACNumber.py
+-rw-r--r--   0        0        0     1850 2023-06-30 01:22:06.488102 tfads_o_builder-0.0.158/tfads_o_builder/feature_types/_Base.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 tfads_o_builder-0.0.158/PKG-INFO
```

### Comparing `tfads_o_builder-0.0.157/LICENSE` & `tfads_o_builder-0.0.158/LICENSE`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/pyproject.toml` & `tfads_o_builder-0.0.158/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tfads-o-builder"
-version = "v0.0.157"
+version = "v0.0.158"
 description = "Helper functions used to build data as tfads-o format."
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/fsai-dev/fsai-cli-tools"
 repository = "https://github.com/fsai-dev/fsai-cli-tools"
```

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/Point.py` & `tfads_o_builder-0.0.158/tfads_o_builder/Point.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/CompilationDate.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/CompilationDate.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/CountryCode.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/CountryCode.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/FACCCode.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/FACCCode.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/FACCName.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/FACCName.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/FeatureTypeCode.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/FeatureTypeCode.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/FeatureTypeName.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/FeatureTypeName.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/ProvinceCode.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/ProvinceCode.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/RevisionDate.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/RevisionDate.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/SourceDate.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/SourceDate.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/TransactionType.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/TransactionType.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/UUID.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/UUID.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/tfads_o_builder/feature_types/_Base.py` & `tfads_o_builder-0.0.158/tfads_o_builder/feature_types/_Base.py`

 * *Files identical despite different names*

### Comparing `tfads_o_builder-0.0.157/PKG-INFO` & `tfads_o_builder-0.0.158/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfads-o-builder
-Version: 0.0.157
+Version: 0.0.158
 Summary: Helper functions used to build data as tfads-o format.
 Home-page: https://github.com/fsai-dev/fsai-cli-tools
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

