# Comparing `tmp/beastiary-1.6.0.tar.gz` & `tmp/beastiary-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beastiary-1.6.0.tar", max compression
+gzip compressed data, was "beastiary-1.6.1.tar", max compression
```

## Comparing `beastiary-1.6.0.tar` & `beastiary-1.6.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1677 2023-04-28 02:32:02.561656 beastiary-1.6.0/PYPI-README.md
--rw-r--r--   0        0        0        1 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/__init__.py
--rw-r--r--   0        0        0       22 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/api/__init__.py
--rw-r--r--   0        0        0     3605 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/api/core.py
--rw-r--r--   0        0        0      190 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/api/deps.py
--rw-r--r--   0        0        0        0 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/api/endpoints/__init__.py
--rw-r--r--   0        0        0     1002 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/api/endpoints/explorer.py
--rw-r--r--   0        0        0     2524 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/api/endpoints/traces.py
--rw-r--r--   0        0        0     2879 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/api/main.py
--rw-r--r--   0        0        0     2541 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/cli.py
--rw-r--r--   0        0        0       62 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/crud/__init__.py
--rw-r--r--   0        0        0     1525 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/crud/base.py
--rw-r--r--   0        0        0      696 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/crud/crud_sample.py
--rw-r--r--   0        0        0      766 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/crud/crud_trace.py
--rw-r--r--   0        0        0       31 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/db/__init__.py
--rw-r--r--   0        0        0     1013 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/db/database.py
--rw-r--r--   0        0        0       60 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/log.py
--rw-r--r--   0        0        0      106 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/schemas/__init__.py
--rw-r--r--   0        0        0      537 2023-04-28 02:32:02.561656 beastiary-1.6.0/beastiary/schemas/sample.py
--rw-r--r--   0        0        0      631 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/schemas/trace.py
--rw-r--r--   0        0        0   357831 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/css/chunk-vendors.5b404c1b.css
--rw-r--r--   0        0        0     3825 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/css/login.4b7f13da.css
--rw-r--r--   0        0        0    32513 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/css/login~main-dashboard.49552835.css
--rw-r--r--   0        0        0    11811 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/css/login~main~main-dashboard.87cb79bc.css
--rw-r--r--   0        0        0    49496 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/css/main-dashboard.02d99ae8.css
--rw-r--r--   0        0        0     9710 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/css/main.38cd41ea.css
--rw-r--r--   0        0        0    22507 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/css/main~main-dashboard.27813474.css
--rw-r--r--   0        0        0    15406 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/favicon.ico
--rw-r--r--   0        0        0     3027 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/index.html
--rw-r--r--   0        0        0    33041 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/js/app.92353b76.js
--rw-r--r--   0        0        0    60737 2023-04-28 02:32:02.565656 beastiary-1.6.0/beastiary/webapp-dist/js/app.92353b76.js.map
--rw-r--r--   0        0        0   503609 2023-04-28 02:32:02.569656 beastiary-1.6.0/beastiary/webapp-dist/js/chunk-vendors.9a0991d8.js
--rw-r--r--   0        0        0  1810656 2023-04-28 02:32:02.581656 beastiary-1.6.0/beastiary/webapp-dist/js/chunk-vendors.9a0991d8.js.map
--rw-r--r--   0        0        0     8974 2023-04-28 02:32:02.581656 beastiary-1.6.0/beastiary/webapp-dist/js/login.ed57607a.js
--rw-r--r--   0        0        0    17094 2023-04-28 02:32:02.581656 beastiary-1.6.0/beastiary/webapp-dist/js/login.ed57607a.js.map
--rw-r--r--   0        0        0    25157 2023-04-28 02:32:02.581656 beastiary-1.6.0/beastiary/webapp-dist/js/login~main-dashboard.3ae3e551.js
--rw-r--r--   0        0        0    49629 2023-04-28 02:32:02.581656 beastiary-1.6.0/beastiary/webapp-dist/js/login~main-dashboard.3ae3e551.js.map
--rw-r--r--   0        0        0    29972 2023-04-28 02:32:02.581656 beastiary-1.6.0/beastiary/webapp-dist/js/login~main~main-dashboard.3a1f6d10.js
--rw-r--r--   0        0        0    67901 2023-04-28 02:32:02.581656 beastiary-1.6.0/beastiary/webapp-dist/js/login~main~main-dashboard.3a1f6d10.js.map
--rw-r--r--   0        0        0  4137121 2023-04-28 02:32:02.605656 beastiary-1.6.0/beastiary/webapp-dist/js/main-dashboard.cdaf674a.js
--rw-r--r--   0        0        0 14341796 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/js/main-dashboard.cdaf674a.js.map
--rw-r--r--   0        0        0    29797 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/js/main.fd1e121b.js
--rw-r--r--   0        0        0    57875 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/js/main.fd1e121b.js.map
--rw-r--r--   0        0        0    37465 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/js/main~main-dashboard.80ebc61e.js
--rw-r--r--   0        0        0    76367 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/js/main~main-dashboard.80ebc61e.js.map
--rw-r--r--   0        0        0      334 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/js/reset-password.cc5953a6.js
--rw-r--r--   0        0        0      976 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/js/reset-password.cc5953a6.js.map
--rw-r--r--   0        0        0     3564 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/js/start.5f1fab73.js
--rw-r--r--   0        0        0     3431 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/js/start.5f1fab73.js.map
--rw-r--r--   0        0        0      315 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/manifest.json
--rw-r--r--   0        0        0     1909 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/precache-manifest.b4123667328a01c6185efab765d92c10.js
--rw-r--r--   0        0        0       24 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/robots.txt
--rw-r--r--   0        0        0     1063 2023-04-28 02:32:02.685657 beastiary-1.6.0/beastiary/webapp-dist/service-worker.js
--rw-r--r--   0        0        0      617 2023-04-28 02:32:02.685657 beastiary-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 beastiary-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1677 2023-06-30 03:36:20.111837 beastiary-1.6.1/PYPI-README.md
+-rw-r--r--   0        0        0        1 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/api/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/api/core.py
+-rw-r--r--   0        0        0      190 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/api/deps.py
+-rw-r--r--   0        0        0        0 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     1002 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/api/endpoints/explorer.py
+-rw-r--r--   0        0        0     2504 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/api/endpoints/traces.py
+-rw-r--r--   0        0        0     2879 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/api/main.py
+-rw-r--r--   0        0        0     2541 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/cli.py
+-rw-r--r--   0        0        0       62 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/crud/__init__.py
+-rw-r--r--   0        0        0     1525 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/crud/base.py
+-rw-r--r--   0        0        0      696 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/crud/crud_sample.py
+-rw-r--r--   0        0        0      766 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/crud/crud_trace.py
+-rw-r--r--   0        0        0       31 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/db/__init__.py
+-rw-r--r--   0        0        0     1013 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/db/database.py
+-rw-r--r--   0        0        0       60 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/log.py
+-rw-r--r--   0        0        0      106 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/schemas/__init__.py
+-rw-r--r--   0        0        0      537 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/schemas/sample.py
+-rw-r--r--   0        0        0      631 2023-06-30 03:36:20.111837 beastiary-1.6.1/beastiary/schemas/trace.py
+-rw-r--r--   0        0        0   357831 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/css/chunk-vendors.5b404c1b.css
+-rw-r--r--   0        0        0     3825 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/css/login.4b7f13da.css
+-rw-r--r--   0        0        0    32513 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/css/login~main-dashboard.49552835.css
+-rw-r--r--   0        0        0    11811 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/css/login~main~main-dashboard.87cb79bc.css
+-rw-r--r--   0        0        0    49496 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/css/main-dashboard.02d99ae8.css
+-rw-r--r--   0        0        0     9710 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/css/main.38cd41ea.css
+-rw-r--r--   0        0        0    22507 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/css/main~main-dashboard.27813474.css
+-rw-r--r--   0        0        0    15406 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/favicon.ico
+-rw-r--r--   0        0        0     3027 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/index.html
+-rw-r--r--   0        0        0    33041 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/js/app.92353b76.js
+-rw-r--r--   0        0        0    60737 2023-06-30 03:36:20.115837 beastiary-1.6.1/beastiary/webapp-dist/js/app.92353b76.js.map
+-rw-r--r--   0        0        0   503609 2023-06-30 03:36:20.119838 beastiary-1.6.1/beastiary/webapp-dist/js/chunk-vendors.9a0991d8.js
+-rw-r--r--   0        0        0  1810656 2023-06-30 03:36:20.127838 beastiary-1.6.1/beastiary/webapp-dist/js/chunk-vendors.9a0991d8.js.map
+-rw-r--r--   0        0        0     8974 2023-06-30 03:36:20.127838 beastiary-1.6.1/beastiary/webapp-dist/js/login.ed57607a.js
+-rw-r--r--   0        0        0    17094 2023-06-30 03:36:20.127838 beastiary-1.6.1/beastiary/webapp-dist/js/login.ed57607a.js.map
+-rw-r--r--   0        0        0    25157 2023-06-30 03:36:20.127838 beastiary-1.6.1/beastiary/webapp-dist/js/login~main-dashboard.3ae3e551.js
+-rw-r--r--   0        0        0    49629 2023-06-30 03:36:20.131838 beastiary-1.6.1/beastiary/webapp-dist/js/login~main-dashboard.3ae3e551.js.map
+-rw-r--r--   0        0        0    29972 2023-06-30 03:36:20.131838 beastiary-1.6.1/beastiary/webapp-dist/js/login~main~main-dashboard.3a1f6d10.js
+-rw-r--r--   0        0        0    67901 2023-06-30 03:36:20.131838 beastiary-1.6.1/beastiary/webapp-dist/js/login~main~main-dashboard.3a1f6d10.js.map
+-rw-r--r--   0        0        0  4137121 2023-06-30 03:36:20.155840 beastiary-1.6.1/beastiary/webapp-dist/js/main-dashboard.cdaf674a.js
+-rw-r--r--   0        0        0 14341796 2023-06-30 03:36:20.231844 beastiary-1.6.1/beastiary/webapp-dist/js/main-dashboard.cdaf674a.js.map
+-rw-r--r--   0        0        0    29797 2023-06-30 03:36:20.231844 beastiary-1.6.1/beastiary/webapp-dist/js/main.fd1e121b.js
+-rw-r--r--   0        0        0    57875 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/js/main.fd1e121b.js.map
+-rw-r--r--   0        0        0    37465 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/js/main~main-dashboard.80ebc61e.js
+-rw-r--r--   0        0        0    76367 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/js/main~main-dashboard.80ebc61e.js.map
+-rw-r--r--   0        0        0      334 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/js/reset-password.cc5953a6.js
+-rw-r--r--   0        0        0      976 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/js/reset-password.cc5953a6.js.map
+-rw-r--r--   0        0        0     3564 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/js/start.5f1fab73.js
+-rw-r--r--   0        0        0     3431 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/js/start.5f1fab73.js.map
+-rw-r--r--   0        0        0      315 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/manifest.json
+-rw-r--r--   0        0        0     1909 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/precache-manifest.b4123667328a01c6185efab765d92c10.js
+-rw-r--r--   0        0        0       24 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/robots.txt
+-rw-r--r--   0        0        0     1063 2023-06-30 03:36:20.235844 beastiary-1.6.1/beastiary/webapp-dist/service-worker.js
+-rw-r--r--   0        0        0      617 2023-06-30 03:36:20.235844 beastiary-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 beastiary-1.6.1/PKG-INFO
```

### Comparing `beastiary-1.6.0/PYPI-README.md` & `beastiary-1.6.1/PYPI-README.md`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/api/core.py` & `beastiary-1.6.1/beastiary/api/core.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/api/endpoints/explorer.py` & `beastiary-1.6.1/beastiary/api/endpoints/explorer.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/api/endpoints/traces.py` & `beastiary-1.6.1/beastiary/api/endpoints/traces.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     trace_id: int,
     skip: int = 0,
     limit: int = 100,
 ) -> Any:
     """
     Retrieve samples.
     """
-    print(trace_id)
     trace = crud.trace.get(db=request.app.db, id=trace_id)
     if not trace:
         raise HTTPException(404, detail="Trace not found!")
 
     samples = crud.sample.get_multi_by_trace(
         request.app.db, trace_id=trace["id"], skip=skip, limit=limit
     )
```

### Comparing `beastiary-1.6.0/beastiary/api/main.py` & `beastiary-1.6.1/beastiary/api/main.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/cli.py` & `beastiary-1.6.1/beastiary/cli.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/crud/base.py` & `beastiary-1.6.1/beastiary/crud/base.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/crud/crud_sample.py` & `beastiary-1.6.1/beastiary/crud/crud_sample.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/crud/crud_trace.py` & `beastiary-1.6.1/beastiary/crud/crud_trace.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/db/database.py` & `beastiary-1.6.1/beastiary/db/database.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/schemas/sample.py` & `beastiary-1.6.1/beastiary/schemas/sample.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/schemas/trace.py` & `beastiary-1.6.1/beastiary/schemas/trace.py`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/css/chunk-vendors.5b404c1b.css` & `beastiary-1.6.1/beastiary/webapp-dist/css/chunk-vendors.5b404c1b.css`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/css/login.4b7f13da.css` & `beastiary-1.6.1/beastiary/webapp-dist/css/login.4b7f13da.css`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/css/login~main-dashboard.49552835.css` & `beastiary-1.6.1/beastiary/webapp-dist/css/login~main-dashboard.49552835.css`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/css/login~main~main-dashboard.87cb79bc.css` & `beastiary-1.6.1/beastiary/webapp-dist/css/login~main~main-dashboard.87cb79bc.css`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/css/main-dashboard.02d99ae8.css` & `beastiary-1.6.1/beastiary/webapp-dist/css/main-dashboard.02d99ae8.css`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/css/main.38cd41ea.css` & `beastiary-1.6.1/beastiary/webapp-dist/css/main.38cd41ea.css`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/css/main~main-dashboard.27813474.css` & `beastiary-1.6.1/beastiary/webapp-dist/css/main~main-dashboard.27813474.css`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/favicon.ico` & `beastiary-1.6.1/beastiary/webapp-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/index.html` & `beastiary-1.6.1/beastiary/webapp-dist/index.html`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/app.92353b76.js` & `beastiary-1.6.1/beastiary/webapp-dist/js/app.92353b76.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/app.92353b76.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/app.92353b76.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/chunk-vendors.9a0991d8.js` & `beastiary-1.6.1/beastiary/webapp-dist/js/chunk-vendors.9a0991d8.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/chunk-vendors.9a0991d8.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/chunk-vendors.9a0991d8.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/login.ed57607a.js` & `beastiary-1.6.1/beastiary/webapp-dist/js/login.ed57607a.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/login.ed57607a.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/login.ed57607a.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/login~main-dashboard.3ae3e551.js` & `beastiary-1.6.1/beastiary/webapp-dist/js/login~main-dashboard.3ae3e551.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/login~main-dashboard.3ae3e551.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/login~main-dashboard.3ae3e551.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/login~main~main-dashboard.3a1f6d10.js` & `beastiary-1.6.1/beastiary/webapp-dist/js/login~main~main-dashboard.3a1f6d10.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/login~main~main-dashboard.3a1f6d10.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/login~main~main-dashboard.3a1f6d10.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/main-dashboard.cdaf674a.js` & `beastiary-1.6.1/beastiary/webapp-dist/js/main-dashboard.cdaf674a.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/main-dashboard.cdaf674a.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/main-dashboard.cdaf674a.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/main.fd1e121b.js` & `beastiary-1.6.1/beastiary/webapp-dist/js/main.fd1e121b.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/main.fd1e121b.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/main.fd1e121b.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/main~main-dashboard.80ebc61e.js` & `beastiary-1.6.1/beastiary/webapp-dist/js/main~main-dashboard.80ebc61e.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/main~main-dashboard.80ebc61e.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/main~main-dashboard.80ebc61e.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/reset-password.cc5953a6.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/reset-password.cc5953a6.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/start.5f1fab73.js` & `beastiary-1.6.1/beastiary/webapp-dist/js/start.5f1fab73.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/js/start.5f1fab73.js.map` & `beastiary-1.6.1/beastiary/webapp-dist/js/start.5f1fab73.js.map`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/precache-manifest.b4123667328a01c6185efab765d92c10.js` & `beastiary-1.6.1/beastiary/webapp-dist/precache-manifest.b4123667328a01c6185efab765d92c10.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/beastiary/webapp-dist/service-worker.js` & `beastiary-1.6.1/beastiary/webapp-dist/service-worker.js`

 * *Files identical despite different names*

### Comparing `beastiary-1.6.0/pyproject.toml` & `beastiary-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beastiary"
-version = "1.6.0"
+version = "1.6.1"
 description = ""
 authors = ["Wytamma Wirth <wytamma.wirth@me.com>"]
 readme = "PYPI-README.md"
 
 [tool.poetry.scripts]
 beastiary = "beastiary.cli:app"
```

### Comparing `beastiary-1.6.0/PKG-INFO` & `beastiary-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beastiary
-Version: 1.6.0
+Version: 1.6.1
 Summary: 
 Author: Wytamma Wirth
 Author-email: wytamma.wirth@me.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beastiary Version: 1.6.0 Summary: Author: Wytamma
+Metadata-Version: 2.1 Name: beastiary Version: 1.6.1 Summary: Author: Wytamma
 Wirth Author-email: wytamma.wirth@me.com Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (<0.6.0) Requires-Dist: fastapi[all] (>=0.95.1,<0.96.0)
 Requires-Dist: typer[all] (>=0.3.2,<0.4.0) Description-Content-Type: text/
```

