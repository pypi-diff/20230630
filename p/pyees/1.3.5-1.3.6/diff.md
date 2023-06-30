# Comparing `tmp/pyees-1.3.5.tar.gz` & `tmp/pyees-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.3.5.tar", last modified: Fri Jun 30 11:36:18 2023, max compression
+gzip compressed data, was "pyees-1.3.6.tar", last modified: Fri Jun 30 12:09:06 2023, max compression
```

## Comparing `pyees-1.3.5.tar` & `pyees-1.3.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 11:36:18.111613 pyees-1.3.5/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-06-30 11:36:18.117598 pyees-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 11:36:17.919128 pyees-1.3.5/pyees/
--rw-rw-rw-   0        0        0      320 2023-06-30 11:36:17.451378 pyees-1.3.5/pyees/__init__.py
--rw-rw-rw-   0        0        0    12847 2023-06-28 06:38:17.000000 pyees-1.3.5/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-06-30 11:36:17.509368 pyees-1.3.5/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10013 2023-06-30 11:34:55.000000 pyees-1.3.5/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.5/pyees/sheet.py
--rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.3.5/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.5/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-06-28 06:38:39.000000 pyees-1.3.5/pyees/testFit.py
--rw-rw-rw-   0        0        0    13373 2023-06-30 11:31:13.000000 pyees-1.3.5/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.5/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.5/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.3.5/pyees/testSolve.py
--rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.3.5/pyees/testUnit.py
--rw-rw-rw-   0        0        0    83073 2023-06-28 06:43:51.000000 pyees-1.3.5/pyees/testVariable.py
--rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.3.5/pyees/unit.py
--rw-rw-rw-   0        0        0    35206 2023-06-28 06:43:10.000000 pyees-1.3.5/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:36:18.086680 pyees-1.3.5/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-06-30 11:36:16.000000 pyees-1.3.5/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-06-30 11:36:17.000000 pyees-1.3.5/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 11:36:16.000000 pyees-1.3.5/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-30 11:36:16.000000 pyees-1.3.5/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-30 11:36:16.000000 pyees-1.3.5/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-30 11:36:18.145524 pyees-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-06-30 11:36:01.000000 pyees-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:09:06.717398 pyees-1.3.6/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-06-30 12:09:06.723383 pyees-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 12:09:06.518934 pyees-1.3.6/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.6/pyees/__init__.py
+-rw-rw-rw-   0        0        0    13756 2023-06-30 12:08:37.000000 pyees-1.3.6/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.3.6/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10013 2023-06-30 11:34:55.000000 pyees-1.3.6/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.6/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.3.6/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.6/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-06-30 12:05:47.000000 pyees-1.3.6/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13373 2023-06-30 11:31:13.000000 pyees-1.3.6/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.6/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.6/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.3.6/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.3.6/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    83073 2023-06-28 06:43:51.000000 pyees-1.3.6/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.3.6/pyees/unit.py
+-rw-rw-rw-   0        0        0    35206 2023-06-28 06:43:10.000000 pyees-1.3.6/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:09:06.691468 pyees-1.3.6/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 12:09:05.000000 pyees-1.3.6/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-30 12:09:06.749313 pyees-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-06-30 12:08:56.000000 pyees-1.3.6/setup.py
```

### Comparing `pyees-1.3.5/LICENSE.txt` & `pyees-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/PKG-INFO` & `pyees-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.5
+Version: 1.3.6
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.5/README.md` & `pyees-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/fit.py` & `pyees-1.3.6/pyees/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,21 +63,21 @@
                 self.coefficients[i].addCovariance(
                     var = self.coefficients[j],
                     covariance = regression.cov_beta[i,j],
                     unitStr = str(self.coefficients[i]._unitObject * self.coefficients[j]._unitObject)
                 )
 
         # determine r-squared
-        self._residuals = y - self.predict(x)
+        self._residuals = y - self._predict(x)
         ss_res = sum(self._residuals**2)
         ss_tot = sum((y - np.mean(y))**2)
         if ss_tot != 0:
             self.r_squared = 1 - (ss_res / ss_tot)
         else:
-            self.r_squared = 1
+            self.r_squared = variable(1)
         np.seterr('warn')
 
     def __str__(self):
         return self.func_name() + ',  ' + self._r2_name()
 
     def _r2_name(self):
         return f'$R^2 = {self.r_squared.value:.5f}$'
@@ -155,17 +155,35 @@
         else:
             raise ValueError('The label has to be a string, a bool or None')
 
         ax.plot(self.xVal, self.yVal, label=label, **kwargs)
 
     def predict(self, x):
         if not isinstance(x, scalarVariable):
+            raise ValueError('The input "x" has to be a variable')
+        return self.func(x)
+    
+    def _predict(self, x):
+        if not isinstance(x, scalarVariable):
             x = variable(x, self.xUnit)
         return self.func(x)
 
+    def plotUncertanty(self, ax, x = None, **kwargs):
+        
+        if x is None:
+            x = variable(np.linspace(np.min(self.xVal), np.max(self.xVal), 100), self.xUnit)
+        else:
+            if not isinstance(x, arrayVariable):
+                raise ValueError('The input "x" has to be a variable')
+            
+        y = self.predict(x)
+        y = list(y.value + y.uncert) + [np.nan] + list(y.value - y.uncert)
+        x = list(x.value) + [np.nan] + list(x.value)
+        ax.plot(x, y, **kwargs)
+
     def plot(self, ax, label=True, x=None, **kwargs):
 
         # parse label
         if isinstance(label, str):
             label = label
         elif label == True:
             label = self.__str__()
@@ -173,16 +191,22 @@
             label = None
         elif label is None:
             label = None
         else:
             raise ValueError('The label has to be a string, a bool or None')
 
         if x is None:
-            x = np.linspace(np.min(self.xVal), np.max(self.xVal), 100)
+            x = variable(np.linspace(np.min(self.xVal), np.max(self.xVal), 100), self.xUnit)
+        else:
+            if not isinstance(x, arrayVariable):
+                raise ValueError('The input "x" has to be a variable')
+
         y = self.predict(x).value
+        x = x.value
+        
         ax.plot(x, y, label=label, **kwargs)
           
     def addUnitToLabels(self, ax):
         self.addUnitToXLabel(ax)
         self.addUnitToYLabel(ax)
 
     def addUnitToXLabel(self, ax):
@@ -201,15 +225,15 @@
 
     def func(self, x):
         return self._func(self.coefficients, x)
 
     def evaluateFit(self):
         ## TODO evaluate the fit - use the degrees of freedom as in the book
         
-        pred = self.predict(self.xVal)
+        pred = self._predict(self.xVal)
         
         count = 0
         for yi, uyi, pi in zip(self.yVal, self.yUncert, pred):
             
             ## count the number of datapoints were the prediction is within 1 standard deviation
             if yi == pi:
                 count += 1
```

### Comparing `pyees-1.3.5/pyees/profilePyees.py` & `pyees-1.3.6/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/prop.py` & `pyees-1.3.6/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/sheet.py` & `pyees-1.3.6/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/solve.py` & `pyees-1.3.6/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/stackOverflowODR.py` & `pyees-1.3.6/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/testFit.py` & `pyees-1.3.6/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/testProp.py` & `pyees-1.3.6/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/testPyees.py` & `pyees-1.3.6/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/testSheet.py` & `pyees-1.3.6/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/testSolve.py` & `pyees-1.3.6/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/testUnit.py` & `pyees-1.3.6/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/testVariable.py` & `pyees-1.3.6/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/unit.py` & `pyees-1.3.6/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees/variable.py` & `pyees-1.3.6/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.5/pyees.egg-info/PKG-INFO` & `pyees-1.3.6/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.5
+Version: 1.3.6
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.5/setup.py` & `pyees-1.3.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.3.5',
+    version='1.3.6',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

