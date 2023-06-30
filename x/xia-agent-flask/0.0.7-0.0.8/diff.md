# Comparing `tmp/xia_agent_flask-0.0.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_agent_flask-0.0.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2742 bytes, number of entries: 7
--rw-r--r--  2.0 unx      251 b- defN 23-Jun-29 20:35 xia_agent_flask/__init__.py
--rw-r--r--  2.0 unx     1888 b- defN 23-Jun-29 20:32 xia_agent_flask/api.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:38 xia_agent_flask-0.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      755 b- defN 23-Jun-29 20:38 xia_agent_flask-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:38 xia_agent_flask-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:38 xia_agent_flask-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      590 b- defN 23-Jun-29 20:38 xia_agent_flask-0.0.7.dist-info/RECORD
-7 files, 3750 bytes uncompressed, 1684 bytes compressed:  55.1%
+Zip file size: 2660 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      251 b- defN 23-Jun-30 11:13 xia_agent_flask/__init__.py
+-rw-r--r--  2.0 unx     1888 b- defN 23-Jun-30 11:13 xia_agent_flask/api.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      520 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      590 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/RECORD
+7 files, 3515 bytes uncompressed, 1602 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_agent_flask/__init__.py
 Comment: 
 
 Filename: xia_agent_flask/api.py
 Comment: 
 
-Filename: xia_agent_flask-0.0.7.dist-info/LICENSE.txt
+Filename: xia_agent_flask-0.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_agent_flask-0.0.7.dist-info/METADATA
+Filename: xia_agent_flask-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_agent_flask-0.0.7.dist-info/WHEEL
+Filename: xia_agent_flask-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_agent_flask-0.0.7.dist-info/top_level.txt
+Filename: xia_agent_flask-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_agent_flask-0.0.7.dist-info/RECORD
+Filename: xia_agent_flask-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_agent_flask/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
    "AgentFunctionApi",
    "FlaskRequestParser", "GcpLogParser", "PubsubLogParser"
 ]
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

## Comparing `xia_agent_flask-0.0.7.dist-info/METADATA` & `xia_agent_flask-0.0.8.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,25 @@
 Metadata-Version: 2.1
 Name: xia-agent-flask
-Version: 0.0.7
-Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-agent-flask/0.0.7/index.html
+Version: 0.0.8
+Summary: UNKNOWN
+Home-page: https://develop.x-i-a.com/docs/xia-agent-flask/0.0.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: Flask
 Requires-Dist: xia-engine
 Requires-Dist: xia-models
 Requires-Dist: xia-logger
 Requires-Dist: xia-agent
 
-.. image:: https://img.shields.io/pypi/v/xia-agent-flask.svg?color=blue
-   :alt: PyPI-Server
-   :target: https://pypi.org/project/xia-agent-flask/
-
-====================================
-X-I-A
-====================================
-
-
-
-Quick start
+Introduction
 =============================
 
-Install the package::
-
-   pip install
-
+Welcome to use X-I-A's software
```

## Comparing `xia_agent_flask-0.0.7.dist-info/RECORD` & `xia_agent_flask-0.0.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_agent_flask/__init__.py,sha256=mTPZF29feerWivvvNnqg_HlnYEdZIKmQAd5Evd3D1HI,251
+xia_agent_flask/__init__.py,sha256=EDTfmeY_IWFTb74iC_PlKkxfms3Xu4W9cys3ZcEFDMc,251
 xia_agent_flask/api.py,sha256=c31xCrGqcKy3WfpkDRmPuMnF7UIf49NOwyMYs1pze-0,1888
-xia_agent_flask-0.0.7.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_agent_flask-0.0.7.dist-info/METADATA,sha256=EHXcVZO-JuiKym2cYchKIgb-mSnAbsZH8XRPsw1nMM0,755
-xia_agent_flask-0.0.7.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_agent_flask-0.0.7.dist-info/top_level.txt,sha256=5A45GyDFwmSRa9wqMcpfxsUxldoTCCwG6aJG_iVIKp4,16
-xia_agent_flask-0.0.7.dist-info/RECORD,,
+xia_agent_flask-0.0.8.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_agent_flask-0.0.8.dist-info/METADATA,sha256=RTAQzL9spdODzMk2sOp_7U2nJWye_vc58r3neYDezQg,520
+xia_agent_flask-0.0.8.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_agent_flask-0.0.8.dist-info/top_level.txt,sha256=5A45GyDFwmSRa9wqMcpfxsUxldoTCCwG6aJG_iVIKp4,16
+xia_agent_flask-0.0.8.dist-info/RECORD,,
```

