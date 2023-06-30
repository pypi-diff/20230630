# Comparing `tmp/cfr-2023.6.29.tar.gz` & `tmp/cfr-2023.6.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-2023.6.29.tar", last modified: Thu Jun 29 20:56:00 2023, max compression
+gzip compressed data, was "cfr-2023.6.30.tar", last modified: Fri Jun 30 11:57:53 2023, max compression
```

## Comparing `cfr-2023.6.29.tar` & `cfr-2023.6.30.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-29 20:56:00.807814 cfr-2023.6.29/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-2023.6.29/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-06-29 20:56:00.807612 cfr-2023.6.29/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1421 2023-06-28 18:00:43.000000 cfr-2023.6.29/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-29 20:56:00.800472 cfr-2023.6.29/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     5134 2023-06-22 22:28:33.000000 cfr-2023.6.29/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-29 20:56:00.804417 cfr-2023.6.29/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-2023.6.29/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-2023.6.29/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-29 20:56:00.807197 cfr-2023.6.29/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-2023.6.29/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-2023.6.29/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-2023.6.29/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-2023.6.29/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    67171 2023-06-29 20:53:21.000000 cfr-2023.6.29/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-2023.6.29/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    57520 2023-06-29 20:52:53.000000 cfr-2023.6.29/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     4551 2023-06-26 04:44:01.000000 cfr-2023.6.29/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-06-26 04:41:16.000000 cfr-2023.6.29/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    26818 2023-06-26 23:02:19.000000 cfr-2023.6.29/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    55370 2023-06-26 05:04:39.000000 cfr-2023.6.29/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-29 20:56:00.806452 cfr-2023.6.29/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-06-29 20:56:00.000000 cfr-2023.6.29/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-29 20:56:00.000000 cfr-2023.6.29/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-29 20:56:00.000000 cfr-2023.6.29/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-2023.6.29/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      201 2023-06-29 20:56:00.000000 cfr-2023.6.29/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-29 20:56:00.000000 cfr-2023.6.29/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-29 20:56:00.807908 cfr-2023.6.29/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1404 2023-06-29 20:53:50.000000 cfr-2023.6.29/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.936493 cfr-2023.6.30/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-2023.6.30/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-06-30 11:57:53.936313 cfr-2023.6.30/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1421 2023-06-28 18:00:43.000000 cfr-2023.6.30/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.925572 cfr-2023.6.30/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     5134 2023-06-22 22:28:33.000000 cfr-2023.6.30/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.932745 cfr-2023.6.30/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-2023.6.30/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-2023.6.30/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.935807 cfr-2023.6.30/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-2023.6.30/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-2023.6.30/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-2023.6.30/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-2023.6.30/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    67397 2023-06-30 11:55:02.000000 cfr-2023.6.30/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-2023.6.30/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    57520 2023-06-29 20:52:53.000000 cfr-2023.6.30/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     4551 2023-06-26 04:44:01.000000 cfr-2023.6.30/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-06-26 04:41:16.000000 cfr-2023.6.30/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    26818 2023-06-26 23:02:19.000000 cfr-2023.6.30/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    58412 2023-06-30 11:55:02.000000 cfr-2023.6.30/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.935003 cfr-2023.6.30/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-2023.6.30/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      201 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-30 11:57:53.936564 cfr-2023.6.30/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1404 2023-06-30 11:57:28.000000 cfr-2023.6.30/setup.py
```

### Comparing `cfr-2023.6.29/LICENSE` & `cfr-2023.6.30/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/PKG-INFO` & `cfr-2023.6.30/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2023.6.29
+Version: 2023.6.30
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-2023.6.29/README.md` & `cfr-2023.6.30/README.md`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/bin/cfr` & `cfr-2023.6.30/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/__init__.py` & `cfr-2023.6.30/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/climate.py` & `cfr-2023.6.30/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/da/enkf.py` & `cfr-2023.6.30/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/gcm.py` & `cfr-2023.6.30/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/ml.py` & `cfr-2023.6.30/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/proxy.py` & `cfr-2023.6.30/cfr/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1293,28 +1293,39 @@
             fig, ax, gs = visual.plot_proxies(df, **kws)
             return fig, ax, gs
         else:
             fig, ax = visual.plot_proxies(df, **kws)
             return fig, ax
 
 
+    # def plotly(self, **kwargs):
+    #     ''' Plot the database on an interactive map utilizing Plotly
+    #     '''
+    #     df = self.to_df()
+    #     fig = px.scatter_geo(
+    #         df, lat='lat', lon='lon',
+    #         color='ptype',
+    #         hover_name='pid',
+    #         projection='natural earth',
+    #         **kwargs,
+    #     )
+
+    #     return fig
+
+
     def plotly(self, **kwargs):
-        ''' Plot the database on an interactive map utilizing Plotly
+        '''Plot the database on an interactive map utilizing Plotly
         '''
-        df = self.to_df()
-        fig = px.scatter_geo(
-            df, lat='lat', lon='lon',
-            color='ptype',
-            hover_name='pid',
-            projection='natural earth',
-            **kwargs,
-        )
 
+        df = self.to_df()
+        fig = visual.plotly_proxies(df)
         return fig
 
+
+
     def make_composite(self, obs=None, obs_nc_path=None, vn='tas', lat_name=None, lon_name=None, bin_width=10, n_bootstraps=1000, qs=(0.025, 0.975), stat_func=np.nanmean, anom_period=[1951, 1980]):
         ''' Make composites of the records in the proxy database.'''
         if obs is None and obs_nc_path is not None:
             obs = ClimateField().load_nc(obs_nc_path, vn=vn, lat_name=lat_name, lon_name=lon_name)
 
         for pid, pobj in tqdm(self.records.items(), total=self.nrec, desc='Analyzing ProxyRecord'):
             pobj_stdd = pobj.standardize()
```

### Comparing `cfr-2023.6.29/cfr/psm.py` & `cfr-2023.6.30/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/reconjob.py` & `cfr-2023.6.30/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/reconres.py` & `cfr-2023.6.30/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/ts.py` & `cfr-2023.6.30/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/utils.py` & `cfr-2023.6.30/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.29/cfr/visual.py` & `cfr-2023.6.30/cfr/visual.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,14 +153,62 @@
         'lake.pollen': '^',
         'lake.alkenone': 'h',
         'borehole': '8',
         'hybrid': 'P',
         'documents': 'X',
         'peat.pollen': 'o',
     }
+    markers_dict_plotly = {
+        'coral.calc': 'cross',
+        'coral.SrCa': 'x',
+        'coral.d18O': 'circle',
+        'coral.d18Osw': 'hexagon2',
+        'ice.melt': 'traingle-left',
+        'ice.d18O': 'diamond-tall',
+        'ice.dD': 'traingle-right',
+        'ice.d-excess': 'circle',
+        'ice.isotope_diffusion': 'hexagon',
+        'ice.hybrid': 'arrow-left',
+        'tree.TRW': 'triangle-up',
+        'tree.MXD': 'triangle-down',
+        'tree.ENSO': 'triangle-up',
+        'pollen.temp': 'circle',
+        'land.temp': 'circle',
+        'ocean.temp': 'triangle-down',
+        'tas': 'triangle-up',
+        'pr': 'circle',
+        'speleothem.d18O': 'circle',
+        'speleothem.dD': 'triangle-right',
+        'bivalve.d18O': 'circle',
+        'marine.TEX86': 'star',
+        'marine.MgCa': 'triangle-down',
+        'marine.d18O': 'circle',
+        'marine.MAT': 'hexagon2',
+        'marine.alkenone': 'hexagon',
+        'marine.foram': 'arrow-left',
+        'marine.diatom': 'traingle-up',
+        'marine.dinocyst': 'triangle-right',
+        'marine.radiolaria': 'traingle-left',
+        'marine.GDGT': 'square',
+        'lake.varve_thickness': 'hexagon2',
+        'lake.varve_property': 'square',
+        'lake.accumulation': 'triangle-down',
+        'lake.chironomid': 'triangle-down',
+        'lake.midge': 'triangle-right',
+        'lake.TEX86': 'star',
+        'lake.BSi': 'arrow-left',
+        'lake.chrysophyte': 'diamond-tall',
+        'lake.reflectance': 'triangle-left',
+        'lake.pollen': 'triangle-up',
+        'lake.alkenone': 'hexagon',
+        'borehole': 'arrow-left',
+        'hybrid': 'cross',
+        'documents': 'x',
+        'peat.pollen': 'circle',
+    }
 
 class CartopySettings:
     projection_dict = {
         'Robinson': ccrs.Robinson,
         'NorthPolarStereo': ccrs.NorthPolarStereo,
         'SouthPolarStereo': ccrs.SouthPolarStereo,
         'PlateCarree': ccrs.PlateCarree,
@@ -566,14 +614,56 @@
             setlabel(ax['count'], '(b)', prop=enumerate_prop, bbox_to_anchor=enumerate_anchor_count)
 
     if not return_gs:
         return fig, ax
     else:
         return fig, ax, gs
 
+def plotly_proxies(df):
+    import plotly.graph_objects as go
+    # from .visual import STYLE
+
+    # df = self.to_df()
+    fig = go.Figure()
+    ptype_ls = df['ptype'].unique() 
+    for ptype in ptype_ls:  # draw every ptype
+        dfu = df.loc[df['ptype'] == ptype]
+        fig.add_trace(
+        go.Scattergeo(
+            lon=dfu.lon,
+            lat=dfu.lat,
+            text=ptype,
+            marker_color=STYLE.colors_dict[ptype],
+            marker=dict(symbol=STYLE.markers_dict_plotly[ptype],
+                        line=dict(width=0.5, color="black")),
+            marker_size=10,
+            hovertext=dfu['pid'],
+            name=f'{ptype} (n={len(dfu)})',
+            hoverinfo='lon+lat',
+            hovertemplate= \
+            "<br>pid: %{hovertext}</br>ptype: %{data.text}<br>lon: %{lon}</br>lat: %{lat}<extra></extra>",
+        ))
+    fig.update_geos(projection_type="natural earth",
+                center_lon=180,
+                lonaxis_range=[0, 360],
+                lataxis_range=[-90, 90],
+                showocean=True,
+                showland=True,
+                oceancolor="#70A0C1",
+                landcolor="#CBCBBA")
+    fig.update_layout(
+        margin=dict(l=35, r=35, t=35, b=35),
+        legend_x=1,
+        width=1000,
+        height=450,
+    )
+    fig.layout.dragmode = False
+    return fig
+
+
 def plot_proxy_age_map(df, lon_col='lon', lat_col='lat', type_col='type', time_col='time',
                        title=None, title_weight='normal', font_scale=1.5,
                        figsize=[12, 10], projection=ccrs.Robinson, central_longitude=0, markersize=150,
                        plot_cbar=True, marker_color=None, transform=ccrs.PlateCarree(), p=STYLE,
                        add_nino34_box=False, add_nino12_box=False, add_box=False, add_box_lf=None, add_box_ur=None):
 
     fig = plt.figure(figsize=figsize)
```

### Comparing `cfr-2023.6.29/cfr.egg-info/PKG-INFO` & `cfr-2023.6.30/cfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2023.6.29
+Version: 2023.6.30
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-2023.6.29/setup.py` & `cfr-2023.6.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='2023.6.29',
+    version='2023.6.30',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

