# Comparing `tmp/foma_bindings-0.1.0.tar.gz` & `tmp/foma_bindings-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foma_bindings-0.1.0.tar", last modified: Wed Jun 28 13:24:01 2023, max compression
+gzip compressed data, was "foma_bindings-0.1.1.tar", last modified: Fri Jun 30 02:06:01 2023, max compression
```

## Comparing `foma_bindings-0.1.0.tar` & `foma_bindings-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-28 13:24:01.278561 foma_bindings-0.1.0/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    11361 2023-06-22 16:58:19.000000 foma_bindings-0.1.0/LICENSE.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3783 2023-06-28 13:24:01.278561 foma_bindings-0.1.0/PKG-INFO
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     2986 2023-06-23 15:26:24.000000 foma_bindings-0.1.0/README.md
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-28 13:24:01.278561 foma_bindings-0.1.0/foma_bindings.egg-info/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3783 2023-06-28 13:24:01.000000 foma_bindings-0.1.0/foma_bindings.egg-info/PKG-INFO
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)      229 2023-06-28 13:24:01.000000 foma_bindings-0.1.0/foma_bindings.egg-info/SOURCES.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-06-28 13:24:01.000000 foma_bindings-0.1.0/foma_bindings.egg-info/dependency_links.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       11 2023-06-28 13:24:01.000000 foma_bindings-0.1.0/foma_bindings.egg-info/requires.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-06-28 13:24:01.000000 foma_bindings-0.1.0/foma_bindings.egg-info/top_level.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       98 2023-06-23 14:47:50.000000 foma_bindings-0.1.0/pyproject.toml
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       38 2023-06-28 13:24:01.278561 foma_bindings-0.1.0/setup.cfg
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     1676 2023-06-23 14:31:13.000000 foma_bindings-0.1.0/setup.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:06:01.067374 foma_bindings-0.1.1/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    11361 2023-06-22 16:58:19.000000 foma_bindings-0.1.1/LICENSE.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3783 2023-06-30 02:06:01.067374 foma_bindings-0.1.1/PKG-INFO
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     2986 2023-06-23 15:26:24.000000 foma_bindings-0.1.1/README.md
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:06:01.067374 foma_bindings-0.1.1/foma_bindings.egg-info/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3783 2023-06-30 02:06:01.000000 foma_bindings-0.1.1/foma_bindings.egg-info/PKG-INFO
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)      193 2023-06-30 02:06:01.000000 foma_bindings-0.1.1/foma_bindings.egg-info/SOURCES.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-06-30 02:06:01.000000 foma_bindings-0.1.1/foma_bindings.egg-info/dependency_links.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-06-30 02:06:01.000000 foma_bindings-0.1.1/foma_bindings.egg-info/top_level.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       98 2023-06-23 14:47:50.000000 foma_bindings-0.1.1/pyproject.toml
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       38 2023-06-30 02:06:01.067374 foma_bindings-0.1.1/setup.cfg
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     1615 2023-06-30 02:05:55.000000 foma_bindings-0.1.1/setup.py
```

### Comparing `foma_bindings-0.1.0/LICENSE.txt` & `foma_bindings-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.0/PKG-INFO` & `foma_bindings-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foma_bindings
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python bindings for the foma finite-state technology suite
 Home-page: https://github.com/CultureFoundryCA/foma_bindings
 Author: CultureFoundry
 Author-email: info@culturefoundrystudios.com
 License: Apache 2.0
 Keywords: foma,xfst,hfst,fst,fsm,mtfst,mtfsm
 Platform: UNKNOWN
```

### Comparing `foma_bindings-0.1.0/README.md` & `foma_bindings-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.0/foma_bindings.egg-info/PKG-INFO` & `foma_bindings-0.1.1/foma_bindings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foma-bindings
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python bindings for the foma finite-state technology suite
 Home-page: https://github.com/CultureFoundryCA/foma_bindings
 Author: CultureFoundry
 Author-email: info@culturefoundrystudios.com
 License: Apache 2.0
 Keywords: foma,xfst,hfst,fst,fsm,mtfst,mtfsm
 Platform: UNKNOWN
```

### Comparing `foma_bindings-0.1.0/setup.py` & `foma_bindings-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 from setuptools import setup, find_packages
 
 setup(
     name='foma_bindings',
-    version='0.1.0',
+    version='0.1.1',
     description='Python bindings for the foma finite-state technology suite',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/CultureFoundryCA/foma_bindings',
     author='CultureFoundry',
     author_email='info@culturefoundrystudios.com',
     license='Apache 2.0',
@@ -32,12 +32,8 @@
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3'
     ],
     keywords=['foma', 'xfst', 'hfst', 'fst', 'fsm', 'mtfst', 'mtfsm'],
     packages=find_packages(include=['fst', 'mtfst']),
     python_requires='>=3, <4',
-    install_requires=[
-        'sys',
-        'ctypes'
-    ]
 )
```

