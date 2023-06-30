# Comparing `tmp/open_source_insights_api-0.1.7.tar.gz` & `tmp/open_source_insights_api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_source_insights_api-0.1.7.tar", max compression
+gzip compressed data, was "open_source_insights_api-0.1.8.tar", max compression
```

## Comparing `open_source_insights_api-0.1.7.tar` & `open_source_insights_api-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1090 2023-06-29 12:25:06.013868 open_source_insights_api-0.1.7/LICENSE
--rw-r--r--   0        0        0     1398 2023-06-29 12:18:46.133876 open_source_insights_api-0.1.7/README.md
--rw-r--r--   0        0        0       92 2023-06-29 12:19:48.163874 open_source_insights_api-0.1.7/open_source_insights_api/__init__.py
--rw-r--r--   0        0        0    16592 2023-06-29 14:16:21.553731 open_source_insights_api-0.1.7/open_source_insights_api/os_insights.py
--rw-r--r--   0        0        0      958 2023-06-29 12:42:04.523847 open_source_insights_api-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-29 12:25:06.013868 open_source_insights_api-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1398 2023-06-29 12:18:46.133876 open_source_insights_api-0.1.8/README.md
+-rw-r--r--   0        0        0       92 2023-06-30 16:18:22.076458 open_source_insights_api-0.1.8/open_source_insights_api/__init__.py
+-rw-r--r--   0        0        0    16632 2023-06-30 16:17:34.206457 open_source_insights_api-0.1.8/open_source_insights_api/os_insights.py
+-rw-r--r--   0        0        0      958 2023-06-30 16:18:15.726458 open_source_insights_api-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 open_source_insights_api-0.1.8/PKG-INFO
```

### Comparing `open_source_insights_api-0.1.7/LICENSE` & `open_source_insights_api-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `open_source_insights_api-0.1.7/README.md` & `open_source_insights_api-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `open_source_insights_api-0.1.7/open_source_insights_api/os_insights.py` & `open_source_insights_api-0.1.8/open_source_insights_api/os_insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,24 +370,24 @@
                 "versionKey.name": pkg_name,
                 "versionKey.version": pkg_version
             }
         else:
             params = {}
 
         if len(params) != 0:
-            try:
-                async with AsyncClient(base_url=url) as client:
+            async with AsyncClient(base_url=url) as client:
+                try:
                     r = await client.get('/query', params=params, timeout=10)
-            except:
-                return {"error": f"Connection with {url} status invalid", "status_code": r.status_code}
-            
-            if r.status_code == 404:
-                return {"error": f"Connection with {url} status invalid", "status_code": r.status_code}
-            
-            try:
-                r_json = json.loads(r.content)
-            except:
-                return {"error": "JSON returned from API is not serializable", "response": r.content.decode('utf-8')}
+                except:
+                    return {"error": f"Connection with {url} status invalid", "status_code": r.status_code}
+                
+                if r.status_code == 404:
+                    return {"error": f"Connection with {url} status invalid", "status_code": r.status_code}
+                
+                try:
+                    r_json = json.loads(r.content)
+                except:
+                    return {"error": "JSON returned from API is not serializable", "response": r.content.decode('utf-8')}
         else:
             return {"error": "Incomplete parameters"}
         
         return r_json
```

### Comparing `open_source_insights_api-0.1.7/pyproject.toml` & `open_source_insights_api-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-source-insights-api"
-version = "0.1.7"
+version = "0.1.8"
 license = "MIT"
 description = "Library to consume project Open Source Insights Project from Google"
 authors = ["Cristiano Henrique <cristianovisk@gmail.com>"]
 readme = "README.md"
 packages = [{include = "open_source_insights_api"}]
 classifiers = [
     "Topic :: Internet",
```

### Comparing `open_source_insights_api-0.1.7/PKG-INFO` & `open_source_insights_api-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-source-insights-api
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library to consume project Open Source Insights Project from Google
 License: MIT
 Author: Cristiano Henrique
 Author-email: cristianovisk@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

