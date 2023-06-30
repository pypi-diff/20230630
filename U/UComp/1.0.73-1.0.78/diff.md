# Comparing `tmp/UComp-1.0.73.tar.gz` & `tmp/UComp-1.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.73.tar", last modified: Thu Jun 22 08:42:26 2023, max compression
+gzip compressed data, was "UComp-1.0.78.tar", last modified: Fri Jun 30 11:47:12 2023, max compression
```

## Comparing `UComp-1.0.73.tar` & `UComp-1.0.78.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 08:42:26.878253 UComp-1.0.73/
--rw-rw-rw-   0        0        0      403 2023-06-19 10:16:42.000000 UComp-1.0.73/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-22 08:42:26.878253 UComp-1.0.73/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.73/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 08:42:26.837018 UComp-1.0.73/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-06-19 14:44:58.000000 UComp-1.0.73/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.73/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11479 2023-06-22 08:39:51.000000 UComp-1.0.73/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0     3378 2023-06-19 10:14:45.000000 UComp-1.0.73/UComp/Nile.bin
--rw-rw-rw-   0        0        0    11803 2023-06-22 08:39:36.000000 UComp-1.0.73/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-06-19 14:46:05.000000 UComp-1.0.73/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   897024 2023-06-16 11:32:46.000000 UComp-1.0.73/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24622 2023-06-22 08:39:44.000000 UComp-1.0.73/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.73/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.73/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.73/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.73/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.73/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    30193 2023-06-22 08:39:27.000000 UComp-1.0.73/UComp/tools.py
--rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.73/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-22 08:42:26.878253 UComp-1.0.73/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-22 08:42:26.000000 UComp-1.0.73/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 08:42:26.878253 UComp-1.0.73/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-22 08:42:23.000000 UComp-1.0.73/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:47:12.703754 UComp-1.0.78/
+-rw-rw-rw-   0        0        0      403 2023-06-19 10:16:42.000000 UComp-1.0.78/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-30 11:47:12.704748 UComp-1.0.78/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.78/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 11:47:12.658866 UComp-1.0.78/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-06-19 14:44:58.000000 UComp-1.0.78/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.78/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11479 2023-06-30 11:44:39.000000 UComp-1.0.78/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0     3378 2023-06-19 10:14:45.000000 UComp-1.0.78/UComp/Nile.bin
+-rw-rw-rw-   0        0        0    11803 2023-06-30 11:44:33.000000 UComp-1.0.78/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-06-19 14:46:05.000000 UComp-1.0.78/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   897024 2023-06-16 11:32:46.000000 UComp-1.0.78/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24640 2023-06-30 11:44:26.000000 UComp-1.0.78/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.78/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.78/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.78/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.78/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.78/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    30950 2023-06-30 11:44:22.000000 UComp-1.0.78/UComp/tools.py
+-rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.78/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:47:12.701756 UComp-1.0.78/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-30 11:47:12.000000 UComp-1.0.78/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-06-30 11:47:12.000000 UComp-1.0.78/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:47:12.000000 UComp-1.0.78/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-30 11:47:12.000000 UComp-1.0.78/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 11:47:12.000000 UComp-1.0.78/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 11:47:12.707747 UComp-1.0.78/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-30 11:46:25.000000 UComp-1.0.78/setup.py
```

### Comparing `UComp-1.0.73/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.78/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/UComp/ETSmodule.py` & `UComp-1.0.78/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/UComp/Nile.bin` & `UComp-1.0.78/UComp/Nile.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/UComp/PTSmodule.py` & `UComp-1.0.78/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.78/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/UComp/UCmodule.py` & `UComp-1.0.78/UComp/UCmodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 RunningFromPackage = True
 if RunningFromPackage:
     from UComp import UCc
     from UComp import tsfile
 else:
     import UCc
+    import tsfile
 
 
 class UCmodel:
     """
     UCmodel
     Estimates and forecasts UC general time series models
```

### Comparing `UComp-1.0.73/UComp/airpas.bin` & `UComp-1.0.78/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/UComp/gdp.bin` & `UComp-1.0.78/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/UComp/ipi.bin` & `UComp-1.0.78/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/UComp/libopenblas.dll` & `UComp-1.0.78/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/UComp/tools.py` & `UComp-1.0.78/UComp/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,30 +43,43 @@
         s = y.resample('Y').count()[1]
         x = y.values
     elif isinstance(y, np.ndarray):
         x = y
     return x, s
 
 
+def lags(x, l):
+    n = x.shape[0]
+    out = np.full((n - l, l + 1), 0.0)
+    for i in range(l + 1):
+        out[:, i] = x[l - i : n - i]
+    return out
+
 def pacfFun(ACF):
     nCoef = len(ACF)
     fi = np.zeros(nCoef)
     fi[0] = ACF[0]
     PACF = np.zeros(nCoef)
     PACF[0] = fi[0]
     # for p in range(1, nCoef):
     #     fi[p] = (PACF[p] - np.sum(fi[:p] * np.flip(PACF[:p]))) / (1 - np.sum(fi * PACF))
     #     PACF[p] = fi[p]
     #     fi[:p] = fi[:p] - fi[p] * np.flip(fi[:p])
     for i in range(nCoef - 1):
-         iACF = ACF[: i + 1]
-         fi[i + 1] = (ACF[i + 1] - (sum(fi[0 : i + 1] * iACF[::-1]))) / (1 - sum(fi * ACF))
-         PACF[i + 1] = fi[i + 1]
-         iACF = fi[0 : i + 1]
-         fi[0 : i + 1] -= fi[i + 1] * iACF[::-1]
+        iACF = ACF[: i + 1]
+        fi[i + 1] = (ACF[i + 1] - (sum(fi[0 : i + 1] * iACF[::-1]))) / (1 - sum(fi * ACF))
+        # Habría que corregir los PACF que salen > 1 con la regresión
+        # if abs(fi[i + 1] > 1):
+        #     X = lags(x, i + 1)
+        #     X = np.column_stack((X, np.ones(X.shape[1])))
+        #     coefficients, residuals, _, _ = np.linalg.lstsq(X[:, 1:], X[:, 0], rcond=None)
+        #     fi[i + 1] =
+        PACF[i + 1] = fi[i + 1]
+        iACF = fi[0 : i + 1]
+        fi[: i + 1] -= fi[i + 1] * iACF[::-1]
     return PACF
 
 
 def removeNaNs(x):
     """
     Remove nans at beginning or end of vector
 
@@ -212,15 +225,15 @@
 
     Author: Diego J. Pedregal
     """
     x, s = obj2array(y)
     if nCoef is None:
         nCoef = max(min(37, int(np.floor(len(x) / 4))), s)
     nCoef = int(nCoef)
-    x = (x - np.nanmean(x))  / np.nanstd(x)
+    x = (x - np.nanmean(x))  / np.sqrt(np.nanvar(x) * len(x) / (len(x) - 1))
     n = len(x[~np.isnan(x)])
     # ACF and PACF with Ljung Box tests and plots
     ACF = np.full(nCoef, 0.0)
     BAND = 2 / np.sqrt(n)
     for i in range(nCoef):
         prod = x[-n + i + 1: ] * x[: n - i - 1]
         prod1 = prod[~np.isnan(prod)]
@@ -399,15 +412,17 @@
         xs = y
         timeSeries = False
     q = len(MA)
     p = len(AR) - 1
     x = np.convolve(np.array(xs, dtype=float), MA)
     if p > 0:
         if isinstance(AR, list):
-            ARpoly = -np.array(AR[1:])
+            ARpoly = -np.flip(np.array(AR[1:]))
+        else:
+            ARpoly = -np.flip(AR[1:])
         for t in range(p, len(y)):
             x[t] += sum(ARpoly * x[t - p : t])
         x = x[:len(xs)]
         if timeSeries:
             x = pd.Series(x[:len(xs)], index=y.index)
             x = x[:len(xs)]
     else:
@@ -617,24 +632,29 @@
     Returns:
         A vector with all the dimensions
 
     Author: Diego J. Pedregal
     """
     # Rolling for nSeries
     # out = [h, nOrigs, nModels, nSeries]
-    if isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
-        y = y.values
+    if isinstance(y, np.ndarray):
+        time = pd.date_range(start="1990-01-31", periods=y.shape[0], freq="y")
+        y = pd.DataFrame(y, time)
     if y.ndim == 1:
-        y = y.reshape(-1, 1)
-    nSeries = y.shape[1]
+        nSeries = 1
+    else:
+        nSeries = len(y.columns)
     n = y.shape[0]
-    dataList = [y[:, j] for j in range(nSeries)]
+    if nSeries == 1:
+        dataList = [y for j in range(nSeries)]
+    else:
+        dataList = [y.iloc[:, j] for j in range(nSeries)]
     nOr = len(range(orig, n - h + 1, step))
     if not parallel or (nSeries == 1 and nOr == 1):
-        listOut = [slideAux(data, orig, forecFun, h, step, output, False, window, False, *args, **kwargs) for data in dataList]
+         listOut = [slideAux(data, orig, forecFun, h, step, output, False, window, False, *args, **kwargs) for data in dataList]
     else:
         # if nSeries > 1:
         #     with mp.Pool() as pool:
         #         listOut = pool.starmap(slideAux,
         #                                [(data, orig, forecFun, h, step, output, False, window, False, *args, **kwargs) for data in
         #                                 dataList])
         # elif nOr > 1:
@@ -665,33 +685,33 @@
     """
     # Rolling for 1 series
     # out = [h, nOrigs, nModels]
     n = len(y)
     origs = range(orig, n - h + 1, step)
     nOr = len(origs)
     if window is None:
-        outi = forecFun(y[:orig], h, *args, **kwargs)
+        outi = forecFun(y.iloc[:orig], h, *args, **kwargs)
     else:
-        outi = forecFun(y[orig - window + 1:orig], h, *args, **kwargs)
+        outi = forecFun(y.iloc[orig - window + 1:orig], h, *args, **kwargs)
     outi = np.array(outi)
     if outi.ndim > 1:
         nMethods = outi.shape[1]
     else:
         nMethods = 1
         outi = np.reshape(outi, (-1, 1))
     out = np.empty((h, nOr, nMethods))
     out[:, 0, :] = outi
     # colnames = list(outi.columns)
     dataList = []
     if nOr > 1:
         for j in range(1, nOr):
             if window is None:
-                dataList.append(y[:orig + j])
+                dataList.append(y.iloc[:orig + j])
             else:
-                dataList.append(y[orig - window + step:orig + j])
+                dataList.append(y.iloc[orig - window + step:orig + j])
     if parallel:
         with mp.Pool() as pool:
             listOut = pool.map(forecFun, dataList, (h, ) + args)
     else:
         listOut = [forecFun(data, h, *args, **kwargs) for data in dataList]
     if nOr > 1:
         for i in range(1, nOr):
```

### Comparing `UComp-1.0.73/UComp/tsfile.py` & `UComp-1.0.78/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.73/setup.py` & `UComp-1.0.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.73',
+    version='1.0.78',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

