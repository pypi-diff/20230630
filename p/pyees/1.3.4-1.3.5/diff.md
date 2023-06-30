# Comparing `tmp/pyees-1.3.4.tar.gz` & `tmp/pyees-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.3.4.tar", last modified: Thu Jun 29 06:36:38 2023, max compression
+gzip compressed data, was "pyees-1.3.5.tar", last modified: Fri Jun 30 11:36:18 2023, max compression
```

## Comparing `pyees-1.3.4.tar` & `pyees-1.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 06:36:38.226601 pyees-1.3.4/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.4/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-06-29 06:36:38.242227 pyees-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 06:36:37.960965 pyees-1.3.4/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.3.4/pyees/__init__.py
--rw-rw-rw-   0        0        0    12847 2023-06-28 06:38:17.000000 pyees-1.3.4/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.3.4/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.3.4/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.4/pyees/sheet.py
--rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.3.4/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.4/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-06-28 06:38:39.000000 pyees-1.3.4/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.3.4/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.4/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.4/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.3.4/pyees/testSolve.py
--rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.3.4/pyees/testUnit.py
--rw-rw-rw-   0        0        0    83073 2023-06-28 06:43:51.000000 pyees-1.3.4/pyees/testVariable.py
--rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.3.4/pyees/unit.py
--rw-rw-rw-   0        0        0    35206 2023-06-28 06:43:10.000000 pyees-1.3.4/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:36:38.179724 pyees-1.3.4/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-29 06:36:36.000000 pyees-1.3.4/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 06:36:38.289104 pyees-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-06-29 06:36:29.000000 pyees-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:36:18.111613 pyees-1.3.5/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.3.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-06-30 11:36:18.117598 pyees-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 11:36:17.919128 pyees-1.3.5/pyees/
+-rw-rw-rw-   0        0        0      320 2023-06-30 11:36:17.451378 pyees-1.3.5/pyees/__init__.py
+-rw-rw-rw-   0        0        0    12847 2023-06-28 06:38:17.000000 pyees-1.3.5/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-06-30 11:36:17.509368 pyees-1.3.5/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10013 2023-06-30 11:34:55.000000 pyees-1.3.5/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.3.5/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.3.5/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.3.5/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-06-28 06:38:39.000000 pyees-1.3.5/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13373 2023-06-30 11:31:13.000000 pyees-1.3.5/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.3.5/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.3.5/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.3.5/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.3.5/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    83073 2023-06-28 06:43:51.000000 pyees-1.3.5/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.3.5/pyees/unit.py
+-rw-rw-rw-   0        0        0    35206 2023-06-28 06:43:10.000000 pyees-1.3.5/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:36:18.086680 pyees-1.3.5/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-06-30 11:36:16.000000 pyees-1.3.5/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-06-30 11:36:17.000000 pyees-1.3.5/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:36:16.000000 pyees-1.3.5/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-30 11:36:16.000000 pyees-1.3.5/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 11:36:16.000000 pyees-1.3.5/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-30 11:36:18.145524 pyees-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-06-30 11:36:01.000000 pyees-1.3.5/setup.py
```

### Comparing `pyees-1.3.4/LICENSE.txt` & `pyees-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/PKG-INFO` & `pyees-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.4
+Version: 1.3.5
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.4/README.md` & `pyees-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/fit.py` & `pyees-1.3.5/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/profilePyees.py` & `pyees-1.3.5/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/prop.py` & `pyees-1.3.5/pyees/prop.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dx = 0.000001
 
 def prop(property, fluid, **kwargs):
 
     if not fluid in knownFluids:
         raise ValueError(f"The fluid {fluid} is unknown")
 
-    method = knownFluids[fluid][0]
+    method = knownFluids[fluid]
         
     return method(property, kwargs)
 
 def isAllArgumentsUsed(arguments: dict):
     if (len(arguments.keys()) > 0):
         raise ValueError(f'The inputs {list(arguments.keys())} are not appropriate for this fluid')
 
@@ -85,63 +85,73 @@
         
         grads.append((y2-y1) / (2*dx*i0.value))
     
     return vars, grads
     
 
 def outputFromParameters(scalarMethod, property, params):
-
-    if (all([type(elem) == scalarVariable for elem in params if not elem is None])):
-        ## all inputs are scalars
-        out = scalarMethod(property, *params)
-        return out
-    
-    out = []
-    ns = []
-    paramVecs = [None] * len(params)
-
-    for i, param in enumerate(params):
-        if type(param) == arrayVariable:
-            paramVecs[i] = param
-            ns.append(len(param))
-    
-    if not (all([ns[0] == n] for n in ns)):
-        raise ValueError('All parameters has to have the same length')
-    
-    if ns:
-        n = ns[0]
-        for i, param in enumerate(params):
-            if param is None:
-                paramVecs[i] = [None] * n
-            elif not type(param) == arrayVariable:
-                paramVecs[i] = variable([param.value] * n, param.unit, [param.uncert] * n)
-        for i in range(n):
-            params = [elem[i] for elem in paramVecs]
-            out.append(scalarMethod(property, *params))
-        return variable([elem.value for elem in out], out[0].unit, [elem.uncert for elem in out])
+    
+    ## determine which of the parameters that are arrayVariables
+    isArrayVariable = [hasattr(param, '__len__') for param in params]
+    
+    ## return the scalarmethod if all parameters are scalarvariables
+    if sum(isArrayVariable) == 0:
+        return scalarMethod(property, *params)
+    
+    ## make sure, that all arrayVariables have the same length
+    indexesOfArrayVariables = [i for i, elem in enumerate(isArrayVariable) if elem == True]
+    n = len(params[indexesOfArrayVariables[0]])
+    for i in indexesOfArrayVariables:
+        if len(params[i]) != n:
+            raise ValueError('All parameters has to have the same length')
+    
+    ## create a list of scalar variables. This list will have the same length as the arrayVariables supplied
+    listOfScalarVariables = []
+    
+    ## loop over the length of the arrayVariables
+    for i in range(n):
+        
+        ## create a list of scalarparameter
+        scalarParams = []
+        
+        ## loop over the parameters
+        for ii, param in enumerate(params):
+            
+            ## if the current parameter is an arrayVariable, then append the i'th scalarVaraible of the arrayVariable to the list of the scalar parameters
+            if ii in indexesOfArrayVariables:
+                scalarParams.append(param[i])
+            
+            ## if the current parameter is a scalarvariable, then simply append the parameter to the scalarparameters
+            else:
+                scalarParams.append(param)
+                
+        ## append the output of the scalarmethods to the list of scalar variables
+        listOfScalarVariables.append(scalarMethod(property, *scalarParams))
         
-    return scalarMethod(property, *params)
+    ## return an arrayVariable, which is created from a list of scalarvariables
+    return arrayVariable(scalarVariables=listOfScalarVariables)
+    
+    
 
 def propWater(property, arguments):
-    
     ## find the appropriate arguments from the list
     arguments, T = findArgument(arguments, 'T', 'K')
     arguments, P = findArgument(arguments, 'P', 'Pa')
     isAllArgumentsUsed(arguments)
     
     ## store the default unit of the arguments
     Tunit = T.unit
     Punit = P.unit
     
     ## convert in to the units of pyfluids
     T.convert('C')
     P.convert('Pa')
     
     out = outputFromParameters(propWaterScalar, property, [T,P])
-        
+
     ## convert the arguments back in to the original units
     T.convert(Tunit)
     P.convert(Punit)
     
     return out
 
 def propWaterScalar(property, T,P):
@@ -211,15 +221,14 @@
     ## convert the arguments back in to the original units
     T.convert(Tunit)
     P.convert(Punit)
     
     ## return the variable
     return var
     
-
 def propHumidAir(property, arguments):
 
 
     arguments, H = findArgument(arguments, 'h', 'm', raiseError=False)
     arguments, P = findArgument(arguments, 'P', 'Pa', raiseError=False)
     arguments, T = findArgument(arguments, 'T', 'C', raiseError=True)
     arguments, Rh = findArgument(arguments, 'Rh', '', raiseError=True)
@@ -294,19 +303,23 @@
 knownProperties = [
     "density",
     "specific_heat",
     "dynamic_viscosity"
 ]
 
 knownFluids = {
-    'water': [propWater],
-    'MEG': [propMEG],
-    'air': [propHumidAir]
+    'water': propWater,
+    'MEG': propMEG,
+    'air': propHumidAir
 }
 
 
 if __name__ == "__main__":
+
+    T = variable([20,25,30], 'C', [0.1, 0.2, 0.15])
+    P = variable([1, 1.1, 1.2], 'bar', [0.03, 0.04, 0.025])
     
-    T = variable([20,30], 'C', [1,1])
-    P = variable(1, 'bar', 0.01)
-    C = variable(50,'%', 2)
+    rho = prop('density', 'water', T = T, P = P)
+    for elem in rho:
+        for key, item in elem.dependsOn.items():
+            print(key, item[1])
```

### Comparing `pyees-1.3.4/pyees/sheet.py` & `pyees-1.3.5/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/solve.py` & `pyees-1.3.5/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/stackOverflowODR.py` & `pyees-1.3.5/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/testFit.py` & `pyees-1.3.5/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/testProp.py` & `pyees-1.3.5/pyees/testProp.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,9 +261,30 @@
         compareVariableAndEESData(cp_meg[0], row1, 0)
         compareVariableAndEESData(cp_meg[1], row2, 0)
 
         mu_meg = prop('dynamic_viscosity', 'MEG', T = T, P = P, C = C)       
         compareVariableAndEESData(mu_meg[0], row1, 2)
         compareVariableAndEESData(mu_meg[1], row2, 2)
 
+    def testDependscies(self):
+        T = variable([20,25,30], 'C', [0.1, 0.2, 0.15])
+        P = variable([100000, 110000, 90000], 'Pa', [2500, 3000, 4000])
+
+        rho = prop('density', 'water', T = T, P = P)
+        
+        flow = variable(0.0016, 'm3/s', 0.0001)
+        
+        massFlow = flow * rho
+        
+        dMassFlow_dFlow = [998.206543497641114, 997.05155024142658, 995.644405820880468]
+        dMassFlow_dP = [7.32946279081818364e-10, 7.21788150328467529e-10, 7.13326743322344253e-10]
+        dMassFlow_dT = [-0.000330293371618005199, -0.000410463892510075697, -0.000483157770611803349]
+        
+        for i, elem in enumerate(massFlow):
+            self.assertAlmostEqual(elem.dependsOn[flow][1], dMassFlow_dFlow[i], 6)
+            self.assertAlmostEqual(elem.dependsOn[T[i]][1], dMassFlow_dT[i], 6)
+            self.assertAlmostEqual(elem.dependsOn[P[i]][1], dMassFlow_dP[i], 6)
+        
+      
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyees-1.3.4/pyees/testPyees.py` & `pyees-1.3.5/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/testSheet.py` & `pyees-1.3.5/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/testSolve.py` & `pyees-1.3.5/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/testUnit.py` & `pyees-1.3.5/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/testVariable.py` & `pyees-1.3.5/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/unit.py` & `pyees-1.3.5/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees/variable.py` & `pyees-1.3.5/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.3.4/pyees.egg-info/PKG-INFO` & `pyees-1.3.5/pyees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.3.4
+Version: 1.3.5
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.3.4/setup.py` & `pyees-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.3.4',
+    version='1.3.5',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

