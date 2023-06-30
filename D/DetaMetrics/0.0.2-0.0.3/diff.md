# Comparing `tmp/DetaMetrics-0.0.2.tar.gz` & `tmp/DetaMetrics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DetaMetrics-0.0.2.tar", last modified: Fri Jun 30 14:29:46 2023, max compression
+gzip compressed data, was "DetaMetrics-0.0.3.tar", last modified: Fri Jun 30 14:35:29 2023, max compression
```

## Comparing `DetaMetrics-0.0.2.tar` & `DetaMetrics-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 14:29:46.876166 DetaMetrics-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-30 14:29:46.860634 DetaMetrics-0.0.2/DetaMetrics.egg-info/
--rw-rw-rw-   0        0        0     1301 2023-06-30 14:29:46.000000 DetaMetrics-0.0.2/DetaMetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-30 14:29:46.000000 DetaMetrics-0.0.2/DetaMetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 14:29:46.000000 DetaMetrics-0.0.2/DetaMetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 14:29:46.000000 DetaMetrics-0.0.2/DetaMetrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-06-30 12:12:35.000000 DetaMetrics-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1301 2023-06-30 14:29:46.874870 DetaMetrics-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      923 2023-06-30 14:06:48.000000 DetaMetrics-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 14:29:46.872287 DetaMetrics-0.0.2/detametrics/
--rw-rw-rw-   0        0        0       28 2023-06-30 12:00:58.000000 DetaMetrics-0.0.2/detametrics/__init__.py
--rw-rw-rw-   0        0        0      734 2023-06-30 14:11:22.000000 DetaMetrics-0.0.2/detametrics/sdk.py
--rw-rw-rw-   0        0        0      502 2023-06-30 12:00:54.000000 DetaMetrics-0.0.2/detametrics/tf.py
--rw-rw-rw-   0        0        0      457 2023-06-30 14:29:32.000000 DetaMetrics-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 14:29:46.876166 DetaMetrics-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 14:35:29.484120 DetaMetrics-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-30 14:35:29.474998 DetaMetrics-0.0.3/DetaMetrics.egg-info/
+-rw-rw-rw-   0        0        0     1301 2023-06-30 14:35:29.000000 DetaMetrics-0.0.3/DetaMetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-30 14:35:29.000000 DetaMetrics-0.0.3/DetaMetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:35:29.000000 DetaMetrics-0.0.3/DetaMetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 14:35:29.000000 DetaMetrics-0.0.3/DetaMetrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-06-30 12:12:35.000000 DetaMetrics-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1301 2023-06-30 14:35:29.484120 DetaMetrics-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2023-06-30 14:06:48.000000 DetaMetrics-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 14:35:29.484120 DetaMetrics-0.0.3/detametrics/
+-rw-rw-rw-   0        0        0       28 2023-06-30 12:00:58.000000 DetaMetrics-0.0.3/detametrics/__init__.py
+-rw-rw-rw-   0        0        0      696 2023-06-30 14:35:04.000000 DetaMetrics-0.0.3/detametrics/sdk.py
+-rw-rw-rw-   0        0        0      502 2023-06-30 12:00:54.000000 DetaMetrics-0.0.3/detametrics/tf.py
+-rw-rw-rw-   0        0        0      457 2023-06-30 14:34:53.000000 DetaMetrics-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 14:35:29.484120 DetaMetrics-0.0.3/setup.cfg
```

### Comparing `DetaMetrics-0.0.2/DetaMetrics.egg-info/PKG-INFO` & `DetaMetrics-0.0.3/DetaMetrics.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DetaMetrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: SDK for DetaMetrics TensorBoard alternative.
 Author: SamTheProgrammer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `DetaMetrics-0.0.2/LICENSE` & `DetaMetrics-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DetaMetrics-0.0.2/PKG-INFO` & `DetaMetrics-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DetaMetrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: SDK for DetaMetrics TensorBoard alternative.
 Author: SamTheProgrammer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `DetaMetrics-0.0.2/README.md` & `DetaMetrics-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `DetaMetrics-0.0.2/detametrics/sdk.py` & `DetaMetrics-0.0.3/detametrics/sdk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import httpx
 
 class DetaMetrics:
-    def __init__(self, urlId: str, apiKey: str) -> None:
+    def __init__(self, urlId: str) -> None:
         self.url = "https://" + urlId + ".deta.app"
-        self.__apiKey = apiKey
-        self.__headers = {"User-Agent": "DetaMetrics", "X-Space-App-Key": self.__apiKey}
-        print(f"Using DetaMetrics at {self.url}")
+        # self.__apiKey = apiKey
+        self.__headers = {"User-Agent": "DetaMetrics"}
+        print(f"Using DetaMetrics Server at {self.url}")
 
     def __repr__(self) -> str:
         return f"<DetaMetrics url={self.url}>"
 
     def __str__(self) -> str:
         return f"DetaMetrics(url={self.url})"
```

