# Comparing `tmp/server-roberta-0.4.3.tar.gz` & `tmp/server-roberta-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server-roberta-0.4.3.tar", last modified: Fri Jun 30 19:03:54 2023, max compression
+gzip compressed data, was "server-roberta-0.4.4.tar", last modified: Fri Jun 30 19:27:27 2023, max compression
```

## Comparing `server-roberta-0.4.3.tar` & `server-roberta-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:03:54.959348 server-roberta-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 19:03:54.959348 server-roberta-0.4.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:03:54.959348 server-roberta-0.4.3/serverRoberta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/datos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/robertaModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/roberta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/roberta_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:03:54.959348 server-roberta-0.4.3/server_roberta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:03:54.959348 server-roberta-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-30 19:02:17.000000 server-roberta-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:27.943363 server-roberta-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 19:27:27.943363 server-roberta-0.4.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:27.943363 server-roberta-0.4.4/serverRoberta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:25:31.000000 server-roberta-0.4.4/serverRoberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:25:31.000000 server-roberta-0.4.4/serverRoberta/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 19:25:31.000000 server-roberta-0.4.4/serverRoberta/datos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-30 19:25:31.000000 server-roberta-0.4.4/serverRoberta/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-30 19:25:31.000000 server-roberta-0.4.4/serverRoberta/robertaModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-30 19:25:31.000000 server-roberta-0.4.4/serverRoberta/roberta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-30 19:25:31.000000 server-roberta-0.4.4/serverRoberta/roberta_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-30 19:25:31.000000 server-roberta-0.4.4/serverRoberta/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:27:27.943363 server-roberta-0.4.4/server_roberta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 19:27:27.000000 server-roberta-0.4.4/server_roberta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-30 19:27:27.000000 server-roberta-0.4.4/server_roberta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:27:27.000000 server-roberta-0.4.4/server_roberta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 19:27:27.000000 server-roberta-0.4.4/server_roberta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 19:27:27.000000 server-roberta-0.4.4/server_roberta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 19:27:27.000000 server-roberta-0.4.4/server_roberta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:27:27.943363 server-roberta-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-30 19:25:31.000000 server-roberta-0.4.4/setup.py
```

### Comparing `server-roberta-0.4.3/serverRoberta/encrypt.py` & `server-roberta-0.4.4/serverRoberta/encrypt.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.4.3/serverRoberta/robertaModel.py` & `server-roberta-0.4.4/serverRoberta/robertaModel.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.4.3/serverRoberta/roberta_pb2.py` & `server-roberta-0.4.4/serverRoberta/roberta_pb2.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.4.3/serverRoberta/roberta_pb2_grpc.py` & `server-roberta-0.4.4/serverRoberta/roberta_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.4.3/serverRoberta/server.py` & `server-roberta-0.4.4/serverRoberta/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,19 @@
             pred = self.roberta.evalObfuscation(self.map,data)
             logging.info('time data obfuscation eval ready %r ',time.time()-inicio)   
         else:  
             pred = self.roberta.eval(data) 
             logging.info('time data eval ready %r ',time.time()-inicio) 
 
         out=[]
-        out.append(modDataLog(label=pred.label,decision=pred.decision))
+        if isinstance(pred, float):
+            decisionPred=pred
+        else:
+            decisionPred=pred.decision[0]
+        out.append(modDataLog(label=pred.label,decision=decisionPred))
         with open(self.dataBPE+"/dataTime.csv", 'a') as f:
             f.write(str(self.roberta.token)+","+str(self.roberta.timeTokenize)+","+str(self.roberta.timeApply_bpe)+","+str(self.roberta.timeObfuscate)+","+str(self.roberta.timeBinarize)+","+str(self.roberta.timeExtract_features)+","+str(self.roberta.timePredict)+","+str(self.roberta.timeDecision)+","+str(self.roberta.total)+"\n")
             f.close()
             
         return out    
 
 def main():
```

### Comparing `server-roberta-0.4.3/setup.py` & `server-roberta-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 base_dir = os.path.dirname(__file__)
 setup(
    name='server-roberta',
-   version='0.4.3',
+   version='0.4.4',
    description='To classify, BPE, ROBERTA and SVM are used',
    long_description_content_type="text/markdown",
    long_description="README",
    author='Tilsor',
    author_email='tilsor@tilsor.com.uy',
    setup_requires='setuptools',
    entry_points={
```

