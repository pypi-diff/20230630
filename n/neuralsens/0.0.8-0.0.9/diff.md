# Comparing `tmp/neuralsens-0.0.8.tar.gz` & `tmp/neuralsens-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralsens-0.0.8.tar", max compression
+gzip compressed data, was "neuralsens-0.0.9.tar", max compression
```

## Comparing `neuralsens-0.0.8.tar` & `neuralsens-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1633 2022-06-24 22:36:11.987342 neuralsens-0.0.8/LICENSE
--rw-r--r--   0        0        0      159 2022-06-24 22:36:12.023347 neuralsens-0.0.8/neuralsens/__init__.py
--rw-r--r--   0        0        0    14216 2022-09-11 15:48:06.415610 neuralsens-0.0.8/neuralsens/activation_functions.py
--rw-r--r--   0        0        0     1338 2022-06-24 22:36:12.025344 neuralsens-0.0.8/neuralsens/daily_demand_tr.py
--rw-r--r--   0        0        0    92707 2022-06-24 22:36:12.027341 neuralsens-0.0.8/neuralsens/data/daily_demand_tr.csv
--rw-r--r--   0        0        0      263 2022-06-24 22:36:12.027341 neuralsens-0.0.8/neuralsens/data/daily_demand_tv.csv
--rw-r--r--   0        0        0      860 2022-10-08 10:16:42.845215 neuralsens-0.0.8/neuralsens/meta.yaml
--rw-r--r--   0        0        0    60344 2022-10-09 13:36:36.773269 neuralsens-0.0.8/neuralsens/partial_derivatives.py
--rw-r--r--   0        0        0      731 2022-10-09 13:36:45.527504 neuralsens-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5520 2022-06-26 20:49:00.759041 neuralsens-0.0.8/README.md
--rw-r--r--   0        0        0     6292 2022-10-09 13:37:03.834685 neuralsens-0.0.8/setup.py
--rw-r--r--   0        0        0     6162 2022-10-09 13:37:03.834685 neuralsens-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1633 2022-06-24 22:36:11.000000 neuralsens-0.0.9/LICENSE
+-rw-r--r--   0        0        0      159 2022-06-24 22:36:12.000000 neuralsens-0.0.9/neuralsens/__init__.py
+-rw-r--r--   0        0        0    14216 2022-09-11 15:48:06.000000 neuralsens-0.0.9/neuralsens/activation_functions.py
+-rw-r--r--   0        0        0     1338 2022-06-24 22:36:12.000000 neuralsens-0.0.9/neuralsens/daily_demand_tr.py
+-rw-r--r--   0        0        0    92707 2022-06-24 22:36:12.000000 neuralsens-0.0.9/neuralsens/data/daily_demand_tr.csv
+-rw-r--r--   0        0        0      263 2022-06-24 22:36:12.000000 neuralsens-0.0.9/neuralsens/data/daily_demand_tv.csv
+-rw-r--r--   0        0        0      860 2022-10-09 13:56:22.000000 neuralsens-0.0.9/neuralsens/meta.yaml
+-rw-r--r--   0        0        0    66719 2023-01-25 20:06:06.268281 neuralsens-0.0.9/neuralsens/partial_derivatives.py
+-rw-r--r--   0        0        0      731 2023-01-02 11:57:24.800573 neuralsens-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5520 2022-06-26 20:49:00.000000 neuralsens-0.0.9/README.md
+-rw-r--r--   0        0        0     6292 2023-01-25 20:07:04.921743 neuralsens-0.0.9/setup.py
+-rw-r--r--   0        0        0     6162 2023-01-25 20:07:04.921743 neuralsens-0.0.9/PKG-INFO
```

### Comparing `neuralsens-0.0.8/LICENSE` & `neuralsens-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralsens-0.0.8/neuralsens/activation_functions.py` & `neuralsens-0.0.9/neuralsens/activation_functions.py`

 * *Files identical despite different names*

### Comparing `neuralsens-0.0.8/neuralsens/daily_demand_tr.py` & `neuralsens-0.0.9/neuralsens/daily_demand_tr.py`

 * *Files identical despite different names*

### Comparing `neuralsens-0.0.8/neuralsens/data/daily_demand_tr.csv` & `neuralsens-0.0.9/neuralsens/data/daily_demand_tr.csv`

 * *Files identical despite different names*

### Comparing `neuralsens-0.0.8/neuralsens/partial_derivatives.py` & `neuralsens-0.0.9/neuralsens/partial_derivatives.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 def jacobian_mlp(
     wts: list[float],
     bias: list[float],
     actfunc: list[str],
     X: pd.core.frame.DataFrame,
     y: pd.core.frame.DataFrame,
     sens_origin_layer: int = 0,
-    sens_end_layer: str | int = "last",
+    sens_end_layer = "last",
     sens_origin_input: bool = True,
     sens_end_input: bool = False,
     dev: str = "cpu",
     use_torch: bool = False,
 ):
     """Obtain first derivatives of MLP model given an input space.
     
@@ -402,15 +402,15 @@
 def hessian_mlp(
     wts: list[float],
     bias: list[float],
     actfunc: list[str],
     X: pd.core.frame.DataFrame,
     y: pd.core.frame.DataFrame,
     sens_origin_layer: int = 0,
-    sens_end_layer: str = "last",
+    sens_end_layer = "last",
     sens_origin_input: bool = True,
     sens_end_input: bool = False,
     dev: str = "cpu",
     use_torch: bool = False,
 ):
     """Obtain second derivatives of MLP model given an input space.
     
@@ -827,15 +827,93 @@
 
     def featurePlots(self):
         pass
 
     def timePlots(self):
         pass
 
-    def hesstosens(self):
+    def hesstosens(self, dev="gpu"):
+        # Import necessary modules based on processor, use torch when processor is gpu or use_torch is True
+        if dev == "gpu" or use_torch:
+            try:
+                from torch import (
+                    eye as identity,
+                    vstack,
+                    ones,
+                    mean,
+                    std,
+                    tensor,
+                    device,
+                    square,
+                    matmul,
+                    from_numpy,
+                    is_tensor,
+                    stack,
+                    zeros,
+                )
+                from numpy import ndarray, asarray
+
+                def float_array(x, dev="cpu") -> tensor:
+                    dev = device(dev)
+                    if isinstance(x, pd.DataFrame):
+                        return from_numpy(x.to_numpy()).float().to(dev)
+                    if isinstance(x, list):
+                        if isinstance(x[0], ndarray):
+                            x = asarray(x)
+                        elif is_tensor(x[0]):
+                            return stack(x).float().to(dev)
+                    if isinstance(x, ndarray):
+                        return from_numpy(x).float().to(dev)
+                    if is_tensor(x):
+                        return x.clone().detach().to(dev)
+                    return tensor(x, device=dev)
+
+                use_torch = True
+
+            except ImportError:
+                warnings.warn(
+                    "Pytorch installation could not be found, numpy would be used instead",
+                    ImportWarning,
+                )
+                from numpy import (
+                    identity,
+                    vstack,
+                    array,
+                    ones,
+                    mean,
+                    std,
+                    array,
+                    square,
+                    zeros,
+                    matmul,
+                )
+
+                def float_array(x, dev="cpu") -> array:
+                    return array(x.numpy())
+
+                use_torch = False
+
+        else:
+            from numpy import (
+                identity,
+                vstack,
+                array,
+                ones,
+                mean,
+                std,
+                array,
+                square,
+                matmul,
+                zeros,
+            )
+
+            def float_array(x, dev="cpu") -> array:
+                return array(x)
+
+            use_torch = False
         # Function to convert from hessian to jacobian
         temp_self = self
         for out in range(len(self.raw_sens)):
             n_inputs = len(temp_self.input_name)
             index_of_interest = triu_indices(n_inputs)
             mean = temp_self.sens[out]["mean"].to_numpy()[index_of_interest]
             std = temp_self.sens[out]["std"].to_numpy()[index_of_interest]
@@ -873,15 +951,15 @@
 # def jerkian_mlp(
 #     wts: list[float],
 #     bias: list[float],
 #     actfunc: list[str],
 #     X: pd.core.frame.DataFrame,
 #     y: pd.core.frame.DataFrame,
 #     sens_origin_layer: int = 0,
-#     sens_end_layer: str = "last",
+#     sens_end_layer = "last",
 #     sens_origin_input: bool = True,
 #     sens_end_input: bool = False,
 #     dev: str = "cpu",
 #     use_torch: bool = False,
 # ):
 #     # Import necessary modules based on processor, use torch when processor is gpu or use_torch is True
 #     if dev == "gpu" or use_torch:
@@ -1363,15 +1441,17 @@
     max_alpha: int = 100,
     alpha_step: int = 1,
     curve_equal_origin: bool = False,
     dev: str = "cpu",
     use_torch: bool = False,
     columns: list[str] = None,
     title: str = 'alpha-curves',
-    show_scaled: bool = True 
+    show_scaled: bool = True,
+    alpha_bar: int = 1,
+    kind: str = 'line'
 ):
     """Generate plots of alpha curves of partial derivatives
 
     Args:
         jacobian (list[Float] | Jacobian_mlp): Object storing partial derivatives
         tol (float, optional): Minimum change between consecutive alpha-mean values to continue calculating
             means. If None, Defaults to None.
@@ -1383,34 +1463,70 @@
             Only available if pytorch installation could be found. Defaults to "cpu".
         use_torch (bool, optional): Flag to indicate if pytorch Tensor shall be used. Defaults to False.
         columns (list[str], optional): List of variable names to show in alpha curves. If None,
             a list of str [X1, ..., Xn] is generated and used as input variables. Defaults to None.
         title [str]: title to show above alpha sensitivity curves plot
         show_scaled (bool, optional): Flag to indicate if second plot of curves divided by maximum shall be plotted. 
             Defaults to True.
+        alpha_bar ([int], [str]): alpha to create bar plot. Could be defined as 'inf' to show bar plot for alpha=np.inf.
+            Defaults to 1.
+        kind [str]: type of alpha plot that should be created. Options are 'bar' (alpha mean value for a given alpha_bar)
+            or 'line' (default alpha-means plot). Defaults to 'line'.
     """
     # Import necessary modules based on processor, use torch when processor is gpu or use_torch is True
+     # Import necessary modules based on processor, use torch when processor is gpu or use_torch is True
     if dev == "gpu" or use_torch:
         try:
-            from torch import arange
+            from torch import tensor, device, arange, log10, abs, from_numpy, is_tensor
+            from numpy import ndarray, asarray, empty, inf
+
+            def float_array(x, dev="cpu") -> tensor:
+                dev = device(dev)
+                if isinstance(x, pd.DataFrame):
+                    return from_numpy(x.to_numpy()).float()
+                if isinstance(x, list):
+                    x = asarray(x)
+                if isinstance(x, ndarray):
+                    return from_numpy(x).float()
+                if is_tensor(x):
+                    return x.clone().detach()
+                return tensor(x, device=dev)
 
         except ImportError:
             warnings.warn(
                 "Pytorch installation could not be found, numpy would be used instead",
                 ImportWarning,
             )
             from numpy import (
+                array,
                 arange,
+                floor,
+                log10,
+                abs,
+                empty, 
+                inf
             )
 
+            def float_array(x, dev="cpu") -> array:
+                return array(x.numpy())
+
     else:
         from numpy import (
+            array,
             arange,
+            floor,
+            log10,
+            abs,
+            empty, 
+            inf
         )
 
+        def float_array(x, dev="cpu") -> array:
+            return array(x)
+
     # Check if field in variable 
     if hasattr(jacobian, 'raw_sens'):
         # Initialize variables
         raw_sens = jacobian.raw_sens
         input_name = jacobian.X.columns
     else:
         input_name = columns
@@ -1421,109 +1537,146 @@
         if columns is None:
             input_name = ['X{}'.format(x) for x in (arange(0, jacobian.shape[1]))]
         raw_sens = [pd.DataFrame(jacobian, columns=input_name)]
     alphas = arange(1, max_alpha + 1, alpha_step)
     # Select the color map named rainbow
     cmap = cm.get_cmap(name="rainbow")
     
+    # Detect type of alpha plot
+    if kind not in ['line', 'bar']:
+        raise ValueError(f"Plot type {kind} not admitted. Choose 'line' or 'bar' to create the alpha plot.")
+    
     # Go through each output although this analysis is meant only for regression
-    if show_scaled:
-        fig, ax = plt.subplots(len(raw_sens), 2)
-        fig.suptitle(title)
-        for out, rs in enumerate(raw_sens):
-            if len(ax.shape) > 1:
-                axes = [[out, 0], [out, 1]]
-            else:
-                axes = [0, 1]
-            for inp, input in enumerate(input_name):
-                alpha_curves = alpha_curve(
-                    rs.iloc[:, inp], tol=tol, max_alpha=max_alpha, alpha_step=alpha_step, dev=dev
-                )
-                if curve_equal_origin:
-                    alpha_curves -= alpha_curves[0]
-                
-                alpha_curves_scl = alpha_curves
-                max_alpha_mean = max(abs(rs.iloc[:, inp]))
-                if max_alpha_mean != 0:
-                    alpha_curves_scl = alpha_curves / max_alpha_mean
-                var_color = cmap(inp / rs.shape[1])
-                ax[axes[0]].plot(
-                    alphas, alpha_curves, label=input, color=var_color
-                )
-                ax[axes[0]].axhline(
-                    y=max_alpha_mean, color=var_color, linestyle="dashed"
-                )
-                ax[axes[0]].text(
-                    alphas[-1], alpha_curves[-1],
-                    input, 
-                    color=var_color,
-                    path_effects=[pe.withStroke(linewidth=1, foreground="gray")]
-                )
-                ax[axes[0]].text(
-                    max([1,max_alpha - 20]), max_alpha_mean,
-                    'max({0}): {1:.{2}f}'.format(input, max_alpha_mean, 2),
-                    color=var_color,
-                    path_effects=[pe.withStroke(linewidth=1, foreground="gray")]
-                )
-                ax[axes[1]].plot(
-                    alphas, alpha_curves_scl, label=input, color=var_color
-                )
-            ax[axes[1]].axhline(y=1, color="gray", linestyle="dashed")
-            ax[axes[1]].legend()
-            ax[axes[0]].title.set_text("Alpha curves")
-            ax[axes[1]].title.set_text("Alpha curves / max(sens)")
-            ax[axes[0]].xaxis.get_major_locator().set_params(integer=True)
-            ax[axes[1]].xaxis.get_major_locator().set_params(integer=True)
-            ax[axes[0]].set_ylabel(r'$(ms_{X,j}^\alpha(f))^\alpha$')
-            ax[axes[1]].set_ylabel(r'$(ms_{X,j}^\alpha(f))^\alpha$')
-            ax[axes[0]].set_xlabel(r'$\alpha$')
-            ax[axes[1]].set_xlabel(r'$\alpha$')
-            return ax
-    else:
+    if kind == 'line':
+        if show_scaled:
+            fig, ax = plt.subplots(len(raw_sens), 2)
+            fig.suptitle(title)
+            for out, rs in enumerate(raw_sens):
+                if len(ax.shape) > 1:
+                    axes = [[out, 0], [out, 1]]
+                else:
+                    axes = [0, 1]
+                for inp, input in enumerate(input_name):
+                    alpha_curves = alpha_curve(
+                        rs.iloc[:, inp], tol=tol, max_alpha=max_alpha, alpha_step=alpha_step, dev=dev
+                    )
+                    if curve_equal_origin:
+                        alpha_curves -= alpha_curves[0]
+                    
+                    alpha_curves_scl = alpha_curves
+                    max_alpha_mean = max(abs(rs.iloc[:, inp]))
+                    if max_alpha_mean != 0:
+                        alpha_curves_scl = alpha_curves / max_alpha_mean
+                    var_color = cmap(inp / rs.shape[1])
+                    ax[axes[0]].plot(
+                        alphas, alpha_curves, label=input, color=var_color
+                    )
+                    ax[axes[0]].axhline(
+                        y=max_alpha_mean, color=var_color, linestyle="dashed"
+                    )
+                    ax[axes[0]].text(
+                        alphas[-1], alpha_curves[-1],
+                        input, 
+                        color=var_color,
+                        path_effects=[pe.withStroke(linewidth=1, foreground="gray")]
+                    )
+                    ax[axes[0]].text(
+                        max([1,max_alpha - 20]), max_alpha_mean,
+                        'max({0}): {1:.{2}f}'.format(input, max_alpha_mean, 2),
+                        color=var_color,
+                        path_effects=[pe.withStroke(linewidth=1, foreground="gray")]
+                    )
+                    ax[axes[1]].plot(
+                        alphas, alpha_curves_scl, label=input, color=var_color
+                    )
+                ax[axes[1]].axhline(y=1, color="gray", linestyle="dashed")
+                ax[axes[1]].legend()
+                ax[axes[0]].title.set_text("Alpha curves")
+                ax[axes[1]].title.set_text("Alpha curves / max(sens)")
+                ax[axes[0]].xaxis.get_major_locator().set_params(integer=True)
+                ax[axes[1]].xaxis.get_major_locator().set_params(integer=True)
+                ax[axes[0]].set_ylabel(r'$(ms_{X,j}^\alpha(f))^\alpha$')
+                ax[axes[1]].set_ylabel(r'$(ms_{X,j}^\alpha(f))^\alpha$')
+                ax[axes[0]].set_xlabel(r'$\alpha$')
+                ax[axes[1]].set_xlabel(r'$\alpha$')
+                return ax
+        else:
+            fig, ax = plt.subplots(len(raw_sens), 1)
+            # fig.suptitle("Alpha sensitivity curves")
+            for out, rs in enumerate(raw_sens):
+                if len(raw_sens) > 1:
+                    axes = [[out, 0]]
+                else:
+                    axes = [0]
+                for inp, input in enumerate(input_name):
+                    alpha_curves = alpha_curve(
+                        rs.iloc[:, inp], tol=tol, max_alpha=max_alpha, alpha_step=alpha_step, dev=dev
+                    )
+                    if curve_equal_origin:
+                        alpha_curves -= alpha_curves[0]
+                    
+                    alpha_curves_scl = alpha_curves
+                    max_alpha_mean = max(abs(rs.iloc[:, inp]))
+                    if max_alpha_mean != 0:
+                        alpha_curves_scl = alpha_curves / max_alpha_mean
+                    var_color = cmap(inp / rs.shape[1])
+                    ax.plot(
+                        alphas, alpha_curves, label=input, color=var_color
+                    )
+                    ax.axhline(
+                        y=max_alpha_mean, color=var_color, linestyle="dashed"
+                    )
+                    ax.text(
+                        alphas[-1], alpha_curves[-1],
+                        input, 
+                        color=var_color,
+                        path_effects=[pe.withStroke(linewidth=1, foreground="gray")]
+                    )
+                    ax.text(
+                        max([1,max_alpha - 20]), max_alpha_mean,
+                        'max({0}): {1:.{2}f}'.format(input, max_alpha_mean, 2),
+                        color=var_color,
+                        path_effects=[pe.withStroke(linewidth=1, foreground="gray")]
+                    )
+                ax.set_ylabel(r'$(ms_{X,j}^\alpha(f))$')
+                ax.set_xlabel(r'$\alpha$')
+                ax.title.set_text(title)
+                ax.xaxis.get_major_locator().set_params(integer=True)
+                return ax
+    elif kind == 'bar':
         fig, ax = plt.subplots(len(raw_sens), 1)
-        # fig.suptitle("Alpha sensitivity curves")
         for out, rs in enumerate(raw_sens):
-            if len(raw_sens) > 1:
-                axes = [[out, 0]]
+            # Calculate scale factor
+            N = rs.shape[0]
+            alpha_values = empty(rs.shape[1])
+            var_color = []
+            if alpha_bar == 'inf':
+                for inp, input in enumerate(input_name):
+                    alpha_values[inp] = max(abs(rs[input]))
+                    var_color.append(cmap(inp / rs.shape[1]))
             else:
-                axes = [0]
-            for inp, input in enumerate(input_name):
-                alpha_curves = alpha_curve(
-                    rs.iloc[:, inp], tol=tol, max_alpha=max_alpha, alpha_step=alpha_step, dev=dev
-                )
-                if curve_equal_origin:
-                    alpha_curves -= alpha_curves[0]
-                
-                alpha_curves_scl = alpha_curves
-                max_alpha_mean = max(abs(rs.iloc[:, inp]))
-                if max_alpha_mean != 0:
-                    alpha_curves_scl = alpha_curves / max_alpha_mean
-                var_color = cmap(inp / rs.shape[1])
-                ax.plot(
-                    alphas, alpha_curves, label=input, color=var_color
-                )
-                ax.axhline(
-                    y=max_alpha_mean, color=var_color, linestyle="dashed"
-                )
-                ax.text(
-                    alphas[-1], alpha_curves[-1],
-                    input, 
-                    color=var_color,
-                    path_effects=[pe.withStroke(linewidth=1, foreground="gray")]
-                )
-                ax.text(
-                    max([1,max_alpha - 20]), max_alpha_mean,
-                    'max({0}): {1:.{2}f}'.format(input, max_alpha_mean, 2),
-                    color=var_color,
-                    path_effects=[pe.withStroke(linewidth=1, foreground="gray")]
-                )
+                for inp, input in enumerate(input_name):
+                    scl_factor = 1
+                    if not all(v == 0 for v in rs[input]):
+                        scl_factor = 10 ** (max(floor(log10(abs(rs[rs != 0.0][input])))) + 1) 
+                    scl_rs = abs(rs[input]) / scl_factor
+                    alpha_values[inp] = scl_factor * sum(scl_rs ** alpha_bar / N) ** (1 / alpha_bar) 
+                    if alpha_values[inp] == inf:
+                        scl_factor *= 5
+                        scl_rs = abs(rs) / scl_factor
+                        alpha_values[inp] = scl_factor * sum(scl_rs ** alpha_bar / N) ** (1 / alpha_bar) 
+                    var_color.append(cmap(inp / rs.shape[1]))
+            alpha_order = alpha_values.argsort()
+            alpha_values = alpha_values[alpha_order]
+            var_color = [var_color[i] for i in alpha_order]
+            input_name = [input_name[i] for i in alpha_order]
+            ax.bar(input_name, alpha_values, color=var_color)
             ax.set_ylabel(r'$(ms_{X,j}^\alpha(f))$')
-            ax.set_xlabel(r'$\alpha$')
-            ax.title.set_text(title)
-            ax.xaxis.get_major_locator().set_params(integer=True)
+            ax.set_xlabel('Input variables')
+            ax.title.set_text(title + f'. Alpha: {alpha_bar}')
             return ax
         
 def alpha_curve(
     raw_sens: list,
     tol: float = None,
     max_alpha: int = 100,
     alpha_step: int = 1,
```

### Comparing `neuralsens-0.0.8/pyproject.toml` & `neuralsens-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neuralsens"
-version = "0.0.8"
+version = "0.0.9"
 description = "Calculate word counts in a text file."
 authors = ["Jaime Pizarroso Gonzalo", "Jose Portela Gonzalez", "Antonio Munoz San Roque"]
 license = "GPU-3"
 readme = "README.md"
 homepage = "https://github.com/JaiPizGon/NeuralSens"
 repository = "https://github.com/JaiPizGon/NeuralSens/python"
 include = [
```

### Comparing `neuralsens-0.0.8/README.md` & `neuralsens-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `neuralsens-0.0.8/setup.py` & `neuralsens-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['matplotlib>=3.5.2,<4.0.0',
  'numpy>=1.22.4,<2.0.0',
  'pandas>=1.4.2,<2.0.0',
  'scipy>=1.8.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'neuralsens',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Calculate word counts in a text file.',
     'long_description': '# NeuralSens <img src="docs/source/_static/NeuralSens.PNG" width="135px" height="140px" align="right" style="padding-left:10px;background-color:white;" />\n\n#### *Jaime Pizarroso Gonzalo, jpizarroso@comillas.edu*\n#### *Antonio Muñoz San Roque, Antonio.Munoz@iit.comillas.edu*\n#### *José Portela González, jose.portela@iit.comillas.edu*\n<!-- badges: start -->\n\n[![Documentation Status](https://readthedocs.org/projects/neuralsens/badge/?version=latest)](https://neuralsens.readthedocs.io/en/latest/?version=latest)\n[![pypi](https://img.shields.io/pypi/v/neuralsens.svg)](https://pypi.python.org/pypi/neuralsens)\n[![python](https://img.shields.io/badge/python-%5E3.8-blue)]()\n[![os](https://img.shields.io/badge/OS-Ubuntu%2C%20Mac%2C%20Windows-purple)]()\n<!-- badges: end -->\nThis is the development repository for the `neuralsens` package.  Functions within this package can be used for the analysis of neural network models created in Python. \n\nThe last version of this package can be installed using pip:\n\n```bash\n$ pip install neuralsens\n```\n\nIt can also be installed with conda:\n```bash\n$ conda install -c jaipizgon neuralsens\n```\n\n### Bug reports\n\nPlease submit any bug reports (or suggestions) using the [issues](https://github.com/JaiPizGon/NeuralSens/issues) tab of the GitHub page.\n\n### Functions\n\nOne function is available to analyze the sensitivity of a multilayer perceptron, evaluating variable importance and plotting the analysis results.\n\n```python\n# Import necessary packages to reproduce the example\nimport neuralsens.partial_derivatives as ns\nfrom neuralsens.daily_demand_tr import load_daily_data_demand_tr\nimport pandas as pd\nfrom sklearn.neural_network import MLPRegressor\n\n# Load data and scale variables\ndaily_demand_tr = load_daily_data_demand_tr()\nX_train = daily_demand_tr[["WD","TEMP"]]\nX_train.iloc[:, 1] = X_train.iloc[:, 1] / 10\ny_train = daily_demand_tr["DEM"] / 100\n```\n\nThe `jacobian_mlp` function analyze the sensitivity of the output to the input and  plots three graphics with information about this analysis. To calculate this sensitivity it calculates the partial derivatives of the output to the inputs using the training data. \nThe first plot shows information between the mean and the standard deviation of the sensitivity among the training data:\n- if the mean is different from zero, it means that the output depends on the input because the output changes when the input change.\n- if the mean is nearly zero, it means that the output could not depend on the input. If the standard deviation is also near zero it almost sure that the output does not depend on the variable because for all the training data the partial derivative is zero.\n- if the standard deviation is different from zero it means the the output has a non-linear relation with the input because the partial derivative derivative of the output depends on the value of the input.\n- if the standard deviation is nearly zero it means that the output has a linear relation with the input because the partial derivative of the output does not depend on the value of the input.\nThe second plot gives an absolute measure to the importance of the inputs, by calculating the sum of the squares of the partial derivatives of the output to the inputs.\nThe third plot is a density plot of the partial derivatives of the output to the inputs among the training data, giving similar information as the first plot.\n\n```python\n### Create MLP model\nmodel = MLPRegressor(solver=\'sgd\', # Update function\n                    hidden_layer_sizes=[40], # #neurons in hidden layers\n                    learning_rate_init=0.1, # initial learning rate\n                    activation=\'logistic\', # Logistic sigmoid activation function\n                    alpha=0.005, # L2 regularization term\n                    learning_rate=\'adaptive\', # Type of learning rate used in training\n                    max_iter=500, # Maximum number of iterations\n                    batch_size=10, # Size of batch when training\n                    random_state=150)\n\n# Train model\nmodel.fit(X_train, y_train)\n\n# Obtain parameters to perform jacobian\nwts = model.coefs_\nbias = model.intercepts_\nactfunc = [\'identity\',model.get_params()[\'activation\'],model.out_activation_]\nX = pd.DataFrame(X_train, columns=["WD","TEMP"])\ny = pd.DataFrame(y_train, columns=["DEM"])\nsens_end_layer = \'last\'\nsens_end_input = False\nsens_origin_layer = 0\nsens_origin_input = True\n\n# Perform jacobian of the model\njacobian = ns.jacobian_mlp(wts, bias, actfunc, X, y)\njacobian.plot("sens")\n```\n\n![](docs/source/_static/readme_example_sensplots.png)<!-- -->\n\nApart from the plot created with the `"sens"` argument by an internal call\nto `sensitivity_plots()`, other plots can be obtained to analyze the neural \nnetwork model (although they are yet to be coded, thanks for your patience!).\n\n### Citation\n\nPlease, to cite NeuralSens in publications use:\n\nPizarroso J, Portela J, Muñoz A (2022). “NeuralSens: Sensitivity Analysis of Neural Networks.” _Journal of\nStatistical Software_, *102*(7), 1-36. doi: 10.18637/jss.v102.i07 (URL:\nhttps://doi.org/10.18637/jss.v102.i07).\n\n### License\n\nThis package is released in the public domain under the General Public License [GPL](https://www.gnu.org/licenses/gpl-3.0.en.html). \n\n### Association\nPackage created in the Institute for Research in Technology (IIT), [link to homepage](https://www.iit.comillas.edu/index.php.en) \n',
     'author': 'Jaime Pizarroso Gonzalo',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/JaiPizGon/NeuralSens',
```

### Comparing `neuralsens-0.0.8/PKG-INFO` & `neuralsens-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralsens
-Version: 0.0.8
+Version: 0.0.9
 Summary: Calculate word counts in a text file.
 Home-page: https://github.com/JaiPizGon/NeuralSens
 License: GPU-3
 Author: Jaime Pizarroso Gonzalo
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

