# Comparing `tmp/arcan-1.2.0.tar.gz` & `tmp/arcan-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-1.2.0.tar", max compression
+gzip compressed data, was "arcan-1.2.1.tar", max compression
```

## Comparing `arcan-1.2.0.tar` & `arcan-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1566 2023-06-30 06:40:09.018062 arcan-1.2.0/LICENSE
--rw-r--r--   0        0        0     4003 2023-06-30 06:40:09.018062 arcan-1.2.0/README.md
--rw-r--r--   0        0        0      942 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/engines/__init__.py
--rw-r--r--   0        0        0       24 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/engines/io.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/governance/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/governance/catalog/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/governance/lifecycle/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/governance/mdm/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/governance/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/ml/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/processing/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/processing/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/processing/transformations/__init__.py
--rw-r--r--   0        0        0       91 2023-06-30 06:40:09.022062 arcan-1.2.0/arcan/session/__init__.py
--rw-r--r--   0        0        0       62 2023-06-30 06:40:09.022062 arcan-1.2.0/main.py
--rw-r--r--   0        0        0      695 2023-06-30 06:40:09.022062 arcan-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 arcan-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1711 2023-06-30 14:16:11.865680 arcan-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4003 2023-06-30 14:16:11.865680 arcan-1.2.1/README.md
+-rw-r--r--   0        0        0      907 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/engines/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/engines/io.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/governance/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/governance/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/governance/lifecycle/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/governance/mdm/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/governance/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/processing/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/processing/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/processing/transformations/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-30 14:16:11.865680 arcan-1.2.1/arcan/session/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-30 14:16:11.865680 arcan-1.2.1/main.py
+-rw-r--r--   0        0        0      735 2023-06-30 14:16:11.865680 arcan-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4726 1970-01-01 00:00:00.000000 arcan-1.2.1/PKG-INFO
```

### Comparing `arcan-1.2.0/README.md` & `arcan-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `arcan-1.2.0/arcan/__init__.py` & `arcan-1.2.1/arcan/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # %%
-from fastapi import FastAPI
 from modal import Stub, web_endpoint
 from modal import Image, Stub, web_endpoint
-import toml, os
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 
 # %%
 # %%
 def get_arcan_version():
     try:
         import arcan
-        return(arcan.__version__)
+
+        return arcan.__version__
     except Exception as e:
         print(e)
         return f"No arcan package is installed"
 
 
 # %%
-image = Image.debian_slim().pip_install("fastapi", "uvicorn", "databricks_session", "arcan")
-#api = FastAPI()
+image = Image.debian_slim().pip_install(
+    "fastapi", "uvicorn", "databricks_session", "arcan"
+)
+# api = FastAPI()
 stub = Stub(
     name="arcan",
     image=image,
 )
 
+
 @stub.function()
 @web_endpoint(method="GET")
-#@api.get("/")
+# @api.get("/")
 def entrypoint():
     return {"message": "Arcan is running"}
 
 
 @stub.function()
 @web_endpoint(method="GET")
-#@api.get("/api/version")
+# @api.get("/api/version")
 def version():
     print("Arcan is installed")
     # return the installed version of Arcan package from the pyproject.toml file
     version = get_arcan_version()
     return {"message": f"Arcan version {version} is installed"}
 
 
 # %%
-
```

### Comparing `arcan-1.2.0/PKG-INFO` & `arcan-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: arcan
-Version: 1.2.0
+Version: 1.2.1
 Summary: A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools
-License: MIT
+License: arcan.ai Non-Commercial Open Source License
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.98.0,<0.99.0)
 Requires-Dist: modal-client (>=0.49.2509,<0.50.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: arcan Version: 1.2.0 Summary: A multiheaded modern
+Metadata-Version: 2.1 Name: arcan Version: 1.2.1 Summary: A multiheaded modern
 data bridging package based on pipeline manifests to integrate between any
-modern (and old) data stack tools License: MIT Author: Carlos D. Escobar-
-Valbuena Author-email: carlosdavidescobar@gmail.com Requires-Python:
->=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
-fastapi (>=0.98.0,<0.99.0) Requires-Dist: modal-client (>=0.49.2509,<0.50.0)
-Requires-Dist: uvicorn (>=0.22.0,<0.23.0) Description-Content-Type: text/
-markdown
+modern (and old) data stack tools License: arcan.ai Non-Commercial Open Source
+License Author: Carlos D. Escobar-Valbuena Author-email:
+carlosdavidescobar@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
+:: Other/Proprietary License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: fastapi (>=0.98.0,<0.99.0) Requires-
+Dist: modal-client (>=0.49.2509,<0.50.0) Requires-Dist: uvicorn
+(>=0.22.0,<0.23.0) Description-Content-Type: text/markdown
    [https://assets.vercel.com/image/upload/v1588805858/repositories/vercel/
                                    logo.png]
                                 ****_arcan_****
 Next.js & FastAPI Vercel Arcan Deployment. Check out source template at Vercel
                                    Template.
 
 # Arcan **A multiheaded modern data bridging package based on pipeline
```

