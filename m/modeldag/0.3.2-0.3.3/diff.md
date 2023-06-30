# Comparing `tmp/modeldag-0.3.2.tar.gz` & `tmp/modeldag-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modeldag-0.3.2.tar", last modified: Fri Jun  2 09:18:10 2023, max compression
+gzip compressed data, was "modeldag-0.3.3.tar", last modified: Fri Jun 30 08:44:12 2023, max compression
```

## Comparing `modeldag-0.3.2.tar` & `modeldag-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 09:18:10.174135 modeldag-0.3.2/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-05-31 13:06:56.000000 modeldag-0.3.2/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-02 09:18:10.174199 modeldag-0.3.2/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     1896 2023-06-02 08:39:03.000000 modeldag-0.3.2/README.md
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 09:18:10.173397 modeldag-0.3.2/modeldag/
--rw-r--r--   0 rigault   (2358) staff       (20)       47 2023-06-02 09:18:01.000000 modeldag-0.3.2/modeldag/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    14448 2023-06-02 09:10:36.000000 modeldag-0.3.2/modeldag/modeldag.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 09:18:10.174044 modeldag-0.3.2/modeldag.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      268 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 13:38:23.000000 modeldag-0.3.2/modeldag.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)       55 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        9 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/top_level.txt
--rw-r--r--   0 rigault   (2358) staff       (20)     1020 2023-06-02 09:18:10.174517 modeldag-0.3.2/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-05-31 13:36:34.000000 modeldag-0.3.2/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 08:44:12.647832 modeldag-0.3.3/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-05-31 13:06:56.000000 modeldag-0.3.3/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      725 2023-06-30 08:44:12.647877 modeldag-0.3.3/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     1896 2023-06-30 08:42:53.000000 modeldag-0.3.3/README.md
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 08:44:12.647116 modeldag-0.3.3/modeldag/
+-rw-r--r--   0 rigault   (2358) staff       (20)       47 2023-06-30 08:40:07.000000 modeldag-0.3.3/modeldag/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    15196 2023-06-26 15:11:38.000000 modeldag-0.3.3/modeldag/modeldag.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-30 08:44:12.647734 modeldag-0.3.3/modeldag.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      725 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      268 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 13:38:23.000000 modeldag-0.3.3/modeldag.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)       55 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        9 2023-06-30 08:44:12.000000 modeldag-0.3.3/modeldag.egg-info/top_level.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)     1004 2023-06-30 08:44:12.648128 modeldag-0.3.3/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-05-31 13:36:34.000000 modeldag-0.3.3/setup.py
```

### Comparing `modeldag-0.3.2/LICENSE` & `modeldag-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modeldag-0.3.2/PKG-INFO` & `modeldag-0.3.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: modeldag
-Version: 0.3.2
+Version: 0.3.3
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/modeldag
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
-License: BSD 3-Clause "New" or "Revised" License
+License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `modeldag-0.3.2/README.md` & `modeldag-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ## Dependency
 - numpy
 - pandas
 - graphviz (optional, used for visualize)
 
 # Concept
 
-Build a simple dictionary forming a DAG ; this is the `model` and call `mdag = ModelDAG(model)`.
+Build a simple dictionary forming a DAG (this is the `model`) and call `mdag = ModelDAG(model)`.
 
 The model dictionary is a simple nested directory with the following format: 
 ```python
 model = {key1 : {'func': func, 'kwargs': dict, 'as': None_str_list'},
          key2 : {'func': func, 'kwargs': dict, 'as': None_str_list'},
          ...
          }
```

### Comparing `modeldag-0.3.2/modeldag/modeldag.py` & `modeldag-0.3.3/modeldag/modeldag.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         # naming convention
         f_ = dd["as"].fillna( dict(dd["model_name"]) )
         f_.name = "entry"
         dd = dd.join(f_) # merge and explode the names and inputs
         
     return dd
 
-
 class ModelDAG( object ):
     """
     Models are dict of arguments that may have 3 entries:
     model = {key1 : {'func': func, 'kwargs': dict, 'as': None_str_list'},
              key2 : {'func': func, 'kwargs': dict, 'as': None_str_list'},
              ...
              }
@@ -129,29 +128,54 @@
         Returns
         -------
         dict
            a copy of the model (with param potentially updated)
         """
         model = deepcopy(self.model)
         for k,v in kwargs.items():
-            model[k]["kwargs"].update(v)
+            model[k]["kwargs"] = {**model[k].get("kwargs",{}), **v}
 
         return model
     
     def change_model(self, **kwargs):
         """ change the model attached to this instance
         
         **kwargs will update the entry  parameters ("param", e.g. t0["kwargs"])
 
         See also
         --------
         get_model: get a copy of the model
         """
         self.model = self.get_model(**kwargs)
 
+    def get_func_parameters(self, valdefault="unknown"):
+        """ get a dictionary with the parameters name of all model functions
+        
+        Parameters
+        ----------
+        valdefault: str, None
+            value used with function inspection fails
+            (like e.g. np.random.rand).
+
+        Returns
+        -------
+        dict
+        """
+        import inspect
+        inspected = {}
+        for k, m in self.model.items():
+            func = self._parse_input_func(name=k, func=m.get("func", None))
+            try:
+                params = inspect.getfullargspec(func).args
+            except:
+                params = valdefault
+            inspected[k] = params
+
+        return inspected
+    
     def get_backward_entries(self, name, incl_input=True):
         """ get the list of entries that affects the input on.
         Changing any of the return entry name impact the given name.
 
         Parameters
         ----------
         name: str
```

### Comparing `modeldag-0.3.2/modeldag.egg-info/PKG-INFO` & `modeldag-0.3.3/modeldag.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: modeldag
-Version: 0.3.2
+Version: 0.3.3
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/modeldag
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
-License: BSD 3-Clause "New" or "Revised" License
+License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `modeldag-0.3.2/setup.cfg` & `modeldag-0.3.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = modeldag
 version = attr: modeldag.__version__
 description = Access and Interact with ZTF Fields
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Mickael Rigault
 author_email = m.rigault@ipnl.in2p3.fr
-license = BSD 3-Clause "New" or "Revised" License
+license = Apache Software License
 license_files = LICENSE
 url = https://github.com/MickaelRigault/modeldag
 keywords = astronomy, astrophysics
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
```

