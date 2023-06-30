# Comparing `tmp/foma_bindings-0.1.1.tar.gz` & `tmp/foma_bindings-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foma_bindings-0.1.1.tar", last modified: Fri Jun 30 02:06:01 2023, max compression
+gzip compressed data, was "foma_bindings-0.1.2.tar", last modified: Fri Jun 30 02:20:31 2023, max compression
```

## Comparing `foma_bindings-0.1.1.tar` & `foma_bindings-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:06:01.067374 foma_bindings-0.1.1/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    11361 2023-06-22 16:58:19.000000 foma_bindings-0.1.1/LICENSE.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3783 2023-06-30 02:06:01.067374 foma_bindings-0.1.1/PKG-INFO
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     2986 2023-06-23 15:26:24.000000 foma_bindings-0.1.1/README.md
-drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:06:01.067374 foma_bindings-0.1.1/foma_bindings.egg-info/
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3783 2023-06-30 02:06:01.000000 foma_bindings-0.1.1/foma_bindings.egg-info/PKG-INFO
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)      193 2023-06-30 02:06:01.000000 foma_bindings-0.1.1/foma_bindings.egg-info/SOURCES.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-06-30 02:06:01.000000 foma_bindings-0.1.1/foma_bindings.egg-info/dependency_links.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-06-30 02:06:01.000000 foma_bindings-0.1.1/foma_bindings.egg-info/top_level.txt
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       98 2023-06-23 14:47:50.000000 foma_bindings-0.1.1/pyproject.toml
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       38 2023-06-30 02:06:01.067374 foma_bindings-0.1.1/setup.cfg
--rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     1615 2023-06-30 02:05:55.000000 foma_bindings-0.1.1/setup.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:20:31.135646 foma_bindings-0.1.2/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)    11361 2023-06-22 16:58:19.000000 foma_bindings-0.1.2/LICENSE.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3786 2023-06-30 02:20:31.135646 foma_bindings-0.1.2/PKG-INFO
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     2986 2023-06-23 15:26:24.000000 foma_bindings-0.1.2/README.md
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:20:31.135646 foma_bindings-0.1.2/foma_bindings/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     4769 2023-06-23 12:54:26.000000 foma_bindings-0.1.2/foma_bindings/__init__.py
+drwxrwxr-x   0 parkhill  (1000) parkhill  (1000)        0 2023-06-30 02:20:31.135646 foma_bindings-0.1.2/foma_bindings.egg-info/
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     3786 2023-06-30 02:20:31.000000 foma_bindings-0.1.2/foma_bindings.egg-info/PKG-INFO
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)      219 2023-06-30 02:20:31.000000 foma_bindings-0.1.2/foma_bindings.egg-info/SOURCES.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)        1 2023-06-30 02:20:31.000000 foma_bindings-0.1.2/foma_bindings.egg-info/dependency_links.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       14 2023-06-30 02:20:31.000000 foma_bindings-0.1.2/foma_bindings.egg-info/top_level.txt
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       98 2023-06-23 14:47:50.000000 foma_bindings-0.1.2/pyproject.toml
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)       38 2023-06-30 02:20:31.135646 foma_bindings-0.1.2/setup.cfg
+-rw-rw-r--   0 parkhill  (1000) parkhill  (1000)     1635 2023-06-30 02:20:25.000000 foma_bindings-0.1.2/setup.py
```

### Comparing `foma_bindings-0.1.1/LICENSE.txt` & `foma_bindings-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.1/PKG-INFO` & `foma_bindings-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: foma_bindings
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python bindings for the foma finite-state technology suite
 Home-page: https://github.com/CultureFoundryCA/foma_bindings
 Author: CultureFoundry
 Author-email: info@culturefoundrystudios.com
 License: Apache 2.0
 Keywords: foma,xfst,hfst,fst,fsm,mtfst,mtfsm
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3, <4
+Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # foma_bindings: Foma Python Bindings
 
 These are python bindings for `foma`, [a finite-state toolkit](https://fomafst.github.io/) developed by [Dr. Mans Hulden](https://www.colorado.edu/linguistics/mans-hulden). These bindings are a subset of the functionality of `foma`, and are a modification of the file(s) in the `python` folder in the above `foma` repo. Those file(s) are edited, expanded, cleaned up, and packaged for distribution through `pip`; the changes made are listed below.
```

### Comparing `foma_bindings-0.1.1/README.md` & `foma_bindings-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `foma_bindings-0.1.1/foma_bindings.egg-info/PKG-INFO` & `foma_bindings-0.1.2/foma_bindings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: foma-bindings
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python bindings for the foma finite-state technology suite
 Home-page: https://github.com/CultureFoundryCA/foma_bindings
 Author: CultureFoundry
 Author-email: info@culturefoundrystudios.com
 License: Apache 2.0
 Keywords: foma,xfst,hfst,fst,fsm,mtfst,mtfsm
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3, <4
+Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # foma_bindings: Foma Python Bindings
 
 These are python bindings for `foma`, [a finite-state toolkit](https://fomafst.github.io/) developed by [Dr. Mans Hulden](https://www.colorado.edu/linguistics/mans-hulden). These bindings are a subset of the functionality of `foma`, and are a modification of the file(s) in the `python` folder in the above `foma` repo. Those file(s) are edited, expanded, cleaned up, and packaged for distribution through `pip`; the changes made are listed below.
```

### Comparing `foma_bindings-0.1.1/setup.py` & `foma_bindings-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 from setuptools import setup, find_packages
 
 setup(
     name='foma_bindings',
-    version='0.1.1',
+    version='0.1.2',
     description='Python bindings for the foma finite-state technology suite',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/CultureFoundryCA/foma_bindings',
     author='CultureFoundry',
     author_email='info@culturefoundrystudios.com',
     license='Apache 2.0',
@@ -30,10 +30,10 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3'
     ],
     keywords=['foma', 'xfst', 'hfst', 'fst', 'fsm', 'mtfst', 'mtfsm'],
-    packages=find_packages(include=['fst', 'mtfst']),
-    python_requires='>=3, <4',
+    packages=find_packages(include=['foma_bindings', 'fst', 'mtfst']),
+    python_requires='>=3.10, <4',
 )
```

